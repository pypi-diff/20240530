# Comparing `tmp/airbyte_source_hubspot-4.2.0.tar.gz` & `tmp/airbyte_source_hubspot-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_hubspot-4.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_hubspot-4.2.1.tar", max compression
```

## Comparing `airbyte_source_hubspot-4.2.0.tar` & `airbyte_source_hubspot-4.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     4524 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/README.md
--rw-r--r--   0        0        0      796 2024-05-25 00:24:44.303227 airbyte_source_hubspot-4.2.0/pyproject.toml
--rw-r--r--   0        0        0      124 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/__init__.py
--rw-r--r--   0        0        0      154 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/constants.py
--rw-r--r--   0        0        0     1885 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/errors.py
--rw-r--r--   0        0        0     3809 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/helpers.py
--rw-r--r--   0        0        0      233 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/run.py
--rw-r--r--   0        0        0     6624 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/campaigns.json
--rw-r--r--   0        0        0      905 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/companies.json
--rw-r--r--   0        0        0     1415 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/companies_property_history.json
--rw-r--r--   0        0        0     6086 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contact_lists.json
--rw-r--r--   0        0        0      933 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts.json
--rw-r--r--   0        0        0     1866 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_form_submissions.json
--rw-r--r--   0        0        0     1008 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_list_memberships.json
--rw-r--r--   0        0        0     6620 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_merged_audit.json
--rw-r--r--   0        0        0     2093 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_property_history.json
--rw-r--r--   0        0        0     3046 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deal_pipelines.json
--rw-r--r--   0        0        0    30732 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deals.json
--rw-r--r--   0        0        0    18631 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deals_archived.json
--rw-r--r--   0        0        0     1276 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deals_property_history.json
--rw-r--r--   0        0        0     9554 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/email_events.json
--rw-r--r--   0        0        0     1670 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/email_subscriptions.json
--rw-r--r--   0        0        0    26695 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements.json
--rw-r--r--   0        0        0    18505 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_calls.json
--rw-r--r--   0        0        0    25799 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_emails.json
--rw-r--r--   0        0        0    17798 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_meetings.json
--rw-r--r--   0        0        0    11074 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_notes.json
--rw-r--r--   0        0        0    20314 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_tasks.json
--rw-r--r--   0        0        0     5736 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/feedback_submissions.json
--rw-r--r--   0        0        0     1332 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/form_submissions.json
--rw-r--r--   0        0        0     8454 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/forms.json
--rw-r--r--   0        0        0     3717 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/goals.json
--rw-r--r--   0        0        0      692 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/line_items.json
--rw-r--r--   0        0        0    24533 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/marketing_emails.json
--rw-r--r--   0        0        0     1763 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/owners.json
--rw-r--r--   0        0        0     1733 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/owners_archived.json
--rw-r--r--   0        0        0      676 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/products.json
--rw-r--r--   0        0        0     3742 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/shared/default_event_properties.json
--rw-r--r--   0        0        0     2414 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/subscription_changes.json
--rw-r--r--   0        0        0     2976 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/ticket_pipelines.json
--rw-r--r--   0        0        0     1304 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/tickets.json
--rw-r--r--   0        0        0     7534 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/schemas/workflows.json
--rw-r--r--   0        0        0     9749 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/source.py
--rw-r--r--   0        0        0     4559 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/spec.yaml
--rw-r--r--   0        0        0    96992 2024-05-24 21:49:03.000000 airbyte_source_hubspot-4.2.0/source_hubspot/streams.py
--rw-r--r--   0        0        0     5228 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4524 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/README.md
+-rw-r--r--   0        0        0      796 2024-05-30 16:59:19.088627 airbyte_source_hubspot-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/__init__.py
+-rw-r--r--   0        0        0      154 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/constants.py
+-rw-r--r--   0        0        0     1885 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/errors.py
+-rw-r--r--   0        0        0     3809 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/helpers.py
+-rw-r--r--   0        0        0      233 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/run.py
+-rw-r--r--   0        0        0     6624 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/campaigns.json
+-rw-r--r--   0        0        0      905 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/companies.json
+-rw-r--r--   0        0        0     1415 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/companies_property_history.json
+-rw-r--r--   0        0        0     6086 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contact_lists.json
+-rw-r--r--   0        0        0      933 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts.json
+-rw-r--r--   0        0        0     1866 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_form_submissions.json
+-rw-r--r--   0        0        0     1008 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_list_memberships.json
+-rw-r--r--   0        0        0     6620 2024-05-30 16:54:21.663133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_merged_audit.json
+-rw-r--r--   0        0        0     2093 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_property_history.json
+-rw-r--r--   0        0        0     3046 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deal_pipelines.json
+-rw-r--r--   0        0        0    30732 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deals.json
+-rw-r--r--   0        0        0    18631 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deals_archived.json
+-rw-r--r--   0        0        0     1276 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deals_property_history.json
+-rw-r--r--   0        0        0     9554 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/email_events.json
+-rw-r--r--   0        0        0     1670 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/email_subscriptions.json
+-rw-r--r--   0        0        0    26695 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements.json
+-rw-r--r--   0        0        0    18505 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_calls.json
+-rw-r--r--   0        0        0    25799 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_emails.json
+-rw-r--r--   0        0        0    17798 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_meetings.json
+-rw-r--r--   0        0        0    11074 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_notes.json
+-rw-r--r--   0        0        0    20314 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_tasks.json
+-rw-r--r--   0        0        0     5736 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/feedback_submissions.json
+-rw-r--r--   0        0        0     1332 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/form_submissions.json
+-rw-r--r--   0        0        0     8454 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/forms.json
+-rw-r--r--   0        0        0     3717 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/goals.json
+-rw-r--r--   0        0        0      692 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/line_items.json
+-rw-r--r--   0        0        0    24533 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/marketing_emails.json
+-rw-r--r--   0        0        0     1763 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/owners.json
+-rw-r--r--   0        0        0     1733 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/owners_archived.json
+-rw-r--r--   0        0        0      676 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/products.json
+-rw-r--r--   0        0        0     3742 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/shared/default_event_properties.json
+-rw-r--r--   0        0        0     2414 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/subscription_changes.json
+-rw-r--r--   0        0        0     2976 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/ticket_pipelines.json
+-rw-r--r--   0        0        0     1304 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/tickets.json
+-rw-r--r--   0        0        0     7534 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/schemas/workflows.json
+-rw-r--r--   0        0        0    10534 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/source.py
+-rw-r--r--   0        0        0     4559 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/spec.yaml
+-rw-r--r--   0        0        0    96992 2024-05-30 16:54:21.667133 airbyte_source_hubspot-4.2.1/source_hubspot/streams.py
+-rw-r--r--   0        0        0     5228 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.2.1/PKG-INFO
```

### Comparing `airbyte_source_hubspot-4.2.0/README.md` & `airbyte_source_hubspot-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/pyproject.toml` & `airbyte_source_hubspot-4.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.2.0"
+version = "4.2.1"
 name = "airbyte-source-hubspot"
 description = "Source implementation for HubSpot."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/errors.py` & `airbyte_source_hubspot-4.2.1/source_hubspot/errors.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/helpers.py` & `airbyte_source_hubspot-4.2.1/source_hubspot/helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/campaigns.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/companies.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/companies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/companies_property_history.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/companies_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contact_lists.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contact_lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_form_submissions.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_form_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_list_memberships.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_list_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_merged_audit.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_merged_audit.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/contacts_property_history.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/contacts_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deal_pipelines.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deal_pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deals.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deals_archived.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deals_archived.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/deals_property_history.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/deals_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/email_events.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/email_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/email_subscriptions.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/email_subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_calls.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_calls.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_emails.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_emails.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_meetings.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_meetings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_notes.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_notes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/engagements_tasks.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/engagements_tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/feedback_submissions.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/feedback_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/form_submissions.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/form_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/forms.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/forms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/goals.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/goals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/line_items.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/marketing_emails.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/marketing_emails.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/owners.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/owners.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/owners_archived.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/owners_archived.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/products.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/shared/default_event_properties.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/shared/default_event_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/subscription_changes.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/subscription_changes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/ticket_pipelines.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/ticket_pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/tickets.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/schemas/workflows.json` & `airbyte_source_hubspot-4.2.1/source_hubspot/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/source.py` & `airbyte_source_hubspot-4.2.1/source_hubspot/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
+import traceback
 from http import HTTPStatus
 from itertools import chain
-from typing import Any, Generator, List, Mapping, Optional, Tuple
+from typing import Any, Generator, List, Mapping, Optional, Tuple, Union
 
-import requests
+from airbyte_cdk.models import FailureType
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
+from airbyte_cdk.sources.streams.http import HttpClient
+from airbyte_cdk.sources.streams.http.error_handlers import ErrorResolution, HttpStatusErrorHandler, ResponseAction
 from requests import HTTPError
 from source_hubspot.errors import HubspotInvalidAuth
 from source_hubspot.streams import (
     API,
     Campaigns,
     Companies,
     CompaniesPropertyHistory,
@@ -93,15 +96,24 @@
             error_msg = repr(e)
         return alive, error_msg
 
     def get_granted_scopes(self, authenticator):
         try:
             access_token = authenticator.get_access_token()
             url = f"https://api.hubapi.com/oauth/v1/access-tokens/{access_token}"
-            response = requests.get(url=url)
+            error_resolution = ErrorResolution(
+                ResponseAction.RETRY, FailureType.transient_error, "Internal error attempting to get scopes."
+            )
+            error_mapping = {500: error_resolution, 502: error_resolution, 504: error_resolution}
+            http_client = HttpClient(
+                name="get hubspot granted scopes client",
+                logger=self.logger,
+                error_handler=HttpStatusErrorHandler(logger=self.logger, error_mapping=error_mapping),
+            )
+            request, response = http_client.send_request("get", url, request_kwargs={})
             response.raise_for_status()
             response_json = response.json()
             granted_scopes = response_json["scopes"]
             return granted_scopes
         except Exception as e:
             return False, repr(e)
```

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/spec.yaml` & `airbyte_source_hubspot-4.2.1/source_hubspot/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/source_hubspot/streams.py` & `airbyte_source_hubspot-4.2.1/source_hubspot/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.2.0/PKG-INFO` & `airbyte_source_hubspot-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-hubspot
-Version: 4.2.0
+Version: 4.2.1
 Summary: Source implementation for HubSpot.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

