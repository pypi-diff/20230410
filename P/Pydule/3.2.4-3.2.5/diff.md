# Comparing `tmp/Pydule-3.2.4.tar.gz` & `tmp/Pydule-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.2.4.tar", last modified: Mon Apr  3 12:47:12 2023, max compression
+gzip compressed data, was "Pydule-3.2.5.tar", last modified: Mon Apr 10 14:42:46 2023, max compression
```

## Comparing `Pydule-3.2.4.tar` & `Pydule-3.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 12:47:12.280925 Pydule-3.2.4/
--rw-rw-rw-   0        0        0     1994 2023-04-03 12:47:12.280409 Pydule-3.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1216 2023-04-03 12:43:42.000000 Pydule-3.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-03 12:47:12.280925 Pydule-3.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-04-03 12:42:59.000000 Pydule-3.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:47:11.691226 Pydule-3.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-03 12:47:12.272394 Pydule-3.2.4/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     1994 2023-04-03 12:47:11.000000 Pydule-3.2.4/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-03 12:47:11.000000 Pydule-3.2.4/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 12:47:11.000000 Pydule-3.2.4/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-04-03 12:47:11.000000 Pydule-3.2.4/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-03 12:47:11.000000 Pydule-3.2.4/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6784 2023-04-03 12:39:04.000000 Pydule-3.2.4/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:46.017458 Pydule-3.2.5/
+-rw-rw-rw-   0        0        0     2013 2023-04-10 14:42:46.017458 Pydule-3.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1235 2023-04-10 14:40:07.000000 Pydule-3.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:42:46.017458 Pydule-3.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-04-10 14:39:29.000000 Pydule-3.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:45.688574 Pydule-3.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:46.008915 Pydule-3.2.5/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2013 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 14:42:45.000000 Pydule-3.2.5/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7606 2023-04-10 01:54:45.000000 Pydule-3.2.5/src/Pydule.py
```

### Comparing `Pydule-3.2.4/PKG-INFO` & `Pydule-3.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.4
+Version: 3.2.5
 Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -19,14 +19,15 @@
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Text Translation
+- Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
 - Get Hex of a any Color
 - Convert Text to Speech
```

### Comparing `Pydule-3.2.4/README.md` & `Pydule-3.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Text Translation
+- Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
 - Get Hex of a any Color
 - Convert Text to Speech
```

### Comparing `Pydule-3.2.4/setup.py` & `Pydule-3.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.2.4',
+	version='3.2.5',
 	description="Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
```

### Comparing `Pydule-3.2.4/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.2.5/src/Pydule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.4
+Version: 3.2.5
 Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -19,14 +19,15 @@
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Text Translation
+- Edit JSON Files
 - Replace Letters in String
 - Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
 - Get Hex of a any Color
 - Convert Text to Speech
```

### Comparing `Pydule-3.2.4/src/Pydule.py` & `Pydule-3.2.5/src/Pydule.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,46 @@
 
 err='\n \U0000274C Something Went Wrong \U0000274C\n'
 
 def openapp(appname):
 	from AppOpener import open
 	open(appname)
 
+def deljsonele(path):
+	import json
+	jsonfile=json.load(open(path))
+	copy=jsonfile.copy()
+	k=eval(input('Enter the Key : '))
+	del copy[k]
+	with open(path,'w') as json_file:
+		json.dump(copy,json_file)	
+
+def rejson(path):
+	import json
+	jsonfile=json.load(open(path))
+	copy=jsonfile.copy()
+	k=eval(input('Enter the Key : '))
+	v=eval(input('Enter the Value : '))
+	copy[k]=v
+	with open(path,'w') as json_file:
+		json.dump(copy,json_file)
+
+def num(n):
+	if isinstance(n,int):
+		if n==1:
+			n='1st'
+		elif n==2:
+			n='2nd'
+		elif n==3:
+			n='3rd'
+		else:
+			n=str(n)+'th'
+		return n
+	else:
+		print(err)	
 def intuple(x,index,element):
 	if isinstance(x,tuple):
 		new=()
 		if len(x)<=index:
 			new+=x+(element,)
 		else:	
 			for i,j in zip(range(len(x)),x):
@@ -41,15 +73,15 @@
 				else:
 					new+=j
 		return new
 	else:
 		print(err)			
 
 def functions():
-	l=['translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
+	l=['deljsonele(<path>)','rejson(<path>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
 	print('Available Functions : ')
 	for i in l:
 		print(i)
 
 def summatrix(x,y):
 	import numpy as np
 	result = np.array(x) + np.array(y)
@@ -151,42 +183,44 @@
 	else:
 		print(err)	
 
 def clist(mx):
 	List=[]
 	print('Enter Values One by One \U0001F447\n')
 	for i in range(mx):
-		l=eval(input(f'Enter {i+1} Value :'))
+		l=eval(input(f'Enter {num(i+1)} Value :'))
 		List.append(l)
-	print('\nList Created Successfully \U00002714\n')
+	print('\nList Created Successfully \U00002714')
 	return List
 
 def ctuple(mx):
 	Tuple=()
 	print('Enter Values One by One \U0001F447\n')
 	for i in range(mx):
-		t=eval(input(f'Enter {i+1} Value :'))
+		t=eval(input(f'Enter {num(i+1)} Value :'))
 		Tuple+=(t,)
-	print('\nTuple Created Successfully \U00002714\n')
+	print('\nTuple Created Successfully \U00002714')
 	return Tuple
 
 def cdict(mx):
 	Dict={}
+	print('Enter Values One by One \U0001F447\n')
 	for i in range(mx):
-		key=eval(input(f'Enter the Key of No.{i+1} Element :'))
-		value=eval(input(f'Enter the Value of No.{i+1} Element :'))
+		key=eval(input(f'Enter the Key of No.{num(i+1)} Element :'))
+		value=eval(input(f'Enter the Value of No.{num(i+1)} Element :'))
+		print()
 		Dict[key]=value
-	print('\nDictionary Created Successfully \U00002714')	
+	print('Dictionary Created Successfully \U00002714')	
 	return Dict
 
 def cset(mx):
 	Set=set()
 	print('Enter Values One by One \U0001F447\n')
 	for i in range(mx):
-		s=eval(input(f'Enter {i+1} Values : '))
+		s=eval(input(f'Enter {num(i+1)} Values : '))
 		Set.add(s)
 	print('\nSet Created Successfully \U00002714')	
 	return Set
 
 def pickcolor():
 	root=Tk()
 	root.geometry('250x100')
```

