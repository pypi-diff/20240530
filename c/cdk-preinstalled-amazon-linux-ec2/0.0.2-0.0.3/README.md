# Comparing `tmp/cdk-preinstalled-amazon-linux-ec2-0.0.2.tar.gz` & `tmp/cdk-preinstalled-amazon-linux-ec2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-preinstalled-amazon-linux-ec2-0.0.2.tar", last modified: Wed May 29 13:07:26 2024, max compression
+gzip compressed data, was "cdk-preinstalled-amazon-linux-ec2-0.0.3.tar", last modified: Wed May 29 14:00:22 2024, max compression
```

## Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2.tar` & `cdk-preinstalled-amazon-linux-ec2-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.812539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.812539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26913 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:07:16.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:07:26.816539 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 13:07:26.000000 cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:00:22.606273 cdk-preinstalled-amazon-linux-ec2-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-29 14:00:22.606273 cdk-preinstalled-amazon-linux-ec2-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:00:22.606273 cdk-preinstalled-amazon-linux-ec2-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:00:22.602273 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:00:22.602273 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    54304 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:00:22.606273 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26938 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:00:11.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:00:22.602273 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-29 14:00:22.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-29 14:00:22.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:00:22.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 14:00:22.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 14:00:22.000000 cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/LICENSE` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/PKG-INFO` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-preinstalled-amazon-linux-ec2
-Version: 0.0.2
+Version: 0.0.3
 Summary: CDK Construct for creating an Amazon Linux EC2 instance with pre-installed software
 Home-page: https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -57,15 +57,15 @@
   vpc,
   instanceType: ec2.InstanceType.of(ec2.InstanceClass.T3, ec2.InstanceSize.NANO),
   machineImage: new ec2.AmazonLinuxImage({
     generation: ec2.AmazonLinuxGeneration.AMAZON_LINUX_2023,
   }),
   // Specify preinstalled software
   preinstalledSoftware: {
-    type: [
+    packages: [
       PreinstalledSoftwareType.NODEJS,
       PreinstalledSoftwareType.VSCODE,
       PreinstalledSoftwareType.GIT,
     ],
     others: ['rsyslog'], // You can specify other software packages. These parameters are used as `sudo dnf install ${parameter}`
 });
 ```
@@ -104,12 +104,12 @@
 ```
 
 Ofcourse, you can customize the additional user data script by calling `instance.userData.addCommands()` method.
 
 ```python
 declare const instance: PreinstalledAmazonLinuxInstance;
 
-// install Postgresql
+// install yarn
 instance.userData.addCommands(
-  'sudo dnf install -y postgresql15-server'
+  'npm install -g yarn'
 );
 ```
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/README.md` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   vpc,
   instanceType: ec2.InstanceType.of(ec2.InstanceClass.T3, ec2.InstanceSize.NANO),
   machineImage: new ec2.AmazonLinuxImage({
     generation: ec2.AmazonLinuxGeneration.AMAZON_LINUX_2023,
   }),
   // Specify preinstalled software
   preinstalledSoftware: {
-    type: [
+    packages: [
       PreinstalledSoftwareType.NODEJS,
       PreinstalledSoftwareType.VSCODE,
       PreinstalledSoftwareType.GIT,
     ],
     others: ['rsyslog'], // You can specify other software packages. These parameters are used as `sudo dnf install ${parameter}`
 });
 ```
@@ -81,12 +81,12 @@
 ```
 
 Ofcourse, you can customize the additional user data script by calling `instance.userData.addCommands()` method.
 
 ```python
 declare const instance: PreinstalledAmazonLinuxInstance;
 
-// install Postgresql
+// install yarn
 instance.userData.addCommands(
-  'sudo dnf install -y postgresql15-server'
+  'npm install -g yarn'
 );
 ```
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/setup.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-preinstalled-amazon-linux-ec2",
-    "version": "0.0.2",
+    "version": "0.0.3",
     "description": "CDK Construct for creating an Amazon Linux EC2 instance with pre-installed software",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_preinstalled_amazon_linux_ec2",
         "cdk_preinstalled_amazon_linux_ec2._jsii"
     ],
     "package_data": {
         "cdk_preinstalled_amazon_linux_ec2._jsii": [
-            "cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz"
+            "cdk-preinstalled-amazon-linux-ec2@0.0.3.jsii.tgz"
         ],
         "cdk_preinstalled_amazon_linux_ec2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/__init__.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   vpc,
   instanceType: ec2.InstanceType.of(ec2.InstanceClass.T3, ec2.InstanceSize.NANO),
   machineImage: new ec2.AmazonLinuxImage({
     generation: ec2.AmazonLinuxGeneration.AMAZON_LINUX_2023,
   }),
   // Specify preinstalled software
   preinstalledSoftware: {
-    type: [
+    packages: [
       PreinstalledSoftwareType.NODEJS,
       PreinstalledSoftwareType.VSCODE,
       PreinstalledSoftwareType.GIT,
     ],
     others: ['rsyslog'], // You can specify other software packages. These parameters are used as `sudo dnf install ${parameter}`
 });
 ```
@@ -82,17 +82,17 @@
 ```
 
 Ofcourse, you can customize the additional user data script by calling `instance.userData.addCommands()` method.
 
 ```python
 declare const instance: PreinstalledAmazonLinuxInstance;
 
-// install Postgresql
+// install yarn
 instance.userData.addCommands(
-  'sudo dnf install -y postgresql15-server'
+  'npm install -g yarn'
 );
 ```
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
@@ -770,72 +770,72 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="cdk-preinstalled-amazon-linux-ec2.PreinstalledSoftware",
     jsii_struct_bases=[],
-    name_mapping={"others": "others", "type": "type"},
+    name_mapping={"others": "others", "packages": "packages"},
 )
 class PreinstalledSoftware:
     def __init__(
         self,
         *,
         others: typing.Optional[typing.Sequence[builtins.str]] = None,
-        type: typing.Optional[typing.Sequence["PreinstalledSoftwareType"]] = None,
+        packages: typing.Optional[typing.Sequence["PreinstalledSoftwarePackage"]] = None,
     ) -> None:
         '''The configuration for preinstalled software.
 
         :param others: Whether to install other software. This is a list of software to install and passed to ``dnf install <software>`` Default: - no other software is preinstalled
-        :param type: The type of preinstalled software. Default: - no software is preinstalled
+        :param packages: The type of preinstalled software. Default: - no software is preinstalled
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__657dec901feded435d209f20ab5a0de458a54fdf89665912ea70cb5dfd6220fa)
             check_type(argname="argument others", value=others, expected_type=type_hints["others"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument packages", value=packages, expected_type=type_hints["packages"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if others is not None:
             self._values["others"] = others
-        if type is not None:
-            self._values["type"] = type
+        if packages is not None:
+            self._values["packages"] = packages
 
     @builtins.property
     def others(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Whether to install other software.
 
         This is a list of software to install and passed to ``dnf install <software>``
 
         :default: - no other software is preinstalled
         '''
         result = self._values.get("others")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
-    def type(self) -> typing.Optional[typing.List["PreinstalledSoftwareType"]]:
+    def packages(self) -> typing.Optional[typing.List["PreinstalledSoftwarePackage"]]:
         '''The type of preinstalled software.
 
         :default: - no software is preinstalled
         '''
-        result = self._values.get("type")
-        return typing.cast(typing.Optional[typing.List["PreinstalledSoftwareType"]], result)
+        result = self._values.get("packages")
+        return typing.cast(typing.Optional[typing.List["PreinstalledSoftwarePackage"]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "PreinstalledSoftware(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.enum(jsii_type="cdk-preinstalled-amazon-linux-ec2.PreinstalledSoftwareType")
-class PreinstalledSoftwareType(enum.Enum):
+@jsii.enum(jsii_type="cdk-preinstalled-amazon-linux-ec2.PreinstalledSoftwarePackage")
+class PreinstalledSoftwarePackage(enum.Enum):
     '''The type of preinstalled software.'''
 
     NODEJS = "NODEJS"
     '''Node.js.'''
     DOCKER = "DOCKER"
     '''Docker.'''
     VSCODE = "VSCODE"
@@ -844,15 +844,15 @@
     '''Git.'''
 
 
 __all__ = [
     "PreinstalledAmazonLinuxInstance",
     "PreinstalledAmazonLinuxInstanceProps",
     "PreinstalledSoftware",
-    "PreinstalledSoftwareType",
+    "PreinstalledSoftwarePackage",
 ]
 
 publication.publish()
 
 def _typecheckingstub__5c9a1423334dfc78f723231d72b2d552a8bf34ab8b88aebe51ca10138593a85d(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
@@ -924,11 +924,11 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__657dec901feded435d209f20ab5a0de458a54fdf89665912ea70cb5dfd6220fa(
     *,
     others: typing.Optional[typing.Sequence[builtins.str]] = None,
-    type: typing.Optional[typing.Sequence[PreinstalledSoftwareType]] = None,
+    packages: typing.Optional[typing.Sequence[PreinstalledSoftwarePackage]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-preinstalled-amazon-linux-ec2",
-    "0.0.2",
+    "0.0.3",
     __name__[0:-6],
-    "cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz",
+    "cdk-preinstalled-amazon-linux-ec2@0.0.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-preinstalled-amazon-linux-ec2
-Version: 0.0.2
+Version: 0.0.3
 Summary: CDK Construct for creating an Amazon Linux EC2 instance with pre-installed software
 Home-page: https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-preinstalled-amazon-linux-ec2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -57,15 +57,15 @@
   vpc,
   instanceType: ec2.InstanceType.of(ec2.InstanceClass.T3, ec2.InstanceSize.NANO),
   machineImage: new ec2.AmazonLinuxImage({
     generation: ec2.AmazonLinuxGeneration.AMAZON_LINUX_2023,
   }),
   // Specify preinstalled software
   preinstalledSoftware: {
-    type: [
+    packages: [
       PreinstalledSoftwareType.NODEJS,
       PreinstalledSoftwareType.VSCODE,
       PreinstalledSoftwareType.GIT,
     ],
     others: ['rsyslog'], // You can specify other software packages. These parameters are used as `sudo dnf install ${parameter}`
 });
 ```
@@ -104,12 +104,12 @@
 ```
 
 Ofcourse, you can customize the additional user data script by calling `instance.userData.addCommands()` method.
 
 ```python
 declare const instance: PreinstalledAmazonLinuxInstance;
 
-// install Postgresql
+// install yarn
 instance.userData.addCommands(
-  'sudo dnf install -y postgresql15-server'
+  'npm install -g yarn'
 );
 ```
```

### Comparing `cdk-preinstalled-amazon-linux-ec2-0.0.2/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt` & `cdk-preinstalled-amazon-linux-ec2-0.0.3/src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_preinstalled_amazon_linux_ec2/py.typed
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/PKG-INFO
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/SOURCES.txt
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/dependency_links.txt
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/requires.txt
 src/cdk_preinstalled_amazon_linux_ec2.egg-info/top_level.txt
 src/cdk_preinstalled_amazon_linux_ec2/_jsii/__init__.py
-src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.2.jsii.tgz
+src/cdk_preinstalled_amazon_linux_ec2/_jsii/cdk-preinstalled-amazon-linux-ec2@0.0.3.jsii.tgz
```

