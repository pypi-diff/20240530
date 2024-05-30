# Comparing `tmp/contourplots-0.3.0.tar.gz` & `tmp/contourplots-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contourplots-0.3.0.tar", last modified: Tue May 28 01:41:09 2024, max compression
+gzip compressed data, was "contourplots-0.3.1.tar", last modified: Thu May 30 04:22:42 2024, max compression
```

## Comparing `contourplots-0.3.0.tar` & `contourplots-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 01:41:09.729453 contourplots-0.3.0/
--rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      704 2024-05-28 01:41:09.727484 contourplots-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 01:41:09.717850 contourplots-0.3.0/contourplots/
--rw-rw-rw-   0        0        0      892 2024-05-28 01:35:27.000000 contourplots-0.3.0/contourplots/__init__.py
--rw-rw-rw-   0        0        0    64395 2024-05-15 05:16:55.000000 contourplots-0.3.0/contourplots/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:41:09.726473 contourplots-0.3.0/contourplots.egg-info/
--rw-rw-rw-   0        0        0      704 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-28 01:41:09.000000 contourplots-0.3.0/contourplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 01:41:09.730449 contourplots-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-28 01:35:18.000000 contourplots-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:22:42.937276 contourplots-0.3.1/
+-rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      704 2024-05-30 04:22:42.936278 contourplots-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 04:22:42.927020 contourplots-0.3.1/contourplots/
+-rw-rw-rw-   0        0        0      892 2024-05-30 04:22:20.000000 contourplots-0.3.1/contourplots/__init__.py
+-rw-rw-rw-   0        0        0    65056 2024-05-30 04:06:50.000000 contourplots-0.3.1/contourplots/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:22:42.935254 contourplots-0.3.1/contourplots.egg-info/
+-rw-rw-rw-   0        0        0      704 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 04:22:42.938247 contourplots-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-30 04:20:08.000000 contourplots-0.3.1/setup.py
```

### Comparing `contourplots-0.3.0/LICENSE.txt` & `contourplots-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contourplots-0.3.0/PKG-INFO` & `contourplots-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.3.0
+Version: 0.3.1
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.3.0/contourplots/__init__.py` & `contourplots-0.3.1/contourplots/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ContourPlots: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 # Copyright (C) 2022-2023, Sarang Bhagwat <sarang.bhagwat.git@gmail.com>
 # 
 # This module is under the MIT open-source license. See 
 # https://github.com/sarangbhagwat/contourplots/blob/main/LICENSE
 # for license details.
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 __author__ = 'Sarang S. Bhagwat'
 
 # %% Initialize ContourPlots 
 
 from . import utils
 
 animated_contourplot = utils.animated_contourplot
```

### Comparing `contourplots-0.3.0/contourplots/utils.py` & `contourplots-0.3.1/contourplots/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1179,19 +1179,24 @@
                           save_file=True,
                           filename='box_and_whiskers_plot',
                           dpi=600,
                           fig_width=1.5,
                           fig_height=5.5,
                           box_width=1.5,
                           height_ratios = [1, 20],
-                          
+                          xlabelpad=5,
+                          ylabelpad=5,
+                          xticks_fontsize = 17,
+                          ylabel_fontsize = 19,
+                          yticks_fontsize = 17,
+                          default_fontsize = 15,
                           ):
     n_boxes = 1. if not hasattr(uncertainty_data[0], '__iter__') else len(uncertainty_data)
     plt.rcParams['font.sans-serif'] = "Arial Unicode"
-    plt.rcParams['font.size'] = "14"
+    plt.rcParams['font.size'] = str(default_fontsize)
 
     gridspec_kw={'height_ratios': height_ratios,},
 
     fig, axs = plt.subplots(1, 1, constrained_layout=True, 
                             # gridspec_kw=gridspec_kw,
                             )
     ax = axs
@@ -1232,15 +1237,15 @@
 
     if not (ranges_for_comparison==() or ranges_for_comparison==[] or ranges_for_comparison==None):
         for i in range(len(ranges_for_comparison)):
             range_for_comparison, range_for_comparison_color = ranges_for_comparison[i], ranges_for_comparison_colors[i]
             ax.fill_between(list(range(0, n_boxes+2)), [range_for_comparison[0]], [range_for_comparison[1]], color=range_for_comparison_color, alpha=1., zorder=1)
 
     if not (values_for_comparison==() or values_for_comparison==[] or values_for_comparison==None):
-        1
+        1 # not implemented
     
     ax.yaxis.set_minor_locator(AutoMinorLocator(n_minor_ticks+1))
     
     if not show_x_ticks:
         ax.tick_params(
             axis='x',          # changes apply to the x-axis
             which='both',      # both major and minor ticks are affected
@@ -1255,24 +1260,25 @@
             top=False,         # ticks along the top edge are off
             direction='inout',
             length=5,
             width=1,
             labelbottom=False if x_tick_labels is None else True)
     
     if show_x_ticks and (x_tick_labels is not None):
-        ax.set_xticks(ticks=list(range(1,n_boxes+1)), labels=x_tick_labels,)
+        ax.set_xticks(ticks=list(range(1,n_boxes+1)), labels=x_tick_labels, fontsize=xticks_fontsize)
         wrap_labels(ax, width=x_tick_wrap_width, fontsize=x_tick_fontsize)
     
 
     ax.tick_params(
         axis='y',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction='inout',
         # right=True,
         width=1,
+        labelsize=yticks_fontsize,
         )
 
     ax.tick_params(
         axis='y',          
         which='major',      
         length=5,
         )
@@ -1320,20 +1326,24 @@
     ax2.tick_params(
         axis='y',          
         which='both',      
         direction='in',
         # right=True,
         labelright=False,
         width=1,
+        labelsize=yticks_fontsize,
         )
     
     ax.set_ylabel(y_label + " [" + y_units + "]", 
-                  {'fontname':'Arial Unicode'}, fontsize=14, 
+                  {'fontname':'Arial Unicode'}, fontsize=ylabel_fontsize, 
+                  labelpad=ylabelpad,
                # fontweight='bold',
                )
+    ax.xaxis.labelpad = xlabelpad
+    ax.tick_params(axis='x', which='major', pad=xlabelpad)
     
     # ax.set_ylim(min(y_ticks), max(y_ticks))
 
 
 
     plt.savefig(filename+'.png', dpi=dpi)
 
@@ -1353,14 +1363,16 @@
                        fig_width=7,
                        fig_height=5.5*1.1777,
                        show_totals=False,
                        totals=[],
                        sig_figs_for_totals=3,
                        units_list=[],
                        totals_label_text=r"$\bfsum:$",
+                       xlabelpad=5,
+                       ylabelpad=5,
                        ):
     
     plt.rcParams['font.sans-serif'] = "Arial Unicode"
     plt.rcParams['font.size'] = "14"
     
     ax = dataframe.T.plot(kind='bar', stacked=True, edgecolor='k', linewidth=linewidth,
                           color=colors,
@@ -1425,15 +1437,17 @@
                 if bar_hatch_dict[bar_num] is not None:
                     if curr_facecolor in used_facecolors:
                         patch.set_hatch(bar_hatch_dict[bar_num])
         bar_num+=1
     # print(bar_hatch_dict)
     ax.legend(bbox_to_anchor=(1.05, 1.0), loc='upper left', edgecolor='white')
 
-    ax.set_ylabel(y_label + " [" + y_units + "]", fontsize=14)
+    ax.set_ylabel(y_label + " [" + y_units + "]", fontsize=14, labelpad=ylabelpad)
+    
+    ax.xaxis.labelpad=xlabelpad
     
     # ax.set_xlabel(x_labels, fontsize=14)
     
     wrap_labels(ax,10)
     
     ax.axhline(y=0,  color='k', linestyle='-', linewidth=linewidth)
```

### Comparing `contourplots-0.3.0/contourplots.egg-info/PKG-INFO` & `contourplots-0.3.1/contourplots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.3.0
+Version: 0.3.1
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.3.0/setup.py` & `contourplots-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from setuptools import setup
 
 setup(
     name='contourplots',
     packages=['contourplots'],
-    version='0.3.0',    
+    version='0.3.1',    
     description='A toolkit for generating multi-dimensional plots easily, usefully, and legibly.',
     url='https://github.com/sarangbhagwat/contourplots',
     author='Sarang S. Bhagwat',
     author_email='sarang.bhagwat.git@gmail.com',
     license='MIT',
     # packages=['contourplots'],
     install_requires=['matplotlib==3.5.2',
```

