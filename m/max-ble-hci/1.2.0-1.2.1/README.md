# Comparing `tmp/max_ble_hci-1.2.0.tar.gz` & `tmp/max_ble_hci-1.2.1.tar.gz`

## Comparing `max_ble_hci-1.2.0.tar` & `max_ble_hci-1.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/install.bat
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/install.sh
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/black-format-check.yml
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/black-format-run.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/pypi-deploy.yml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/requirements.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.github/workflows/test-installer.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/make.bat
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/ble_hci.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/ble_standard.rst
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/constants.rst
--rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/controller_cmds.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/data_params.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/examples.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/hci_packets.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/hci_reference.rst
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/informational_cmds.rst
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/installation.rst
--rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/le_controller_cmds.rst
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/link_control_cmds.rst
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/modules.rst
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/overview.rst
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/packet_codes.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/packet_defs.rst
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/status_cmds.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/utils.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/vendor_spec.rst
--rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/vendor_spec_cmds.rst
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/examples/dtm.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/examples/hello_hci.py
--rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/docs/source/images/ble_stack_diagram.jpeg
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/examples/dtm.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/examples/hello_hci.py
--rw-r--r--   0        0        0    26039 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci_cli.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/__init__.py
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/_hci_logger.py
--rw-r--r--   0        0        0    15976 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/_transport.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/ad_types.py
--rw-r--r--   0        0        0    16450 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/ble_hci.py
--rw-r--r--   0        0        0    23932 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/ble_standard_cmds.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/constants.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/data_params.py
--rw-r--r--   0        0        0    19610 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/hci_packets.py
--rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/packet_codes.py
--rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/packet_defs.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/utils.py
--rw-r--r--   0        0        0    56073 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/src/max_ble_hci/vendor_spec_cmds.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/tests/test.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/LICENSE
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/README.md
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 max_ble_hci-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/install.bat
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/install.sh
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/black-format-check.yml
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/black-format-run.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/pypi-deploy.yml
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/requirements.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.github/workflows/test-installer.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/ble_hci.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/ble_standard.rst
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/constants.rst
+-rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/controller_cmds.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/data_params.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/examples.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/hci_packets.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/hci_reference.rst
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/informational_cmds.rst
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/installation.rst
+-rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/le_controller_cmds.rst
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/link_control_cmds.rst
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/modules.rst
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/overview.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/packet_codes.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/packet_defs.rst
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/status_cmds.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/utils.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/vendor_spec.rst
+-rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/vendor_spec_cmds.rst
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/examples/dtm.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/examples/hello_hci.py
+-rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/docs/source/images/ble_stack_diagram.jpeg
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/examples/dtm.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/examples/hello_hci.py
+-rw-r--r--   0        0        0    26788 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci_cli.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/__init__.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/_hci_logger.py
+-rw-r--r--   0        0        0    15976 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/_transport.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/ad_types.py
+-rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/ble_hci.py
+-rw-r--r--   0        0        0    23932 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/ble_standard_cmds.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/constants.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/data_params.py
+-rw-r--r--   0        0        0    19610 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/hci_packets.py
+-rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/packet_codes.py
+-rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/packet_defs.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/utils.py
+-rw-r--r--   0        0        0    56073 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/src/max_ble_hci/vendor_spec_cmds.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/tests/test.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 max_ble_hci-1.2.1/PKG-INFO
```

### Comparing `max_ble_hci-1.2.0/.github/workflows/black-format-run.yml` & `max_ble_hci-1.2.1/.github/workflows/black-format-run.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/.github/workflows/documentation.yml` & `max_ble_hci-1.2.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/.github/workflows/pylint.yml` & `max_ble_hci-1.2.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/.github/workflows/python-package-conda.yml` & `max_ble_hci-1.2.1/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/.github/workflows/test-installer.yml` & `max_ble_hci-1.2.1/.github/workflows/test-installer.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/Makefile` & `max_ble_hci-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/make.bat` & `max_ble_hci-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/conf.py` & `max_ble_hci-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/controller_cmds.rst` & `max_ble_hci-1.2.1/docs/source/controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/examples.rst` & `max_ble_hci-1.2.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/index.rst` & `max_ble_hci-1.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/informational_cmds.rst` & `max_ble_hci-1.2.1/docs/source/informational_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/installation.rst` & `max_ble_hci-1.2.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/le_controller_cmds.rst` & `max_ble_hci-1.2.1/docs/source/le_controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/link_control_cmds.rst` & `max_ble_hci-1.2.1/docs/source/link_control_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/overview.rst` & `max_ble_hci-1.2.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/status_cmds.rst` & `max_ble_hci-1.2.1/docs/source/status_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/vendor_spec_cmds.rst` & `max_ble_hci-1.2.1/docs/source/vendor_spec_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/examples/connection.py` & `max_ble_hci-1.2.1/docs/source/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/examples/dtm.py` & `max_ble_hci-1.2.1/docs/source/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/examples/hello_hci.py` & `max_ble_hci-1.2.1/docs/source/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/docs/source/images/ble_stack_diagram.jpeg` & `max_ble_hci-1.2.1/docs/source/images/ble_stack_diagram.jpeg`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/examples/connection.py` & `max_ble_hci-1.2.1/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/examples/dtm.py` & `max_ble_hci-1.2.1/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/examples/hello_hci.py` & `max_ble_hci-1.2.1/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci_cli.py` & `max_ble_hci-1.2.1/src/max_ble_hci_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         """
 
     # Parse the command line arguments
     parser = argparse.ArgumentParser(
         description=cli_description, formatter_class=RawTextHelpFormatter
     )
 
-    parser.add_argument("--version", action="version", version="%(prog)s 1.1.1")
+    parser.add_argument("--version", action="version", version="%(prog)s 1.1.2")
 
     parser.add_argument("serial_port", help="Serial port path or COM#")
     parser.add_argument(
         "-b",
         "--baud",
         dest="baudRate",
         type=int,
@@ -490,14 +490,37 @@
     rssi_parser = subparsers.add_parser(
         "rssi",
         help="Get an RSSI sample using CCA",
         formatter_class=RawTextHelpFormatter,
     )
     rssi_parser.add_argument("-c", "--channel", default=0)
 
+    ls_parser = subparsers.add_parser(
+        "ls",
+        help="List directory",
+        formatter_class=RawTextHelpFormatter,
+    )
+    ls_parser.add_argument("ls", default=".")
+    ls_parser.set_defaults(func=lambda args: [print(x) for x in os.listdir(args.ls)])
+
+    pwd_parser = subparsers.add_parser(
+        "pwd",
+        help="print working directory",
+        formatter_class=RawTextHelpFormatter,
+    )
+    pwd_parser.set_defaults(func=lambda args: print(os.getcwd()))
+
+    run_parser = subparsers.add_parser(
+        "run",
+        help="run command via os",
+        formatter_class=RawTextHelpFormatter,
+    )
+    run_parser.add_argument("run", nargs="+")
+    run_parser.set_defaults(func=lambda args: os.system(" ".join(args.run)))
+
     def _print_rssi(_args):
         rssi, status = hci.get_rssi_vs(_args.channel)
         print(f"RSSI (dBm): {rssi}")
         print(status)
 
     rssi_parser.set_defaults(func=_print_rssi)
```

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/__init__.py` & `max_ble_hci-1.2.1/src/max_ble_hci/__init__.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/_hci_logger.py` & `max_ble_hci-1.2.1/src/max_ble_hci/_hci_logger.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/_transport.py` & `max_ble_hci-1.2.1/src/max_ble_hci/_transport.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/ad_types.py` & `max_ble_hci-1.2.1/src/max_ble_hci/ad_types.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/ble_hci.py` & `max_ble_hci-1.2.1/src/max_ble_hci/ble_hci.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
         ------
         ValueError
             If both `addr` and `conn_params` are None.
         ValueError
             If `addr` is more than 6 bytes in size.
 
         """
-        print(addr)
+
         if conn_params is None:
             if addr is None:
                 raise ValueError(
                     "Either connection parameters or address must be provided."
                 )
 
             if max((addr.bit_length() + 7) // 8, 1) > 6:
```

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/ble_standard_cmds.py` & `max_ble_hci-1.2.1/src/max_ble_hci/ble_standard_cmds.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/constants.py` & `max_ble_hci-1.2.1/src/max_ble_hci/constants.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/data_params.py` & `max_ble_hci-1.2.1/src/max_ble_hci/data_params.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/hci_packets.py` & `max_ble_hci-1.2.1/src/max_ble_hci/hci_packets.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/packet_codes.py` & `max_ble_hci-1.2.1/src/max_ble_hci/packet_codes.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/packet_defs.py` & `max_ble_hci-1.2.1/src/max_ble_hci/packet_defs.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/utils.py` & `max_ble_hci-1.2.1/src/max_ble_hci/utils.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/src/max_ble_hci/vendor_spec_cmds.py` & `max_ble_hci-1.2.1/src/max_ble_hci/vendor_spec_cmds.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/tests/test.py` & `max_ble_hci-1.2.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/LICENSE` & `max_ble_hci-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/README.md` & `max_ble_hci-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.2.0/pyproject.toml` & `max_ble_hci-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/max_ble_hci", "src/max_ble_hci_cli.py"]
 
 [project]
 name = "max_ble_hci"
-version = "1.2.0"
+version = "1.2.1"
 dependencies = [
     "pyserial",
     "pyreadline3 ; platform_system == 'Windows'",
     "gnureadline ; platform_system == 'Darwin'",
     "colorlog"
 ]
 requires-python = ">=3.8"
```

### Comparing `max_ble_hci-1.2.0/PKG-INFO` & `max_ble_hci-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: max_ble_hci
-Version: 1.2.0
+Version: 1.2.1
 Summary: BLE HCI Test interface for controllers capable of the UART transport
 Project-URL: Homepage, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Repository, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Documentation, https://analog-devices-msdk.github.io/MAX-BLE-HCI/
 Project-URL: Bug Tracker, https://github.com/Analog-Devices-MSDK/BLE-HCI/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
```

