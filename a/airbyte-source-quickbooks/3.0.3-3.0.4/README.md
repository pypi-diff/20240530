# Comparing `tmp/airbyte_source_quickbooks-3.0.3.tar.gz` & `tmp/airbyte_source_quickbooks-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_quickbooks-3.0.3.tar", max compression
+gzip compressed data, was "airbyte_source_quickbooks-3.0.4.tar", max compression
```

## Comparing `airbyte_source_quickbooks-3.0.3.tar` & `airbyte_source_quickbooks-3.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     4059 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/README.md
--rw-r--r--   0        0        0      809 2024-04-11 14:26:26.281180 airbyte_source_quickbooks-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      211 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/__init__.py
--rw-r--r--   0        0        0     3406 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/components.py
--rw-r--r--   0        0        0     8879 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/manifest.yaml
--rw-r--r--   0        0        0      242 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/run.py
--rw-r--r--   0        0        0     1711 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/accounts.json
--rw-r--r--   0        0        0     3325 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bill_payments.json
--rw-r--r--   0        0        0     5593 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bills.json
--rw-r--r--   0        0        0     2556 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/budgets.json
--rw-r--r--   0        0        0     1105 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/classes.json
--rw-r--r--   0        0        0     5800 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/credit_memos.json
--rw-r--r--   0        0        0     4833 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/customers.json
--rw-r--r--   0        0        0     1110 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/departments.json
--rw-r--r--   0        0        0     4319 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/deposits.json
--rw-r--r--   0        0        0     2165 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/employees.json
--rw-r--r--   0        0        0     7073 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/estimates.json
--rw-r--r--   0        0        0     9527 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/invoices.json
--rw-r--r--   0        0        0     2135 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/items.json
--rw-r--r--   0        0        0     5356 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/journal_entries.json
--rw-r--r--   0        0        0      867 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payment_methods.json
--rw-r--r--   0        0        0     4442 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payments.json
--rw-r--r--   0        0        0     6937 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchase_orders.json
--rw-r--r--   0        0        0     6575 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchases.json
--rw-r--r--   0        0        0     5123 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/refund_receipts.json
--rw-r--r--   0        0        0     6847 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/sales_receipts.json
--rw-r--r--   0        0        0      974 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_agencies.json
--rw-r--r--   0        0        0     1945 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_codes.json
--rw-r--r--   0        0        0     2213 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_rates.json
--rw-r--r--   0        0        0     1253 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/terms.json
--rw-r--r--   0        0        0     1865 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/time_activities.json
--rw-r--r--   0        0        0     1581 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/transfers.json
--rw-r--r--   0        0        0     3795 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendor_credits.json
--rw-r--r--   0        0        0     3243 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendors.json
--rw-r--r--   0        0        0      479 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/source.py
--rw-r--r--   0        0        0     3392 2024-04-11 13:05:44.000000 airbyte_source_quickbooks-3.0.3/source_quickbooks/spec.json
--rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 airbyte_source_quickbooks-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6695 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/README.md
+-rw-r--r--   0        0        0      806 2024-05-30 14:09:02.769828 airbyte_source_quickbooks-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/__init__.py
+-rw-r--r--   0        0        0     3406 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/components.py
+-rw-r--r--   0        0        0     8879 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/manifest.yaml
+-rw-r--r--   0        0        0      242 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/run.py
+-rw-r--r--   0        0        0     1711 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/accounts.json
+-rw-r--r--   0        0        0     3325 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/bill_payments.json
+-rw-r--r--   0        0        0     5593 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/bills.json
+-rw-r--r--   0        0        0     2556 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/budgets.json
+-rw-r--r--   0        0        0     1105 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/classes.json
+-rw-r--r--   0        0        0     5800 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/credit_memos.json
+-rw-r--r--   0        0        0     4833 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/customers.json
+-rw-r--r--   0        0        0     1110 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/departments.json
+-rw-r--r--   0        0        0     4319 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/deposits.json
+-rw-r--r--   0        0        0     2165 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/employees.json
+-rw-r--r--   0        0        0     7073 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/estimates.json
+-rw-r--r--   0        0        0     9527 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/invoices.json
+-rw-r--r--   0        0        0     2135 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/items.json
+-rw-r--r--   0        0        0     5356 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/journal_entries.json
+-rw-r--r--   0        0        0      867 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/payment_methods.json
+-rw-r--r--   0        0        0     4442 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/payments.json
+-rw-r--r--   0        0        0     6937 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/purchase_orders.json
+-rw-r--r--   0        0        0     6575 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/purchases.json
+-rw-r--r--   0        0        0     5123 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/refund_receipts.json
+-rw-r--r--   0        0        0     6847 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/sales_receipts.json
+-rw-r--r--   0        0        0      974 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/tax_agencies.json
+-rw-r--r--   0        0        0     1945 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/tax_codes.json
+-rw-r--r--   0        0        0     2213 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/tax_rates.json
+-rw-r--r--   0        0        0     1253 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/terms.json
+-rw-r--r--   0        0        0     1865 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/time_activities.json
+-rw-r--r--   0        0        0     1581 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/transfers.json
+-rw-r--r--   0        0        0     3795 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/vendor_credits.json
+-rw-r--r--   0        0        0     3243 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/vendors.json
+-rw-r--r--   0        0        0      479 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/source.py
+-rw-r--r--   0        0        0     3392 2024-05-30 13:46:29.000000 airbyte_source_quickbooks-3.0.4/source_quickbooks/spec.json
+-rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 airbyte_source_quickbooks-3.0.4/PKG-INFO
```

### Comparing `airbyte_source_quickbooks-3.0.3/pyproject.toml` & `airbyte_source_quickbooks-3.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.3"
+version = "3.0.4"
 name = "airbyte-source-quickbooks"
 description = "Source implementation for quickbooks."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_quickbooks" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "==0.63.2"
+airbyte-cdk = "1.0.0"
 vcrpy = "==4.1.1"
 urllib3 = "==1.26.18"
 
 [tool.poetry.scripts]
 source-quickbooks = "source_quickbooks.run:run"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/components.py` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/manifest.yaml` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/accounts.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bill_payments.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/bill_payments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/bills.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/bills.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/budgets.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/budgets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/classes.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/classes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/credit_memos.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/credit_memos.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/customers.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/departments.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/departments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/deposits.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/deposits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/employees.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/employees.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/estimates.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/estimates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/invoices.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/items.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/journal_entries.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/journal_entries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payment_methods.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/payment_methods.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/payments.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/payments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchase_orders.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/purchase_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/purchases.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/purchases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/refund_receipts.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/refund_receipts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/sales_receipts.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/sales_receipts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_agencies.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/tax_agencies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_codes.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/tax_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/tax_rates.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/tax_rates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/terms.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/terms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/time_activities.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/time_activities.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/transfers.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/transfers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendor_credits.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/vendor_credits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/schemas/vendors.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/schemas/vendors.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/source_quickbooks/spec.json` & `airbyte_source_quickbooks-3.0.4/source_quickbooks/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_quickbooks-3.0.3/PKG-INFO` & `airbyte_source_quickbooks-3.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,126 @@
-Metadata-Version: 2.1
-Name: airbyte-source-quickbooks
-Version: 3.0.3
-Summary: Source implementation for quickbooks.
-Home-page: https://airbyte.com
-License: MIT
-Author: Airbyte
-Author-email: contact@airbyte.io
-Requires-Python: >=3.9,<3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.63.2)
-Requires-Dist: urllib3 (==1.26.18)
-Requires-Dist: vcrpy (==4.1.1)
-Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/quickbooks
-Project-URL: Repository, https://github.com/airbytehq/airbyte
-Description-Content-Type: text/markdown
-
 # Quickbooks Source
 
 This is the repository for the Quickbooks configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/quickbooks).
 
 ## Local development
 
 #### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/quickbooks)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_quickbooks/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
 **If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source quickbooks test creds`
 and place them into `secrets/config.json`.
 
 ### Locally running the connector docker image
 
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+
+#### Use `airbyte-ci` to build your connector
+The Airbyte way of building this connector is to use our `airbyte-ci` tool.
+You can follow install instructions [here](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md#L1).
+Then running the following command will build your connector:
+
 ```bash
-airbyte-ci connectors --name=source-quickbooks build
+airbyte-ci connectors --name source-quickbooks build
 ```
+Once the command is done, you will find your connector image in your local docker registry: `airbyte/source-quickbooks:dev`.
+
+##### Customizing our build process
+When contributing on our connector you might need to customize the build process to add a system dependency or set an env var.
+You can customize our build process by adding a `build_customization.py` module to your connector.
+This module should contain a `pre_connector_install` and `post_connector_install` async function that will mutate the base image and the connector container respectively.
+It will be imported at runtime by our build process and the functions will be called if they exist.
+
+Here is an example of a `build_customization.py` module:
+```python
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
-An image will be built with the tag `airbyte/source-quickbooks:dev`.
+if TYPE_CHECKING:
+    # Feel free to check the dagger documentation for more information on the Container object and its methods.
+    # https://dagger-io.readthedocs.io/en/sdk-python-v0.6.4/
+    from dagger import Container
+
+
+async def pre_connector_install(base_image_container: Container) -> Container:
+    return await base_image_container.with_env_variable("MY_PRE_BUILD_ENV_VAR", "my_pre_build_env_var_value")
+
+async def post_connector_install(connector_container: Container) -> Container:
+    return await connector_container.with_env_variable("MY_POST_BUILD_ENV_VAR", "my_post_build_env_var_value")
+```
+
+#### Build your own connector image
+This connector is built using our dynamic built process in `airbyte-ci`.
+The base image used to build it is defined within the metadata.yaml file under the `connectorBuildOptions`.
+The build logic is defined using [Dagger](https://dagger.io/) [here](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/pipelines/builds/python_connectors.py).
+It does not rely on a Dockerfile.
+
+If you would like to patch our connector and build your own a simple approach would be to:
+
+1. Create your own Dockerfile based on the latest version of the connector image.
+```Dockerfile
+FROM airbyte/source-quickbooks:latest
+
+COPY . ./airbyte/integration_code
+RUN pip install ./airbyte/integration_code
+
+# The entrypoint and default env vars are already set in the base image
+# ENV AIRBYTE_ENTRYPOINT "python /airbyte/integration_code/main.py"
+# ENTRYPOINT ["python", "/airbyte/integration_code/main.py"]
+```
+Please use this as an example. This is not optimized.
 
-**Via `docker build`:**
+2. Build your image:
 ```bash
 docker build -t airbyte/source-quickbooks:dev .
+# Running the spec command against your patched connector
+docker run airbyte/source-quickbooks:dev spec
 ```
-
 #### Run
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-quickbooks:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-quickbooks:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-quickbooks:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-quickbooks:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ## Testing
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-quickbooks test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ## Dependency Management
+
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+
+- required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
+- required for the testing need to go to `TEST_REQUIREMENTS` list
 
 ### Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-quickbooks test`
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/quickbooks.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
-7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
-
+7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
```

