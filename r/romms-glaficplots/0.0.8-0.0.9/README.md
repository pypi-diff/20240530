# Comparing `tmp/romms_glaficplots-0.0.8.tar.gz` & `tmp/romms_glaficplots-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romms_glaficplots-0.0.8.tar", last modified: Tue Apr 16 19:14:03 2024, max compression
+gzip compressed data, was "romms_glaficplots-0.0.9.tar", last modified: Tue Apr 16 20:51:35 2024, max compression
```

## Comparing `romms_glaficplots-0.0.8.tar` & `romms_glaficplots-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 19:14:03.442904 romms_glaficplots-0.0.8/
--rw-r--r--   0 ainsleylewis   (501) staff       (20)     1074 2024-03-10 06:10:18.000000 romms_glaficplots-0.0.8/LICENSE.md
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-04-16 19:14:03.442679 romms_glaficplots-0.0.8/PKG-INFO
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      708 2024-04-16 19:12:58.000000 romms_glaficplots-0.0.8/README.md
-drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 19:14:03.441400 romms_glaficplots-0.0.8/romms_glaficplots/
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       64 2024-03-10 07:57:51.000000 romms_glaficplots-0.0.8/romms_glaficplots/__init__.py
--rw-r--r--   0 ainsleylewis   (501) staff       (20)     6170 2024-04-16 19:13:04.000000 romms_glaficplots-0.0.8/romms_glaficplots/plots.py
-drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 19:14:03.442454 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/PKG-INFO
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      290 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/SOURCES.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)        1 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/dependency_links.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       32 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/requires.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       18 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/top_level.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       38 2024-04-16 19:14:03.442952 romms_glaficplots-0.0.8/setup.cfg
--rw-r--r--   0 ainsleylewis   (501) staff       (20)     1121 2024-04-16 19:14:00.000000 romms_glaficplots-0.0.8/setup.py
+drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 20:51:35.913491 romms_glaficplots-0.0.9/
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)     1074 2024-03-10 06:10:18.000000 romms_glaficplots-0.0.9/LICENSE.md
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-04-16 20:51:35.913286 romms_glaficplots-0.0.9/PKG-INFO
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      708 2024-04-16 19:12:58.000000 romms_glaficplots-0.0.9/README.md
+drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 20:51:35.912268 romms_glaficplots-0.0.9/romms_glaficplots/
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       64 2024-03-10 07:57:51.000000 romms_glaficplots-0.0.9/romms_glaficplots/__init__.py
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)     6120 2024-04-16 20:51:26.000000 romms_glaficplots-0.0.9/romms_glaficplots/plots.py
+drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 20:51:35.913076 romms_glaficplots-0.0.9/romms_glaficplots.egg-info/
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-04-16 20:51:35.000000 romms_glaficplots-0.0.9/romms_glaficplots.egg-info/PKG-INFO
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      290 2024-04-16 20:51:35.000000 romms_glaficplots-0.0.9/romms_glaficplots.egg-info/SOURCES.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)        1 2024-04-16 20:51:35.000000 romms_glaficplots-0.0.9/romms_glaficplots.egg-info/dependency_links.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       32 2024-04-16 20:51:35.000000 romms_glaficplots-0.0.9/romms_glaficplots.egg-info/requires.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       18 2024-04-16 20:51:35.000000 romms_glaficplots-0.0.9/romms_glaficplots.egg-info/top_level.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       38 2024-04-16 20:51:35.913534 romms_glaficplots-0.0.9/setup.cfg
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)     1121 2024-04-16 20:51:24.000000 romms_glaficplots-0.0.9/setup.py
```

### Comparing `romms_glaficplots-0.0.8/LICENSE.md` & `romms_glaficplots-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `romms_glaficplots-0.0.8/PKG-INFO` & `romms_glaficplots-0.0.9/romms_glaficplots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: romms_glaficplots
-Version: 0.0.8
+Name: romms-glaficplots
+Version: 0.0.9
 Summary: A python package to make basic plots (errors and critical curves) for glafic
 Home-page: https://github.com/romms921/romms_glaficplots.git
 Author: Rommulus Lewis
 Author-email: rommuluslewis@gmail.com
 License: BSD 2-clause
 Keywords: astronomy,astrophysics,gravitationallensing,lensing,glafic
 Classifier: Development Status :: 1 - Planning
```

### Comparing `romms_glaficplots-0.0.8/README.md` & `romms_glaficplots-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `romms_glaficplots-0.0.8/romms_glaficplots/plots.py` & `romms_glaficplots-0.0.9/romms_glaficplots/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     x = np.arange(4)
     width = 0.3
 
     # Plotting Flux Error Graph
     plt.figure(figsize =(8,6))
     plt.bar(x-0.15, data_df[2], width, color='cyan', edgecolor ='k') 
     plt.bar(x+0.15, df_pred[3], width, color='red', edgecolor='k') 
-    plt.errorbar(x-0.15, data_df[2], yerr=data_df[4], fmt='o', color='black', capsize=4, label='1 σ Error')
     plt.errorbar(x-0.15, data_df[2], yerr=3*np.array(data_df[4]), fmt='o', color='black', capsize=4, label='3 σ Error')
     plt.xticks(x, data_df['Label']) 
     plt.xlabel("Image") 
     plt.ylabel("Flux Ratio") 
     plt.legend(labels=['Observed Flux Ratio', 'Predicted Flux Ratio', '3 σ Error'])
     plt.title(plot_name + ' Flux Ratio Error')
     plt.show() 
@@ -167,26 +166,26 @@
         
     de = de.drop(columns =[3])
 
     labels = ['A', 'B', 'C', 'D']
 
     # Plotting Critial Curves
     plt.figure(figsize=(8, 8))
-    plt.scatter(df[0]*100, df[1]*100, s=2)
-    plt.scatter(df[2]*100, df[3]*100, s=2)
-    plt.scatter(df[4]*100, df[5]*100, s=2)
-    plt.scatter(df[6]*100, df[7]*100, s=2)
+    plt.scatter(df[0]*100, df[1]*100, s=4)
+    plt.scatter(df[2]*100, df[3]*100, s=4)
+    plt.scatter(df[4]*100, df[5]*100, s=4)
+    plt.scatter(df[6]*100, df[7]*100, s=4)
 
     # Plotting obs image positions and labels 
-    plt.scatter(data_df[0]*100, data_df[1]*100, s=20)
-    plt.scatter(de[0]*100, de[1]*100, s = 180, marker= '+', label = 'Predicted Position')
+    plt.scatter(data_df[0]*100, data_df[1]*100, s=15, color = 'blue', label = 'Observed Position')
+    plt.scatter(de[0]*100, de[1]*100, s = 180, marker= '+', label = 'Predicted Position', color = 'orange')
     for x, y, txt in zip(data_df[0]*100, data_df[1]*100, labels):
         plt.text(x, y-17, txt, fontsize=13, ha='center', va='bottom')
 
     plt.title(plot_name + ' Critical Curves')
     plt.xlabel('x [pixel]')
     plt.ylabel('y [pixel]')
     plt.xlim(-170,170)
     plt.ylim(-170,170)
     plt.show()
     
-    return data_df, df, de
+    return data_df, df
```

### Comparing `romms_glaficplots-0.0.8/romms_glaficplots.egg-info/PKG-INFO` & `romms_glaficplots-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: romms-glaficplots
-Version: 0.0.8
+Name: romms_glaficplots
+Version: 0.0.9
 Summary: A python package to make basic plots (errors and critical curves) for glafic
 Home-page: https://github.com/romms921/romms_glaficplots.git
 Author: Rommulus Lewis
 Author-email: rommuluslewis@gmail.com
 License: BSD 2-clause
 Keywords: astronomy,astrophysics,gravitationallensing,lensing,glafic
 Classifier: Development Status :: 1 - Planning
```

### Comparing `romms_glaficplots-0.0.8/setup.py` & `romms_glaficplots-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='romms_glaficplots',
-    version='0.0.8',    
+    version='0.0.9',    
     description='A python package to make basic plots (errors and critical curves) for glafic',
     url='https://github.com/romms921/romms_glaficplots.git',
     author='Rommulus Lewis',
     author_email='rommuluslewis@gmail.com',
     license='BSD 2-clause',
     keywords=['astronomy','astrophysics','gravitationallensing', 'lensing', 'glafic'], 
     packages=['romms_glaficplots'],
```

