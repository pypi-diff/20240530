# Comparing `tmp/ncompare-1.8.0.tar.gz` & `tmp/ncompare-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncompare-1.8.0.tar", max compression
+gzip compressed data, was "ncompare-1.9.0.tar", max compression
```

## Comparing `ncompare-1.8.0.tar` & `ncompare-1.9.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     9474 2024-03-12 19:25:31.383816 ncompare-1.8.0/README.md
--rw-r--r--   0        0        0       44 2024-03-12 19:25:31.383816 ncompare-1.8.0/ncompare/__init__.py
--rwxr-xr-x   0        0        0     2730 2024-03-12 19:25:31.383816 ncompare-1.8.0/ncompare/console.py
--rw-r--r--   0        0        0    22643 2024-03-12 19:25:31.383816 ncompare-1.8.0/ncompare/core.py
--rw-r--r--   0        0        0    12412 2024-03-12 19:25:31.383816 ncompare-1.8.0/ncompare/printing.py
--rw-r--r--   0        0        0     2262 2024-03-12 19:25:31.383816 ncompare-1.8.0/ncompare/sequence_operations.py
--rw-r--r--   0        0        0     1802 2024-03-12 19:25:31.383816 ncompare-1.8.0/ncompare/utils.py
--rw-r--r--   0        0        0     2024 2024-03-12 19:25:49.356037 ncompare-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    10573 1970-01-01 00:00:00.000000 ncompare-1.8.0/setup.py
--rw-r--r--   0        0        0    10866 1970-01-01 00:00:00.000000 ncompare-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 23:58:12.217452 ncompare-1.9.0/LICENSE
+-rw-r--r--   0        0        0     8451 2024-05-29 23:58:12.217452 ncompare-1.9.0/README.md
+-rw-r--r--   0        0        0     1512 2024-05-29 23:58:12.217452 ncompare-1.9.0/ncompare/__init__.py
+-rwxr-xr-x   0        0        0     4198 2024-05-29 23:58:12.217452 ncompare-1.9.0/ncompare/console.py
+-rw-r--r--   0        0        0    24082 2024-05-29 23:58:12.217452 ncompare-1.9.0/ncompare/core.py
+-rw-r--r--   0        0        0    13880 2024-05-29 23:58:12.217452 ncompare-1.9.0/ncompare/printing.py
+-rw-r--r--   0        0        0     3730 2024-05-29 23:58:12.217452 ncompare-1.9.0/ncompare/sequence_operations.py
+-rw-r--r--   0        0        0     3270 2024-05-29 23:58:12.217452 ncompare-1.9.0/ncompare/utils.py
+-rw-r--r--   0        0        0     1972 2024-05-29 23:58:31.333494 ncompare-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9542 1970-01-01 00:00:00.000000 ncompare-1.9.0/setup.py
+-rw-r--r--   0        0        0     9792 1970-01-01 00:00:00.000000 ncompare-1.9.0/PKG-INFO
```

### Comparing `ncompare-1.8.0/README.md` & `ncompare-1.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,22 +49,24 @@
 To compare two netCDF files,
 pass the filepaths for each of the two netCDF files directly to ncompare, as follows:
 
 ```console
 ncompare <netcdf file #1> <netcdf file #2>
 ```
 
+<img src="https://github.com/nasa/ncompare/assets/114174502/1964096e-829d-4fe1-96a5-63581ade2d38" width="600" />
+
+
 With an additional `--file-text` argument specified,
 a common use of _ncompare_ may look like this example:
 
 ```console
 ncompare S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt
 ```
 
-
 **A more complete usage demonstration with example output is shown in
 [this example notebook](https://ncompare.readthedocs.io/en/latest/example/ncompare-example-usage/).**
 
 ### Options
 
 - `-h`, `--help` : Show this help message and exit.
 - `--file-text` [FILE_PATH]: Text file to write output to.
@@ -78,17 +80,16 @@
 - `-g` (`--comparison_var_group`) [VAR_GROUP]: Group that contains the `comparison_var_name`.
 - `--column-widths` [WIDTH, WIDTH, WIDTH]: Width, in number of characters, of the three columns in the comparison report
 - `--version` : Show the current version and then exit.
 
 ## Contributing
 
 Contributions are welcome! For more information, see [CONTRIBUTING.md](CONTRIBUTING.md).
-_ncompare_ is licensed under the NASA Open Source Agreement, which is included
-[in this repository's license directory](license/LAR-20274-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf)
-and [on the Open Source Initiative website](https://opensource.org/license/nasa1-3-php/).
+_ncompare_ is licensed under the Apache License 2.0,
+which is included in the [LICENSE](LICENSE) file.
 
 
 ### Developing
 
 Development within this repository should occur on a feature branch.
 Pull Requests (PRs) are created with a target of the `develop` branch before being reviewed and merged.
 
@@ -148,45 +149,40 @@
 - `ncompare` uses `xarray` to access the root-level dimensions.
 In some cases, `xarray` will miss dimensions whose names do not also exist as variable names in the dataset
   (also known as non-coordinate dimensions).
 - Some underlying HDF5 properties, such as _Netcdf4Dimid or _Netcdf4Coordinates, are not currently assesssed by `ncompare`.
 
 # Notices:
 
-Copyright 2023 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
+Copyright 2023 United States Government as represented by the Administrator of the
+National Aeronautics and Space Administration. All Rights Reserved.
 
-### Third-Party Software:
-This software calls the following third-party software, which is subject to the terms and conditions of its licensor,
-as applicable at the time of licensing. Third-party software is not bundled with this software,
-but may be available from the licensor.
+This software calls the following third-party software,
+which is subject to the terms and conditions of its licensor,
+as applicable at the time of licensing.
+The third-party software is not bundled with this software but may be available from the licensor.
 
-License hyperlinks are provided here for information purposes only:
+License hyperlinks are provided here for information purposes only.
 
-| item     |                               license                               | link                                                          |
+
+| Title    |                               license                               | link                                                          |
 |:---------|:-------------------------------------------------------------------:|:--------------------------------------------------------------|
 | colorama |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |
 | netCDF4  |                             MIT License                             | https://opensource.org/licenses/MIT                           |
 | numpy    |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |
 | openpyxl |                             MIT License                             | https://opensource.org/licenses/MIT                           |
 | xarray   |                     Apache License, version 2.0                     | https://www.apache.org/licenses/LICENSE-2.0                   |
 | Python   | Standard Library Python Software Foundation (PSF) License Agreement | https://docs.python.org/3/license.html#psf-licenseDisclaimers |
 
 
-### No Warranty:
-THE SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER EXPRESSED, IMPLIED,
-OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS,
-ANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM FROM INFRINGEMENT,
-ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE, OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED,
-WILL CONFORM TO THE SUBJECT SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER,
-CONSTITUTE AN ENDORSEMENT BY GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS, HARDWARE,
-SOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE SUBJECT SOFTWARE.
-FURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND LIABILITIES REGARDING THIRD-PARTY SOFTWARE,
-IF PRESENT IN THE ORIGINAL SOFTWARE, AND DISTRIBUTES IT "AS IS."
-
-### Waiver and Indemnity:
-RECIPIENT AGREES TO WAIVE ANY AND ALL CLAIMS AGAINST THE UNITED STATES GOVERNMENT,
-ITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT. IF RECIPIENT'S USE OF THE SUBJECT SOFTWARE RESULTS
-IN ANY LIABILITIES, DEMANDS, DAMAGES, EXPENSES OR LOSSES ARISING FROM SUCH USE, INCLUDING ANY DAMAGES FROM PRODUCTS
-BASED ON, OR RESULTING FROM, RECIPIENT'S USE OF THE SUBJECT SOFTWARE, RECIPIENT SHALL INDEMNIFY AND HOLD HARMLESS
-THE UNITED STATES GOVERNMENT, ITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT,
-TO THE EXTENT PERMITTED BY LAW. RECIPIENT'S SOLE
-REMEDY FOR ANY SUCH MATTER SHALL BE THE IMMEDIATE, UNILATERAL TERMINATION OF THIS AGREEMENT.
+The ncompare: NetCDF structural comparison tool framework is licensed under the Apache License,
+Version 2.0 (the "License");
+you may not use this application except in compliance with the License.
+You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
+
+Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and limitations under the License.
+
+---
+This package is NASA Software Release Authorization (SRA) # LAR-20274-1
```

#### html2text {}

```diff
@@ -3,95 +3,82 @@
 _S_t_a_t_u_s_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]
 _[_C_o_n_t_r_i_b_u_t_i_o_n_s_ _w_e_l_c_o_m_e_]_[_Z_e_n_o_d_o_]_[_p_y_O_p_e_n_S_c_i_]Compare the structure of two NetCDF
 files at the command line. `ncompare` generates a view of the matching and non-
 matching groups and variables between two NetCDF datasets. ## Installing
 Install the latest version of the package from the Python Package Index (PyPI):
 ```console pip install ncompare ``` ## Usage To compare two netCDF files, pass
 the filepaths for each of the two netCDF files directly to ncompare, as
-follows: ```console ncompare ``` With an additional `--file-text` argument
-specified, a common use of _ncompare_ may look like this example: ```console
-ncompare S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt ``` **A
-more complete usage demonstration with example output is shown in [this example
-notebook](https://ncompare.readthedocs.io/en/latest/example/ncompare-example-
-usage/).** ### Options - `-h`, `--help` : Show this help message and exit. - `-
--file-text` [FILE_PATH]: Text file to write output to. - `--file-csv`
-[FILE_PATH]: Comma-separated values (CSV) file to write output to. - `--file-
-xlsx` [FILE_PATH]: Excel file to write output to. - `--only-diffs` : Only
-display variables and attributes that are different - `--no-color` : Turn off
-all colorized output. - `--show-attributes` : Include variable attributes in
-the table that compares variables. - `--show-chunks` : Include chunk sizes in
-the table that compares variables. - `-v` (`--comparison_var_name`) [VAR_NAME]:
-Compare specific values for this variable. - `-g` (`--comparison_var_group`)
-[VAR_GROUP]: Group that contains the `comparison_var_name`. - `--column-widths`
-[WIDTH, WIDTH, WIDTH]: Width, in number of characters, of the three columns in
-the comparison report - `--version` : Show the current version and then exit.
-## Contributing Contributions are welcome! For more information, see
-[CONTRIBUTING.md](CONTRIBUTING.md). _ncompare_ is licensed under the NASA Open
-Source Agreement, which is included [in this repository's license directory]
-(license/LAR-20274-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf)
-and [on the Open Source Initiative website](https://opensource.org/license/
-nasa1-3-php/). ### Developing Development within this repository should occur
-on a feature branch. Pull Requests (PRs) are created with a target of the
-`develop` branch before being reviewed and merged. ### Installing locally For
-local development, one can clone the repository and then use poetry or pip from
-the local directory: ```console git clone https://github.com/nasa/ncompare.git
-``` ###### (Option A) using poetry: ii) Follow the instructions for installing
-`poetry` [here](https://python-poetry.org/docs/). iii) Run ```poetry install```
-from the repository directory. ###### (Option B) using pip: ii) Run ```pip
-install .``` from the repository directory. ### Testing locally If installed
-using a `poetry` environment, the tests can be run with: ```console poetry run
-pytest tests ``` Or from another virtual environment, one can use: ```console
-pytest tests ``` ### To run as a locally installed poetry module ```console
-poetry run ncompare ``` ## Why ncompare? The `cdo` (climate data operators)
-tool [does not support NetCDF4 groups](https://code.mpimet.mpg.de/boards/2/
-topics/12073). Moreover, `nco` operators' `ncdiff` function computes value
-differences, but --- as far as the developers of this tool are aware --- `nco`
-does not have a simple function to show structural differences between NetCDF4
-datasets. Note that `h5diff`, provided in the HDF5 software, can also be used
-to find differences. In comparison to `h5diff`, `ncompare` is written and
-runnable in Python; `ncompare` provides _aligned_ and _colorized_ difference
-report for quicker assessments of groups, variable names, types, shapes, and
-attributes; and can generate report files formatted for other applications.
-However, note that `h5diff` provides comparison of some otherwise "hidden" hdf5
-properties, such as _Netcdf4Dimid or _Netcdf4Coordinates, which are not
-currently assessed by `ncompare`. ## Known limitations - `ncompare` uses
-`xarray` to access the root-level dimensions. In some cases, `xarray` will miss
-dimensions whose names do not also exist as variable names in the dataset (also
-known as non-coordinate dimensions). - Some underlying HDF5 properties, such as
-_Netcdf4Dimid or _Netcdf4Coordinates, are not currently assesssed by
-`ncompare`. # Notices: Copyright 2023 United States Government as represented
-by the Administrator of the National Aeronautics and Space Administration. All
-Rights Reserved. ### Third-Party Software: This software calls the following
+follows: ```console ncompare ``` [https://github.com/nasa/ncompare/assets/
+114174502/1964096e-829d-4fe1-96a5-63581ade2d38]With an additional `--file-text`
+argument specified, a common use of _ncompare_ may look like this example:
+```console ncompare S001G01.nc S001G01_SUBSET.nc --file-text
+subset_comparison.txt ``` **A more complete usage demonstration with example
+output is shown in [this example notebook](https://ncompare.readthedocs.io/en/
+latest/example/ncompare-example-usage/).** ### Options - `-h`, `--help` : Show
+this help message and exit. - `--file-text` [FILE_PATH]: Text file to write
+output to. - `--file-csv` [FILE_PATH]: Comma-separated values (CSV) file to
+write output to. - `--file-xlsx` [FILE_PATH]: Excel file to write output to. -
+`--only-diffs` : Only display variables and attributes that are different - `--
+no-color` : Turn off all colorized output. - `--show-attributes` : Include
+variable attributes in the table that compares variables. - `--show-chunks` :
+Include chunk sizes in the table that compares variables. - `-v` (`--
+comparison_var_name`) [VAR_NAME]: Compare specific values for this variable. -
+`-g` (`--comparison_var_group`) [VAR_GROUP]: Group that contains the
+`comparison_var_name`. - `--column-widths` [WIDTH, WIDTH, WIDTH]: Width, in
+number of characters, of the three columns in the comparison report - `--
+version` : Show the current version and then exit. ## Contributing
+Contributions are welcome! For more information, see [CONTRIBUTING.md]
+(CONTRIBUTING.md). _ncompare_ is licensed under the Apache License 2.0, which
+is included in the [LICENSE](LICENSE) file. ### Developing Development within
+this repository should occur on a feature branch. Pull Requests (PRs) are
+created with a target of the `develop` branch before being reviewed and merged.
+### Installing locally For local development, one can clone the repository and
+then use poetry or pip from the local directory: ```console git clone https://
+github.com/nasa/ncompare.git ``` ###### (Option A) using poetry: ii) Follow the
+instructions for installing `poetry` [here](https://python-poetry.org/docs/).
+iii) Run ```poetry install``` from the repository directory. ###### (Option B)
+using pip: ii) Run ```pip install .``` from the repository directory. ###
+Testing locally If installed using a `poetry` environment, the tests can be run
+with: ```console poetry run pytest tests ``` Or from another virtual
+environment, one can use: ```console pytest tests ``` ### To run as a locally
+installed poetry module ```console poetry run ncompare ``` ## Why ncompare? The
+`cdo` (climate data operators) tool [does not support NetCDF4 groups](https://
+code.mpimet.mpg.de/boards/2/topics/12073). Moreover, `nco` operators' `ncdiff`
+function computes value differences, but --- as far as the developers of this
+tool are aware --- `nco` does not have a simple function to show structural
+differences between NetCDF4 datasets. Note that `h5diff`, provided in the HDF5
+software, can also be used to find differences. In comparison to `h5diff`,
+`ncompare` is written and runnable in Python; `ncompare` provides _aligned_ and
+_colorized_ difference report for quicker assessments of groups, variable
+names, types, shapes, and attributes; and can generate report files formatted
+for other applications. However, note that `h5diff` provides comparison of some
+otherwise "hidden" hdf5 properties, such as _Netcdf4Dimid or
+_Netcdf4Coordinates, which are not currently assessed by `ncompare`. ## Known
+limitations - `ncompare` uses `xarray` to access the root-level dimensions. In
+some cases, `xarray` will miss dimensions whose names do not also exist as
+variable names in the dataset (also known as non-coordinate dimensions). - Some
+underlying HDF5 properties, such as _Netcdf4Dimid or _Netcdf4Coordinates, are
+not currently assesssed by `ncompare`. # Notices: Copyright 2023 United States
+Government as represented by the Administrator of the National Aeronautics and
+Space Administration. All Rights Reserved. This software calls the following
 third-party software, which is subject to the terms and conditions of its
-licensor, as applicable at the time of licensing. Third-party software is not
-bundled with this software, but may be available from the licensor. License
-hyperlinks are provided here for information purposes only: | item | license |
+licensor, as applicable at the time of licensing. The third-party software is
+not bundled with this software but may be available from the licensor. License
+hyperlinks are provided here for information purposes only. | Title | license |
 link | |:---------|:-----------------------------------------------------------
 --------:|:--------------------------------------------------------------| |
 colorama | BSD-3-Clause | https://opensource.org/licenses/BSD-3-Clause | |
 netCDF4 | MIT License | https://opensource.org/licenses/MIT | | numpy | BSD-3-
 Clause | https://opensource.org/licenses/BSD-3-Clause | | openpyxl | MIT
 License | https://opensource.org/licenses/MIT | | xarray | Apache License,
 version 2.0 | https://www.apache.org/licenses/LICENSE-2.0 | | Python | Standard
 Library Python Software Foundation (PSF) License Agreement | https://
-docs.python.org/3/license.html#psf-licenseDisclaimers | ### No Warranty: THE
-SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER
-EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY
-THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM
-FROM INFRINGEMENT, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE,
-OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED, WILL CONFORM TO THE SUBJECT
-SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER, CONSTITUTE AN ENDORSEMENT BY
-GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS,
-HARDWARE, SOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE
-SUBJECT SOFTWARE. FURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND
-LIABILITIES REGARDING THIRD-PARTY SOFTWARE, IF PRESENT IN THE ORIGINAL
-SOFTWARE, AND DISTRIBUTES IT "AS IS." ### Waiver and Indemnity: RECIPIENT
-AGREES TO WAIVE ANY AND ALL CLAIMS AGAINST THE UNITED STATES GOVERNMENT, ITS
-CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT. IF RECIPIENT'S
-USE OF THE SUBJECT SOFTWARE RESULTS IN ANY LIABILITIES, DEMANDS, DAMAGES,
-EXPENSES OR LOSSES ARISING FROM SUCH USE, INCLUDING ANY DAMAGES FROM PRODUCTS
-BASED ON, OR RESULTING FROM, RECIPIENT'S USE OF THE SUBJECT SOFTWARE, RECIPIENT
-SHALL INDEMNIFY AND HOLD HARMLESS THE UNITED STATES GOVERNMENT, ITS CONTRACTORS
-AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT, TO THE EXTENT PERMITTED BY
-LAW. RECIPIENT'S SOLE REMEDY FOR ANY SUCH MATTER SHALL BE THE IMMEDIATE,
-UNILATERAL TERMINATION OF THIS AGREEMENT.
+docs.python.org/3/license.html#psf-licenseDisclaimers | The ncompare: NetCDF
+structural comparison tool framework is licensed under the Apache License,
+Version 2.0 (the "License"); you may not use this application except in
+compliance with the License. You may obtain a copy of the License at http://
+www.apache.org/licenses/LICENSE-2.0. Unless required by applicable law or
+agreed to in writing, software distributed under the License is distributed on
+an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
+or implied. See the License for the specific language governing permissions and
+limitations under the License. --- This package is NASA Software Release
+Authorization (SRA) # LAR-20274-1
```

### Comparing `ncompare-1.8.0/ncompare/core.py` & `ncompare-1.9.0/ncompare/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,37 @@
-"""Compare the structure of two NetCDF files."""
-
+# Copyright 2024 United States Government as represented by the Administrator of the
+# National Aeronautics and Space Administration. All Rights Reserved.
+#
+# This software calls the following third-party software,
+# which is subject to the terms and conditions of its licensor, as applicable.
+# Users must license their own copies; the links are provided for convenience only.
+#
+# colorama - BSD-3-Clause - https://opensource.org/licenses/BSD-3-Clause
+# netCDF4 - MIT License - https://opensource.org/licenses/MIT
+# numpy - BSD-3-Clause - https://opensource.org/licenses/BSD-3-Clause
+# openpyxl - MIT License - https://opensource.org/licenses/MIT
+# xarray - Apache License, version 2.0 - https://www.apache.org/licenses/LICENSE-2.0
+# Python Standard Library - Python Software Foundation (PSF) License Agreement-
+#   https://docs.python.org/3/license.html#psf-license
+#
+# The ncompare: NetCDF structural comparison tool platform is licensed under the
+# Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and limitations under the License.
 # pylint: disable=too-many-arguments
 # pylint: disable=consider-using-f-string
 # pylint: disable=no-member
 # pylint: disable=fixme
+
+"""Compare the structure of two NetCDF files."""
 import random
 import traceback
 from collections import namedtuple
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Optional, Union
 
@@ -143,37 +167,36 @@
     list_a = _get_groups(nc_a)
     list_b = _get_groups(nc_b)
     _, _, _ = out.lists_diff(list_a, list_b)
 
     if comparison_var_group:
         # Show the variables within the selected group.
         out.print(
-            Fore.LIGHTBLUE_EX + "\nVariables within specified group <%s>:" % comparison_var_group,
+            Fore.LIGHTBLUE_EX + f"\nVariables within specified group <{comparison_var_group}>:",
             add_to_history=True,
         )
         vlist_a = _get_vars(nc_a, comparison_var_group)
         vlist_b = _get_vars(nc_b, comparison_var_group)
         _, _, _ = out.lists_diff(vlist_a, vlist_b)
 
         # TODO: Remove comparison variable/val?
         if comparison_var_name:
             try:
                 # Print the first part of the values array for the selected variable.
                 out.print(
                     Fore.LIGHTBLUE_EX
-                    + "\nSample values within specified variable <%s>:" % comparison_var_name
+                    + f"\nSample values within specified variable <{comparison_var_name}>:"
                 )
                 _print_sample_values(out, nc_a, comparison_var_group, comparison_var_name)
                 _print_sample_values(out, nc_b, comparison_var_group, comparison_var_name)
                 # compare_sample_values(nc_a, nc_b, groupname=comparison_var_group, varname=comparison_var_name)
 
                 out.print(
                     Fore.LIGHTBLUE_EX
-                    + "\nChecking multiple random values within specified variable <%s>:"
-                    % comparison_var_name
+                    + f"\nChecking multiple random values within specified variable <{comparison_var_name}>:"
                 )
                 compare_multiple_random_values(
                     out, nc_a, nc_b, groupname=comparison_var_group, varname=comparison_var_name
                 )
 
             except KeyError:
                 out.print(
@@ -258,15 +281,15 @@
         )
         for (_, group_a_name, group_b_name) in common_elements(
             top_a.groups if top_a is not None else "", top_b.groups if top_b is not None else ""
         )
     )
 
     for _, subgroup_a_name, subgroup_b_name in common_elements(
-        top_a.groups if top_a is not None else "", top_b.groups if top_a is not None else ""
+        top_a.groups if top_a is not None else "", top_b.groups if top_b is not None else ""
     ):
         yield from walk_common_groups_tree(
             top_a_name + "/" + subgroup_a_name if subgroup_a_name else "",
             (
                 top_a[subgroup_a_name]
                 if (subgroup_a_name and (subgroup_a_name in top_a.groups))
                 else None
@@ -593,15 +616,15 @@
     return ""
 
 
 def _get_vars(nc_filepath: Union[str, Path], groupname: str) -> list:
     try:
         grp = xr.open_dataset(nc_filepath, backend_kwargs={"group": groupname})
     except OSError as err:
-        print("\nError occurred when attempting to open group within <%s>.\n" % nc_filepath)
+        print(f"\nError occurred when attempting to open group within <{nc_filepath}>.\n")
         raise err
     grp_varlist = sorted(list(grp.variables.keys()))  # type:ignore[type-var]
 
     return grp_varlist
 
 
 def _get_groups(nc_filepath: Union[str, Path]) -> list:
```

### Comparing `ncompare-1.8.0/ncompare/printing.py` & `ncompare-1.9.0/ncompare/printing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,34 @@
-"""Utility functions for printing to the console or a text file."""
+# Copyright 2024 United States Government as represented by the Administrator of the
+# National Aeronautics and Space Administration. All Rights Reserved.
+#
+# This software calls the following third-party software,
+# which is subject to the terms and conditions of its licensor, as applicable.
+# Users must license their own copies; the links are provided for convenience only.
+#
+# colorama - BSD-3-Clause - https://opensource.org/licenses/BSD-3-Clause
+# netCDF4 - MIT License - https://opensource.org/licenses/MIT
+# numpy - BSD-3-Clause - https://opensource.org/licenses/BSD-3-Clause
+# openpyxl - MIT License - https://opensource.org/licenses/MIT
+# xarray - Apache License, version 2.0 - https://www.apache.org/licenses/LICENSE-2.0
+# Python Standard Library - Python Software Foundation (PSF) License Agreement-
+#   https://docs.python.org/3/license.html#psf-license
+#
+# The ncompare: NetCDF structural comparison tool platform is licensed under the
+# Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and limitations under the License.
 # pylint: disable=too-many-arguments
+
+"""Utility functions for printing to the console or a text file."""
 import csv
 import re
 import warnings
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Optional, TextIO, Union
```

### Comparing `ncompare-1.8.0/pyproject.toml` & `ncompare-1.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "ncompare"
-version = "1.8.0"
+version = "1.9.0"
 description = "Compare the structure of two NetCDF files at the command line"
 authors = ["Daniel Kaufman <daniel.kaufman@nasa.gov>"]
 readme = "README.md"
 repository = "https://github.com/nasa/ncompare"
-license = "license/LAR-20274-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf"
+license = "Apache-2.0"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
@@ -28,22 +28,22 @@
 netCDF4 = "^1.6.4"
 xarray = ">=2023.9,<2025.0"
 colorama = "^0.4.6"
 openpyxl = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.2,<9.0.0"
-ruff = ">=0.0.291,<0.3.3"
+ruff = ">=0.0.291,<0.4.6"
 black = ">=23.9.1,<25.0.0"
 mypy = "^1.5.1"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 mkdocs = "^1.5.3"
 markdown-callouts = "^0.4.0"
 markdown-include = "^0.8.1"
-mkdocstrings = "^0.24.1"
+mkdocstrings = ">=0.24.1,<0.26.0"
 mkdocs-jupyter = "^0.24.6"
 mkdocs-material = "^9.5.12"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ncompare-1.8.0/setup.py` & `ncompare-1.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'xarray>=2023.9,<2025.0']
 
 entry_points = \
 {'console_scripts': ['ncompare = ncompare.console:main']}
 
 setup_kwargs = {
     'name': 'ncompare',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Compare the structure of two NetCDF files at the command line',
-    'long_description': '# ncompare\n_____\n\n<a href="https://www.repostatus.org/#active" target="_blank">\n    <img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed">\n</a>\n<a href="https://codecov.io/gh/nasa/ncompare">\n <img src="https://codecov.io/gh/nasa/ncompare/graph/badge.svg?token=5JJUNA1Z6S" alt="Code coverage">\n</a>\n<a href="https://ncompare.readthedocs.io/en/latest/?badge=latest">\n    <img src="https://readthedocs.org/projects/ncompare/badge/?version=latest" alt="Documentation Status">\n</a>\n<a href="https://pypi.org/project/ncompare/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/ncompare.svg" alt="Python Versions">\n</a>\n<a href="https://pypi.org/project/ncompare" target="_blank">\n    <img src="https://img.shields.io/pypi/v/ncompare?color=%2334D058label=pypi%20package" alt="Package version">\n</a>\n<a href="https://github.com/python/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">\n</a>\n<a href="https://mypy-lang.org/" target="_blank">\n    <img src="https://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">\n</a>\n<a href="https://github.com/nasa/ncompare/issues" target="_blank">\n    <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?" alt="Contributions welcome">\n</a>\n<a href="https://doi.org/10.5281/zenodo.10625407" target="_blank">\n    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.10625407.svg" alt="Zenodo">\n</a>\n<a href="https://github.com/pyOpenSci/software-review/issues/146" target="_blank">\n    <img src="https://tinyurl.com/y22nb8up?" alt="pyOpenSci">\n</a>\n\nCompare the structure of two NetCDF files at the command line.\n`ncompare` generates a view of the matching and non-matching groups and variables between two NetCDF datasets.\n\n\n## Installing\n\nInstall the latest version of the package from the Python Package Index (PyPI):\n```console\npip install ncompare\n```\n\n\n## Usage\n\nTo compare two netCDF files,\npass the filepaths for each of the two netCDF files directly to ncompare, as follows:\n\n```console\nncompare <netcdf file #1> <netcdf file #2>\n```\n\nWith an additional `--file-text` argument specified,\na common use of _ncompare_ may look like this example:\n\n```console\nncompare S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt\n```\n\n\n**A more complete usage demonstration with example output is shown in\n[this example notebook](https://ncompare.readthedocs.io/en/latest/example/ncompare-example-usage/).**\n\n### Options\n\n- `-h`, `--help` : Show this help message and exit.\n- `--file-text` [FILE_PATH]: Text file to write output to.\n- `--file-csv` [FILE_PATH]: Comma-separated values (CSV) file to write output to.\n- `--file-xlsx` [FILE_PATH]: Excel file to write output to.\n- `--only-diffs` : Only display variables and attributes that are different\n- `--no-color` : Turn off all colorized output.\n- `--show-attributes` : Include variable attributes in the table that compares variables.\n- `--show-chunks` : Include chunk sizes in the table that compares variables.\n- `-v` (`--comparison_var_name`) [VAR_NAME]: Compare specific values for this variable.\n- `-g` (`--comparison_var_group`) [VAR_GROUP]: Group that contains the `comparison_var_name`.\n- `--column-widths` [WIDTH, WIDTH, WIDTH]: Width, in number of characters, of the three columns in the comparison report\n- `--version` : Show the current version and then exit.\n\n## Contributing\n\nContributions are welcome! For more information, see [CONTRIBUTING.md](CONTRIBUTING.md).\n_ncompare_ is licensed under the NASA Open Source Agreement, which is included\n[in this repository\'s license directory](license/LAR-20274-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf)\nand [on the Open Source Initiative website](https://opensource.org/license/nasa1-3-php/).\n\n\n### Developing\n\nDevelopment within this repository should occur on a feature branch.\nPull Requests (PRs) are created with a target of the `develop` branch before being reviewed and merged.\n\n### Installing locally\n\nFor local development, one can clone the repository and then use poetry or pip from the local directory:\n\n```console\ngit clone https://github.com/nasa/ncompare.git\n```\n\n###### (Option A) using poetry:\nii) Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n\niii) Run ```poetry install``` from the repository directory.\n\n###### (Option B) using pip:\n\nii) Run ```pip install .``` from the repository directory.\n\n\n### Testing locally\n\nIf installed using a `poetry` environment, the tests can be run with:\n```console\npoetry run pytest tests\n```\n\nOr from another virtual environment, one can use:\n```console\npytest tests\n```\n\n### To run as a locally installed poetry module\n\n```console\npoetry run ncompare <netcdf file #1> <netcdf file #2>\n```\n\n\n## Why ncompare?\n\nThe `cdo` (climate data operators) tool\n[does not support NetCDF4 groups](https://code.mpimet.mpg.de/boards/2/topics/12073).\nMoreover, `nco` operators\' `ncdiff` function computes value differences, but\n--- as far as the developers of this tool are aware ---\n`nco` does not have a simple function to show structural differences between NetCDF4 datasets.\n Note that `h5diff`, provided in the HDF5 software, can also be used to find differences.\nIn comparison to `h5diff`, `ncompare` is written and runnable in Python; `ncompare` provides _aligned_ and\n_colorized_ difference report for quicker assessments of groups, variable names, types, shapes, and attributes;\nand can generate report files formatted for other applications. However, note that\n`h5diff` provides comparison of some otherwise "hidden" hdf5 properties, such as _Netcdf4Dimid or _Netcdf4Coordinates,\nwhich are not currently assessed by `ncompare`.\n\n## Known limitations\n\n- `ncompare` uses `xarray` to access the root-level dimensions.\nIn some cases, `xarray` will miss dimensions whose names do not also exist as variable names in the dataset\n  (also known as non-coordinate dimensions).\n- Some underlying HDF5 properties, such as _Netcdf4Dimid or _Netcdf4Coordinates, are not currently assesssed by `ncompare`.\n\n# Notices:\n\nCopyright 2023 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.\n\n### Third-Party Software:\nThis software calls the following third-party software, which is subject to the terms and conditions of its licensor,\nas applicable at the time of licensing. Third-party software is not bundled with this software,\nbut may be available from the licensor.\n\nLicense hyperlinks are provided here for information purposes only:\n\n| item     |                               license                               | link                                                          |\n|:---------|:-------------------------------------------------------------------:|:--------------------------------------------------------------|\n| colorama |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |\n| netCDF4  |                             MIT License                             | https://opensource.org/licenses/MIT                           |\n| numpy    |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |\n| openpyxl |                             MIT License                             | https://opensource.org/licenses/MIT                           |\n| xarray   |                     Apache License, version 2.0                     | https://www.apache.org/licenses/LICENSE-2.0                   |\n| Python   | Standard Library Python Software Foundation (PSF) License Agreement | https://docs.python.org/3/license.html#psf-licenseDisclaimers |\n\n\n### No Warranty:\nTHE SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER EXPRESSED, IMPLIED,\nOR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS,\nANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM FROM INFRINGEMENT,\nANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE, OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED,\nWILL CONFORM TO THE SUBJECT SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER,\nCONSTITUTE AN ENDORSEMENT BY GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS, HARDWARE,\nSOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE SUBJECT SOFTWARE.\nFURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND LIABILITIES REGARDING THIRD-PARTY SOFTWARE,\nIF PRESENT IN THE ORIGINAL SOFTWARE, AND DISTRIBUTES IT "AS IS."\n\n### Waiver and Indemnity:\nRECIPIENT AGREES TO WAIVE ANY AND ALL CLAIMS AGAINST THE UNITED STATES GOVERNMENT,\nITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT. IF RECIPIENT\'S USE OF THE SUBJECT SOFTWARE RESULTS\nIN ANY LIABILITIES, DEMANDS, DAMAGES, EXPENSES OR LOSSES ARISING FROM SUCH USE, INCLUDING ANY DAMAGES FROM PRODUCTS\nBASED ON, OR RESULTING FROM, RECIPIENT\'S USE OF THE SUBJECT SOFTWARE, RECIPIENT SHALL INDEMNIFY AND HOLD HARMLESS\nTHE UNITED STATES GOVERNMENT, ITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT,\nTO THE EXTENT PERMITTED BY LAW. RECIPIENT\'S SOLE\nREMEDY FOR ANY SUCH MATTER SHALL BE THE IMMEDIATE, UNILATERAL TERMINATION OF THIS AGREEMENT.\n',
+    'long_description': '# ncompare\n_____\n\n<a href="https://www.repostatus.org/#active" target="_blank">\n    <img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed">\n</a>\n<a href="https://codecov.io/gh/nasa/ncompare">\n <img src="https://codecov.io/gh/nasa/ncompare/graph/badge.svg?token=5JJUNA1Z6S" alt="Code coverage">\n</a>\n<a href="https://ncompare.readthedocs.io/en/latest/?badge=latest">\n    <img src="https://readthedocs.org/projects/ncompare/badge/?version=latest" alt="Documentation Status">\n</a>\n<a href="https://pypi.org/project/ncompare/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/ncompare.svg" alt="Python Versions">\n</a>\n<a href="https://pypi.org/project/ncompare" target="_blank">\n    <img src="https://img.shields.io/pypi/v/ncompare?color=%2334D058label=pypi%20package" alt="Package version">\n</a>\n<a href="https://github.com/python/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">\n</a>\n<a href="https://mypy-lang.org/" target="_blank">\n    <img src="https://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">\n</a>\n<a href="https://github.com/nasa/ncompare/issues" target="_blank">\n    <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?" alt="Contributions welcome">\n</a>\n<a href="https://doi.org/10.5281/zenodo.10625407" target="_blank">\n    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.10625407.svg" alt="Zenodo">\n</a>\n<a href="https://github.com/pyOpenSci/software-review/issues/146" target="_blank">\n    <img src="https://tinyurl.com/y22nb8up?" alt="pyOpenSci">\n</a>\n\nCompare the structure of two NetCDF files at the command line.\n`ncompare` generates a view of the matching and non-matching groups and variables between two NetCDF datasets.\n\n\n## Installing\n\nInstall the latest version of the package from the Python Package Index (PyPI):\n```console\npip install ncompare\n```\n\n\n## Usage\n\nTo compare two netCDF files,\npass the filepaths for each of the two netCDF files directly to ncompare, as follows:\n\n```console\nncompare <netcdf file #1> <netcdf file #2>\n```\n\n<img src="https://github.com/nasa/ncompare/assets/114174502/1964096e-829d-4fe1-96a5-63581ade2d38" width="600" />\n\n\nWith an additional `--file-text` argument specified,\na common use of _ncompare_ may look like this example:\n\n```console\nncompare S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt\n```\n\n**A more complete usage demonstration with example output is shown in\n[this example notebook](https://ncompare.readthedocs.io/en/latest/example/ncompare-example-usage/).**\n\n### Options\n\n- `-h`, `--help` : Show this help message and exit.\n- `--file-text` [FILE_PATH]: Text file to write output to.\n- `--file-csv` [FILE_PATH]: Comma-separated values (CSV) file to write output to.\n- `--file-xlsx` [FILE_PATH]: Excel file to write output to.\n- `--only-diffs` : Only display variables and attributes that are different\n- `--no-color` : Turn off all colorized output.\n- `--show-attributes` : Include variable attributes in the table that compares variables.\n- `--show-chunks` : Include chunk sizes in the table that compares variables.\n- `-v` (`--comparison_var_name`) [VAR_NAME]: Compare specific values for this variable.\n- `-g` (`--comparison_var_group`) [VAR_GROUP]: Group that contains the `comparison_var_name`.\n- `--column-widths` [WIDTH, WIDTH, WIDTH]: Width, in number of characters, of the three columns in the comparison report\n- `--version` : Show the current version and then exit.\n\n## Contributing\n\nContributions are welcome! For more information, see [CONTRIBUTING.md](CONTRIBUTING.md).\n_ncompare_ is licensed under the Apache License 2.0,\nwhich is included in the [LICENSE](LICENSE) file.\n\n\n### Developing\n\nDevelopment within this repository should occur on a feature branch.\nPull Requests (PRs) are created with a target of the `develop` branch before being reviewed and merged.\n\n### Installing locally\n\nFor local development, one can clone the repository and then use poetry or pip from the local directory:\n\n```console\ngit clone https://github.com/nasa/ncompare.git\n```\n\n###### (Option A) using poetry:\nii) Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n\niii) Run ```poetry install``` from the repository directory.\n\n###### (Option B) using pip:\n\nii) Run ```pip install .``` from the repository directory.\n\n\n### Testing locally\n\nIf installed using a `poetry` environment, the tests can be run with:\n```console\npoetry run pytest tests\n```\n\nOr from another virtual environment, one can use:\n```console\npytest tests\n```\n\n### To run as a locally installed poetry module\n\n```console\npoetry run ncompare <netcdf file #1> <netcdf file #2>\n```\n\n\n## Why ncompare?\n\nThe `cdo` (climate data operators) tool\n[does not support NetCDF4 groups](https://code.mpimet.mpg.de/boards/2/topics/12073).\nMoreover, `nco` operators\' `ncdiff` function computes value differences, but\n--- as far as the developers of this tool are aware ---\n`nco` does not have a simple function to show structural differences between NetCDF4 datasets.\n Note that `h5diff`, provided in the HDF5 software, can also be used to find differences.\nIn comparison to `h5diff`, `ncompare` is written and runnable in Python; `ncompare` provides _aligned_ and\n_colorized_ difference report for quicker assessments of groups, variable names, types, shapes, and attributes;\nand can generate report files formatted for other applications. However, note that\n`h5diff` provides comparison of some otherwise "hidden" hdf5 properties, such as _Netcdf4Dimid or _Netcdf4Coordinates,\nwhich are not currently assessed by `ncompare`.\n\n## Known limitations\n\n- `ncompare` uses `xarray` to access the root-level dimensions.\nIn some cases, `xarray` will miss dimensions whose names do not also exist as variable names in the dataset\n  (also known as non-coordinate dimensions).\n- Some underlying HDF5 properties, such as _Netcdf4Dimid or _Netcdf4Coordinates, are not currently assesssed by `ncompare`.\n\n# Notices:\n\nCopyright 2023 United States Government as represented by the Administrator of the\nNational Aeronautics and Space Administration. All Rights Reserved.\n\nThis software calls the following third-party software,\nwhich is subject to the terms and conditions of its licensor,\nas applicable at the time of licensing.\nThe third-party software is not bundled with this software but may be available from the licensor.\n\nLicense hyperlinks are provided here for information purposes only.\n\n\n| Title    |                               license                               | link                                                          |\n|:---------|:-------------------------------------------------------------------:|:--------------------------------------------------------------|\n| colorama |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |\n| netCDF4  |                             MIT License                             | https://opensource.org/licenses/MIT                           |\n| numpy    |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |\n| openpyxl |                             MIT License                             | https://opensource.org/licenses/MIT                           |\n| xarray   |                     Apache License, version 2.0                     | https://www.apache.org/licenses/LICENSE-2.0                   |\n| Python   | Standard Library Python Software Foundation (PSF) License Agreement | https://docs.python.org/3/license.html#psf-licenseDisclaimers |\n\n\nThe ncompare: NetCDF structural comparison tool framework is licensed under the Apache License,\nVersion 2.0 (the "License");\nyou may not use this application except in compliance with the License.\nYou may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.\n\nUnless required by applicable law or agreed to in writing,\nsoftware distributed under the License is distributed on an "AS IS" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and limitations under the License.\n\n---\nThis package is NASA Software Release Authorization (SRA) # LAR-20274-1\n',
     'author': 'Daniel Kaufman',
     'author_email': 'daniel.kaufman@nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nasa/ncompare',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,51 +1,49 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['ncompare']
 package_data = \ {'': ['*']} install_requires = \ ['colorama>=0.4.6,<0.5.0',
 'netCDF4>=1.6.4,<2.0.0', 'numpy>=1.26.0,<2.0.0', 'openpyxl>=3.1.2,<4.0.0',
 'xarray>=2023.9,<2025.0'] entry_points = \ {'console_scripts': ['ncompare =
 ncompare.console:main']} setup_kwargs = { 'name': 'ncompare', 'version':
-'1.8.0', 'description': 'Compare the structure of two NetCDF files at the
+'1.9.0', 'description': 'Compare the structure of two NetCDF files at the
 command line', 'long_description': '# ncompare\n_____\n\n_\_n_ _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:
 _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d_ _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y
 _d_e_v_e_l_o_p_e_d_]_\_n\n_\_n_ _[_C_o_d_e_ _c_o_v_e_r_a_g_e_]_\_n\n_\_n_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_\_n\n_\_n_ _[_P_y_t_h_o_n
 _V_e_r_s_i_o_n_s_]_\_n\n_\_n_ _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_\_n\n_\_n_ _[_C_o_d_e_ _s_t_y_l_e_]_\_n\n_\_n_ _[_M_y_p_y_ _c_h_e_c_k_e_d_]_\_n\n_\_n
 _[_C_o_n_t_r_i_b_u_t_i_o_n_s_ _w_e_l_c_o_m_e_]_\_n\n_\_n_ _[_Z_e_n_o_d_o_]_\_n\n_\_n_ _[_p_y_O_p_e_n_S_c_i_]_\_n\n\nCompare the
 structure of two NetCDF files at the command line.\n`ncompare` generates a view
 of the matching and non-matching groups and variables between two NetCDF
 datasets.\n\n\n## Installing\n\nInstall the latest version of the package from
 the Python Package Index (PyPI):\n```console\npip install ncompare\n```\n\n\n##
 Usage\n\nTo compare two netCDF files,\npass the filepaths for each of the two
 netCDF files directly to ncompare, as follows:\n\n```console\nncompare
-\n```\n\nWith an additional `--file-text` argument specified,\na common use of
-_ncompare_ may look like this example:\n\n```console\nncompare S001G01.nc
-S001G01_SUBSET.nc --file-text subset_comparison.txt\n```\n\n\n**A more complete
-usage demonstration with example output is shown in\n[this example notebook]
-(https://ncompare.readthedocs.io/en/latest/example/ncompare-example-usage/
-).**\n\n### Options\n\n- `-h`, `--help` : Show this help message and exit.\n-
-`--file-text` [FILE_PATH]: Text file to write output to.\n- `--file-csv`
-[FILE_PATH]: Comma-separated values (CSV) file to write output to.\n- `--file-
-xlsx` [FILE_PATH]: Excel file to write output to.\n- `--only-diffs` : Only
+\n```\n\n[https://github.com/nasa/ncompare/assets/114174502/1964096e-829d-4fe1-
+96a5-63581ade2d38]\n\n\nWith an additional `--file-text` argument specified,\na
+common use of _ncompare_ may look like this example:\n\n```console\nncompare
+S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt\n```\n\n**A more
+complete usage demonstration with example output is shown in\n[this example
+notebook](https://ncompare.readthedocs.io/en/latest/example/ncompare-example-
+usage/).**\n\n### Options\n\n- `-h`, `--help` : Show this help message and
+exit.\n- `--file-text` [FILE_PATH]: Text file to write output to.\n- `--file-
+csv` [FILE_PATH]: Comma-separated values (CSV) file to write output to.\n- `--
+file-xlsx` [FILE_PATH]: Excel file to write output to.\n- `--only-diffs` : Only
 display variables and attributes that are different\n- `--no-color` : Turn off
 all colorized output.\n- `--show-attributes` : Include variable attributes in
 the table that compares variables.\n- `--show-chunks` : Include chunk sizes in
 the table that compares variables.\n- `-v` (`--comparison_var_name`)
 [VAR_NAME]: Compare specific values for this variable.\n- `-g` (`--
 comparison_var_group`) [VAR_GROUP]: Group that contains the
 `comparison_var_name`.\n- `--column-widths` [WIDTH, WIDTH, WIDTH]: Width, in
 number of characters, of the three columns in the comparison report\n- `--
 version` : Show the current version and then exit.\n\n##
 Contributing\n\nContributions are welcome! For more information, see
-[CONTRIBUTING.md](CONTRIBUTING.md).\n_ncompare_ is licensed under the NASA Open
-Source Agreement, which is included\n[in this repository\'s license directory]
-(license/LAR-20274-
-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf)\nand [on the Open
-Source Initiative website](https://opensource.org/license/nasa1-3-php/
-).\n\n\n### Developing\n\nDevelopment within this repository should occur on a
-feature branch.\nPull Requests (PRs) are created with a target of the `develop`
-branch before being reviewed and merged.\n\n### Installing locally\n\nFor local
+[CONTRIBUTING.md](CONTRIBUTING.md).\n_ncompare_ is licensed under the Apache
+License 2.0,\nwhich is included in the [LICENSE](LICENSE) file.\n\n\n###
+Developing\n\nDevelopment within this repository should occur on a feature
+branch.\nPull Requests (PRs) are created with a target of the `develop` branch
+before being reviewed and merged.\n\n### Installing locally\n\nFor local
 development, one can clone the repository and then use poetry or pip from the
 local directory:\n\n```console\ngit clone https://github.com/nasa/
 ncompare.git\n```\n\n###### (Option A) using poetry:\nii) Follow the
 instructions for installing `poetry` [here](https://python-poetry.org/docs/
 ).\n\niii) Run ```poetry install``` from the repository directory.\n\n######
 (Option B) using pip:\n\nii) Run ```pip install .``` from the repository
 directory.\n\n\n### Testing locally\n\nIf installed using a `poetry`
@@ -67,49 +65,36 @@
 _Netcdf4Coordinates,\nwhich are not currently assessed by `ncompare`.\n\n##
 Known limitations\n\n- `ncompare` uses `xarray` to access the root-level
 dimensions.\nIn some cases, `xarray` will miss dimensions whose names do not
 also exist as variable names in the dataset\n (also known as non-coordinate
 dimensions).\n- Some underlying HDF5 properties, such as _Netcdf4Dimid or
 _Netcdf4Coordinates, are not currently assesssed by `ncompare`.\n\n# Notices:
 \n\nCopyright 2023 United States Government as represented by the Administrator
-of the National Aeronautics and Space Administration. All Rights
-Reserved.\n\n### Third-Party Software:\nThis software calls the following
-third-party software, which is subject to the terms and conditions of its
-licensor,\nas applicable at the time of licensing. Third-party software is not
-bundled with this software,\nbut may be available from the licensor.\n\nLicense
-hyperlinks are provided here for information purposes only:\n\n| item | license
-| link |\n|:---------|:--------------------------------------------------------
------------:|:--------------------------------------------------------------
-|\n| colorama | BSD-3-Clause | https://opensource.org/licenses/BSD-3-Clause
-|\n| netCDF4 | MIT License | https://opensource.org/licenses/MIT |\n| numpy |
-BSD-3-Clause | https://opensource.org/licenses/BSD-3-Clause |\n| openpyxl | MIT
-License | https://opensource.org/licenses/MIT |\n| xarray | Apache License,
-version 2.0 | https://www.apache.org/licenses/LICENSE-2.0 |\n| Python |
-Standard Library Python Software Foundation (PSF) License Agreement | https://
-docs.python.org/3/license.html#psf-licenseDisclaimers |\n\n\n### No Warranty:
-\nTHE SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND,
-EITHER EXPRESSED, IMPLIED,\nOR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY
-WARRANTY THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS,\nANY IMPLIED
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM
-FROM INFRINGEMENT,\nANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE,
-OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED,\nWILL CONFORM TO THE SUBJECT
-SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER,\nCONSTITUTE AN ENDORSEMENT BY
-GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS,
-HARDWARE,\nSOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF
-THE SUBJECT SOFTWARE.\nFURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND
-LIABILITIES REGARDING THIRD-PARTY SOFTWARE,\nIF PRESENT IN THE ORIGINAL
-SOFTWARE, AND DISTRIBUTES IT "AS IS."\n\n### Waiver and Indemnity:\nRECIPIENT
-AGREES TO WAIVE ANY AND ALL CLAIMS AGAINST THE UNITED STATES GOVERNMENT,\nITS
-CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT. IF RECIPIENT\'S
-USE OF THE SUBJECT SOFTWARE RESULTS\nIN ANY LIABILITIES, DEMANDS, DAMAGES,
-EXPENSES OR LOSSES ARISING FROM SUCH USE, INCLUDING ANY DAMAGES FROM
-PRODUCTS\nBASED ON, OR RESULTING FROM, RECIPIENT\'S USE OF THE SUBJECT
-SOFTWARE, RECIPIENT SHALL INDEMNIFY AND HOLD HARMLESS\nTHE UNITED STATES
-GOVERNMENT, ITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR
-RECIPIENT,\nTO THE EXTENT PERMITTED BY LAW. RECIPIENT\'S SOLE\nREMEDY FOR ANY
-SUCH MATTER SHALL BE THE IMMEDIATE, UNILATERAL TERMINATION OF THIS
-AGREEMENT.\n', 'author': 'Daniel Kaufman', 'author_email':
-'daniel.kaufman@nasa.gov', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'https://github.com/nasa/ncompare', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.9,<3.13', } setup
-(**setup_kwargs)
+of the\nNational Aeronautics and Space Administration. All Rights
+Reserved.\n\nThis software calls the following third-party software,\nwhich is
+subject to the terms and conditions of its licensor,\nas applicable at the time
+of licensing.\nThe third-party software is not bundled with this software but
+may be available from the licensor.\n\nLicense hyperlinks are provided here for
+information purposes only.\n\n\n| Title | license | link |\n|:---------|:------
+-------------------------------------------------------------:|:---------------
+-----------------------------------------------|\n| colorama | BSD-3-Clause |
+https://opensource.org/licenses/BSD-3-Clause |\n| netCDF4 | MIT License |
+https://opensource.org/licenses/MIT |\n| numpy | BSD-3-Clause | https://
+opensource.org/licenses/BSD-3-Clause |\n| openpyxl | MIT License | https://
+opensource.org/licenses/MIT |\n| xarray | Apache License, version 2.0 | https:/
+/www.apache.org/licenses/LICENSE-2.0 |\n| Python | Standard Library Python
+Software Foundation (PSF) License Agreement | https://docs.python.org/3/
+license.html#psf-licenseDisclaimers |\n\n\nThe ncompare: NetCDF structural
+comparison tool framework is licensed under the Apache License,\nVersion 2.0
+(the "License");\nyou may not use this application except in compliance with
+the License.\nYou may obtain a copy of the License at http://www.apache.org/
+licenses/LICENSE-2.0.\n\nUnless required by applicable law or agreed to in
+writing,\nsoftware distributed under the License is distributed on an "AS IS"
+BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+implied.\nSee the License for the specific language governing permissions and
+limitations under the License.\n\n---\nThis package is NASA Software Release
+Authorization (SRA) # LAR-20274-1\n', 'author': 'Daniel Kaufman',
+'author_email': 'daniel.kaufman@nasa.gov', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://github.com/nasa/ncompare',
+'packages': packages, 'package_data': package_data, 'install_requires':
+install_requires, 'entry_points': entry_points, 'python_requires':
+'>=3.9,<3.13', } setup(**setup_kwargs)
```

### Comparing `ncompare-1.8.0/PKG-INFO` & `ncompare-1.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ncompare
-Version: 1.8.0
+Version: 1.9.0
 Summary: Compare the structure of two NetCDF files at the command line
 Home-page: https://github.com/nasa/ncompare
-License: license/LAR-20274-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf
+License: Apache-2.0
 Author: Daniel Kaufman
 Author-email: daniel.kaufman@nasa.gov
 Requires-Python: >=3.9,<3.13
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -81,22 +81,24 @@
 To compare two netCDF files,
 pass the filepaths for each of the two netCDF files directly to ncompare, as follows:
 
 ```console
 ncompare <netcdf file #1> <netcdf file #2>
 ```
 
+<img src="https://github.com/nasa/ncompare/assets/114174502/1964096e-829d-4fe1-96a5-63581ade2d38" width="600" />
+
+
 With an additional `--file-text` argument specified,
 a common use of _ncompare_ may look like this example:
 
 ```console
 ncompare S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt
 ```
 
-
 **A more complete usage demonstration with example output is shown in
 [this example notebook](https://ncompare.readthedocs.io/en/latest/example/ncompare-example-usage/).**
 
 ### Options
 
 - `-h`, `--help` : Show this help message and exit.
 - `--file-text` [FILE_PATH]: Text file to write output to.
@@ -110,17 +112,16 @@
 - `-g` (`--comparison_var_group`) [VAR_GROUP]: Group that contains the `comparison_var_name`.
 - `--column-widths` [WIDTH, WIDTH, WIDTH]: Width, in number of characters, of the three columns in the comparison report
 - `--version` : Show the current version and then exit.
 
 ## Contributing
 
 Contributions are welcome! For more information, see [CONTRIBUTING.md](CONTRIBUTING.md).
-_ncompare_ is licensed under the NASA Open Source Agreement, which is included
-[in this repository's license directory](license/LAR-20274-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf)
-and [on the Open Source Initiative website](https://opensource.org/license/nasa1-3-php/).
+_ncompare_ is licensed under the Apache License 2.0,
+which is included in the [LICENSE](LICENSE) file.
 
 
 ### Developing
 
 Development within this repository should occur on a feature branch.
 Pull Requests (PRs) are created with a target of the `develop` branch before being reviewed and merged.
 
@@ -180,46 +181,41 @@
 - `ncompare` uses `xarray` to access the root-level dimensions.
 In some cases, `xarray` will miss dimensions whose names do not also exist as variable names in the dataset
   (also known as non-coordinate dimensions).
 - Some underlying HDF5 properties, such as _Netcdf4Dimid or _Netcdf4Coordinates, are not currently assesssed by `ncompare`.
 
 # Notices:
 
-Copyright 2023 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
+Copyright 2023 United States Government as represented by the Administrator of the
+National Aeronautics and Space Administration. All Rights Reserved.
 
-### Third-Party Software:
-This software calls the following third-party software, which is subject to the terms and conditions of its licensor,
-as applicable at the time of licensing. Third-party software is not bundled with this software,
-but may be available from the licensor.
+This software calls the following third-party software,
+which is subject to the terms and conditions of its licensor,
+as applicable at the time of licensing.
+The third-party software is not bundled with this software but may be available from the licensor.
 
-License hyperlinks are provided here for information purposes only:
+License hyperlinks are provided here for information purposes only.
 
-| item     |                               license                               | link                                                          |
+
+| Title    |                               license                               | link                                                          |
 |:---------|:-------------------------------------------------------------------:|:--------------------------------------------------------------|
 | colorama |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |
 | netCDF4  |                             MIT License                             | https://opensource.org/licenses/MIT                           |
 | numpy    |                            BSD-3-Clause                             | https://opensource.org/licenses/BSD-3-Clause                  |
 | openpyxl |                             MIT License                             | https://opensource.org/licenses/MIT                           |
 | xarray   |                     Apache License, version 2.0                     | https://www.apache.org/licenses/LICENSE-2.0                   |
 | Python   | Standard Library Python Software Foundation (PSF) License Agreement | https://docs.python.org/3/license.html#psf-licenseDisclaimers |
 
 
-### No Warranty:
-THE SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER EXPRESSED, IMPLIED,
-OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS,
-ANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM FROM INFRINGEMENT,
-ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE, OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED,
-WILL CONFORM TO THE SUBJECT SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER,
-CONSTITUTE AN ENDORSEMENT BY GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS, HARDWARE,
-SOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE SUBJECT SOFTWARE.
-FURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND LIABILITIES REGARDING THIRD-PARTY SOFTWARE,
-IF PRESENT IN THE ORIGINAL SOFTWARE, AND DISTRIBUTES IT "AS IS."
-
-### Waiver and Indemnity:
-RECIPIENT AGREES TO WAIVE ANY AND ALL CLAIMS AGAINST THE UNITED STATES GOVERNMENT,
-ITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT. IF RECIPIENT'S USE OF THE SUBJECT SOFTWARE RESULTS
-IN ANY LIABILITIES, DEMANDS, DAMAGES, EXPENSES OR LOSSES ARISING FROM SUCH USE, INCLUDING ANY DAMAGES FROM PRODUCTS
-BASED ON, OR RESULTING FROM, RECIPIENT'S USE OF THE SUBJECT SOFTWARE, RECIPIENT SHALL INDEMNIFY AND HOLD HARMLESS
-THE UNITED STATES GOVERNMENT, ITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT,
-TO THE EXTENT PERMITTED BY LAW. RECIPIENT'S SOLE
-REMEDY FOR ANY SUCH MATTER SHALL BE THE IMMEDIATE, UNILATERAL TERMINATION OF THIS AGREEMENT.
+The ncompare: NetCDF structural comparison tool framework is licensed under the Apache License,
+Version 2.0 (the "License");
+you may not use this application except in compliance with the License.
+You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
+
+Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and limitations under the License.
+
+---
+This package is NASA Software Release Authorization (SRA) # LAR-20274-1
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: ncompare Version: 1.8.0 Summary: Compare the
+Metadata-Version: 2.1 Name: ncompare Version: 1.9.0 Summary: Compare the
 structure of two NetCDF files at the command line Home-page: https://
-github.com/nasa/ncompare License: license/LAR-20274-
-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf Author: Daniel
-Kaufman Author-email: daniel.kaufman@nasa.gov Requires-Python: >=3.9,<3.13
-Classifier: Environment :: Console Classifier: Intended Audience :: Science/
-Research Classifier: License :: Other/Proprietary License Classifier: Operating
-System :: MacOS Classifier: Operating System :: Microsoft :: Windows
+github.com/nasa/ncompare License: Apache-2.0 Author: Daniel Kaufman Author-
+email: daniel.kaufman@nasa.gov Requires-Python: >=3.9,<3.13 Classifier:
+Environment :: Console Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Dist:
@@ -22,95 +21,81 @@
 _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]_[_C_o_n_t_r_i_b_u_t_i_o_n_s
 _w_e_l_c_o_m_e_]_[_Z_e_n_o_d_o_]_[_p_y_O_p_e_n_S_c_i_]Compare the structure of two NetCDF files at the
 command line. `ncompare` generates a view of the matching and non-matching
 groups and variables between two NetCDF datasets. ## Installing Install the
 latest version of the package from the Python Package Index (PyPI): ```console
 pip install ncompare ``` ## Usage To compare two netCDF files, pass the
 filepaths for each of the two netCDF files directly to ncompare, as follows:
-```console ncompare ``` With an additional `--file-text` argument specified, a
-common use of _ncompare_ may look like this example: ```console ncompare
-S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt ``` **A more
-complete usage demonstration with example output is shown in [this example
+```console ncompare ``` [https://github.com/nasa/ncompare/assets/114174502/
+1964096e-829d-4fe1-96a5-63581ade2d38]With an additional `--file-text` argument
+specified, a common use of _ncompare_ may look like this example: ```console
+ncompare S001G01.nc S001G01_SUBSET.nc --file-text subset_comparison.txt ``` **A
+more complete usage demonstration with example output is shown in [this example
 notebook](https://ncompare.readthedocs.io/en/latest/example/ncompare-example-
 usage/).** ### Options - `-h`, `--help` : Show this help message and exit. - `-
 -file-text` [FILE_PATH]: Text file to write output to. - `--file-csv`
 [FILE_PATH]: Comma-separated values (CSV) file to write output to. - `--file-
 xlsx` [FILE_PATH]: Excel file to write output to. - `--only-diffs` : Only
 display variables and attributes that are different - `--no-color` : Turn off
 all colorized output. - `--show-attributes` : Include variable attributes in
 the table that compares variables. - `--show-chunks` : Include chunk sizes in
 the table that compares variables. - `-v` (`--comparison_var_name`) [VAR_NAME]:
 Compare specific values for this variable. - `-g` (`--comparison_var_group`)
 [VAR_GROUP]: Group that contains the `comparison_var_name`. - `--column-widths`
 [WIDTH, WIDTH, WIDTH]: Width, in number of characters, of the three columns in
 the comparison report - `--version` : Show the current version and then exit.
 ## Contributing Contributions are welcome! For more information, see
-[CONTRIBUTING.md](CONTRIBUTING.md). _ncompare_ is licensed under the NASA Open
-Source Agreement, which is included [in this repository's license directory]
-(license/LAR-20274-1_ncompare_NetCDF_structural_comparison_tool_NOSA_1.3.pdf)
-and [on the Open Source Initiative website](https://opensource.org/license/
-nasa1-3-php/). ### Developing Development within this repository should occur
-on a feature branch. Pull Requests (PRs) are created with a target of the
-`develop` branch before being reviewed and merged. ### Installing locally For
-local development, one can clone the repository and then use poetry or pip from
-the local directory: ```console git clone https://github.com/nasa/ncompare.git
-``` ###### (Option A) using poetry: ii) Follow the instructions for installing
-`poetry` [here](https://python-poetry.org/docs/). iii) Run ```poetry install```
-from the repository directory. ###### (Option B) using pip: ii) Run ```pip
-install .``` from the repository directory. ### Testing locally If installed
-using a `poetry` environment, the tests can be run with: ```console poetry run
-pytest tests ``` Or from another virtual environment, one can use: ```console
-pytest tests ``` ### To run as a locally installed poetry module ```console
-poetry run ncompare ``` ## Why ncompare? The `cdo` (climate data operators)
-tool [does not support NetCDF4 groups](https://code.mpimet.mpg.de/boards/2/
-topics/12073). Moreover, `nco` operators' `ncdiff` function computes value
-differences, but --- as far as the developers of this tool are aware --- `nco`
-does not have a simple function to show structural differences between NetCDF4
-datasets. Note that `h5diff`, provided in the HDF5 software, can also be used
-to find differences. In comparison to `h5diff`, `ncompare` is written and
-runnable in Python; `ncompare` provides _aligned_ and _colorized_ difference
-report for quicker assessments of groups, variable names, types, shapes, and
-attributes; and can generate report files formatted for other applications.
-However, note that `h5diff` provides comparison of some otherwise "hidden" hdf5
-properties, such as _Netcdf4Dimid or _Netcdf4Coordinates, which are not
-currently assessed by `ncompare`. ## Known limitations - `ncompare` uses
-`xarray` to access the root-level dimensions. In some cases, `xarray` will miss
-dimensions whose names do not also exist as variable names in the dataset (also
-known as non-coordinate dimensions). - Some underlying HDF5 properties, such as
-_Netcdf4Dimid or _Netcdf4Coordinates, are not currently assesssed by
-`ncompare`. # Notices: Copyright 2023 United States Government as represented
-by the Administrator of the National Aeronautics and Space Administration. All
-Rights Reserved. ### Third-Party Software: This software calls the following
-third-party software, which is subject to the terms and conditions of its
-licensor, as applicable at the time of licensing. Third-party software is not
-bundled with this software, but may be available from the licensor. License
-hyperlinks are provided here for information purposes only: | item | license |
-link | |:---------|:-----------------------------------------------------------
---------:|:--------------------------------------------------------------| |
-colorama | BSD-3-Clause | https://opensource.org/licenses/BSD-3-Clause | |
-netCDF4 | MIT License | https://opensource.org/licenses/MIT | | numpy | BSD-3-
-Clause | https://opensource.org/licenses/BSD-3-Clause | | openpyxl | MIT
-License | https://opensource.org/licenses/MIT | | xarray | Apache License,
-version 2.0 | https://www.apache.org/licenses/LICENSE-2.0 | | Python | Standard
-Library Python Software Foundation (PSF) License Agreement | https://
-docs.python.org/3/license.html#psf-licenseDisclaimers | ### No Warranty: THE
-SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER
-EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY
-THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM
-FROM INFRINGEMENT, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE,
-OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED, WILL CONFORM TO THE SUBJECT
-SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER, CONSTITUTE AN ENDORSEMENT BY
-GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS,
-HARDWARE, SOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE
-SUBJECT SOFTWARE. FURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND
-LIABILITIES REGARDING THIRD-PARTY SOFTWARE, IF PRESENT IN THE ORIGINAL
-SOFTWARE, AND DISTRIBUTES IT "AS IS." ### Waiver and Indemnity: RECIPIENT
-AGREES TO WAIVE ANY AND ALL CLAIMS AGAINST THE UNITED STATES GOVERNMENT, ITS
-CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT. IF RECIPIENT'S
-USE OF THE SUBJECT SOFTWARE RESULTS IN ANY LIABILITIES, DEMANDS, DAMAGES,
-EXPENSES OR LOSSES ARISING FROM SUCH USE, INCLUDING ANY DAMAGES FROM PRODUCTS
-BASED ON, OR RESULTING FROM, RECIPIENT'S USE OF THE SUBJECT SOFTWARE, RECIPIENT
-SHALL INDEMNIFY AND HOLD HARMLESS THE UNITED STATES GOVERNMENT, ITS CONTRACTORS
-AND SUBCONTRACTORS, AS WELL AS ANY PRIOR RECIPIENT, TO THE EXTENT PERMITTED BY
-LAW. RECIPIENT'S SOLE REMEDY FOR ANY SUCH MATTER SHALL BE THE IMMEDIATE,
-UNILATERAL TERMINATION OF THIS AGREEMENT.
+[CONTRIBUTING.md](CONTRIBUTING.md). _ncompare_ is licensed under the Apache
+License 2.0, which is included in the [LICENSE](LICENSE) file. ### Developing
+Development within this repository should occur on a feature branch. Pull
+Requests (PRs) are created with a target of the `develop` branch before being
+reviewed and merged. ### Installing locally For local development, one can
+clone the repository and then use poetry or pip from the local directory:
+```console git clone https://github.com/nasa/ncompare.git ``` ###### (Option A)
+using poetry: ii) Follow the instructions for installing `poetry` [here](https:
+//python-poetry.org/docs/). iii) Run ```poetry install``` from the repository
+directory. ###### (Option B) using pip: ii) Run ```pip install .``` from the
+repository directory. ### Testing locally If installed using a `poetry`
+environment, the tests can be run with: ```console poetry run pytest tests ```
+Or from another virtual environment, one can use: ```console pytest tests ```
+### To run as a locally installed poetry module ```console poetry run ncompare
+``` ## Why ncompare? The `cdo` (climate data operators) tool [does not support
+NetCDF4 groups](https://code.mpimet.mpg.de/boards/2/topics/12073). Moreover,
+`nco` operators' `ncdiff` function computes value differences, but --- as far
+as the developers of this tool are aware --- `nco` does not have a simple
+function to show structural differences between NetCDF4 datasets. Note that
+`h5diff`, provided in the HDF5 software, can also be used to find differences.
+In comparison to `h5diff`, `ncompare` is written and runnable in Python;
+`ncompare` provides _aligned_ and _colorized_ difference report for quicker
+assessments of groups, variable names, types, shapes, and attributes; and can
+generate report files formatted for other applications. However, note that
+`h5diff` provides comparison of some otherwise "hidden" hdf5 properties, such
+as _Netcdf4Dimid or _Netcdf4Coordinates, which are not currently assessed by
+`ncompare`. ## Known limitations - `ncompare` uses `xarray` to access the root-
+level dimensions. In some cases, `xarray` will miss dimensions whose names do
+not also exist as variable names in the dataset (also known as non-coordinate
+dimensions). - Some underlying HDF5 properties, such as _Netcdf4Dimid or
+_Netcdf4Coordinates, are not currently assesssed by `ncompare`. # Notices:
+Copyright 2023 United States Government as represented by the Administrator of
+the National Aeronautics and Space Administration. All Rights Reserved. This
+software calls the following third-party software, which is subject to the
+terms and conditions of its licensor, as applicable at the time of licensing.
+The third-party software is not bundled with this software but may be available
+from the licensor. License hyperlinks are provided here for information
+purposes only. | Title | license | link | |:---------|:------------------------
+-------------------------------------------:|:---------------------------------
+-----------------------------| | colorama | BSD-3-Clause | https://
+opensource.org/licenses/BSD-3-Clause | | netCDF4 | MIT License | https://
+opensource.org/licenses/MIT | | numpy | BSD-3-Clause | https://opensource.org/
+licenses/BSD-3-Clause | | openpyxl | MIT License | https://opensource.org/
+licenses/MIT | | xarray | Apache License, version 2.0 | https://www.apache.org/
+licenses/LICENSE-2.0 | | Python | Standard Library Python Software Foundation
+(PSF) License Agreement | https://docs.python.org/3/license.html#psf-
+licenseDisclaimers | The ncompare: NetCDF structural comparison tool framework
+is licensed under the Apache License, Version 2.0 (the "License"); you may not
+use this application except in compliance with the License. You may obtain a
+copy of the License at http://www.apache.org/licenses/LICENSE-2.0. Unless
+required by applicable law or agreed to in writing, software distributed under
+the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
+CONDITIONS OF ANY KIND, either express or implied. See the License for the
+specific language governing permissions and limitations under the License. --
+- This package is NASA Software Release Authorization (SRA) # LAR-20274-1
```

