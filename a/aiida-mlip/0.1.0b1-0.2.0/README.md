# Comparing `tmp/aiida_mlip-0.1.0b1.tar.gz` & `tmp/aiida_mlip-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_mlip-0.1.0b1.tar", max compression
+gzip compressed data, was "aiida_mlip-0.2.0.tar", max compression
```

## Comparing `aiida_mlip-0.1.0b1.tar` & `aiida_mlip-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1533 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/LICENSE
--rw-r--r--   0        0        0     8039 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/README.md
--rw-r--r--   0        0        0       87 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/__init__.py
--rw-r--r--   0        0        0       34 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/__init__.py
--rw-r--r--   0        0        0     9272 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/base.py
--rw-r--r--   0        0        0     4497 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/geomopt.py
--rw-r--r--   0        0        0     4409 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/md.py
--rw-r--r--   0        0        0     3496 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/singlepoint.py
--rw-r--r--   0        0        0       43 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/data/__init__.py
--rw-r--r--   0        0        0     4349 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/data/config.py
--rw-r--r--   0        0        0     8231 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/data/model.py
--rw-r--r--   0        0        0       40 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/helpers/__init__.py
--rw-r--r--   0        0        0     2826 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/helpers/converters.py
--rw-r--r--   0        0        0     2650 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/helpers/help_load.py
--rw-r--r--   0        0        0       34 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/__init__.py
--rw-r--r--   0        0        0     2409 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/base_parser.py
--rw-r--r--   0        0        0     3719 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/md_parser.py
--rw-r--r--   0        0        0     2583 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/opt_parser.py
--rw-r--r--   0        0        0     2912 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/sp_parser.py
--rw-r--r--   0        0        0     3344 2024-05-02 17:21:52.828970 aiida_mlip-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     9132 1970-01-01 00:00:00.000000 aiida_mlip-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8765 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/README.md
+-rw-r--r--   0        0        0       85 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/calculations/__init__.py
+-rw-r--r--   0        0        0     9498 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/calculations/base.py
+-rw-r--r--   0        0        0     4496 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/calculations/geomopt.py
+-rw-r--r--   0        0        0     4408 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/calculations/md.py
+-rw-r--r--   0        0        0     3495 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/calculations/singlepoint.py
+-rw-r--r--   0        0        0     8023 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/calculations/train.py
+-rw-r--r--   0        0        0       43 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/data/__init__.py
+-rw-r--r--   0        0        0     4349 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/data/config.py
+-rw-r--r--   0        0        0     8231 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/data/model.py
+-rw-r--r--   0        0        0       40 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/helpers/__init__.py
+-rw-r--r--   0        0        0     2826 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/helpers/converters.py
+-rw-r--r--   0        0        0     3003 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/helpers/help_load.py
+-rw-r--r--   0        0        0       34 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/parsers/__init__.py
+-rw-r--r--   0        0        0     2404 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/parsers/base_parser.py
+-rw-r--r--   0        0        0     3718 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/parsers/md_parser.py
+-rw-r--r--   0        0        0     2582 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/parsers/opt_parser.py
+-rw-r--r--   0        0        0     2911 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/parsers/sp_parser.py
+-rw-r--r--   0        0        0     6328 2024-05-30 09:44:32.106045 aiida_mlip-0.2.0/aiida_mlip/parsers/train_parser.py
+-rw-r--r--   0        0        0     3456 2024-05-30 09:44:32.110045 aiida_mlip-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9856 1970-01-01 00:00:00.000000 aiida_mlip-0.2.0/PKG-INFO
```

### Comparing `aiida_mlip-0.1.0b1/LICENSE` & `aiida_mlip-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b1/README.md` & `aiida_mlip-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,37 +18,38 @@
   - CHGNET
 - [x] Single point calculations
 - [x] Geometry optimisation
 - [x] Molecular Dynamics:
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
-- [ ] Training ML potentials (MACE only planned)
+- [x] Training ML potentials (MACE only planned)
 - [ ] Fine tunning MLIPs (MACE only planned)
 
 The code relies heavily on [janus-core](https://github.com/stfc/janus-core), which handles mlip calculations using ASE.
 
 
 
 ## Installation
 
 ```shell
 pip install aiida-mlip
 verdi quicksetup  # better to set up a new profile
 verdi plugin list aiida.calculations
 ```
-The last command should show a list of AiiDA pre-installed calculations and the aiida-mlip plugin calculations (janus.opt, janus.sp)
+The last command should show a list of AiiDA pre-installed calculations and the aiida-mlip plugin calculations (mlip.opt, mlip.sp)
 ```
 Registered entry points for aiida.calculations:
 * core.arithmetic.add
 * core.templatereplacer
 * core.transfer
-* janus.opt
-* janus.sp
-* janus.md
+* mlip.opt
+* mlip.sp
+* mlip.md
+* mlip.train
 ```
 
 
 ## Usage
 
 A quick demo of how to submit a calculation using the provided example files:
 ```shell
@@ -56,14 +57,19 @@
 cd examples/calculations
 verdi run submit_singlepoint.py "janus@localhost" --struct "path/to/structure" --architecture mace --model "/path/to/model"    # run singlepoint calculation
 verdi run submit_geomopt.py "janus@localhost" --struct "path/to/structure" --model "path/to/model" --steps 5 --fully_opt True # run geometry optimisation
 verdi run submit_md.py "janus@localhost" --struct "path/to/structure" --model "path/to/model" --ensemble "nve" --md_dict_str "{'temp':300,'steps':4,'traj-every':3,'stats-every':1}" # run molecular dynamics
 
 verdi process list -a  # check record of calculation
 ```
+Models can be trained by using the Train calcjob. In that case the needed inputs are a config file containig the path to train, test and validation xyz file and other optional parameters. Running
+```shell
+verdi run submit_train.py
+```
+a model will be trained using the provided example config file and xyz files (can be found in the tests folder)
 
 ## Development
 
 1. Install [poetry](https://python-poetry.org/docs/#installation)
 2. (Optional) Create a virtual environment
 3. Install `aiida-mlip` with dependencies:
 
@@ -93,33 +99,37 @@
     * [`geomopt.py`](aiida_mlip/calculations/geomopt.py): `Calcjob` class to perform geometry optimization using mlips
     * [`md.py`](aiida_mlip/calculations/md.py): `Calcjob` class to perform molecular dynamics using mlips
   * [`parsers/`](aiida_mlip/parsers/): `Parsers` for the calculations
     * [`base_parser.py`](aiida_mlip/parsers/base_parser.py): Base `Parser` for all calculations.
     * [`sp_parser.py`](aiida_mlip/parsers/sp_parser.py): `Parser` for `Singlepoint` calculation.
     * [`opt_parser.py`](aiida_mlip/parsers/opt_parser.py): `Parser` for `Geomopt` calculation.
     * [`md_parser.py`](aiida_mlip/parsers/md_parser.py): `Parser` for `MD` calculation.
+    * [`train_parser.py`](aiida_mlip/parsers/train_parser.py): `Parser` for `Train` calculation.
   * [`helpers/`](aiida_mlip/helpers/): `Helpers` to run calculations.
 * [`docs/`](docs/source/): Code documentation
   * [`apidoc/`](docs/source/apidoc/): API documentation
   * [`developer_guide/`](docs/source/developer_guide/): Documentation for developers
   * [`user_guide/`](docs/source/user_guide/): Documentation for users
   * [`images/`](docs/source/images/): Logos etc used in the documentation
 * [`examples/`](examples/): Examples for submitting calculations using this plugin
   * [`calculations/`](examples/calculations/): Scripts for submitting calculations
     * [`submit_singlepoint.py`](examples/calculations/submit_singlepoint.py): Script for submitting a singlepoint calculation
     * [`submit_geomopt.py`](examples/calculations/submit_geomopt.py): Script for submitting a geometry optimisation calculation
     * [`submit_md.py`](examples/calculations/submit_md.py): Script for submitting a molecular dynamics calculation
+    * [`submit_train.py`](examples/calculations/submit_train.py): Script for submitting a train calculation.
 * [`tests/`](tests/): Basic regression tests using the [pytest](https://docs.pytest.org/en/latest/) framework (submitting a calculation, ...). Install `pip install -e .[testing]` and run `pytest`.
   * [`conftest.py`](tests/conftest.py): Configuration of fixtures for [pytest](https://docs.pytest.org/en/latest/)
   * [`calculations/`](tests/calculations): Calculations
     * [`test_singlepoint.py`](tests/calculations/test_singlepoint.py): Test `SinglePoint` calculation
     * [`test_geomopt.py`](tests/calculations/test_geomopt.py): Test `Geomopt` calculation
     * [`test_md.py`](tests/calculations/test_md.py): Test `MD` calculation
+    * [`test_train.py`](tests/calculations/test_train.py): Test `Train` calculation
   * [`data/`](tests/data): `ModelData`
     * [`test_model.py`](tests/data/test_model.py): Test `ModelData` type
+    * [`test_config.py`](tests/data/test_config.py): Test `JanusConfigfile` type
 * [`.gitignore`](.gitignore): Telling git which files to ignore
 * [`.pre-commit-config.yaml`](.pre-commit-config.yaml): Configuration of [pre-commit hooks](https://pre-commit.com/) that sanitize coding style and check for syntax errors. Enable via `pip install -e .[pre-commit] && pre-commit install`
 * [`LICENSE`](LICENSE): License for the plugin
 * [`README.md`](README.md): This file
 * [`tox.ini`](tox.ini): File to set up tox
 * [`pyproject.toml`](pyproject.toml): Python package metadata for registration on [PyPI](https://pypi.org/) and the [AiiDA plugin registry](https://aiidateam.github.io/aiida-registry/) (including entry points)
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/calculations/base.py` & `aiida_mlip-0.2.0/aiida_mlip/calculations/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,20 +214,24 @@
         )
 
         if architecture:
             cmd_line["arch"] = architecture
 
         model_path = None
         if "model" in self.inputs:
+            # Raise error if model is None
+            if self.inputs.model is None:
+                raise ValueError("Model cannot be None")
             model_path = self.inputs.model.filepath
         else:
             if "config" in self.inputs and "model" in self.inputs.config:
                 model_path = None
             else:
                 if "arch" in self.inputs:
+                    # if model is not given (which is different than it being None)
                     model_path = ModelData.download(
                         "https://github.com/stfc/janus-core/raw/main/tests/models/mace_mp_small.model",  # pylint: disable=line-too-long
                         architecture,
                     ).filepath
         if model_path:
             cmd_line.setdefault("calc-kwargs", {})["model"] = model_path
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/calculations/geomopt.py` & `aiida_mlip-0.2.0/aiida_mlip/calculations/geomopt.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         spec.input(
             "opt_kwargs",
             valid_type=Dict,
             required=False,
             help="Other optimisation keywords",
         )
 
-        spec.inputs["metadata"]["options"]["parser_name"].default = "janus.opt_parser"
+        spec.inputs["metadata"]["options"]["parser_name"].default = "mlip.opt_parser"
 
         spec.output("traj_file", valid_type=SinglefileData)
         spec.output("traj_output", valid_type=TrajectoryData)
         spec.output("final_structure", valid_type=StructureData)
 
     def prepare_for_submission(
         self, folder: aiida.common.folders.Folder
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/calculations/md.py` & `aiida_mlip-0.2.0/aiida_mlip/calculations/md.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     "stats-file": cls.DEFAULT_STATS_FILE,
                     "summary": cls.DEFAULT_SUMMARY_FILE,
                 }
             ),
             help="Keywords for molecular dynamics",
         )
 
-        spec.inputs["metadata"]["options"]["parser_name"].default = "janus.md_parser"
+        spec.inputs["metadata"]["options"]["parser_name"].default = "mlip.md_parser"
 
         spec.output(
             "results_dict",
             valid_type=Dict,
             help="The `results_dict` output node of the successful calculation.",
         )
         spec.output("summary", valid_type=SinglefileData)
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/calculations/singlepoint.py` & `aiida_mlip-0.2.0/aiida_mlip/calculations/singlepoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         spec.input(
             "properties",
             valid_type=Str,
             required=False,
             help="Properties to calculate",
         )
 
-        spec.inputs["metadata"]["options"]["parser_name"].default = "janus.sp_parser"
+        spec.inputs["metadata"]["options"]["parser_name"].default = "mlip.sp_parser"
 
         # Define outputs. The default is a dictionary with the content of the xyz file
         spec.output(
             "results_dict",
             valid_type=Dict,
             help="The `results_dict` output node of the successful calculation.",
         )
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/data/config.py` & `aiida_mlip-0.2.0/aiida_mlip/data/config.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/data/model.py` & `aiida_mlip-0.2.0/aiida_mlip/data/model.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/helpers/converters.py` & `aiida_mlip-0.2.0/aiida_mlip/helpers/converters.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/helpers/help_load.py` & `aiida_mlip-0.2.0/aiida_mlip/helpers/help_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,32 +19,38 @@
     architecture: str,
     cache_dir: Optional[Union[str, Path]] = None,
 ) -> ModelData:
     """
     Load a model from a file path or URL.
 
     If the string represents a file path, the model will be loaded from that path.
-    Otherwise, the model will be downloaded from the specified location.
+    If it's a URL, the model will be downloaded from the specified location.
+    If the input model is None it returns a default model corresponding to the
+    default used in the Calcjobs.
 
     Parameters
     ----------
     model : Optional[Union[str, Path]]
-        Model file path or a URL for downloading the model.
+        Model file path or a URL for downloading the model or None to use the default.
     architecture : str
         The architecture of the model.
     cache_dir : Optional[Union[str, Path]]
         Directory where to save the dowloaded model.
 
     Returns
     -------
     ModelData
         The loaded model.
     """
     if model is None:
-        loaded_model = None
+        loaded_model = ModelData.download(
+            "https://github.com/stfc/janus-core/raw/main/tests/models/mace_mp_small.model",  # pylint: disable=line-too-long
+            architecture,
+            cache_dir=cache_dir,
+        )
     elif (file_path := Path(model)).is_file():
         loaded_model = ModelData.local_file(file_path, architecture=architecture)
     else:
         loaded_model = ModelData.download(
             model, architecture=architecture, cache_dir=cache_dir
         )
     return loaded_model
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/parsers/base_parser.py` & `aiida_mlip-0.2.0/aiida_mlip/parsers/base_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,33 +16,33 @@
     ----------
     node : aiida.orm.nodes.process.process.ProcessNode
         ProcessNode of calculation.
 
     Methods
     -------
     __init__(node: aiida.orm.nodes.process.process.ProcessNode)
-        Initialize the SPParser instance.
+        Initialize the BaseParser instance.
 
     parse(**kwargs: Any) -> int:
         Parse outputs, store results in the database.
 
     Returns
     -------
     int
         An exit code.
 
     Raises
     ------
     exceptions.ParsingError
-        If the ProcessNode being passed was not produced by a singlePointCalculation.
+        If the ProcessNode being passed was not produced by a `Base` Calcjob.
     """
 
     def __init__(self, node: ProcessNode):
         """
-        Check that the ProcessNode being passed was produced by a `Singlepoint`.
+        Check that the ProcessNode being passed was produced by a `Base` Calcjob.
 
         Parameters
         ----------
         node : aiida.orm.nodes.process.process.ProcessNode
             ProcessNode of calculation.
         """
         super().__init__(node)
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/parsers/md_parser.py` & `aiida_mlip-0.2.0/aiida_mlip/parsers/md_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from aiida.orm.nodes.process.process import ProcessNode
 from aiida.plugins import CalculationFactory
 
 from aiida_mlip.calculations.md import MD
 from aiida_mlip.helpers.converters import xyz_to_aiida_traj
 from aiida_mlip.parsers.base_parser import BaseParser
 
-MDCalculation = CalculationFactory("janus.md")
+MDCalculation = CalculationFactory("mlip.md")
 
 
 class MDParser(BaseParser):
     """
     Parser class for parsing output of molecular dynamics simulation.
 
     Inherits from SPParser.
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/parsers/opt_parser.py` & `aiida_mlip-0.2.0/aiida_mlip/parsers/opt_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from aiida.orm import SinglefileData
 from aiida.orm.nodes.process.process import ProcessNode
 from aiida.plugins import CalculationFactory
 
 from aiida_mlip.helpers.converters import xyz_to_aiida_traj
 from aiida_mlip.parsers.sp_parser import SPParser
 
-geomoptCalculation = CalculationFactory("janus.opt")
+geomoptCalculation = CalculationFactory("mlip.opt")
 
 
 class GeomOptParser(SPParser):
     """
     Parser class for parsing output of geometry optimisation calculation.
 
     Inherits from SPParser.
```

### Comparing `aiida_mlip-0.1.0b1/aiida_mlip/parsers/sp_parser.py` & `aiida_mlip-0.2.0/aiida_mlip/parsers/sp_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from aiida.orm import Dict, SinglefileData
 from aiida.orm.nodes.process.process import ProcessNode
 from aiida.plugins import CalculationFactory
 
 from aiida_mlip.helpers.converters import convert_numpy
 from aiida_mlip.parsers.base_parser import BaseParser
 
-singlePointCalculation = CalculationFactory("janus.sp")
+singlePointCalculation = CalculationFactory("mlip.sp")
 
 
 class SPParser(BaseParser):
     """
     Parser class for parsing output of calculation.
 
     Parameters
```

### Comparing `aiida_mlip-0.1.0b1/pyproject.toml` & `aiida_mlip-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiida-mlip"
-version = "0.1.0b1"
+version = "0.2.0"
 description = "machine learning interatomic potentials aiida plugin"
 authors = [
     "Federica Zanca",
     "Elliott Kasoar",
     "Jacob Wilkins",
     "Alin M. Elena",
 ]
@@ -29,15 +29,15 @@
 python = "^3.9"
 aiida-core = "^2.5"
 ase = "^3.22.1"
 voluptuous = "^0.14"
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^7.4.1"}
-janus-core = "^0.2.0b4"
+janus-core = "^v0.4.0b0"
 pgtest = "^1.3.2"
 pytest = "^8.0"
 pytest-cov = "^4.1.0"
 tox = "^4.12.1"
 wheel = "^0.42"
 
 [tool.poetry.group.pre-commit]
@@ -60,26 +60,28 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."aiida.data"]
-"janus.modeldata" = "aiida_mlip.data.model:ModelData"
-"janus.config" = "aiida_mlip.data.config:JanusConfigfile"
+"mlip.modeldata" = "aiida_mlip.data.model:ModelData"
+"mlip.config" = "aiida_mlip.data.config:JanusConfigfile"
 
 [tool.poetry.plugins."aiida.calculations"]
-"janus.sp" = "aiida_mlip.calculations.singlepoint:Singlepoint"
-"janus.opt" = "aiida_mlip.calculations.geomopt:GeomOpt"
-"janus.md" = "aiida_mlip.calculations.md:MD"
+"mlip.sp" = "aiida_mlip.calculations.singlepoint:Singlepoint"
+"mlip.opt" = "aiida_mlip.calculations.geomopt:GeomOpt"
+"mlip.md" = "aiida_mlip.calculations.md:MD"
+"mlip.train" = "aiida_mlip.calculations.train:Train"
 
 [tool.poetry.plugins."aiida.parsers"]
-"janus.sp_parser" = "aiida_mlip.parsers.sp_parser:SPParser"
-"janus.opt_parser" = "aiida_mlip.parsers.opt_parser:GeomOptParser"
-"janus.md_parser" = "aiida_mlip.parsers.md_parser:MDParser"
+"mlip.sp_parser" = "aiida_mlip.parsers.sp_parser:SPParser"
+"mlip.opt_parser" = "aiida_mlip.parsers.opt_parser:GeomOptParser"
+"mlip.md_parser" = "aiida_mlip.parsers.md_parser:MDParser"
+"mlip.train_parser" = "aiida_mlip.parsers.train_parser:TrainParser"
 
 [tool.black]
 line-length = 88
 
 [tool.pylint.format]
 max-line-length = 88
```

### Comparing `aiida_mlip-0.1.0b1/PKG-INFO` & `aiida_mlip-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-mlip
-Version: 0.1.0b1
+Version: 0.2.0
 Summary: machine learning interatomic potentials aiida plugin
 Home-page: https://github.com/stfc/aiida-mlip/
 Keywords: aiida,plugin
 Author: Federica Zanca
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
@@ -45,37 +45,38 @@
   - CHGNET
 - [x] Single point calculations
 - [x] Geometry optimisation
 - [x] Molecular Dynamics:
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
-- [ ] Training ML potentials (MACE only planned)
+- [x] Training ML potentials (MACE only planned)
 - [ ] Fine tunning MLIPs (MACE only planned)
 
 The code relies heavily on [janus-core](https://github.com/stfc/janus-core), which handles mlip calculations using ASE.
 
 
 
 ## Installation
 
 ```shell
 pip install aiida-mlip
 verdi quicksetup  # better to set up a new profile
 verdi plugin list aiida.calculations
 ```
-The last command should show a list of AiiDA pre-installed calculations and the aiida-mlip plugin calculations (janus.opt, janus.sp)
+The last command should show a list of AiiDA pre-installed calculations and the aiida-mlip plugin calculations (mlip.opt, mlip.sp)
 ```
 Registered entry points for aiida.calculations:
 * core.arithmetic.add
 * core.templatereplacer
 * core.transfer
-* janus.opt
-* janus.sp
-* janus.md
+* mlip.opt
+* mlip.sp
+* mlip.md
+* mlip.train
 ```
 
 
 ## Usage
 
 A quick demo of how to submit a calculation using the provided example files:
 ```shell
@@ -83,14 +84,19 @@
 cd examples/calculations
 verdi run submit_singlepoint.py "janus@localhost" --struct "path/to/structure" --architecture mace --model "/path/to/model"    # run singlepoint calculation
 verdi run submit_geomopt.py "janus@localhost" --struct "path/to/structure" --model "path/to/model" --steps 5 --fully_opt True # run geometry optimisation
 verdi run submit_md.py "janus@localhost" --struct "path/to/structure" --model "path/to/model" --ensemble "nve" --md_dict_str "{'temp':300,'steps':4,'traj-every':3,'stats-every':1}" # run molecular dynamics
 
 verdi process list -a  # check record of calculation
 ```
+Models can be trained by using the Train calcjob. In that case the needed inputs are a config file containig the path to train, test and validation xyz file and other optional parameters. Running
+```shell
+verdi run submit_train.py
+```
+a model will be trained using the provided example config file and xyz files (can be found in the tests folder)
 
 ## Development
 
 1. Install [poetry](https://python-poetry.org/docs/#installation)
 2. (Optional) Create a virtual environment
 3. Install `aiida-mlip` with dependencies:
 
@@ -120,33 +126,37 @@
     * [`geomopt.py`](aiida_mlip/calculations/geomopt.py): `Calcjob` class to perform geometry optimization using mlips
     * [`md.py`](aiida_mlip/calculations/md.py): `Calcjob` class to perform molecular dynamics using mlips
   * [`parsers/`](aiida_mlip/parsers/): `Parsers` for the calculations
     * [`base_parser.py`](aiida_mlip/parsers/base_parser.py): Base `Parser` for all calculations.
     * [`sp_parser.py`](aiida_mlip/parsers/sp_parser.py): `Parser` for `Singlepoint` calculation.
     * [`opt_parser.py`](aiida_mlip/parsers/opt_parser.py): `Parser` for `Geomopt` calculation.
     * [`md_parser.py`](aiida_mlip/parsers/md_parser.py): `Parser` for `MD` calculation.
+    * [`train_parser.py`](aiida_mlip/parsers/train_parser.py): `Parser` for `Train` calculation.
   * [`helpers/`](aiida_mlip/helpers/): `Helpers` to run calculations.
 * [`docs/`](docs/source/): Code documentation
   * [`apidoc/`](docs/source/apidoc/): API documentation
   * [`developer_guide/`](docs/source/developer_guide/): Documentation for developers
   * [`user_guide/`](docs/source/user_guide/): Documentation for users
   * [`images/`](docs/source/images/): Logos etc used in the documentation
 * [`examples/`](examples/): Examples for submitting calculations using this plugin
   * [`calculations/`](examples/calculations/): Scripts for submitting calculations
     * [`submit_singlepoint.py`](examples/calculations/submit_singlepoint.py): Script for submitting a singlepoint calculation
     * [`submit_geomopt.py`](examples/calculations/submit_geomopt.py): Script for submitting a geometry optimisation calculation
     * [`submit_md.py`](examples/calculations/submit_md.py): Script for submitting a molecular dynamics calculation
+    * [`submit_train.py`](examples/calculations/submit_train.py): Script for submitting a train calculation.
 * [`tests/`](tests/): Basic regression tests using the [pytest](https://docs.pytest.org/en/latest/) framework (submitting a calculation, ...). Install `pip install -e .[testing]` and run `pytest`.
   * [`conftest.py`](tests/conftest.py): Configuration of fixtures for [pytest](https://docs.pytest.org/en/latest/)
   * [`calculations/`](tests/calculations): Calculations
     * [`test_singlepoint.py`](tests/calculations/test_singlepoint.py): Test `SinglePoint` calculation
     * [`test_geomopt.py`](tests/calculations/test_geomopt.py): Test `Geomopt` calculation
     * [`test_md.py`](tests/calculations/test_md.py): Test `MD` calculation
+    * [`test_train.py`](tests/calculations/test_train.py): Test `Train` calculation
   * [`data/`](tests/data): `ModelData`
     * [`test_model.py`](tests/data/test_model.py): Test `ModelData` type
+    * [`test_config.py`](tests/data/test_config.py): Test `JanusConfigfile` type
 * [`.gitignore`](.gitignore): Telling git which files to ignore
 * [`.pre-commit-config.yaml`](.pre-commit-config.yaml): Configuration of [pre-commit hooks](https://pre-commit.com/) that sanitize coding style and check for syntax errors. Enable via `pip install -e .[pre-commit] && pre-commit install`
 * [`LICENSE`](LICENSE): License for the plugin
 * [`README.md`](README.md): This file
 * [`tox.ini`](tox.ini): File to set up tox
 * [`pyproject.toml`](pyproject.toml): Python package metadata for registration on [PyPI](https://pypi.org/) and the [AiiDA plugin registry](https://aiidateam.github.io/aiida-registry/) (including entry points)
```

