# Comparing `tmp/pyclpu-1.1.9.tar.gz` & `tmp/pyclpu-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclpu-1.1.9.tar", last modified: Thu Feb 15 14:06:48 2024, max compression
+gzip compressed data, was "pyclpu-1.2.0.tar", last modified: Thu May 30 09:08:39 2024, max compression
```

## Comparing `pyclpu-1.1.9.tar` & `pyclpu-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 14:06:48.105624 pyclpu-1.1.9/
--rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     8330 2024-02-15 14:06:48.105624 pyclpu-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     7922 2024-02-15 13:58:58.000000 pyclpu-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-02-15 14:06:48.087308 pyclpu-1.1.9/pyclpu/
--rw-rw-rw-   0        0        0      629 2024-02-15 13:59:58.000000 pyclpu-1.1.9/pyclpu/__init__.py
--rw-rw-rw-   0        0        0     1974 2024-02-15 14:03:10.000000 pyclpu-1.1.9/pyclpu/constants.py
--rw-rw-rw-   0        0        0     1083 2024-02-15 14:02:58.000000 pyclpu-1.1.9/pyclpu/formats.py
--rw-rw-rw-   0        0        0    30604 2024-02-15 07:27:48.000000 pyclpu-1.1.9/pyclpu/image.py
--rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.1.9/pyclpu/main.py
--rw-rw-rw-   0        0        0    26126 2024-01-24 13:37:38.000000 pyclpu-1.1.9/pyclpu/manager.py
--rw-rw-rw-   0        0        0    43140 2024-02-13 14:04:20.000000 pyclpu-1.1.9/pyclpu/metrology.py
--rw-rw-rw-   0        0        0     7422 2024-02-14 11:26:25.000000 pyclpu-1.1.9/pyclpu/s33293804.py
--rw-rw-rw-   0        0        0    25476 2024-02-13 14:04:20.000000 pyclpu-1.1.9/pyclpu/waveform.py
-drwxrwxrwx   0        0        0        0 2024-02-15 14:06:48.105308 pyclpu-1.1.9/pyclpu.egg-info/
--rw-rw-rw-   0        0        0     8330 2024-02-15 14:06:47.000000 pyclpu-1.1.9/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-02-15 14:06:47.000000 pyclpu-1.1.9/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 14:06:47.000000 pyclpu-1.1.9/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-02-15 14:06:47.000000 pyclpu-1.1.9/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-15 14:06:47.000000 pyclpu-1.1.9/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2024-02-15 14:06:48.107690 pyclpu-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     2453 2024-01-24 11:20:09.000000 pyclpu-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:08:39.345964 pyclpu-1.2.0/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6189 2024-05-30 09:08:39.346969 pyclpu-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5781 2024-05-30 09:03:09.000000 pyclpu-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 09:08:39.338416 pyclpu-1.2.0/pyclpu/
+-rw-rw-rw-   0        0        0      629 2024-05-30 09:04:11.000000 pyclpu-1.2.0/pyclpu/__init__.py
+-rw-rw-rw-   0        0        0     1974 2024-02-15 14:08:11.000000 pyclpu-1.2.0/pyclpu/constants.py
+-rw-rw-rw-   0        0        0     1083 2024-02-15 14:08:11.000000 pyclpu-1.2.0/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    30604 2024-02-15 14:08:11.000000 pyclpu-1.2.0/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.2.0/pyclpu/main.py
+-rw-rw-rw-   0        0        0    34883 2024-05-30 08:54:25.000000 pyclpu-1.2.0/pyclpu/manager.py
+-rw-rw-rw-   0        0        0    43183 2024-02-16 07:52:17.000000 pyclpu-1.2.0/pyclpu/metrology.py
+-rw-rw-rw-   0        0        0     7422 2024-02-15 14:08:11.000000 pyclpu-1.2.0/pyclpu/s33293804.py
+-rw-rw-rw-   0        0        0    25476 2024-02-13 14:04:20.000000 pyclpu-1.2.0/pyclpu/waveform.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:08:39.345576 pyclpu-1.2.0/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0     6189 2024-05-30 09:08:39.000000 pyclpu-1.2.0/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-30 09:08:39.000000 pyclpu-1.2.0/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:08:39.000000 pyclpu-1.2.0/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-30 09:08:39.000000 pyclpu-1.2.0/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 09:08:39.000000 pyclpu-1.2.0/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2024-05-30 09:08:39.347681 pyclpu-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2468 2024-05-21 15:25:19.000000 pyclpu-1.2.0/setup.py
```

### Comparing `pyclpu-1.1.9/LICENSE` & `pyclpu-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.9/PKG-INFO` & `pyclpu-1.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.1.9
+Version: 1.2.0
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -196,42 +196,9 @@
 channel = 1
 trace = waveform.Waveform(wfm = wfm, channel = channel)
 
 trace.show()
 trace.save("C:\\bin\\output.csv")
 ```
 
-## Scripts in Modules
-
-:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format. :warning: **But relative links work only on GitLab / GitHub, not on PYPI.**
-
-## Developper's Guide
-
-To get started, clone the project into your working directory `git clone https://git.clpu.es/mehret/pyclpu` and hop inside `cd pyclpu`. Create the anaconda environment in Anaconda based on the `clpu.yml` file delivered in the main folder of the project, e.g. in the Anaconda prompt with `conda env create -f clpu.yml` and activate it with `conda activate clpu`.
-
-### Integration and Testing
-
-Install actualized versions from the main folder with `pip install .`.
-
-### Export
-
-Before exporting a new version of the module
-
-- increase the version counters in `pyclpu\__init__.py`,
-- update the `.yml`file if needed via `conda env export --from-history > clpu.yml`,
-- update the documentation via `pdoc --html pyclpu --force && pdoc --template-dir="." -o md pyclpu --force && python text.mako.py`.
-
-Export with `python setup.py sdist` to `dist/`. Then to upload all distributions created under `dist/` execute `twine upload dist/*`or to upload the source distribution with a gpg signature `twine upload dist/pyexample-0.1.0.tar.gz pyexample-0.1.0.tar.gz.asc`. Now the distribution is updated in pyPIP. For the Anaconda version, now,
-
-Note that double factor authentification is mandated on pyPIP, therefore a `.pypirc` file should be stored in your home directory that contains
-```
-[pypi]
-username = __token__
-password = pypi-AgEIcHlwaS5vcmcCJDZkZjMxODk1LTdlNzktNDIzMC1hYjJiLWVkYzVjYmE4Nzk4NwACDlsxLFsicHljbHB1Il1dAAIsWzIsWyI5MTU2MmNiMi05MzM2LTRlYjQtODAxMi04NTVhYWQ0NzA4ZGMiXV0AAAYgaKpKjrh8Ftj4yH-```
-
-(append `63z45A5wEe4WP78SioJJMpgsHc3Q` to the end of the password string in case of error) - update the Anaconda recipe via `grayskull pypi --strict-conda-forge pyCLPU`,
-- ...
-
-Close the procedure orderly:
-- git-commit the code into the developper's branch `dev` with a note on the new version number,
-- git-merge the developper's branch into the main branch `master`.
-
+## Changelog
+...
```

### Comparing `pyclpu-1.1.9/README.md` & `pyclpu-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -182,42 +182,9 @@
 channel = 1
 trace = waveform.Waveform(wfm = wfm, channel = channel)
 
 trace.show()
 trace.save("C:\\bin\\output.csv")
 ```
 
-## Scripts in Modules
-
-:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format. :warning: **But relative links work only on GitLab / GitHub, not on PYPI.**
-
-## Developper's Guide
-
-To get started, clone the project into your working directory `git clone https://git.clpu.es/mehret/pyclpu` and hop inside `cd pyclpu`. Create the anaconda environment in Anaconda based on the `clpu.yml` file delivered in the main folder of the project, e.g. in the Anaconda prompt with `conda env create -f clpu.yml` and activate it with `conda activate clpu`.
-
-### Integration and Testing
-
-Install actualized versions from the main folder with `pip install .`.
-
-### Export
-
-Before exporting a new version of the module
-
-- increase the version counters in `pyclpu\__init__.py`,
-- update the `.yml`file if needed via `conda env export --from-history > clpu.yml`,
-- update the documentation via `pdoc --html pyclpu --force && pdoc --template-dir="." -o md pyclpu --force && python text.mako.py`.
-
-Export with `python setup.py sdist` to `dist/`. Then to upload all distributions created under `dist/` execute `twine upload dist/*`or to upload the source distribution with a gpg signature `twine upload dist/pyexample-0.1.0.tar.gz pyexample-0.1.0.tar.gz.asc`. Now the distribution is updated in pyPIP. For the Anaconda version, now,
-
-Note that double factor authentification is mandated on pyPIP, therefore a `.pypirc` file should be stored in your home directory that contains
-```
-[pypi]
-username = __token__
-password = pypi-AgEIcHlwaS5vcmcCJDZkZjMxODk1LTdlNzktNDIzMC1hYjJiLWVkYzVjYmE4Nzk4NwACDlsxLFsicHljbHB1Il1dAAIsWzIsWyI5MTU2MmNiMi05MzM2LTRlYjQtODAxMi04NTVhYWQ0NzA4ZGMiXV0AAAYgaKpKjrh8Ftj4yH-```
-
-(append `63z45A5wEe4WP78SioJJMpgsHc3Q` to the end of the password string in case of error) - update the Anaconda recipe via `grayskull pypi --strict-conda-forge pyCLPU`,
-- ...
-
-Close the procedure orderly:
-- git-commit the code into the developper's branch `dev` with a note on the new version number,
-- git-merge the developper's branch into the main branch `master`.
-
+## Changelog
+...
```

### Comparing `pyclpu-1.1.9/pyclpu/__init__.py` & `pyclpu-1.2.0/pyclpu/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "1.1.9"
+__version__ = "1.2.0"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-1.1.9/pyclpu/constants.py` & `pyclpu-1.2.0/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.9/pyclpu/formats.py` & `pyclpu-1.2.0/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.9/pyclpu/image.py` & `pyclpu-1.2.0/pyclpu/image.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.9/pyclpu/main.py` & `pyclpu-1.2.0/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.9/pyclpu/manager.py` & `pyclpu-1.2.0/pyclpu/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -609,14 +609,201 @@
         try:
             del self.ident
             del self._event
             del self._process
         except:
             pass
         return None
+        
+# CODE PARSER FOR SIMULATION INPUT/OUTPUT/TRANSLATION/PIPELINES
+class ChoCoLaT_output():
+    """
+    The class allows to load output of a ChoCoLaT simulation into a class object.
+    
+    Args:
+        source  (string, optional) : Source output file.
+        
+    Attributes:
+        status (bool) : True if processing was successfull, else False.
+            Initializes to False.
+        flag_new (bool) : True if processing was successfull, else False.
+            Initializes to False.
+            Intended to be modified from outside in use cases where this routine delivers output for another process.
+    
+    Returns:
+        meta  (dictionary)   : Simulation input parameters and meta information.
+        data  (record array) : Simulation output in named columns of a record array (allows to see `array.keys`).
+        
+    Note:
+        This parser refers to ChoCoLaT version 2 and younger.
+    
+    Examples:
+        The class can be used in a functional way
+
+        ```python 
+        from pyclpu import manager
+        choc = manager.ChoCoLaT_output(source = "path/to/test.dat")
+        ```
+
+        A more object oriented use case can deal with loops
+
+        ```python 
+        from pyclpu import manager
+        choc_it = manager.ChoCoLaT_output()
+        chocs = []
+        
+        simulations = ["1.dat","2.dat","3.dat"]
+        for choc in image_stack:
+            choc_it.source = choc
+            chocs.append[{choc_it.meta["metal_id"] : choc_it.data["Q_[nC]"][-1]}]
+        ```
+        with selected results beeing stored in a list `chocs`.
+    """
+    # INI
+    def __new__(cls, *args, **kwargs):
+        return super().__new__(cls)
+    def __init__(self, *args, **kwargs):
+        self.__dict__.update(kwargs)
+        self.status = False
+        self.flag_new = False
+        # INTEGRITY
+        if not hasattr(self, 'source'):
+            warning(self.__class__.__name__,"No source path defined, expect key `source` as `source=path.dat`.")
+        # IN PLACE
+        if hasattr(self, 'source'):
+            self.__run__()
+        return None
+    def __setattr__(self, name, value):
+        super().__setattr__(name, value)
+        if name == "source":
+            self.__run__()
+        return None
+    def __run__(self):
+        self.status = False
+        # METHODS
+        def load(path):
+            """
+            Loads the file with simulation results into an line-by-line array
+            """
+            # check if file exists
+            if not os.path.isfile(path):
+                warning(self.__class__.__name__,"Invalid source path, expect key `source` as `source=path.dat`.")
+                return None
+            # open file
+            with open(path) as file:
+                # check if file is empty
+                file.seek(0, os.SEEK_END) # go to end of file
+                if file.tell():           # if current position is truish (i.e != 0)
+                    file.seek(0)          # rewind the file for later use 
+                else:
+                    warning(self.__class__.__name__,"Invalid source, file is empty.")
+                    return None           # file is empty
+                # parse file line by line into array
+                line_by_line = [line.rstrip() for line in file]
+            return line_by_line   
+        def find_sim_meta(line_by_line):
+            """
+            Filters the input information to the simulation and meta information from the simulation file array.
+            """
+            # prepare dictionary for file header information (meta and simulation input)
+            meta_dict = {}
+            # ChoCoLaT marks meta information about the simulation with "%",
+            #  and meta information is always in the header od the output file.
+            for line in line_by_line:
+                if "%" in line:
+                    # clean strings
+                    keyed = line.replace("%","").split("=")
+                    key   = keyed[0].strip()
+                    value = keyed[1].strip()
+                    # try to sort out for type
+                    if key == "T_isol":
+                        value = bool(value)
+                    elif key in ["metal", "Nb Th", "diag s", "diag f", "N_iks", "Nb"] : 
+                        value = int(value)
+                    elif key in ["dt", "t_laser", "E_laser", "C_abs", "w_laser", "d_laser", "d_targe", "e_targe", "T_hot_e", "N_tot", "t_life"] : 
+                        value = float(value)
+                    else:
+                        warning(self.__class__.__name__,"Unknown key in header ! `" + key +"` as `" + key +" = " + value +"`.")
+                    # add to dict
+                    meta_dict[key] = value
+                else:
+                    break
+            return meta_dict
+        def wumwum_parse_data(line_by_line):
+            """
+            Filters the data from the output file.
+            """
+            # prepare column header tuple
+            header = ()
+            # prepare data array (will have every output line in one tuple)
+            rows   = []
+            # find column header, located directly after the file header
+            for line in line_by_line:
+                if "%" in line:
+                    continue
+                else:
+                    # column headers are separated by differing amounts of white spaces
+                    words = line.split()
+                    # nearly all column headers have units, always first comes the keyword and after the unit
+                    keys_units  = {}
+                    last_key_poition = 0
+                    for p,phrase in enumerate(words):
+                        # separate keywords and units based on the feature that units are in brackets
+                        if "[" not in phrase and "]" not in phrase:
+                            # one known header includes the keyword `all` and has no units
+                            if last_key_poition == p-1 and "all" not in words[last_key_poition]:
+                                keys_units.pop(words[last_key_poition], None)
+                                keys_units[words[last_key_poition] + "_" + phrase] = None
+                                last_key = words[last_key_poition] + "_" + phrase
+                            else: 
+                                keys_units[phrase] = None
+                                last_key = phrase
+                            # update position of last keyword in array words
+                            last_key_poition = p
+                        else:
+                            # react to type missmatch that produces an off char in from of the unit um
+                            if "Â" in phrase :
+                                unit = phrase.replace("Â","")
+                            else:
+                                unit = phrase
+                            keys_units[last_key] = unit
+                    # combine keys and units to header entry for data columns
+                    for key in keys_units.keys():
+                        if keys_units[key] is not None:
+                            header = header + (key + "_" + keys_units[key],)
+                        else:
+                            header = header + (key,)
+                    break
+            # read out data underneath column header information
+            for line in line_by_line:
+                if "%" in line or key in line:
+                    continue
+                else:
+                    # data is separated by a variable amount of white spaces
+                    data_row = np.array(line.split()).astype(float)
+                    # check if the header and the data are consistent
+                    if data_row.size != len(header):
+                        warning(self.__class__.__name__,"Header and row have different length ! "+str(data_row.size)+" != "+str(len(header)))
+                    # fill data into data array of tuples
+                    rows.append(tuple(data_row))
+            # build 32bit float dtype from keys
+            dtype_info = [(key,'f4') for key in header]
+            # build record array
+            return np.array(rows, dtype=dtype_info)
+        # MAIN
+        # load file to file array
+        input_array = load(self.source)
+        # extract simulation input information from file array header information
+        self.meta   = find_sim_meta(input_array)
+        # extract timesteps
+        self.data   = wumwum_parse_data(input_array)
+        # housekeeping
+        self.status = True
+        self.flag_new = True
+        return None
     
 # =============================================================================
 # PYTHON MAIN
 # =============================================================================
 # SELF AND TEST
 if globals()["__name__"] == '__main__':
     # STARTUP
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyclpu-1.1.9/pyclpu/metrology.py` & `pyclpu-1.2.0/pyclpu/metrology.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         The default trace width is assumed to be 5 pixels. There is currently no build in option to change this.
         
     Examples:
         The class can be used in a functional way
 
         ```python 
         from pyclpu import metrology
-        TP = metrology.ThomsonParabola(source_directory = "C:\\bin", source_files = ["shot_426.tiff"])
+        TP = metrology.ThomsonParabola(source_directory = 'C:\\bin', source_files = ['shot_426.tiff'])
         ```
 
         A more object oriented use case demonstrates how a run can be started after initialization
 
         ```python
         import cv2
         from pyclpu import metrology
@@ -114,20 +114,20 @@
         
         The following example shows how the results from a single analysis can be saved.
         
         ```python
         import os
         from pyclpu import manager
         
-        output_dir = "C:\\bin"
+        output_dir = 'C:\\bin'
 
-        outA = os.path.join(output_dir, "A_no-X")
-        outB = os.path.join(output_dir, "B_row-by-row-maxs")
-        outC = os.path.join(output_dir, "C_trace")
-        outD = os.path.join(output_dir, "D_superposition")
+        outA = os.path.join(output_dir, 'A_no-X')
+        outB = os.path.join(output_dir, 'B_row-by-row-maxs')
+        outC = os.path.join(output_dir, 'C_trace')
+        outD = os.path.join(output_dir, 'D_superposition')
 
         if not os.path.exists(outA):
             os.makedirs(outA)
         if not os.path.exists(outB):
             os.makedirs(outB)
         if not os.path.exists(outC):
             os.makedirs(outC)    
@@ -137,30 +137,30 @@
         if TP.status:
             cv2.imwrite(os.path.join(outA, TP.filename), TP.Xfiltered)
             cv2.imwrite(os.path.join(outB, TP.filename), TP.rowmaxs)
             cv2.imwrite(os.path.join(outC, TP.filename), TP.trace)
             cv2.imwrite(os.path.join(outD, TP.filename), TP.superposition)
             for n in range(len(TP.trace_array)):
                 # coordinates
-                with open(os.path.join(outC,manager.strip_extension(TP.filename) + "_trace_" + str(n) + ".csv"),"w") as f:
-                    f.write("X/[pix], Y/[pix], COUNT\n")
+                with open(os.path.join(outC,manager.strip_extension(TP.filename) + '_trace_' + str(n) + '.csv'),'w') as f:
+                    f.write('X/[pix], Y/[pix], COUNT\n')
                     for line in TP.trace_array[n]:
-                        f.write(", ".join(map(str,line))+"\n")
+                        f.write(', '.join(map(str,line))+'\n')
                 # spectrum
                 if hasattr(TP, 'trace_array_energy'):
-                    with open(os.path.join(outC,manager.strip_extension(TP.filename) + "_spectrum_" + str(n) + ".csv"),"w") as f:
-                        f.write("E/[MeV], COUNT*dx/dE\n")
+                    with open(os.path.join(outC,manager.strip_extension(TP.filename) + '_spectrum_' + str(n) + '.csv'),'w') as f:
+                        f.write('E/[MeV], COUNT*dx/dE\n')
                         for line in TP.trace_array_energy[n]:
-                            f.write(", ".join(map(str,line))+"\n")
+                            f.write(', '.join(map(str,line))+'\n')
                     array = np.array(TP.trace_array_energy[n])
                     plt.plot(array[:,0],array[:,1])
-                    plt.xlabel("Energy / [MeV]")
-                    plt.ylabel("Number-density / [arb.u./MeV]")
-                    plt.savefig(os.path.join(outC,manager.strip_extension(TP.filename) + "_spectrum_" + str(n) + ".png"),dpi=300)
-                    plt.close("all")
+                    plt.xlabel('Energy / [MeV]')
+                    plt.ylabel('Number-density / [arb.u./MeV]')
+                    plt.savefig(os.path.join(outC,manager.strip_extension(TP.filename) + '_spectrum_' + str(n) + '.png'),dpi=300)
+                    plt.close('all')
         ```
         
         It is also possible to analyse a batch of data in a loop.
         
         ```python
         import os
         import cv2
@@ -169,25 +169,25 @@
         from pyclpu import metrology
         from pyclpu import manager
 
         TP = metrology.ThomsonParabola()
 
         TP.X_ray_spot = (1081,1108)
         TP.pixel_per_space = 14875. # with unit of space: [m]
-        TP.dispersion_relation = "C:\\bin\\dispersion_relation.dat"
+        TP.dispersion_relation = 'C:\\bin\\dispersion_relation.dat'
 
-        TP.source_directory = "C:\\bin"
+        TP.source_directory = 'C:\\bin'
 
         output_trace_numbers = [0] # only protons, which are presumably the 1st trace
 
-        output_dir = "C:\\bin"
-        outA = os.path.join(output_dir, "A_no-X")
-        outB = os.path.join(output_dir, "B_row-by-row-maxs")
-        outC = os.path.join(output_dir, "C_trace")
-        outD = os.path.join(output_dir, "D_superposition")
+        output_dir = 'C:\\bin'
+        outA = os.path.join(output_dir, 'A_no-X')
+        outB = os.path.join(output_dir, 'B_row-by-row-maxs')
+        outC = os.path.join(output_dir, 'C_trace')
+        outD = os.path.join(output_dir, 'D_superposition')
         if not os.path.exists(outA):
             os.makedirs(outA)
         if not os.path.exists(outB):
             os.makedirs(outB)
         if not os.path.exists(outC):
             os.makedirs(outC)    
         if not os.path.exists(outD):
@@ -202,30 +202,30 @@
                     cv2.imwrite(os.path.join(outA, TP.filename), TP.Xfiltered)
                     cv2.imwrite(os.path.join(outB, TP.filename), TP.rowmaxs)
                     cv2.imwrite(os.path.join(outC, TP.filename), TP.trace)
                     cv2.imwrite(os.path.join(outD, TP.filename), TP.superposition)
                     for n in range(len(TP.trace_array)):
                         if n in output_trace_numbers:
                             # coordinates
-                            with open(os.path.join(outC,manager.strip_extension(TP.filename) + "_trace_" + str(n) + ".csv"),"w") as f:
-                                f.write("X/[pix], Y/[pix], COUNT\n")
+                            with open(os.path.join(outC,manager.strip_extension(TP.filename) + '_trace_' + str(n) + '.csv'),'w') as f:
+                                f.write('X/[pix], Y/[pix], COUNT\n')
                                 for line in TP.trace_array[n]:
-                                    f.write(", ".join(map(str,line))+"\n")
+                                    f.write(', '.join(map(str,line))+'\n')
                             # spectrum
                             if hasattr(TP, 'trace_array_energy'):
-                                with open(os.path.join(outC,manager.strip_extension(TP.filename) + "_spectrum_" + str(n) + ".csv"),"w") as f:
-                                    f.write("E/[MeV], COUNT*dx/dE\n")
+                                with open(os.path.join(outC,manager.strip_extension(TP.filename) + '_spectrum_' + str(n) + '.csv'),'w') as f:
+                                    f.write('E/[MeV], COUNT*dx/dE\n')
                                     for line in TP.trace_array_energy[n]:
-                                        f.write(", ".join(map(str,line))+"\n")
+                                        f.write(', '.join(map(str,line))+'\n')
                                 array = np.array(TP.trace_array_energy[n])
                                 plt.plot(array[:,0],array[:,1])
-                                plt.xlabel("Energy / [MeV]")
-                                plt.ylabel("Number-density / [arb.u./MeV]")
-                                plt.savefig(os.path.join(outC,manager.strip_extension(TP.filename) + "_spectrum_" + str(n) + ".png"),dpi=300)
-                                plt.close("all")
+                                plt.xlabel('Energy / [MeV]')
+                                plt.ylabel('Number-density / [arb.u./MeV]')
+                                plt.savefig(os.path.join(outC,manager.strip_extension(TP.filename) + '_spectrum_' + str(n) + '.png'),dpi=300)
+                                plt.close('all')
         ```
     """
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         self.__dict__.update(kwargs)
         self.status = False
@@ -367,29 +367,30 @@
         for maxima in localMaxima:
             cv2.circle(clone, maxima, 1, (255, 255, 0))
         # return the local maximum ordered
         return sorted(localmax)
 
     def ThompsomParabolaImageprocessingV2(self, pathDestinationSelected: str, picturesSelected: List[str],
                                           threshold: int = 0, wake: int = 0, quality_n: int = 100):
-        """
-        This function search for the different traces in a Thomson parabola image. For output, five folders are created:
-        - folder input save the original image
-        - folder output save the original image where the traces are painted with different colours
-        - folder mask save the traces with different colours
-        - folder ouput gray save the traces without discrimination
-        - folder text save the sum of the 5 adjacent values in a csv
+        """ Tracefinder for Thomson Parabola Ion Spectrometer
+        This function search for the different traces in a Thomson parabola image.
+        For output, five folders are created:
+        1) folder input save the original image
+        2) folder output save the original image where the traces are painted with different colours
+        3) folder mask save the traces with different colours
+        4) folder ouput gray save the traces without discrimination
+        5) folder text save the sum of the 5 adjacent values in a csv
+   
         Args: 
             pathDestinationSelected (str): output folder
             picturesSelected (list): List of path for the different pictures
             threshold (int, optional): the difference between two point in order to be considered a local maximum, initializes to ``0`` and defaults to ``(max(img)-min(img))/100``.
             wake (int, optional): The maximum number of points tha can be founded with searchpoint function, initializes to ``0`` and defaults to ``size(row)/10``.
             quality_n: the minimum number of real point admmited in a trace
-        Returns:
-            none
+        
         """
         # intialize variables
         self.filename = ""
         
         # fit dispersion relation if available
         if hasattr(self, 'dispersion_relation') and hasattr(self, 'pixel_per_space') and hasattr(self, 'X_ray_spot'):
             conversion = True
```

### Comparing `pyclpu-1.1.9/pyclpu/s33293804.py` & `pyclpu-1.2.0/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.9/pyclpu/waveform.py` & `pyclpu-1.2.0/pyclpu/waveform.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.9/pyclpu.egg-info/PKG-INFO` & `pyclpu-1.2.0/pyclpu.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.1.9
+Version: 1.2.0
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -196,42 +196,9 @@
 channel = 1
 trace = waveform.Waveform(wfm = wfm, channel = channel)
 
 trace.show()
 trace.save("C:\\bin\\output.csv")
 ```
 
-## Scripts in Modules
-
-:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format. :warning: **But relative links work only on GitLab / GitHub, not on PYPI.**
-
-## Developper's Guide
-
-To get started, clone the project into your working directory `git clone https://git.clpu.es/mehret/pyclpu` and hop inside `cd pyclpu`. Create the anaconda environment in Anaconda based on the `clpu.yml` file delivered in the main folder of the project, e.g. in the Anaconda prompt with `conda env create -f clpu.yml` and activate it with `conda activate clpu`.
-
-### Integration and Testing
-
-Install actualized versions from the main folder with `pip install .`.
-
-### Export
-
-Before exporting a new version of the module
-
-- increase the version counters in `pyclpu\__init__.py`,
-- update the `.yml`file if needed via `conda env export --from-history > clpu.yml`,
-- update the documentation via `pdoc --html pyclpu --force && pdoc --template-dir="." -o md pyclpu --force && python text.mako.py`.
-
-Export with `python setup.py sdist` to `dist/`. Then to upload all distributions created under `dist/` execute `twine upload dist/*`or to upload the source distribution with a gpg signature `twine upload dist/pyexample-0.1.0.tar.gz pyexample-0.1.0.tar.gz.asc`. Now the distribution is updated in pyPIP. For the Anaconda version, now,
-
-Note that double factor authentification is mandated on pyPIP, therefore a `.pypirc` file should be stored in your home directory that contains
-```
-[pypi]
-username = __token__
-password = pypi-AgEIcHlwaS5vcmcCJDZkZjMxODk1LTdlNzktNDIzMC1hYjJiLWVkYzVjYmE4Nzk4NwACDlsxLFsicHljbHB1Il1dAAIsWzIsWyI5MTU2MmNiMi05MzM2LTRlYjQtODAxMi04NTVhYWQ0NzA4ZGMiXV0AAAYgaKpKjrh8Ftj4yH-```
-
-(append `63z45A5wEe4WP78SioJJMpgsHc3Q` to the end of the password string in case of error) - update the Anaconda recipe via `grayskull pypi --strict-conda-forge pyCLPU`,
-- ...
-
-Close the procedure orderly:
-- git-commit the code into the developper's branch `dev` with a note on the new version number,
-- git-merge the developper's branch into the main branch `master`.
-
+## Changelog
+...
```

### Comparing `pyclpu-1.1.9/setup.py` & `pyclpu-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     license='MIT',\
     packages=['pyclpu'],
     scripts=glob.glob("pyclpu/*.py"),
 #    package_data={b'RSRTxReadBin': ['lib'+os.path.sep+'RTxReadBin-1.0-py3-none-any.whl']},
 #    include_package_data=True,
     install_requires=[\
         'numpy','scipy','opencv-python','cython','pillow',\
-        'matplotlib','tk','periodictable',\
+        'matplotlib','tk','periodictable','scikit-image',\
     ],\
     # and build in modules cython, importlib.reload, inspect.getsourcefile, glob, math, opencv, pillow, os, sys, time
     classifiers=[\
         'Development Status :: 1 - Planning',\
         'Intended Audience :: Science/Research',\
         'Programming Language :: Python :: 3.11',\
     ],\
```

