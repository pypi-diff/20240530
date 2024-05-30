# Comparing `tmp/cerebrium-1.21.1-py3-none-any.whl.zip` & `tmp/cerebrium-1.21.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,32 @@
-Zip file size: 55193 bytes, number of entries: 29
+Zip file size: 56098 bytes, number of entries: 30
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 cerebrium/__init__.py
 -rw-r--r--  2.0 unx    16245 b- defN 80-Jan-01 00:00 cerebrium/api.py
 -rw-r--r--  2.0 unx     8971 b- defN 80-Jan-01 00:00 cerebrium/commands/app.py
 -rw-r--r--  2.0 unx     4465 b- defN 80-Jan-01 00:00 cerebrium/commands/auth.py
--rw-r--r--  2.0 unx    11305 b- defN 80-Jan-01 00:00 cerebrium/commands/cortex.py
+-rw-r--r--  2.0 unx    12835 b- defN 80-Jan-01 00:00 cerebrium/commands/cortex.py
 -rw-r--r--  2.0 unx     2170 b- defN 80-Jan-01 00:00 cerebrium/commands/project.py
 -rw-r--r--  2.0 unx    17156 b- defN 80-Jan-01 00:00 cerebrium/commands/serve.py
 -rw-r--r--  2.0 unx     3009 b- defN 80-Jan-01 00:00 cerebrium/commands/storage.py
--rw-r--r--  2.0 unx     4572 b- defN 80-Jan-01 00:00 cerebrium/config.py
+-rw-r--r--  2.0 unx     5053 b- defN 80-Jan-01 00:00 cerebrium/config.py
 -rw-r--r--  2.0 unx      801 b- defN 80-Jan-01 00:00 cerebrium/core.py
+-rw-r--r--  2.0 unx      369 b- defN 80-Jan-01 00:00 cerebrium/defaults.py
 -rw-r--r--  2.0 unx      473 b- defN 80-Jan-01 00:00 cerebrium/files.py
 -rwxr-xr-x  2.0 unx     1160 b- defN 80-Jan-01 00:00 cerebrium/main.py
 -rw-r--r--  2.0 unx     5216 b- defN 80-Jan-01 00:00 cerebrium/serve/local_api_server.py
 -rw-r--r--  2.0 unx      326 b- defN 80-Jan-01 00:00 cerebrium/types.py
--rw-r--r--  2.0 unx     9116 b- defN 80-Jan-01 00:00 cerebrium/utils/deploy.py
+-rw-r--r--  2.0 unx     9197 b- defN 80-Jan-01 00:00 cerebrium/utils/deploy.py
 -rw-r--r--  2.0 unx     4913 b- defN 80-Jan-01 00:00 cerebrium/utils/display.py
 -rw-r--r--  2.0 unx     4073 b- defN 80-Jan-01 00:00 cerebrium/utils/files.py
 -rw-r--r--  2.0 unx     6464 b- defN 80-Jan-01 00:00 cerebrium/utils/logging.py
 -rw-r--r--  2.0 unx      599 b- defN 80-Jan-01 00:00 cerebrium/utils/project.py
 -rw-r--r--  2.0 unx     4700 b- defN 80-Jan-01 00:00 cerebrium/utils/requirements.py
 -rw-r--r--  2.0 unx     7717 b- defN 80-Jan-01 00:00 cerebrium/utils/sync_files.py
 -rw-r--r--  2.0 unx     2023 b- defN 80-Jan-01 00:00 cerebrium/utils/termination.py
 -rw-r--r--  2.0 unx     2071 b- defN 80-Jan-01 00:00 cerebrium/utils/verification.py
 -rw-r--r--  2.0 unx     1393 b- defN 80-Jan-01 00:00 cerebrium/utils/watchdog.py
--rw-r--r--  2.0 unx    34594 b- defN 80-Jan-01 00:00 cerebrium-1.21.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3065 b- defN 80-Jan-01 00:00 cerebrium-1.21.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cerebrium-1.21.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 80-Jan-01 00:00 cerebrium-1.21.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2371 b- defN 16-Jan-01 00:00 cerebrium-1.21.1.dist-info/RECORD
-29 files, 159210 bytes uncompressed, 51413 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx    34594 b- defN 80-Jan-01 00:00 cerebrium-1.21.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3065 b- defN 80-Jan-01 00:00 cerebrium-1.21.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cerebrium-1.21.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 80-Jan-01 00:00 cerebrium-1.21.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2448 b- defN 16-Jan-01 00:00 cerebrium-1.21.2.dist-info/RECORD
+30 files, 161748 bytes uncompressed, 52200 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -24,14 +24,17 @@
 
 Filename: cerebrium/config.py
 Comment: 
 
 Filename: cerebrium/core.py
 Comment: 
 
+Filename: cerebrium/defaults.py
+Comment: 
+
 Filename: cerebrium/files.py
 Comment: 
 
 Filename: cerebrium/main.py
 Comment: 
 
 Filename: cerebrium/serve/local_api_server.py
@@ -66,23 +69,23 @@
 
 Filename: cerebrium/utils/verification.py
 Comment: 
 
 Filename: cerebrium/utils/watchdog.py
 Comment: 
 
-Filename: cerebrium-1.21.1.dist-info/LICENSE
+Filename: cerebrium-1.21.2.dist-info/LICENSE
 Comment: 
 
-Filename: cerebrium-1.21.1.dist-info/METADATA
+Filename: cerebrium-1.21.2.dist-info/METADATA
 Comment: 
 
-Filename: cerebrium-1.21.1.dist-info/WHEEL
+Filename: cerebrium-1.21.2.dist-info/WHEEL
 Comment: 
 
-Filename: cerebrium-1.21.1.dist-info/entry_points.txt
+Filename: cerebrium-1.21.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cerebrium-1.21.1.dist-info/RECORD
+Filename: cerebrium-1.21.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cerebrium/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "1.21.1"
+__version__ = "1.21.2"
 # Ignore linting in this file
 # flake8: noqa
 from cerebrium.core import get_secret
```

## cerebrium/commands/cortex.py

```diff
@@ -19,14 +19,15 @@
     HardwareConfig,
     DeploymentConfig,
     DependencyConfig,
 )
 from cerebrium.utils.logging import cerebrium_log
 from cerebrium.utils.requirements import strip_delimiters
 from cerebrium.utils.deploy import package_app
+from cerebrium import defaults
 
 
 _EXAMPLE_MAIN = """
 def run(param_1: str, param_2: str, run_id):  # run_id is optional, injected by Cerebrium at runtime
     my_results = {"1": param_1, "2": param_2}
     my_status_code = 200 # if you want to return a specific status code
 
@@ -51,93 +52,99 @@
         str,
         typer.Option(
             help=(
                 "Optional list of requirements. "
                 "Example: \"['transformers', 'torch==1.31.1']\""
             ),
         ),
-    ] = "['transformers', 'torch']",
+    ] = "[]",
     apt: Annotated[
         str,
         typer.Option(
             help=("Optional list of apt packages. For example: \"['git', 'ffmpeg' ]\""),
         ),
     ] = "[]",
     conda: Annotated[str, typer.Option(help="Optional list of conda packages.")] = "[]",
     cpu: Annotated[
         int,
         typer.Option(
             help=(
                 "Number of vCPUs (cores) to use for the Cortex deployment. " "Defaults to 3."
             ),
         ),
-    ] = 3,
+    ] = defaults.CPU,
     memory: Annotated[
         float,
         typer.Option(
             help=(
                 "Amount of memory (in GB) to use for the Cortex deployment. "
-                "Defaults to 14GB. "
+                "Defaults to 14.0GB. "
             ),
         ),
-    ] = 14,
+    ] = defaults.MEMORY,
     gpu: Annotated[
         str,
         typer.Option(
             help=("Type of GPU to use for the Cortex deployment. " "Defaults to 'AMPERE_A10'."),
         ),
-    ] = "AMPERE_A10",
+    ] = defaults.GPU,
     gpu_count: Annotated[
         int,
         typer.Option(
             help=("Number of GPUs to use for the Cortex deployment. " "Defaults to 1."),
         ),
-    ] = 1,
+    ] = defaults.GPU_COUNT,
     include: Annotated[
         str,
         typer.Option(
             help=(
                 "Comma delimited string list of relative paths to files/folder to include. "
                 "Defaults to all visible files/folders in project root."
             ),
         ),
-    ] = "[./*, main.py, cerebrium.toml]",
+    ] = defaults.INCLUDE,
     exclude: Annotated[
         str,
         typer.Option(
             help=(
                 "Comma delimited string list of relative paths to files/folder to exclude. "
                 "Defaults to all hidden files/folders in project root."
             ),
         ),
-    ] = "[.*]",
+    ] = defaults.EXCLUDE,
+    python_version: Annotated[
+        str,
+        typer.Option(
+            help=("Python version to use. Defaults to the current interpreter version."),
+        ),
+    ] = defaults.PYTHON_VERSION,
     cuda_version: Annotated[
         str,
         typer.Option(
             help=("CUDA version to use. " "Defaults to '12'"),
         ),
-    ] = "12",
+    ] = defaults.CUDA_VERSION,
     min_replicas: Annotated[
         int,
         typer.Option(
             help=("Minimum number of replicas to keep running. " "Defaults to 0."),
         ),
-    ] = 0,
+    ] = defaults.MIN_REPLICAS,
     max_replicas: Annotated[
         int,
         typer.Option(
             help=("Maximum number of replicas to keep running. " "Defaults to 5."),
         ),
-    ] = 5,
+    ] = defaults.MAX_REPLICAS,
     cooldown: Annotated[
         int,
         typer.Option(
             help=("Cooldown period in seconds. " "Defaults to 60 seconds (5 minutes)."),
         ),
-    ] = 60,
+    ] = defaults.COOLDOWN,
 ):
     """
     Initialize an empty Cerebrium Cortex project.
     """
     print(f"Initializing Cerebrium Cortex project in {init_dir}")
     if not name:
         name = os.path.basename(os.path.abspath(init_dir))
@@ -157,39 +164,37 @@
         )
         raise typer.Exit()
 
     if not os.path.exists(os.path.join(init_dir, "main.py")):
         with open(os.path.join(init_dir, "main.py"), "w") as f:
             f.write(_EXAMPLE_MAIN)
 
-    interpreter_version = sys.version_info
-    python_version = f"{interpreter_version.major}.{interpreter_version.minor}"
     pip_dict = strip_delimiters(pip)
     apt_dict = strip_delimiters(apt)
     conda_dict = strip_delimiters(conda)
 
     scaling_config = ScalingConfig(
         min_replicas=min_replicas, max_replicas=max_replicas, cooldown=cooldown
     )
     hardware_config = HardwareConfig(
         cpu=cpu,
         memory=memory,
         gpu=gpu,
         gpu_count=gpu_count,
-        provider="aws",
-        region="us-east-1",
+        provider=defaults.PROVIDER,
+        region=defaults.REGION,
     )
     dependency_config = DependencyConfig(pip=pip_dict, apt=apt_dict, conda=conda_dict)
     deployment_config = DeploymentConfig(
         name=name,
         python_version=python_version,
         cuda_version=cuda_version,
         include=include,
         exclude=exclude,
-        shell_commands=[],
+        shell_commands=defaults.SHELL_COMMANDS,
     )
     config = CerebriumConfig(
         scaling=scaling_config,
         hardware=hardware_config,
         deployment=deployment_config,
         dependencies=dependency_config,
     )
@@ -256,19 +261,51 @@
         assert log_level in [
             "DEBUG",
             "INFO",
             "WARNING",
             "ERROR",
             "INTERNAL",
         ], "Log level must be one of 'DEBUG' or 'INFO'"
-        toml_config = toml.load(config_file)["cerebrium"]
-        scaling_config: ScalingConfig = ScalingConfig(**toml_config["scaling"])
-        hardware_config: HardwareConfig = HardwareConfig(**toml_config["hardware"])
-        deployment_config: DeploymentConfig = DeploymentConfig(**toml_config["deployment"])
-        dependency_config: DependencyConfig = DependencyConfig(**toml_config["dependencies"])
+        try:
+            toml_config = toml.load(config_file)["cerebrium"]
+        except FileNotFoundError:
+            cerebrium_log(
+                message="Could not find cerebrium.toml file. Please run `cerebrium init` to create one.",
+                color="red",
+            )
+            raise typer.Exit()
+        except KeyError:
+            cerebrium_log(
+                message="Could not find 'cerebrium' key in cerebrium.toml file. Please run `cerebrium init` to create one.",
+                color="red",
+            )
+            raise typer.Exit()
+        except Exception as e:
+            cerebrium_log(message=f"Error loading cerebrium.toml file: {e}", color="red")
+            raise typer.Exit()
+
+        deployment_section = toml_config.get("deployment", {})
+        if not deployment_section:
+            cerebrium_log(
+                message="Deployment section is required in cerebrium.toml file. Please add a 'deployment' section.",
+                color="red",
+            )
+            raise typer.Exit()
+        if "name" not in deployment_section:
+            cerebrium_log(
+                message="`deployment.name` is required in cerebrium.toml file. Please add a 'name' field to the 'deployment' section.",
+                color="red",
+            )
+            raise typer.Exit()
+        deployment_config: DeploymentConfig = DeploymentConfig(**deployment_section)
+        scaling_config: ScalingConfig = ScalingConfig(**toml_config.get("scaling", {}))
+        hardware_config: HardwareConfig = HardwareConfig(**toml_config.get("hardware", {}))
+        dependency_config: DependencyConfig = DependencyConfig(
+            **toml_config.get("dependencies", {})
+        )
         config: CerebriumConfig = CerebriumConfig(
             scaling=scaling_config,
             hardware=hardware_config,
             deployment=deployment_config,
             dependencies=dependency_config,
         )
```

## cerebrium/config.py

```diff
@@ -1,26 +1,42 @@
 from abc import abstractmethod
 from atom.api import Atom
 from cerebrium.utils.files import string_hash
+from cerebrium.defaults import (
+    MIN_REPLICAS,
+    MAX_REPLICAS,
+    COOLDOWN,
+    CPU,
+    MEMORY,
+    GPU,
+    GPU_COUNT,
+    PROVIDER,
+    REGION,
+    PYTHON_VERSION,
+    CUDA_VERSION,
+    INCLUDE,
+    EXCLUDE,
+    SHELL_COMMANDS,
+)
 
 
 class TOMLConfig(Atom):
     @abstractmethod
     def __toml__(self) -> str:
         raise NotImplementedError
 
     @abstractmethod
     def __json__(self) -> dict:
         raise NotImplementedError
 
 
 class ScalingConfig(TOMLConfig):
-    min_replicas: int
-    max_replicas: int
-    cooldown: int
+    min_replicas: int = MIN_REPLICAS
+    max_replicas: int = MAX_REPLICAS
+    cooldown: int = COOLDOWN
 
     def __toml__(self) -> str:
         return (
             "[cerebrium.scaling]\n"
             f"min_replicas = {self.min_replicas}\n"
             f"max_replicas = {self.max_replicas}\n"
             f"cooldown = {self.cooldown}\n\n"
@@ -31,20 +47,20 @@
             "min_replicas": self.min_replicas,
             "max_replicas": self.max_replicas,
             "cooldown": self.cooldown,
         }
 
 
 class HardwareConfig(TOMLConfig):
-    cpu: int
-    memory: float
-    gpu: str
-    gpu_count: int
-    provider: str
-    region: str
+    cpu: int = CPU
+    memory: float = MEMORY
+    gpu: str = GPU
+    gpu_count: int = GPU_COUNT
+    provider: str = PROVIDER
+    region: str = REGION
 
     def __toml__(self) -> str:
         return (
             "[cerebrium.hardware]\n"
             f"cpu = {self.cpu}\n"
             f"memory = {self.memory}\n"
             f'gpu = "{self.gpu}"\n'
@@ -62,19 +78,19 @@
             "provider": self.provider,
             "region": self.region,
         }
 
 
 class DeploymentConfig(TOMLConfig):
     name: str
-    python_version: str
-    cuda_version: str
-    include: str
-    exclude: str
-    shell_commands: list[str]
+    python_version: str = PYTHON_VERSION
+    cuda_version: str = CUDA_VERSION
+    include: str = INCLUDE
+    exclude: str = EXCLUDE
+    shell_commands: list[str] = SHELL_COMMANDS
 
     def __toml__(self) -> str:
         return (
             "[cerebrium.deployment]\n"
             f'name = "{self.name}"\n'
             f'python_version = "{self.python_version}"\n'
             f'cuda_version = "{self.cuda_version}"\n'
@@ -117,15 +133,17 @@
         apt_strings = (
             "[cerebrium.dependencies.apt]\n"
             + "\n".join(f'"{key}" = "{value}"' for key, value in self.apt.items())
             + "\n"
             if self.apt != {}
             else ""
         )
-        return pip_strings + conda_strings + apt_strings + "\n"
+        if pip_strings or conda_strings or apt_strings:
+            return pip_strings + conda_strings + apt_strings + "\n"
+        return ""
 
     def __json__(self) -> dict:
         return {"pip": self.pip, "conda": self.conda, "apt": self.apt}
 
 
 class CerebriumConfig(Atom):
     deployment: DeploymentConfig
```

## cerebrium/utils/deploy.py

```diff
@@ -3,14 +3,15 @@
 import threading
 import time
 import typer
 from rich.live import Live
 from rich.spinner import Spinner
 from rich.text import Text
 from typing import Any, Literal
+from cerebrium import __version__
 from cerebrium.api import (
     cerebrium_request,
     upload_cortex_files,
     get_build_status,
     log_build_status,
     poll_build_logs,
     stream_logs,
@@ -106,14 +107,15 @@
     payload = config.to_payload()
     payload["function"] = app_type
     payload["force_rebuild"] = force_rebuild
     payload["init_debug"] = init_debug
     payload["log_level"] = log_level
     payload["disable_build_logs"] = disable_build_logs
     payload["upload_hash"] = file_hash(file_list)
+    payload["cerebrium_version"] = __version__
 
     # if partial_upload:
     #     setup_response = _partial_upload(
     #         cerebrium_config=config,
     #         source=app_type,
     #         file_list=file_list,
     #         force_rebuild=force_rebuild,
```

## Comparing `cerebrium-1.21.1.dist-info/LICENSE` & `cerebrium-1.21.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cerebrium-1.21.1.dist-info/METADATA` & `cerebrium-1.21.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.21.1
+Version: 1.21.2
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

## Comparing `cerebrium-1.21.1.dist-info/RECORD` & `cerebrium-1.21.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-cerebrium/__init__.py,sha256=mJ5rMqWJLYVMOg5p5BKv79FIa-SOeqxouIFa57g9iEU,106
+cerebrium/__init__.py,sha256=fpImRIAorK5DJNWybN0_3U5SjWnnpl7264T130rU2lo,106
 cerebrium/api.py,sha256=wqUpLChdkOBAdECdsrElLBFGSNfB1VjjANXTnuwsLIY,16245
 cerebrium/commands/app.py,sha256=C501fLkqSk2G8RhOzsWwAoCjjS2ijegTuXt9D0Mxbd0,8971
 cerebrium/commands/auth.py,sha256=FO1veuFRKsPs7Ui0bpuKz-q48jDbYbL2_pVMaP5sVws,4465
-cerebrium/commands/cortex.py,sha256=_ug2bpg4AAj4UUOsVG8Sv6pFOEEXp6lfgVMcLOVjfRY,11305
+cerebrium/commands/cortex.py,sha256=GFD-9WpEfZ5RQGUF7qEBMkChX5U786V-9hj2q6tljiY,12835
 cerebrium/commands/project.py,sha256=TL_S-yGAb9ygibLPgaDvrCPiv-kgcfQJXc3fY0nUpCI,2170
 cerebrium/commands/serve.py,sha256=fSgguY_LEmlUEVMA4TT8qgBidXo_JLv8QaFW-5_qsBI,17156
 cerebrium/commands/storage.py,sha256=29G9EgH-XT_gYJCOXZz1j4pEedCph4DfZIywl_eHjZI,3009
-cerebrium/config.py,sha256=qL3gKvCws5C7lvUba-GKUHRrtLbkisjzZKod2efjQus,4572
+cerebrium/config.py,sha256=ehrTotQrEuZba-Gkp1msee57zC-2FyOPYDelxcHQ1pQ,5053
 cerebrium/core.py,sha256=EhJbmttdHh0yd0C85MpNH7nX5RjyepqYkdCETa9d7e8,801
+cerebrium/defaults.py,sha256=FgoNIWPNdsBSPDWHEygs5v6b1wDkZUorFSO5DK-SfKU,369
 cerebrium/files.py,sha256=4OjZ94akeus48jUPMumBs0_0XwE0nURjFUJInfBxwxU,473
 cerebrium/main.py,sha256=lALbmVx4KUYh1LKxOgHee0rFf_9yn0rILuCco6P0pNY,1160
 cerebrium/serve/local_api_server.py,sha256=IRYJiD8aYXNSpedLrWfzSAe-1ie4YFtU0PfA8K7S700,5216
 cerebrium/types.py,sha256=4RRYIDkNMxe6O2yOvsvQ9qF5Qrwm_v5chF-zy_vLbi4,326
-cerebrium/utils/deploy.py,sha256=q5vRhAgqBC_IuCXpGLaHXg0sJnN8CSTaLay_v-ki1JU,9116
+cerebrium/utils/deploy.py,sha256=t4cXnbdzUccKwLCF6BYEYvVIXNSi5WUMv9oIHA6MNe4,9197
 cerebrium/utils/display.py,sha256=e9grqxF_-_503M6Uf-ysdMQ7rFWCh-tWHzFs0rRcMEk,4913
 cerebrium/utils/files.py,sha256=K91Dn9CHPSW0kfO8Pn3kSTjf-AmKHUuDI0SISY8MVPU,4073
 cerebrium/utils/logging.py,sha256=M6pk4fSceLwtDZOZYz9IkxfcqTfHZYl9XXxNtus40Uw,6464
 cerebrium/utils/project.py,sha256=OB6dD1-2dfH4TpP5sU3UE3P_ug2QNa7ppW0_7WrmAwY,599
 cerebrium/utils/requirements.py,sha256=NBdVBJOL1Z8jAQn41AhfYsVlGi-gE5aCkmLWBMRmWV8,4700
 cerebrium/utils/sync_files.py,sha256=LlhVgM9wYgU7uS8dMmuQY4XbzCoAHvu5Wh6EbwsD6t8,7717
 cerebrium/utils/termination.py,sha256=PIDZniyHY-NEwx0ldHKfm_S9HLCn61ZVsE7eOJJ0JYE,2023
 cerebrium/utils/verification.py,sha256=FUty0bBdNyNfh8e4sdxAHIFxlTLgoegtyWB7xmelrEU,2071
 cerebrium/utils/watchdog.py,sha256=BE1dPZ1m_5ODUumCcDGnLfDkPtWPoZKQx-lCM8xwiIE,1393
-cerebrium-1.21.1.dist-info/LICENSE,sha256=QoCdyu_al_XTJCs6xphksUTo6SgGRe_y3AnD6oeKziw,34594
-cerebrium-1.21.1.dist-info/METADATA,sha256=zILPRQVx18g-D3XrAYUwny8oACx2AD6CFpJfxYCuz0E,3065
-cerebrium-1.21.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-cerebrium-1.21.1.dist-info/entry_points.txt,sha256=X8NSRgq1hWqWRFwDhH1YWLG36V8vpPJpWFHr6jHTwwk,48
-cerebrium-1.21.1.dist-info/RECORD,,
+cerebrium-1.21.2.dist-info/LICENSE,sha256=QoCdyu_al_XTJCs6xphksUTo6SgGRe_y3AnD6oeKziw,34594
+cerebrium-1.21.2.dist-info/METADATA,sha256=Jgu26xApYEORrozqxznNSvVf8BrAgkn_ZjU8XCvcqvw,3065
+cerebrium-1.21.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+cerebrium-1.21.2.dist-info/entry_points.txt,sha256=X8NSRgq1hWqWRFwDhH1YWLG36V8vpPJpWFHr6jHTwwk,48
+cerebrium-1.21.2.dist-info/RECORD,,
```

