# Comparing `tmp/arcana_bids-0.2.6.tar.gz` & `tmp/arcana_bids-0.2.7.tar.gz`

## Comparing `arcana_bids-0.2.6.tar` & `arcana_bids-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/_version.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/cli.py
--rw-r--r--   0        0        0    23318 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/data.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/deploy.py
--rw-r--r--   0        0        0    15435 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tasks.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tests/test_cli.py
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tests/test_data.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tests/test_tasks.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/LICENSE
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/README.rst
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/_version.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/cli.py
+-rw-r--r--   0        0        0    23318 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/data.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/deploy.py
+-rw-r--r--   0        0        0    14808 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/tasks.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/tests/test_cli.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/tests/test_data.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/arcana/bids/tests/test_tasks.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/README.rst
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 arcana_bids-0.2.7/PKG-INFO
```

### Comparing `arcana_bids-0.2.6/arcana/bids/cli.py` & `arcana_bids-0.2.7/arcana/bids/cli.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.6/arcana/bids/data.py` & `arcana_bids-0.2.7/arcana/bids/data.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.6/arcana/bids/tasks.py` & `arcana_bids-0.2.7/arcana/bids/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 import tempfile
 import logging
 import typing as ty
 import shutil
 import shlex
 from pathlib import Path
 from pydra import Workflow
-from pydra.engine.task import DockerTask, SingularityTask, ShellCommandTask
+from pydra.engine.task import ShellCommandTask
 from pydra.engine.specs import (
     ShellSpec,
     SpecInfo,
-    DockerSpec,
-    SingularitySpec,
     ShellOutSpec,
 )
+from pydra.engine.environments import Docker, Native
 from arcana.core import __version__
 from arcana.core.data.set import Dataset
 from fileformats.core import FileSet
 from fileformats.generic import Directory
 from arcana.common import Clinical
 from arcana.bids.data import JsonEdit
-from arcana.core.exceptions import ArcanaUsageError
 from arcana.core.utils.serialize import (
     ClassResolver,
     ObjectListConverter,
 )
 from arcana.core.utils.misc import func_task
 from .data import Bids
 
@@ -79,15 +77,15 @@
         The inputs to be inserted into the BIDS dataset. Should be a list of tuples
         consisting of the the path the file/directory should be stored within a BIDS subject/session,
         e.g. anat/T1w, func/bold, and the DataFormat class it should be stored in, e.g.
         arcana.bids.data.NiftiGzX.
     outputs : list[ty.Union[AppField, dict[str, str]]]
         The outputs to be extracted from the derivatives directory. Should be a list of tuples
         consisting of the the path the file/directory is saved by the app within a BIDS subject/session,
-        e.g. freesurfer/recon-all, and the DataFormat class it is stored in, 
+        e.g. freesurfer/recon-all, and the DataFormat class it is stored in,
     executable : str, optional
         Name of the executable within the image to run (i.e. the entrypoint of the image).
         Required when extending the base image and launching Arcana within it. Defaults to
         empty string, i.e. the entrypoint of the BIDS app container image
     container_image : str, optional
         Name of the BIDS app image to wrap
     parameters : dict[str, type], optional
@@ -147,15 +145,15 @@
             name=name + "_dataset",
             leaves=[(DEFAULT_BIDS_ID,)],
             metadata={
                 "authors": [
                     f"Auto-generated by Arcana {__version__}",
                     "Dummy second author",
                 ]
-            }
+            },
         )
         wf_kwargs = {"id": DEFAULT_BIDS_ID}
     else:
         wf_kwargs = {}
 
     # Convert from JSON format inputs/outputs to tuples with resolved data formats
     inputs = ObjectListConverter(BidsInput)(inputs)
@@ -223,54 +221,38 @@
         )
 
     kwargs = {p: getattr(wf.lzin, p) for p in parameters}
 
     # If 'image' is None, don't use any virtualisation (i.e. assume we are running from "inside" the
     # container or extension of it)
     if container_image is None:
-        task_cls = ShellCommandTask
-        base_spec_cls = ShellSpec
-        kwargs["executable"] = executable
         app_output_path = str(app_output_dir)
+        environment = Native()
     else:
-
-        # Set input and output directories to "internal" paths within the
-        # container
-        # app_dataset_path = CONTAINER_DATASET_PATH
+        environment = Docker(container_image)
         app_output_path = CONTAINER_DERIV_PATH
-        kwargs["image"] = container_image
-
-        if container_type == "docker":
-            task_cls = DockerTask
-            base_spec_cls = DockerSpec
-        elif container_type == "singularity":
-            task_cls = SingularityTask
-            base_spec_cls = SingularitySpec
-        else:
-            raise ArcanaUsageError(
-                f"Unrecognised container type {container_type} "
-                "(can be docker or singularity)"
-            )
 
     if row_frequency == Clinical.session:
         analysis_level = "participant"
         kwargs["participant_label"] = wf.lzin.id  # wf.bidsify_id.lzout.no_prefix
     else:
         analysis_level = "group"
 
-    main_task = task_cls(
+    main_task = ShellCommandTask(
         name="bids_app",
-        input_spec=SpecInfo(name="Input", fields=input_fields, bases=(base_spec_cls,)),
+        input_spec=SpecInfo(name="Input", fields=input_fields, bases=(ShellSpec,)),
         output_spec=SpecInfo(
             name="Output", fields=BIDS_APP_OUTPUTS, bases=(ShellOutSpec,)
         ),
         dataset_path=dataset.id,
         output_path=str(app_output_path),
         work_dir=str(app_work_dir),
         analysis_level=analysis_level,
+        executable=executable,
+        environment=environment,
         flags=wf.lzin.flags,
         setup_completed=wf.to_bids.lzout.completed,
         **kwargs,
     )
 
     if container_image is not None:
         main_task.bindings = {
@@ -374,15 +356,17 @@
     id : str
         id of the row to be processed
     app_completed : bool
         a dummy field produced by the main BIDS app task on output, to ensure
         'extract_bids' is run after the app has completed.
     """
     # Copy output dir into BIDS dataset
-    shutil.copytree(output_dir, Path(dataset.id) / "derivatives" / app_name / ("sub-" + id))
+    shutil.copytree(
+        output_dir, Path(dataset.id) / "derivatives" / app_name / ("sub-" + id)
+    )
     output_paths = []
     row = dataset.row(row_frequency, id)
     for output in outputs:
         if output.path:
             path = output.path
         else:
             path = ""  # whole directory
```

### Comparing `arcana_bids-0.2.6/arcana/bids/tests/test_cli.py` & `arcana_bids-0.2.7/arcana/bids/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.6/arcana/bids/tests/test_data.py` & `arcana_bids-0.2.7/arcana/bids/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.6/arcana/bids/tests/test_tasks.py` & `arcana_bids-0.2.7/arcana/bids/tests/test_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import stat
 from pathlib import Path
 import shutil
-from arcana.core import __version__
+import pytest
 from fileformats.medimage import NiftiGzX, NiftiGzXBvec
 from arcana.bids.tasks import bids_app, BidsInput, BidsOutput
 from fileformats.text import Plain as Text
 from fileformats.generic import Directory
 
 
 MOCK_BIDS_APP_NAME = "mockapp"
@@ -21,28 +21,29 @@
 BIDS_OUTPUTS = [
     BidsOutput(name="whole_dir", datatype=Directory),  # whole derivative directory
     BidsOutput(name="a_file", path="file1", datatype=Text),
     BidsOutput(name="another_file", path="file2", datatype=Text),
 ]
 
 
+@pytest.mark.xfail(reason="Need to convert this to new environment syntax")
 def test_bids_app_docker(
     bids_validator_app_image: str, nifti_sample_dir: Path, work_dir: Path
 ):
 
     kwargs = {}
 
     bids_dir = work_dir / "bids"
 
     shutil.rmtree(bids_dir, ignore_errors=True)
 
     task = bids_app(
         name=MOCK_BIDS_APP_NAME,
         container_image=bids_validator_app_image,
-        executable="/launch.sh",  # Extracted using `docker_image_executable(docker_image)`
+        executable=None,  # uses entrypoint
         inputs=BIDS_INPUTS,
         outputs=BIDS_OUTPUTS,
         dataset=bids_dir,
     )
 
     for inpt in BIDS_INPUTS:
         kwargs[inpt.name] = nifti_sample_dir.joinpath(
```

### Comparing `arcana_bids-0.2.6/LICENSE` & `arcana_bids-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.6/README.rst` & `arcana_bids-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.6/pyproject.toml` & `arcana_bids-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.6/PKG-INFO` & `arcana_bids-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: arcana-bids
-Version: 0.2.6
+Version: 0.2.7
 Summary: An Arcana extension for interacting with Brain Imaging Structure (BIDS) datasets and associated "Apps"
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-bids.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

