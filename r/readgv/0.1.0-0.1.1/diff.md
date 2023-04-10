# Comparing `tmp/readgv-0.1.0.tar.gz` & `tmp/readgv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readgv-0.1.0.tar", last modified: Tue Feb 28 17:50:37 2023, max compression
+gzip compressed data, was "readgv-0.1.1.tar", last modified: Mon Apr 10 16:54:31 2023, max compression
```

## Comparing `readgv-0.1.0.tar` & `readgv-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 17:50:37.375271 readgv-0.1.0/
--rw-rw-rw-   0        0        0     1077 2023-02-28 17:48:52.000000 readgv-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      128 2023-02-28 17:50:37.375271 readgv-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2630 2023-02-10 05:19:31.000000 readgv-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 17:50:37.354717 readgv-0.1.0/ReadGV.egg-info/
--rw-rw-rw-   0        0        0      128 2023-02-28 17:50:37.000000 readgv-0.1.0/ReadGV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-02-28 17:50:37.000000 readgv-0.1.0/ReadGV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 17:50:37.000000 readgv-0.1.0/ReadGV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-28 17:50:37.000000 readgv-0.1.0/ReadGV.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-28 17:50:37.373271 readgv-0.1.0/readgv/
--rw-rw-rw-   0        0        0     5124 2023-02-10 03:49:12.000000 readgv-0.1.0/readgv/Plot.py
--rw-rw-rw-   0        0        0       90 2023-02-28 17:44:49.000000 readgv-0.1.0/readgv/__init__.py
--rw-rw-rw-   0        0        0      510 2023-02-28 17:41:59.000000 readgv-0.1.0/readgv/__main__.py
--rw-rw-rw-   0        0        0    11368 2023-02-15 22:56:15.000000 readgv-0.1.0/readgv/fileconversion.py
--rw-rw-rw-   0        0        0     2733 2023-02-10 04:17:47.000000 readgv-0.1.0/readgv/mathstats.py
--rw-rw-rw-   0        0        0    10967 2023-02-04 16:50:50.000000 readgv-0.1.0/readgv/read_outcar.py
--rw-rw-rw-   0        0        0    14798 2023-02-15 23:33:26.000000 readgv-0.1.0/readgv/readgv.py
--rw-rw-rw-   0        0        0       86 2023-02-28 17:50:37.377270 readgv-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      184 2023-02-10 05:02:53.000000 readgv-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:54:31.593000 readgv-0.1.1/
+-rw-rw-rw-   0        0        0     1077 2023-02-28 17:48:52.000000 readgv-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3112 2023-04-10 16:54:31.567000 readgv-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2752 2023-03-08 22:00:06.000000 readgv-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 16:54:31.556000 readgv-0.1.1/ReadGV.egg-info/
+-rw-rw-rw-   0        0        0     3112 2023-04-10 16:54:29.000000 readgv-0.1.1/ReadGV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-04-10 16:54:31.000000 readgv-0.1.1/ReadGV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 16:54:29.000000 readgv-0.1.1/ReadGV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-10 16:54:29.000000 readgv-0.1.1/ReadGV.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 16:54:30.000000 readgv-0.1.1/ReadGV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 16:54:30.000000 readgv-0.1.1/ReadGV.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 16:54:31.522000 readgv-0.1.1/readgv/
+-rw-rw-rw-   0        0        0     5124 2023-02-10 03:49:12.000000 readgv-0.1.1/readgv/Plot.py
+-rw-rw-rw-   0        0        0       59 2023-01-23 16:04:16.000000 readgv-0.1.1/readgv/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-01-23 16:07:28.000000 readgv-0.1.1/readgv/__main__.py
+-rw-rw-rw-   0        0        0    11297 2023-04-10 16:37:29.000000 readgv-0.1.1/readgv/fileconversion.py
+-rw-rw-rw-   0        0        0     4371 2023-03-27 19:38:00.000000 readgv-0.1.1/readgv/mathstats.py
+-rw-rw-rw-   0        0        0    10092 2023-04-04 19:18:04.000000 readgv-0.1.1/readgv/read_gaussian_log.py
+-rw-rw-rw-   0        0        0    10855 2023-03-13 19:35:40.000000 readgv-0.1.1/readgv/read_outcar.py
+-rw-rw-rw-   0        0        0     1313 2023-03-22 21:13:00.000000 readgv-0.1.1/readgv/read_poscar.py
+-rw-rw-rw-   0        0        0     1786 2023-03-22 21:05:45.000000 readgv-0.1.1/readgv/read_procar.py
+-rw-rw-rw-   0        0        0    15968 2023-04-10 16:38:38.000000 readgv-0.1.1/readgv/readgv.py
+-rw-rw-rw-   0        0        0       86 2023-04-10 16:54:31.592000 readgv-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-04-10 16:40:29.000000 readgv-0.1.1/setup.py
```

### Comparing `readgv-0.1.0/LICENSE.txt` & `readgv-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `readgv-0.1.0/README.md` & `readgv-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 ### Installation  
 * pip install -e git+git://github.com/MAJabed/ReadGV.git 
 * With pip `pip install -e ReadGV/` [No available yet]
 
 
 ## Running VaspUtils 
 ```python 
-python  python -m vasputils [-job] [vasp2gaus/gaus2poscar/read_bands] [--file input file] [--fout output file] [--ftype xyz/gaus (gaussian input file)] [--select boolean] [--direct boolean]  
+python  python -m vasputils [-job] [vasp2gaus/gaus2poscar/read_bands**] [--file input file] [--fout output file] [--ftype xyz/gaus (gaussian input file)] [--select boolean] [--direct boolean]  
 ```
 * `-job` option to select task to execute, currently available task 
-    *  `vasp2gaus` : Convert poscar or Contcar file to xyz or gaussian input file format 
+    * `vasp2gaus` : Convert poscar or Contcar file to xyz or gaussian input file format 
     * `gaus2poscar` : Convert gaussian input file to VASP POSCAR file format. Periodic cell (Tv) should be given in the .com file. 
     * `read_bands` : Read selected or all bands from OUTCAR and write in a file, print or plot (follow `--plot`)
     * `get_geom` : Write or print molecular dynamic trajectory from the OUTCAR files 
-    
+    * `abs_gaus` : Read Gaussian TDDFT output file, Dress excited energies using Gaussian fucntion to plot absorption spectra 
+
 * `--file` : The input file name 
 * `--fout` : The output file name 
 * `--ftype` :  Output file format, `xyz` or `gaus` (gaussian input file) 
 * `--select` : `Boolean`, select coordinates in POSCAR file
 * `--direct` : `Boolean`, direct or cartesian coordinates in POSCAR file format 
 * `--bands` : No of bands to read, default 100 
 * `--frames` : MD frames to read,  last frame  `final`, initial frame `initial`, all `all`, last n frames `-n`, first n frame `n`
@@ -39,8 +40,8 @@
 
 ---
 #### Disclaimer:
 #### It is an incomplete package, still under development.
 ---
 #### License: 
 
-VaspUtils is freely available under an [MIT](https://opensource.org/licenses/MIT) License
+ReadGV is freely available under an [MIT](https://opensource.org/licenses/MIT) License
```

### Comparing `readgv-0.1.0/readgv/Plot.py` & `readgv-0.1.1/readgv/Plot.py`

 * *Files identical despite different names*

### Comparing `readgv-0.1.0/readgv/fileconversion.py` & `readgv-0.1.1/readgv/fileconversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     a=np.asarray(a) 
     b=np.asarray(b) 
     unitV1 = a/np.linalg.norm(a)
     unitV2 = b/np.linalg.norm(b)
     return  np.arccos(np.dot(unitV1, unitV2))
 
 
-def contcar2com(name, name_out,Gaus_out=False):  # name is the contcar file name 
+def contcar2com(name, nameout,Gaus_out=False):  # name is the contcar file name 
+    
+    name_out = os.path.splitext(nameout)[0]
+    file_ext = os.path.splitext(nameout)[1] 
     f_cont = open(name,'r') 
     # reading file, and cell normalizing factor  
     line_cont = f_cont.readlines()  
     sys_name  = line_cont[0] #compname  
     sigma = float(line_cont[1].split()[0]) 
 
     #Checking file format, cell dimension check 
@@ -94,51 +97,51 @@
         AA = np.c_[np.asarray(ions_list),Freez]  
         Cord_Str = np.c_[AA,np.asarray(Cart_Cord).round(4)] 
        # print(np.asarray(Cart_Cord).round(4))
     elif selec_dynm is False: 
         Cord_Str = np.c_[np.asarray(ions_list),np.asarray(Cart_Cord).round(4)] 
       #  Cord_Str = np.c_[np.asarray(ions_list),np.asarray(np.array_str(np.asarray(Cart_Cord),precision=4))] 
    
-    print(name_out)
+    #print(name_out)
     if Gaus_out == True: 
         Header = '''%%mem=20GB
 %%nprocshared=40
 %%chk=%s.chk 
 
 #p opt pbe1pbe/gen nosymm pseudo=read scf=maxcycles=10000
 
 %s
 
 0 1
 ''' %(name_out,sys_name.rstrip('\n')) 
 
-        with open('%s.com'%name_out, "w") as fout:
+        with open(name_out+file_ext, "w") as fout:
             fout.write(Header)
    #         print(Cord_Str)
             if selec_dynm is True: 
                 np.savetxt(fout, Cord_Str,fmt='%-5.10s %-5.10s %-10.10s  %-10.10s  %-10.10s') 
                 
             elif selec_dynm is False: 
                 np.savetxt(fout, Cord_Str,fmt='%-5.10s  %-10.6s  %-10.10s  %-10.10s')
                
             PBC = np.c_[np.asarray(['Tv','Tv','Tv']),xyz.astype('<U10')] 
             np.savetxt(fout, PBC,fmt='%-5.10s  %-010.8s  %-10.8s  %-10.10s') 
              
-        print('Gaussian input file is written in the file name %s.com' %name_out)  
+        print('Gaussian input file is written in the file name %s' %(name_out+file_ext))   
         fout.close() 
 
 
     else :
-        with open('%s.xyz'%name_out.rstrip('.xyz'), "a") as fout: 
+        with open(name_out+file_ext, "a") as fout: 
             #print(len(Cord_Str))
             fout.write('%i \n' %len(Cord_Str))
             fout.write('%s \n' %sys_name.rstrip('\n')) 
             np.savetxt(fout,np.c_[Cord_Str[:,0],Cord_Str[:,-3:]],
                        fmt='%-5.10s  %-10.10s  %-10.10s  %-10.10s') 
-        print('xyz file is written in the file name %s.xyz' %name_out) 
+        print('xyz file is written in the file name %s' %(name_out+file_ext)) 
         fout.close() 
 
 def com2poscar(name,name_out=True, select=False, direct=True): 
     def angle(a,b):
         a=np.asarray(a) 
         b=np.asarray(b) 
         unitV1 = a/np.linalg.norm(a)
@@ -147,45 +150,39 @@
     
     file = open(name) 
     line = file.readline() 
     topheader = [] 
     commandkeys = [] 
      
     while line : 
-        print('%' in line)
         if '%' in line: 
-#            print(line)
             topheader.append(line)
             line = file.readline() 
-#            print('command')
         else: 
             break 
     if len(line.strip())==0: 
         line = file.readline() 
     while line : 
         if '#' in line: 
             commandkeys.append(line)
             line=file.readline() 
-#            print('keys')
         else: 
             break 
     if len(line.strip())==0: 
         line=file.readline() 
         
     comp_name = line.strip('\n') 
     line = file.readline() 
-#    print('name')
         
     if len(line.strip())==0: 
         line=file.readline()  
     Coord = []
     TVs= [] 
     while line: 
         if (len(line.split())%2 ==0 ) & all([i.isdigit() for i in line.split()]) :
-#            print('charg_multi')
             chrg_multi = line.strip('\n') 
             line = file.readline() 
             while line :
                 if not 'tv' in line.lower(): 
                     Coord.append(line.strip('\n') )
                 else: 
                     TVs.append(line.strip('\n').split())
```

### Comparing `readgv-0.1.0/readgv/read_outcar.py` & `readgv-0.1.1/readgv/read_outcar.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
         self.positions = None
         self.kpoints = None
         self.array_sizes = {}
         self.species = None
         self.final_data = {}
         self.iteration_data = []
         self.outcar = open(self.filename, 'r').read() 
-        
-        
+                
         self.poscar = None 
         self.paw_ions = []      # Ions from the potential function order in Outcar 
         self.no_ions = []  # Number of ions per ion type 
         self.paw_rwigs_rad = [] #RWIGS from postcar informatio in outcar 
         self.ibrion = None 
         self.incar = {} 
         #self.outcar_distance_warning()
@@ -226,19 +225,14 @@
         return States 
        
     def free_energy(self): 
         f=self.outcar 
         free_en = np.array([i.split() for i in re.findall(r'free  energy.*', f)])[:,-2].astype(float) 
         return free_en 
 
-class read_procar: 
-    def __init__(self, filename='PROCAR') :  
-        self.filename = filename
-    
-
             
 #if __name__ == '__main__': 
 #    f = 'Datafiles/OUTCAR' 
 #    a = Output(filename=f)
 #    print(a.outcar2incar())
 #    a.md_traj(out='Temmp_md.dat')  
 #  'NKPTS', 'NBANDS', 'NEDOS', 'NIONS', 'NGX', 'NGY', 'NGZ', 'NGXF', 'NGYF', 'NGZF', 'ISPIN']:
```

### Comparing `readgv-0.1.0/readgv/readgv.py` & `readgv-0.1.1/readgv/readgv.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,62 +78,87 @@
                             help = 'Absorption spectra in eV or nm unit?, default in eV unit') 
     parser.add_argument("--figsize", dest="figsize",  nargs='+', type=int, default=(7,5), 
                             help = 'Plot figure size, integer list, default (7,5)')    
     
     
     (options, args) = parser.parse_known_args() 
     #print(options)
-   #print( args)
+    #print( args)
     
+    # making some confusing given argument right. 
+    if options.job == 'vasp2com' or options.job =='contcar2com' : 
+       options.job = 'vasp2gaus' 
+       options.ftype = 'gaus' 
+
+ 
+   
     if options.job == 'vasp2gaus': 
         if options.fname is None: 
             options.fname = input('What is the POSCAR file name? :').lstrip().rstrip() 
         fname = options.fname
         Warning.file_not_exist(fname)  
         
         if options.fout is None: 
-            options.fout = os.path.splitext(options.fname)[0]
-        name_out = os.path.splitext(options.fout)[0]  
+            if options.ftype =='gaus' or options.ftype =='com': 
+                file_ext = '.com' 
+            elif options.ftype =='xyz':  
+                file_ext = '.xyz'
+            else: 
+                file_ext = '' 
+            name_out = os.path.splitext(options.fname)[0] 
+        else: 
+            file_ext = os.path.splitext(options.fout)[1] 
+            name_out = options.fout # os.path.splitext(options.fout)[0]  
+            
+        if os.path.isfile(name_out+file_ext ): #'%s.com'%name_out):
+            print ('%s is exist'%(name_out+file_ext ))  
+            name_out_ = input('What should be the output file name?:').rstrip().lstrip() #.rstrip('.com')  
+            if not len(name_out_)==0: 
+                file_ext = os.path.splitext(name_out_)[1]
+                name_out= os.path.splitext(name_out_)[0]   
+            if os.path.isfile(name_out+file_ext ):  # overwritting the file if no name is given 
+                print('Overwriting the file %s' %(name_out+file_ext)) # name_out = name_out+'_'+''.join(random.choices(string.ascii_lowercase, k=5)) 
+                os.remove(name_out+file_ext ) 
         
-        if options.ftype =='gaus': 
+        if options.ftype =='gaus' or options.ftype =='com': 
             Gaus_out = True 
-            if os.path.isfile('%s.com'%name_out):
-                print ('%s.com is exist'%name_out) 
-                name_out_ = input('What should be the output file name?:').rstrip().lstrip().rstrip('.com')  
-                if not len(name_out_)==0: 
-                    name_out= name_out_     
-                if os.path.isfile('%s.com'%name_out):  # overwritting the file if no name is given 
-                    print('Overwriting the file %s.com') # name_out = name_out+'_'+''.join(random.choices(string.ascii_lowercase, k=5)) 
-                    os.remove('%s.com'%name_out) 
-        if options.ftype =='xyz': 
-            Gaus_out = False
-            if os.path.isfile('%s.xyz'%name_out):
-                print ('%s.xyz is exist'%name_out) 
-                name_out_ = input('What should be the output file name?:').rstrip().lstrip().rstrip('.xyz')  
-                if not len(name_out_)==0: 
-                    name_out= name_out_     
-                if os.path.isfile('%s.xyz'%name_out): 
-                    os.remove('%s.xyz'%name_out) 
-                    print('Overwriting the file %s.xyz'%name_out) 
-   
-        contcar2com(fname, name_out,Gaus_out=Gaus_out) 
+# =============================================================================
+#         elif options.ftype =='xyz': 
+#             Gaus_out = False
+#             if os.path.isfile('%s.xyz'%name_out):
+#                 print ('%s.xyz is exist'%name_out) 
+#                 name_out_ = input('What should be the output file name?:').rstrip().lstrip().rstrip('.xyz')  
+#                 if not len(name_out_)==0: 
+#                     name_out= name_out_     
+#                 if os.path.isfile('%s.xyz'%name_out): 
+#                     os.remove('%s.xyz'%name_out) 
+#                     print('Overwriting the file %s.xyz'%name_out) 
+# =============================================================================
+        else: 
+            print('not recognize the file type option, ftype -> %s'%options.ftype) 
+            sys.exit() 
+        print(name_out, file_ext)
+        contcar2com(fname, name_out+file_ext,Gaus_out=Gaus_out) 
     
-    elif options.job == 'gaus2poscar': 
+    elif options.job == 'gaus2poscar' or options.job == 'gaus2vasp' :  
         fname = options.fname 
         
-        Warning.file_exist(fname)  
+        Warning.file_not_exist(fname)  
         
         file = open(fname,'r') 
         lines = file.read() 
         if not 'tv' in lines.lower() :
             print('Warning! Periodic cell vectors are not found in file %s' %fname)   
             exit('Add periodic cell in the com file')
         file.close()  
         
-        name_out = os.path.splitext(options.fout)[0] 
+        if options.fout == None: 
+            name_out = os.path.splitext(fname)[0]+'.POSCAR'
+        else: 
+            name_out = options.fout #os.path.splitext(options.fout) 
         
         com2poscar(fname, name_out=name_out, select=options.select, direct = options.direct)  
 
     elif options.job == 'read_bands':
         fname = options.fname 
         nbands = options.bands 
         frames = options.frames
```

