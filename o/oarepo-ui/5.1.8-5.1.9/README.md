# Comparing `tmp/oarepo-ui-5.1.8.tar.gz` & `tmp/oarepo-ui-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-ui-5.1.8.tar", last modified: Sun Mar 24 16:50:50 2024, max compression
+gzip compressed data, was "oarepo-ui-5.1.9.tar", last modified: Sun Mar 24 17:47:16 2024, max compression
```

## Comparing `oarepo-ui-5.1.8.tar` & `oarepo-ui-5.1.9.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/babel.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/format.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.382331 oarepo-ui-5.1.8/oarepo_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.382331 oarepo-ui-5.1.8/oarepo_ui/css/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/css/builtin.css
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/for_translations_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.386331 oarepo-ui-5.1.8/oarepo_ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/links.py
--rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.386331 oarepo-ui-5.1.8/oarepo_ui/resources/templating/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/templating/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/templating/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/resources/templating/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.386331 oarepo-ui-5.1.8/oarepo_ui/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/services/custom_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.374331 oarepo-ui-5.1.8/oarepo_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.386331 oarepo-ui-5.1.8/oarepo_ui/templates/components/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/Array.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/DefinitionLink.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/EditForm.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/Field.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/Multilingual.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/SearchLink.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/Searchbar.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/SidebarApiLinks.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/URL.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/Value.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.390331 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/IBaseField.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/ICustomFields.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/IField.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/INonEmpty.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/ISection.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/IValue.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/IValueList.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.390331 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/header_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/javascript.html
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/search.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.390331 oarepo-ui-5.1.8/oarepo_ui/theme/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.374331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.378331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.378331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.390331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/custom_fields/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.390331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.390331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/client.js
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/recordSerializer.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.390331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/burgermenu.js
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/ArrayFieldItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/BaseForm.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/BaseFormLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/ConfirmationModal.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/DeleteButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/DatePickerHeader.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDatePickerWrapper.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDateRangePickerField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFSingleDatePickerField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/InputElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/hooks.js
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.394331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/FormFeedback.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/FormikStateLogger.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/I18nRichInputField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nString/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nString/I18nString.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nString/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/I18nTextInputField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/LanguageSelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/MultilingualTextInput.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/PreviewButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/PublishButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiModal.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiResultsList.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/NoResultsMessage.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectFieldInternal.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/SaveButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.398331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/ValidateButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/constants.js
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/contexts.js
--rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/hooks.js
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/util.js
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.402331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ActiveFiltersElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/BucketAggregationElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/BucketAggregationValuesElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ClearFiltersButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/DynamicResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/EmptyResultsElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ErrorElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ResultCount.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ResultsPerPageLabel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppFacets.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResultOptions.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResults.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppSearchbarContainer.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppSort.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchFiltersToggleElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchappSearchbarElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/constants.js
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/util.js
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/theme.js
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.378331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.402331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.406331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)    29356 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/datepicker.less
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/dl_table.less
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_data.less
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_label.less
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/lang_tag.less
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/multilingual_tabs.less
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_footer.less
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_header.less
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/search_link.less
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/section.less
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/separated.less
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/value_list.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.378331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.378331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.406331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/dl_table.variables
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/form.overrides
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/form.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/menu.overrides
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.406331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/elements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/elements/search_link.variables
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/elements/separated.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.406331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/globals/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/globals/site.overrides
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.406331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/accordion.overrides
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/accordion.variables
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/dropdown.overrides
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/field_data.variables
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/field_label.variables
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/lang_tag.variables
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/multilingual_tabs.variables
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/section.variables
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/value_list.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.406331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/views/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/views/page_footer.variables
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/views/page_header.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.378331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ArrayWidget.js
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ComplexWidget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.378331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.382331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.382331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/translations.pot
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/theme/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/translations/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/translations/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.382331 oarepo-ui-5.1.8/oarepo_ui/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.382331 oarepo-ui-5.1.8/oarepo_ui/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/oarepo_ui/vite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 16:50:50.410331 oarepo-ui-5.1.8/oarepo_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-24 16:50:50.000000 oarepo-ui-5.1.8/oarepo_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-03-24 16:50:50.000000 oarepo-ui-5.1.8/oarepo_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 16:50:50.000000 oarepo-ui-5.1.8/oarepo_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-24 16:50:50.000000 oarepo-ui-5.1.8/oarepo_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 16:49:49.000000 oarepo-ui-5.1.8/oarepo_ui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-24 16:50:50.000000 oarepo-ui-5.1.8/oarepo_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-24 16:50:50.000000 oarepo-ui-5.1.8/oarepo_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-24 16:50:50.414331 oarepo-ui-5.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 16:48:20.000000 oarepo-ui-5.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.788971 oarepo-ui-5.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-24 17:47:16.788971 oarepo-ui-5.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/babel.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/format.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.756971 oarepo-ui-5.1.9/oarepo_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.760971 oarepo-ui-5.1.9/oarepo_ui/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/css/builtin.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/for_translations_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.760971 oarepo-ui-5.1.9/oarepo_ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.760971 oarepo-ui-5.1.9/oarepo_ui/resources/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/templating/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/templating/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/resources/templating/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.760971 oarepo-ui-5.1.9/oarepo_ui/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/services/custom_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.748971 oarepo-ui-5.1.9/oarepo_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.764971 oarepo-ui-5.1.9/oarepo_ui/templates/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/Array.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/DefinitionLink.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/EditForm.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/Field.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/Multilingual.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/SearchLink.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/Searchbar.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/SidebarApiLinks.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/URL.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/Value.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.764971 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/IBaseField.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/ICustomFields.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/IField.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/INonEmpty.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/ISection.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/IValue.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/IValueList.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.764971 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.764971 oarepo-ui-5.1.9/oarepo_ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.748971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.752971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.748971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.764971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/custom_fields/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/client.js
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/recordSerializer.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/burgermenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/ArrayFieldItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/BaseForm.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/BaseFormLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.768971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/ConfirmationModal.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/DeleteButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/DatePickerHeader.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDatePickerWrapper.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDateRangePickerField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFSingleDatePickerField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/InputElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/hooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/FormFeedback.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/FormikStateLogger.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/I18nRichInputField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nString/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nString/I18nString.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nString/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/I18nTextInputField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/LanguageSelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/MultilingualTextInput.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.772971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/PreviewButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.776971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/PublishButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.776971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiModal.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiResultsList.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/NoResultsMessage.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectFieldInternal.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.776971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/SaveButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.776971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/ValidateButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/constants.js
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/contexts.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/hooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.780971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ActiveFiltersElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/BucketAggregationElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/BucketAggregationValuesElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ClearFiltersButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/DynamicResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/EmptyResultsElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ErrorElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ResultCount.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ResultsPerPageLabel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppFacets.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResultOptions.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResults.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppSearchbarContainer.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppSort.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchFiltersToggleElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchappSearchbarElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/constants.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.752971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.780971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.780971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)    29356 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/datepicker.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_data.less
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_label.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/lang_tag.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/multilingual_tabs.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_footer.less
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_header.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/search_link.less
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/section.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/separated.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/value_list.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.752971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.752971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.780971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/dl_table.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/form.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/form.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/menu.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.780971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/elements/search_link.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/elements/separated.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/globals/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/globals/site.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/accordion.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/accordion.variables
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/dropdown.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/field_data.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/field_label.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/lang_tag.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/multilingual_tabs.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/section.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/value_list.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/views/page_footer.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/views/page_header.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.752971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ArrayWidget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ComplexWidget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.752971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.752971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.756971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/theme/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.756971 oarepo-ui-5.1.9/oarepo_ui/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.756971 oarepo-ui-5.1.9/oarepo_ui/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.784971 oarepo-ui-5.1.9/oarepo_ui/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/oarepo_ui/vite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:47:16.788971 oarepo-ui-5.1.9/oarepo_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-24 17:47:16.000000 oarepo-ui-5.1.9/oarepo_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-03-24 17:47:16.000000 oarepo-ui-5.1.9/oarepo_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 17:47:16.000000 oarepo-ui-5.1.9/oarepo_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-24 17:47:16.000000 oarepo-ui-5.1.9/oarepo_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 17:46:20.000000 oarepo-ui-5.1.9/oarepo_ui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-24 17:47:16.000000 oarepo-ui-5.1.9/oarepo_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-24 17:47:16.000000 oarepo-ui-5.1.9/oarepo_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-24 17:47:16.788971 oarepo-ui-5.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 17:44:34.000000 oarepo-ui-5.1.9/setup.py
```

### Comparing `oarepo-ui-5.1.8/MANIFEST.in` & `oarepo-ui-5.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/PKG-INFO` & `oarepo-ui-5.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-ui
-Version: 5.1.8
+Version: 5.1.9
 Summary: UI module for invenio 3.5+
 Home-page: https://github.com/oarepo/oarepo-ui
 Author: Mirek Simek
 Author-email: miroslav.simek@vscht.cz
 License: MIT
 Keywords: oarepo ui
 Platform: any
```

### Comparing `oarepo-ui-5.1.8/README.md` & `oarepo-ui-5.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/babel.ini` & `oarepo-ui-5.1.9/babel.ini`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/cli.py` & `oarepo-ui-5.1.9/oarepo_ui/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/config.py` & `oarepo-ui-5.1.9/oarepo_ui/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/css/builtin.css` & `oarepo-ui-5.1.9/oarepo_ui/css/builtin.css`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/ext.py` & `oarepo-ui-5.1.9/oarepo_ui/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/resources/components.py` & `oarepo-ui-5.1.9/oarepo_ui/resources/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/resources/config.py` & `oarepo-ui-5.1.9/oarepo_ui/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/resources/resource.py` & `oarepo-ui-5.1.9/oarepo_ui/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/resources/templating/catalog.py` & `oarepo-ui-5.1.9/oarepo_ui/resources/templating/catalog.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/resources/templating/data.py` & `oarepo-ui-5.1.9/oarepo_ui/resources/templating/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import html
 from typing import Union
 
 from oarepo_runtime.i18n import gettext
 
 
 class FieldData:
@@ -60,16 +61,15 @@
 
                 if idx < len(self.__data):
                     return FieldData(
                         self.__data[idx], self.__ui.get("child", {}), self.__path + [idx]
                     )
                 return EMPTY_FIELD_DATA
             except ValueError:
-                return EMPTY_FIELD_DATA
-                # return self._select(name)
+                return self._select(name)
 
         return EMPTY_FIELD_DATA
 
     def __getattr__(self, name):
         return self.__get(name)
 
     def __getitem__(self, name):
@@ -139,9 +139,19 @@
     def _is_dict(self):
         return isinstance(self.__data, dict)
 
     @property
     def _is_primitive(self):
         return self._has_value and not self._is_array and not self._is_dict
 
+    def __eq__(self, other):
+        if isinstance(other, FieldData):
+            return self.__data == other.__data
+        return False
+
+    def __lt__(self, other):
+        if isinstance(other, FieldData):
+            return json.dumps(self.__data, sort_keys=True) < json.dumps(other.__data, sort_keys=True)
+        return False
+
 
 EMPTY_FIELD_DATA = FieldData({}, {})
```

### Comparing `oarepo-ui-5.1.8/oarepo_ui/resources/templating/filters.py` & `oarepo-ui-5.1.9/oarepo_ui/resources/templating/filters.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/services/custom_fields.py` & `oarepo-ui-5.1.9/oarepo_ui/services/custom_fields.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/components/EditForm.jinja` & `oarepo-ui-5.1.9/oarepo_ui/templates/components/EditForm.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/components/Multilingual.jinja` & `oarepo-ui-5.1.9/oarepo_ui/templates/components/Multilingual.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/ICustomFields.jinja` & `oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/ICustomFields.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/components/datafields/IField.jinja` & `oarepo-ui-5.1.9/oarepo_ui/templates/components/datafields/IField.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/detail.html` & `oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/detail.html`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/footer.html` & `oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/footer.html`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/form.html` & `oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/form.html`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/header.html` & `oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/header.html`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/templates/oarepo_ui/header_login.html` & `oarepo-ui-5.1.9/oarepo_ui/templates/oarepo_ui/header_login.html`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/client.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/client.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/recordSerializer.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/api/recordSerializer.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/burgermenu.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/components/burgermenu.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/custom-components.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/custom-components.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/ArrayFieldItem.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ArrayFieldItem/ArrayFieldItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/BaseForm.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseForm/BaseForm.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/BaseFormLayout.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/BaseFormLayout/BaseFormLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/ConfirmationModal.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ConfirmationModal/ConfirmationModal.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/DeleteButton.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/DeleteButton/DeleteButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/DatePickerHeader.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/DatePickerHeader.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDatePickerWrapper.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDatePickerWrapper.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDateRangePickerField.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFDateRangePickerField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFSingleDatePickerField.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/EDTFSingleDatePickerField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/InputElement.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/InputElement.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/hooks.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/hooks.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/utils.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/EDTFDatePickerField/utils.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/FormFeedback.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormFeedback/FormFeedback.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/FormikStateLogger.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/FormikStateLogger/FormikStateLogger.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/I18nRichInputField.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nRichInputField/I18nRichInputField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/I18nTextInputField.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/I18nTextInputField/I18nTextInputField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/LanguageSelectField.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/LanguageSelectField/LanguageSelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/MultilingualTextInput.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/MultilingualTextInput/MultilingualTextInput.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/PreviewButton.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PreviewButton/PreviewButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/PublishButton.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/PublishButton/PublishButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiModal.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiModal.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiResultsList.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/ExternalApiResultsList.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/NoResultsMessage.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/NoResultsMessage.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectField.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectFieldInternal.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/RelatedSelectField/RelatedSelectFieldInternal.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/SaveButton.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/SaveButton/SaveButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/ValidateButton.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/ValidateButton/ValidateButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/index.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/components/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/hooks.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/hooks.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/util.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/forms/util.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ActiveFiltersElement.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ActiveFiltersElement.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ClearFiltersButton.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ClearFiltersButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/DynamicResultsListItem.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/DynamicResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/EmptyResultsElement.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/EmptyResultsElement.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ResultCount.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/ResultCount.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppLayout.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResultOptions.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResultOptions.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResults.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchAppResults.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchFiltersToggleElement.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchFiltersToggleElement.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchappSearchbarElement.jsx` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/SearchappSearchbarElement.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/constants.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/constants.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/index.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/util.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/search/util.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/util.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/js/oarepo_ui/util.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/custom-components.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/custom-components.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/datepicker.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/datepicker.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/dl_table.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/dl_table.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_data.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_data.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_label.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/field_label.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/lang_tag.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/lang_tag.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/multilingual_tabs.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/multilingual_tabs.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_footer.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_footer.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_header.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/page_header.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/search_link.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/search_link.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/section.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/section.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/separated.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/separated.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/value_list.less` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/definitions/value_list.less`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/menu.overrides` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/collections/menu.overrides`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/globals/site.overrides` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/globals/site.overrides`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/accordion.overrides` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/less/oarepo_ui/themes/default/modules/accordion.overrides`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ArrayWidget.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ArrayWidget.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ComplexWidget.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/templates/custom_fields/ComplexWidget.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/i18next.js` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/LC_MESSAGES/translations.json` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/LC_MESSAGES/translations.json` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/translations.pot` & `oarepo-ui-5.1.9/oarepo_ui/theme/assets/semantic-ui/translations/oarepo_ui/translations.pot`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/theme/webpack.py` & `oarepo-ui-5.1.9/oarepo_ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/translations/cs/LC_MESSAGES/messages.mo` & `oarepo-ui-5.1.9/oarepo_ui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/translations/cs/LC_MESSAGES/messages.po` & `oarepo-ui-5.1.9/oarepo_ui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/translations/en/LC_MESSAGES/messages.mo` & `oarepo-ui-5.1.9/oarepo_ui/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/translations/en/LC_MESSAGES/messages.po` & `oarepo-ui-5.1.9/oarepo_ui/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/translations/messages.pot` & `oarepo-ui-5.1.9/oarepo_ui/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/utils.py` & `oarepo-ui-5.1.9/oarepo_ui/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/views.py` & `oarepo-ui-5.1.9/oarepo_ui/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui/vite.py` & `oarepo-ui-5.1.9/oarepo_ui/vite.py`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/oarepo_ui.egg-info/PKG-INFO` & `oarepo-ui-5.1.9/oarepo_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-ui
-Version: 5.1.8
+Version: 5.1.9
 Summary: UI module for invenio 3.5+
 Home-page: https://github.com/oarepo/oarepo-ui
 Author: Mirek Simek
 Author-email: miroslav.simek@vscht.cz
 License: MIT
 Keywords: oarepo ui
 Platform: any
```

### Comparing `oarepo-ui-5.1.8/oarepo_ui.egg-info/SOURCES.txt` & `oarepo-ui-5.1.9/oarepo_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-ui-5.1.8/setup.cfg` & `oarepo-ui-5.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-ui
-version = 5.1.8
+version = 5.1.9
 description = UI module for invenio 3.5+
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = oarepo ui
 license = MIT
 author = Mirek Simek
 author_email = miroslav.simek@vscht.cz
```

