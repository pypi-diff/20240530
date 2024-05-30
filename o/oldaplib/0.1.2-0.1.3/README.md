# Comparing `tmp/oldaplib-0.1.2.tar.gz` & `tmp/oldaplib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldaplib-0.1.2.tar", max compression
+gzip compressed data, was "oldaplib-0.1.3.tar", max compression
```

## Comparing `oldaplib-0.1.2.tar` & `oldaplib-0.1.3.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0     1406 2024-05-17 21:15:50.741523 oldaplib-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.860798 oldaplib-0.1.2/oldaplib/__init__.py
--rw-r--r--   0        0        0     9892 2024-05-24 22:11:53.229656 oldaplib-0.1.2/oldaplib/ontologies/admin.trig
--rw-r--r--   0        0        0    31964 2024-05-24 20:29:28.376369 oldaplib-0.1.2/oldaplib/ontologies/oldap.shacl.trig
--rw-r--r--   0        0        0    31147 2024-05-24 20:29:28.379250 oldaplib-0.1.2/oldaplib/ontologies/oldap.ttl
--rw-r--r--   0        0        0    17976 2024-05-17 12:28:38.672082 oldaplib-0.1.2/oldaplib/src/ObjectFactory.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.862923 oldaplib-0.1.2/oldaplib/src/__init__.py
--rw-r--r--   0        0        0    19932 2024-05-26 21:39:24.866447 oldaplib-0.1.2/oldaplib/src/connection.py
--rw-r--r--   0        0        0    14065 2024-05-17 16:27:00.108249 oldaplib-0.1.2/oldaplib/src/datamodel.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.863726 oldaplib-0.1.2/oldaplib/src/dtypes/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-17 12:28:38.584913 oldaplib-0.1.2/oldaplib/src/dtypes/bnode.py
--rw-r--r--   0        0        0     4917 2024-05-17 12:28:38.714172 oldaplib-0.1.2/oldaplib/src/dtypes/languagein.py
--rw-r--r--   0        0        0     1067 2024-05-17 12:28:38.356660 oldaplib-0.1.2/oldaplib/src/dtypes/namespaceiri.py
--rw-r--r--   0        0        0     4088 2024-05-17 12:28:38.589960 oldaplib-0.1.2/oldaplib/src/dtypes/rdfset.py
--rw-r--r--   0        0        0     1900 2024-05-17 12:28:38.505893 oldaplib-0.1.2/oldaplib/src/dtypes/xsdset.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.865443 oldaplib-0.1.2/oldaplib/src/enums/__init__.py
--rw-r--r--   0        0        0      828 2024-05-17 12:28:38.730926 oldaplib-0.1.2/oldaplib/src/enums/action.py
--rw-r--r--   0        0        0     4623 2024-05-17 12:28:38.372733 oldaplib-0.1.2/oldaplib/src/enums/language.py
--rw-r--r--   0        0        0     2466 2024-05-17 16:17:14.367204 oldaplib-0.1.2/oldaplib/src/enums/permissions.py
--rw-r--r--   0        0        0      376 2024-05-27 19:57:54.827687 oldaplib-0.1.2/oldaplib/src/enums/permissionsetattr.py
--rw-r--r--   0        0        0     2069 2024-05-16 21:38:25.885179 oldaplib-0.1.2/oldaplib/src/enums/propertyclassattr.py
--rw-r--r--   0        0        0      245 2024-05-24 20:29:28.380276 oldaplib-0.1.2/oldaplib/src/enums/resourceclassattr.py
--rw-r--r--   0        0        0      636 2024-05-16 20:58:19.867251 oldaplib-0.1.2/oldaplib/src/enums/sparql_result_format.py
--rw-r--r--   0        0        0      922 2024-05-17 16:16:02.047994 oldaplib-0.1.2/oldaplib/src/enums/userdataclassattr.py
--rw-r--r--   0        0        0     6133 2024-05-16 20:58:19.867821 oldaplib-0.1.2/oldaplib/src/enums/xsd_datatypes.py
--rw-r--r--   0        0        0      406 2024-05-25 22:49:56.860916 oldaplib-0.1.2/oldaplib/src/globalconfig.py
--rw-r--r--   0        0        0     2054 2024-05-18 20:31:39.060235 oldaplib-0.1.2/oldaplib/src/helpers/Notify.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.868316 oldaplib-0.1.2/oldaplib/src/helpers/__init__.py
--rw-r--r--   0        0        0    13645 2024-05-26 21:25:16.747717 oldaplib-0.1.2/oldaplib/src/helpers/context.py
--rw-r--r--   0        0        0    30931 2024-05-27 21:54:21.002326 oldaplib-0.1.2/oldaplib/src/helpers/langstring.py
--rw-r--r--   0        0        0     2031 2024-05-24 20:29:28.381026 oldaplib-0.1.2/oldaplib/src/helpers/observable_dict.py
--rw-r--r--   0        0        0     5525 2024-05-18 20:48:09.073657 oldaplib-0.1.2/oldaplib/src/helpers/observable_set.py
--rw-r--r--   0        0        0     1265 2024-05-16 21:17:59.026464 oldaplib-0.1.2/oldaplib/src/helpers/oldaperror.py
--rw-r--r--   0        0        0     1141 2024-05-17 12:28:38.168566 oldaplib-0.1.2/oldaplib/src/helpers/propertyclass_singleton.py
--rw-r--r--   0        0        0    10146 2024-05-19 22:50:03.808918 oldaplib-0.1.2/oldaplib/src/helpers/query_processor.py
--rw-r--r--   0        0        0     3218 2024-05-17 12:28:38.445610 oldaplib-0.1.2/oldaplib/src/helpers/semantic_version.py
--rw-r--r--   0        0        0     4086 2024-05-16 20:58:19.870752 oldaplib-0.1.2/oldaplib/src/helpers/serializer.py
--rw-r--r--   0        0        0      332 2024-05-25 22:49:56.844500 oldaplib-0.1.2/oldaplib/src/helpers/singletonmeta.py
--rw-r--r--   0        0        0    12609 2024-05-19 20:59:15.236199 oldaplib-0.1.2/oldaplib/src/helpers/tools.py
--rw-r--r--   0        0        0     2430 2024-05-17 12:28:38.306954 oldaplib-0.1.2/oldaplib/src/iconnection.py
--rw-r--r--   0        0        0     7590 2024-05-22 21:47:27.190971 oldaplib-0.1.2/oldaplib/src/in_project.py
--rw-r--r--   0        0        0     3036 2024-05-17 12:28:38.146377 oldaplib-0.1.2/oldaplib/src/model.py
--rw-r--r--   0        0        0    21622 2024-05-17 16:12:17.599380 oldaplib-0.1.2/oldaplib/src/oldaplist.py
--rw-r--r--   0        0        0     2372 2024-05-17 16:10:49.541460 oldaplib-0.1.2/oldaplib/src/oldaplistnode.py
--rw-r--r--   0        0        0    27015 2024-05-27 19:57:54.834182 oldaplib-0.1.2/oldaplib/src/permissionset.py
--rw-r--r--   0        0        0    33455 2024-05-27 21:38:42.877206 oldaplib-0.1.2/oldaplib/src/project.py
--rw-r--r--   0        0        0    58711 2024-05-20 20:46:37.094562 oldaplib-0.1.2/oldaplib/src/propertyclass.py
--rw-r--r--   0        0        0    54918 2024-05-24 20:29:28.381983 oldaplib-0.1.2/oldaplib/src/resourceclass.py
--rw-r--r--   0        0        0    26623 2024-05-27 21:57:15.307605 oldaplib-0.1.2/oldaplib/src/user.py
--rw-r--r--   0        0        0    30434 2024-05-17 16:06:07.068855 oldaplib-0.1.2/oldaplib/src/user_dataclass.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.874593 oldaplib-0.1.2/oldaplib/src/xsd/__init__.py
--rw-r--r--   0        0        0     7896 2024-05-17 12:28:38.536038 oldaplib-0.1.2/oldaplib/src/xsd/floatingpoint.py
--rw-r--r--   0        0        0     4821 2024-05-26 22:05:53.954324 oldaplib-0.1.2/oldaplib/src/xsd/iri.py
--rw-r--r--   0        0        0     1499 2024-05-16 20:58:19.875428 oldaplib-0.1.2/oldaplib/src/xsd/xsd.py
--rw-r--r--   0        0        0     5523 2024-05-25 22:00:25.651776 oldaplib-0.1.2/oldaplib/src/xsd/xsd_anyuri.py
--rw-r--r--   0        0        0     3543 2024-05-17 12:28:38.710082 oldaplib-0.1.2/oldaplib/src/xsd/xsd_base64binary.py
--rw-r--r--   0        0        0     2648 2024-05-20 20:22:47.068509 oldaplib-0.1.2/oldaplib/src/xsd/xsd_boolean.py
--rw-r--r--   0        0        0      979 2024-05-17 12:28:38.314066 oldaplib-0.1.2/oldaplib/src/xsd/xsd_byte.py
--rw-r--r--   0        0        0     7043 2024-05-17 12:28:38.281355 oldaplib-0.1.2/oldaplib/src/xsd/xsd_date.py
--rw-r--r--   0        0        0     3972 2024-05-17 12:28:38.567099 oldaplib-0.1.2/oldaplib/src/xsd/xsd_datetime.py
--rw-r--r--   0        0        0     3904 2024-05-17 12:28:38.599870 oldaplib-0.1.2/oldaplib/src/xsd/xsd_datetimestamp.py
--rw-r--r--   0        0        0     1376 2024-05-17 12:28:38.696167 oldaplib-0.1.2/oldaplib/src/xsd/xsd_decimal.py
--rw-r--r--   0        0        0     1422 2024-05-17 12:28:38.618206 oldaplib-0.1.2/oldaplib/src/xsd/xsd_double.py
--rw-r--r--   0        0        0     3319 2024-05-17 12:28:38.203063 oldaplib-0.1.2/oldaplib/src/xsd/xsd_duration.py
--rw-r--r--   0        0        0     1242 2024-05-17 12:28:38.746441 oldaplib-0.1.2/oldaplib/src/xsd/xsd_float.py
--rw-r--r--   0        0        0     3517 2024-05-17 12:28:38.705599 oldaplib-0.1.2/oldaplib/src/xsd/xsd_gday.py
--rw-r--r--   0        0        0     3628 2024-05-17 12:28:38.677544 oldaplib-0.1.2/oldaplib/src/xsd/xsd_gmonth.py
--rw-r--r--   0        0        0     3840 2024-05-17 12:28:38.519315 oldaplib-0.1.2/oldaplib/src/xsd/xsd_gmonthday.py
--rw-r--r--   0        0        0     3780 2024-05-17 12:28:38.723526 oldaplib-0.1.2/oldaplib/src/xsd/xsd_gyear.py
--rw-r--r--   0        0        0     4186 2024-05-17 12:28:38.657789 oldaplib-0.1.2/oldaplib/src/xsd/xsd_gyearmonth.py
--rw-r--r--   0        0        0     3073 2024-05-17 12:28:38.595486 oldaplib-0.1.2/oldaplib/src/xsd/xsd_hexbinary.py
--rw-r--r--   0        0        0      617 2024-05-17 12:28:38.552712 oldaplib-0.1.2/oldaplib/src/xsd/xsd_id.py
--rw-r--r--   0        0        0      647 2024-05-17 12:28:38.562362 oldaplib-0.1.2/oldaplib/src/xsd/xsd_idref.py
--rw-r--r--   0        0        0     1123 2024-05-17 12:28:38.236235 oldaplib-0.1.2/oldaplib/src/xsd/xsd_int.py
--rw-r--r--   0        0        0     5727 2024-05-17 12:28:38.644946 oldaplib-0.1.2/oldaplib/src/xsd/xsd_integer.py
--rw-r--r--   0        0        0     3504 2024-05-17 12:28:38.346404 oldaplib-0.1.2/oldaplib/src/xsd/xsd_language.py
--rw-r--r--   0        0        0     1179 2024-05-17 12:28:38.423635 oldaplib-0.1.2/oldaplib/src/xsd/xsd_long.py
--rw-r--r--   0        0        0     3436 2024-05-17 12:28:38.741813 oldaplib-0.1.2/oldaplib/src/xsd/xsd_name.py
--rw-r--r--   0        0        0     5067 2024-05-25 20:39:47.835986 oldaplib-0.1.2/oldaplib/src/xsd/xsd_ncname.py
--rw-r--r--   0        0        0      999 2024-05-17 12:28:38.701096 oldaplib-0.1.2/oldaplib/src/xsd/xsd_negativeinteger.py
--rw-r--r--   0        0        0     3298 2024-05-17 12:28:38.181051 oldaplib-0.1.2/oldaplib/src/xsd/xsd_nmtoken.py
--rw-r--r--   0        0        0     1043 2024-05-17 12:28:38.351243 oldaplib-0.1.2/oldaplib/src/xsd/xsd_nonnegativeinteger.py
--rw-r--r--   0        0        0      964 2024-05-17 12:28:38.499113 oldaplib-0.1.2/oldaplib/src/xsd/xsd_nonpositiveinteger.py
--rw-r--r--   0        0        0     3967 2024-05-17 12:28:38.435583 oldaplib-0.1.2/oldaplib/src/xsd/xsd_normalizedstring.py
--rw-r--r--   0        0        0      945 2024-05-17 12:28:38.528978 oldaplib-0.1.2/oldaplib/src/xsd/xsd_positiveinteger.py
--rw-r--r--   0        0        0     6750 2024-05-17 12:28:38.271692 oldaplib-0.1.2/oldaplib/src/xsd/xsd_qname.py
--rw-r--r--   0        0        0      989 2024-05-17 12:28:38.240593 oldaplib-0.1.2/oldaplib/src/xsd/xsd_short.py
--rw-r--r--   0        0        0     9512 2024-05-17 12:28:38.513898 oldaplib-0.1.2/oldaplib/src/xsd/xsd_string.py
--rw-r--r--   0        0        0     3670 2024-05-17 12:28:38.458232 oldaplib-0.1.2/oldaplib/src/xsd/xsd_time.py
--rw-r--r--   0        0        0     3546 2024-05-17 12:28:38.302060 oldaplib-0.1.2/oldaplib/src/xsd/xsd_token.py
--rw-r--r--   0        0        0     1027 2024-05-17 12:28:38.682094 oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedbyte.py
--rw-r--r--   0        0        0     1040 2024-05-17 12:28:38.576156 oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedint.py
--rw-r--r--   0        0        0     1007 2024-05-17 12:28:38.524210 oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedlong.py
--rw-r--r--   0        0        0     1012 2024-05-17 12:28:38.572122 oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedshort.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.898288 oldaplib-0.1.2/oldaplib/test/__init__.py
--rw-r--r--   0        0        0    14309 2024-05-24 20:29:28.389690 oldaplib-0.1.2/oldaplib/test/gaga.trig
--rw-r--r--   0        0        0     1759 2024-05-18 22:18:06.660501 oldaplib-0.1.2/oldaplib/test/propclass_test.trig
--rw-r--r--   0        0        0    13591 2024-05-26 21:44:40.793610 oldaplib-0.1.2/oldaplib/test/test_connection.py
--rw-r--r--   0        0        0     4777 2024-05-25 22:24:17.528153 oldaplib-0.1.2/oldaplib/test/test_context.py
--rw-r--r--   0        0        0    21746 2024-05-24 20:29:28.392421 oldaplib-0.1.2/oldaplib/test/test_datamodel.py
--rw-r--r--   0        0        0     8221 2024-05-17 12:33:33.047906 oldaplib-0.1.2/oldaplib/test/test_dtypes.py
--rw-r--r--   0        0        0     7774 2024-05-17 16:39:06.614379 oldaplib-0.1.2/oldaplib/test/test_in_project.py
--rw-r--r--   0        0        0    11628 2024-05-17 12:28:38.294685 oldaplib-0.1.2/oldaplib/test/test_langstring.py
--rw-r--r--   0        0        0     8826 2024-05-17 12:28:38.474410 oldaplib-0.1.2/oldaplib/test/test_language_in.py
--rw-r--r--   0        0        0     3645 2024-05-17 16:00:20.113780 oldaplib-0.1.2/oldaplib/test/test_objectfactory.py
--rw-r--r--   0        0        0     6249 2024-05-17 12:28:38.736345 oldaplib-0.1.2/oldaplib/test/test_observable_set.py
--rw-r--r--   0        0        0     7288 2024-05-17 16:40:34.925874 oldaplib-0.1.2/oldaplib/test/test_oldaplist.py
--rw-r--r--   0        0        0    14233 2024-05-27 19:58:31.120104 oldaplib-0.1.2/oldaplib/test/test_permissionset.py
--rw-r--r--   0        0        0    17012 2024-05-27 19:38:39.071380 oldaplib-0.1.2/oldaplib/test/test_project.py
--rw-r--r--   0        0        0    28492 2024-05-17 12:33:32.999538 oldaplib-0.1.2/oldaplib/test/test_propertyclass.py
--rw-r--r--   0        0        0    42274 2024-05-24 20:29:28.394589 oldaplib-0.1.2/oldaplib/test/test_resourceclass.py
--rw-r--r--   0        0        0     3392 2024-05-17 12:28:38.215443 oldaplib-0.1.2/oldaplib/test/test_semantic_version.py
--rw-r--r--   0        0        0    40179 2024-05-25 22:37:42.478850 oldaplib-0.1.2/oldaplib/test/test_user.py
--rw-r--r--   0        0        0    64182 2024-05-17 12:33:33.043637 oldaplib-0.1.2/oldaplib/test/test_xsd_datatypes.py
--rw-r--r--   0        0        0    12312 2024-05-20 22:29:47.421485 oldaplib-0.1.2/oldaplib/testdata/connection_test.trig
--rw-r--r--   0        0        0     1382 2024-05-16 21:56:28.046244 oldaplib-0.1.2/oldaplib/testdata/datamodel_test.trig
--rw-r--r--   0        0        0    14936 2024-05-24 20:29:28.395766 oldaplib-0.1.2/oldaplib/testdata/objectfactory_test.trig
--rw-r--r--   0        0        0      303 2024-05-16 21:56:27.962931 oldaplib-0.1.2/oldaplib/testit.http
--rw-r--r--   0        0        0      914 2024-05-27 22:17:08.143801 oldaplib-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 oldaplib-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1406 2024-05-17 21:15:50.741523 oldaplib-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 20:58:19.860798 oldaplib-0.1.3/oldaplib/__init__.py
+-rw-r--r--   0        0        0     9892 2024-05-24 22:11:53.229656 oldaplib-0.1.3/oldaplib/ontologies/admin.trig
+-rw-r--r--   0        0        0    31964 2024-05-24 20:29:28.376369 oldaplib-0.1.3/oldaplib/ontologies/oldap.shacl.trig
+-rw-r--r--   0        0        0    31147 2024-05-24 20:29:28.379250 oldaplib-0.1.3/oldaplib/ontologies/oldap.ttl
+-rw-r--r--   0        0        0    17976 2024-05-17 12:28:38.672082 oldaplib-0.1.3/oldaplib/src/ObjectFactory.py
+-rw-r--r--   0        0        0        0 2024-05-16 20:58:19.862923 oldaplib-0.1.3/oldaplib/src/__init__.py
+-rw-r--r--   0        0        0    19932 2024-05-26 21:39:24.866447 oldaplib-0.1.3/oldaplib/src/connection.py
+-rw-r--r--   0        0        0    14065 2024-05-17 16:27:00.108249 oldaplib-0.1.3/oldaplib/src/datamodel.py
+-rw-r--r--   0        0        0        0 2024-05-16 20:58:19.863726 oldaplib-0.1.3/oldaplib/src/dtypes/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-17 12:28:38.584913 oldaplib-0.1.3/oldaplib/src/dtypes/bnode.py
+-rw-r--r--   0        0        0     4917 2024-05-17 12:28:38.714172 oldaplib-0.1.3/oldaplib/src/dtypes/languagein.py
+-rw-r--r--   0        0        0     1067 2024-05-17 12:28:38.356660 oldaplib-0.1.3/oldaplib/src/dtypes/namespaceiri.py
+-rw-r--r--   0        0        0     4088 2024-05-17 12:28:38.589960 oldaplib-0.1.3/oldaplib/src/dtypes/rdfset.py
+-rw-r--r--   0        0        0     1900 2024-05-17 12:28:38.505893 oldaplib-0.1.3/oldaplib/src/dtypes/xsdset.py
+-rw-r--r--   0        0        0        0 2024-05-16 20:58:19.865443 oldaplib-0.1.3/oldaplib/src/enums/__init__.py
+-rw-r--r--   0        0        0      828 2024-05-17 12:28:38.730926 oldaplib-0.1.3/oldaplib/src/enums/action.py
+-rw-r--r--   0        0        0     4623 2024-05-17 12:28:38.372733 oldaplib-0.1.3/oldaplib/src/enums/language.py
+-rw-r--r--   0        0        0     2466 2024-05-17 16:17:14.367204 oldaplib-0.1.3/oldaplib/src/enums/permissions.py
+-rw-r--r--   0        0        0      376 2024-05-27 19:57:54.827687 oldaplib-0.1.3/oldaplib/src/enums/permissionsetattr.py
+-rw-r--r--   0        0        0     2069 2024-05-16 21:38:25.885179 oldaplib-0.1.3/oldaplib/src/enums/propertyclassattr.py
+-rw-r--r--   0        0        0      245 2024-05-24 20:29:28.380276 oldaplib-0.1.3/oldaplib/src/enums/resourceclassattr.py
+-rw-r--r--   0        0        0      636 2024-05-16 20:58:19.867251 oldaplib-0.1.3/oldaplib/src/enums/sparql_result_format.py
+-rw-r--r--   0        0        0      922 2024-05-17 16:16:02.047994 oldaplib-0.1.3/oldaplib/src/enums/userdataclassattr.py
+-rw-r--r--   0        0        0     6133 2024-05-16 20:58:19.867821 oldaplib-0.1.3/oldaplib/src/enums/xsd_datatypes.py
+-rw-r--r--   0        0        0      406 2024-05-25 22:49:56.860916 oldaplib-0.1.3/oldaplib/src/globalconfig.py
+-rw-r--r--   0        0        0     2054 2024-05-18 20:31:39.060235 oldaplib-0.1.3/oldaplib/src/helpers/Notify.py
+-rw-r--r--   0        0        0        0 2024-05-16 20:58:19.868316 oldaplib-0.1.3/oldaplib/src/helpers/__init__.py
+-rw-r--r--   0        0        0    13645 2024-05-26 21:25:16.747717 oldaplib-0.1.3/oldaplib/src/helpers/context.py
+-rw-r--r--   0        0        0    30931 2024-05-27 21:54:21.002326 oldaplib-0.1.3/oldaplib/src/helpers/langstring.py
+-rw-r--r--   0        0        0     2031 2024-05-24 20:29:28.381026 oldaplib-0.1.3/oldaplib/src/helpers/observable_dict.py
+-rw-r--r--   0        0        0     5525 2024-05-18 20:48:09.073657 oldaplib-0.1.3/oldaplib/src/helpers/observable_set.py
+-rw-r--r--   0        0        0     1265 2024-05-16 21:17:59.026464 oldaplib-0.1.3/oldaplib/src/helpers/oldaperror.py
+-rw-r--r--   0        0        0     1141 2024-05-17 12:28:38.168566 oldaplib-0.1.3/oldaplib/src/helpers/propertyclass_singleton.py
+-rw-r--r--   0        0        0    10146 2024-05-19 22:50:03.808918 oldaplib-0.1.3/oldaplib/src/helpers/query_processor.py
+-rw-r--r--   0        0        0     3218 2024-05-17 12:28:38.445610 oldaplib-0.1.3/oldaplib/src/helpers/semantic_version.py
+-rw-r--r--   0        0        0     4086 2024-05-16 20:58:19.870752 oldaplib-0.1.3/oldaplib/src/helpers/serializer.py
+-rw-r--r--   0        0        0      332 2024-05-25 22:49:56.844500 oldaplib-0.1.3/oldaplib/src/helpers/singletonmeta.py
+-rw-r--r--   0        0        0    12609 2024-05-19 20:59:15.236199 oldaplib-0.1.3/oldaplib/src/helpers/tools.py
+-rw-r--r--   0        0        0     2430 2024-05-17 12:28:38.306954 oldaplib-0.1.3/oldaplib/src/iconnection.py
+-rw-r--r--   0        0        0     7590 2024-05-22 21:47:27.190971 oldaplib-0.1.3/oldaplib/src/in_project.py
+-rw-r--r--   0        0        0     3036 2024-05-17 12:28:38.146377 oldaplib-0.1.3/oldaplib/src/model.py
+-rw-r--r--   0        0        0    22102 2024-05-30 13:55:57.260190 oldaplib-0.1.3/oldaplib/src/oldaplist.py
+-rw-r--r--   0        0        0     2417 2024-05-30 13:55:57.261370 oldaplib-0.1.3/oldaplib/src/oldaplistnode.py
+-rw-r--r--   0        0        0    27015 2024-05-27 19:57:54.834182 oldaplib-0.1.3/oldaplib/src/permissionset.py
+-rw-r--r--   0        0        0    33301 2024-05-30 13:50:36.508029 oldaplib-0.1.3/oldaplib/src/project.py
+-rw-r--r--   0        0        0    58711 2024-05-20 20:46:37.094562 oldaplib-0.1.3/oldaplib/src/propertyclass.py
+-rw-r--r--   0        0        0    54918 2024-05-24 20:29:28.381983 oldaplib-0.1.3/oldaplib/src/resourceclass.py
+-rw-r--r--   0        0        0    26623 2024-05-27 21:57:15.307605 oldaplib-0.1.3/oldaplib/src/user.py
+-rw-r--r--   0        0        0    30434 2024-05-17 16:06:07.068855 oldaplib-0.1.3/oldaplib/src/user_dataclass.py
+-rw-r--r--   0        0        0        0 2024-05-16 20:58:19.874593 oldaplib-0.1.3/oldaplib/src/xsd/__init__.py
+-rw-r--r--   0        0        0     7896 2024-05-17 12:28:38.536038 oldaplib-0.1.3/oldaplib/src/xsd/floatingpoint.py
+-rw-r--r--   0        0        0     4821 2024-05-26 22:05:53.954324 oldaplib-0.1.3/oldaplib/src/xsd/iri.py
+-rw-r--r--   0        0        0     1499 2024-05-16 20:58:19.875428 oldaplib-0.1.3/oldaplib/src/xsd/xsd.py
+-rw-r--r--   0        0        0     5523 2024-05-25 22:00:25.651776 oldaplib-0.1.3/oldaplib/src/xsd/xsd_anyuri.py
+-rw-r--r--   0        0        0     3543 2024-05-17 12:28:38.710082 oldaplib-0.1.3/oldaplib/src/xsd/xsd_base64binary.py
+-rw-r--r--   0        0        0     2648 2024-05-20 20:22:47.068509 oldaplib-0.1.3/oldaplib/src/xsd/xsd_boolean.py
+-rw-r--r--   0        0        0      979 2024-05-17 12:28:38.314066 oldaplib-0.1.3/oldaplib/src/xsd/xsd_byte.py
+-rw-r--r--   0        0        0     7043 2024-05-17 12:28:38.281355 oldaplib-0.1.3/oldaplib/src/xsd/xsd_date.py
+-rw-r--r--   0        0        0     3972 2024-05-17 12:28:38.567099 oldaplib-0.1.3/oldaplib/src/xsd/xsd_datetime.py
+-rw-r--r--   0        0        0     3904 2024-05-17 12:28:38.599870 oldaplib-0.1.3/oldaplib/src/xsd/xsd_datetimestamp.py
+-rw-r--r--   0        0        0     1376 2024-05-17 12:28:38.696167 oldaplib-0.1.3/oldaplib/src/xsd/xsd_decimal.py
+-rw-r--r--   0        0        0     1422 2024-05-17 12:28:38.618206 oldaplib-0.1.3/oldaplib/src/xsd/xsd_double.py
+-rw-r--r--   0        0        0     3319 2024-05-17 12:28:38.203063 oldaplib-0.1.3/oldaplib/src/xsd/xsd_duration.py
+-rw-r--r--   0        0        0     1242 2024-05-17 12:28:38.746441 oldaplib-0.1.3/oldaplib/src/xsd/xsd_float.py
+-rw-r--r--   0        0        0     3517 2024-05-17 12:28:38.705599 oldaplib-0.1.3/oldaplib/src/xsd/xsd_gday.py
+-rw-r--r--   0        0        0     3628 2024-05-17 12:28:38.677544 oldaplib-0.1.3/oldaplib/src/xsd/xsd_gmonth.py
+-rw-r--r--   0        0        0     3840 2024-05-17 12:28:38.519315 oldaplib-0.1.3/oldaplib/src/xsd/xsd_gmonthday.py
+-rw-r--r--   0        0        0     3780 2024-05-17 12:28:38.723526 oldaplib-0.1.3/oldaplib/src/xsd/xsd_gyear.py
+-rw-r--r--   0        0        0     4186 2024-05-17 12:28:38.657789 oldaplib-0.1.3/oldaplib/src/xsd/xsd_gyearmonth.py
+-rw-r--r--   0        0        0     3073 2024-05-17 12:28:38.595486 oldaplib-0.1.3/oldaplib/src/xsd/xsd_hexbinary.py
+-rw-r--r--   0        0        0      617 2024-05-17 12:28:38.552712 oldaplib-0.1.3/oldaplib/src/xsd/xsd_id.py
+-rw-r--r--   0        0        0      647 2024-05-17 12:28:38.562362 oldaplib-0.1.3/oldaplib/src/xsd/xsd_idref.py
+-rw-r--r--   0        0        0     1123 2024-05-17 12:28:38.236235 oldaplib-0.1.3/oldaplib/src/xsd/xsd_int.py
+-rw-r--r--   0        0        0     5727 2024-05-17 12:28:38.644946 oldaplib-0.1.3/oldaplib/src/xsd/xsd_integer.py
+-rw-r--r--   0        0        0     3504 2024-05-17 12:28:38.346404 oldaplib-0.1.3/oldaplib/src/xsd/xsd_language.py
+-rw-r--r--   0        0        0     1179 2024-05-17 12:28:38.423635 oldaplib-0.1.3/oldaplib/src/xsd/xsd_long.py
+-rw-r--r--   0        0        0     3436 2024-05-17 12:28:38.741813 oldaplib-0.1.3/oldaplib/src/xsd/xsd_name.py
+-rw-r--r--   0        0        0     5067 2024-05-25 20:39:47.835986 oldaplib-0.1.3/oldaplib/src/xsd/xsd_ncname.py
+-rw-r--r--   0        0        0      999 2024-05-17 12:28:38.701096 oldaplib-0.1.3/oldaplib/src/xsd/xsd_negativeinteger.py
+-rw-r--r--   0        0        0     3298 2024-05-17 12:28:38.181051 oldaplib-0.1.3/oldaplib/src/xsd/xsd_nmtoken.py
+-rw-r--r--   0        0        0     1043 2024-05-17 12:28:38.351243 oldaplib-0.1.3/oldaplib/src/xsd/xsd_nonnegativeinteger.py
+-rw-r--r--   0        0        0      964 2024-05-17 12:28:38.499113 oldaplib-0.1.3/oldaplib/src/xsd/xsd_nonpositiveinteger.py
+-rw-r--r--   0        0        0     3967 2024-05-17 12:28:38.435583 oldaplib-0.1.3/oldaplib/src/xsd/xsd_normalizedstring.py
+-rw-r--r--   0        0        0      945 2024-05-17 12:28:38.528978 oldaplib-0.1.3/oldaplib/src/xsd/xsd_positiveinteger.py
+-rw-r--r--   0        0        0     6750 2024-05-17 12:28:38.271692 oldaplib-0.1.3/oldaplib/src/xsd/xsd_qname.py
+-rw-r--r--   0        0        0      989 2024-05-17 12:28:38.240593 oldaplib-0.1.3/oldaplib/src/xsd/xsd_short.py
+-rw-r--r--   0        0        0     9512 2024-05-17 12:28:38.513898 oldaplib-0.1.3/oldaplib/src/xsd/xsd_string.py
+-rw-r--r--   0        0        0     3670 2024-05-17 12:28:38.458232 oldaplib-0.1.3/oldaplib/src/xsd/xsd_time.py
+-rw-r--r--   0        0        0     3546 2024-05-17 12:28:38.302060 oldaplib-0.1.3/oldaplib/src/xsd/xsd_token.py
+-rw-r--r--   0        0        0     1027 2024-05-17 12:28:38.682094 oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedbyte.py
+-rw-r--r--   0        0        0     1040 2024-05-17 12:28:38.576156 oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedint.py
+-rw-r--r--   0        0        0     1007 2024-05-17 12:28:38.524210 oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedlong.py
+-rw-r--r--   0        0        0     1012 2024-05-17 12:28:38.572122 oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedshort.py
+-rw-r--r--   0        0        0        0 2024-05-16 20:58:19.898288 oldaplib-0.1.3/oldaplib/test/__init__.py
+-rw-r--r--   0        0        0    14309 2024-05-24 20:29:28.389690 oldaplib-0.1.3/oldaplib/test/gaga.trig
+-rw-r--r--   0        0        0     1759 2024-05-18 22:18:06.660501 oldaplib-0.1.3/oldaplib/test/propclass_test.trig
+-rw-r--r--   0        0        0    13591 2024-05-26 21:44:40.793610 oldaplib-0.1.3/oldaplib/test/test_connection.py
+-rw-r--r--   0        0        0     4777 2024-05-25 22:24:17.528153 oldaplib-0.1.3/oldaplib/test/test_context.py
+-rw-r--r--   0        0        0    21746 2024-05-24 20:29:28.392421 oldaplib-0.1.3/oldaplib/test/test_datamodel.py
+-rw-r--r--   0        0        0     8221 2024-05-17 12:33:33.047906 oldaplib-0.1.3/oldaplib/test/test_dtypes.py
+-rw-r--r--   0        0        0     7774 2024-05-17 16:39:06.614379 oldaplib-0.1.3/oldaplib/test/test_in_project.py
+-rw-r--r--   0        0        0    11628 2024-05-17 12:28:38.294685 oldaplib-0.1.3/oldaplib/test/test_langstring.py
+-rw-r--r--   0        0        0     8826 2024-05-17 12:28:38.474410 oldaplib-0.1.3/oldaplib/test/test_language_in.py
+-rw-r--r--   0        0        0     3645 2024-05-17 16:00:20.113780 oldaplib-0.1.3/oldaplib/test/test_objectfactory.py
+-rw-r--r--   0        0        0     6249 2024-05-17 12:28:38.736345 oldaplib-0.1.3/oldaplib/test/test_observable_set.py
+-rw-r--r--   0        0        0     7288 2024-05-17 16:40:34.925874 oldaplib-0.1.3/oldaplib/test/test_oldaplist.py
+-rw-r--r--   0        0        0    14233 2024-05-27 19:58:31.120104 oldaplib-0.1.3/oldaplib/test/test_permissionset.py
+-rw-r--r--   0        0        0    16060 2024-05-30 13:54:17.909367 oldaplib-0.1.3/oldaplib/test/test_project.py
+-rw-r--r--   0        0        0    28492 2024-05-17 12:33:32.999538 oldaplib-0.1.3/oldaplib/test/test_propertyclass.py
+-rw-r--r--   0        0        0    42274 2024-05-24 20:29:28.394589 oldaplib-0.1.3/oldaplib/test/test_resourceclass.py
+-rw-r--r--   0        0        0     3392 2024-05-17 12:28:38.215443 oldaplib-0.1.3/oldaplib/test/test_semantic_version.py
+-rw-r--r--   0        0        0    40179 2024-05-25 22:37:42.478850 oldaplib-0.1.3/oldaplib/test/test_user.py
+-rw-r--r--   0        0        0    64182 2024-05-17 12:33:33.043637 oldaplib-0.1.3/oldaplib/test/test_xsd_datatypes.py
+-rw-r--r--   0        0        0    12312 2024-05-20 22:29:47.421485 oldaplib-0.1.3/oldaplib/testdata/connection_test.trig
+-rw-r--r--   0        0        0     1382 2024-05-16 21:56:28.046244 oldaplib-0.1.3/oldaplib/testdata/datamodel_test.trig
+-rw-r--r--   0        0        0    14936 2024-05-24 20:29:28.395766 oldaplib-0.1.3/oldaplib/testdata/objectfactory_test.trig
+-rw-r--r--   0        0        0      303 2024-05-16 21:56:27.962931 oldaplib-0.1.3/oldaplib/testit.http
+-rw-r--r--   0        0        0      914 2024-05-30 13:56:31.977934 oldaplib-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 oldaplib-0.1.3/PKG-INFO
```

### Comparing `oldaplib-0.1.2/README.md` & `oldaplib-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/ontologies/admin.trig` & `oldaplib-0.1.3/oldaplib/ontologies/admin.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/ontologies/oldap.shacl.trig` & `oldaplib-0.1.3/oldaplib/ontologies/oldap.shacl.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/ontologies/oldap.ttl` & `oldaplib-0.1.3/oldaplib/ontologies/oldap.ttl`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/ObjectFactory.py` & `oldaplib-0.1.3/oldaplib/src/ObjectFactory.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/connection.py` & `oldaplib-0.1.3/oldaplib/src/connection.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/datamodel.py` & `oldaplib-0.1.3/oldaplib/src/datamodel.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/dtypes/bnode.py` & `oldaplib-0.1.3/oldaplib/src/dtypes/bnode.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/dtypes/languagein.py` & `oldaplib-0.1.3/oldaplib/src/dtypes/languagein.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/dtypes/namespaceiri.py` & `oldaplib-0.1.3/oldaplib/src/dtypes/namespaceiri.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/dtypes/rdfset.py` & `oldaplib-0.1.3/oldaplib/src/dtypes/rdfset.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/dtypes/xsdset.py` & `oldaplib-0.1.3/oldaplib/src/dtypes/xsdset.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/enums/action.py` & `oldaplib-0.1.3/oldaplib/src/enums/action.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/enums/language.py` & `oldaplib-0.1.3/oldaplib/src/enums/language.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/enums/permissions.py` & `oldaplib-0.1.3/oldaplib/src/enums/permissions.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/enums/propertyclassattr.py` & `oldaplib-0.1.3/oldaplib/src/enums/propertyclassattr.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/enums/sparql_result_format.py` & `oldaplib-0.1.3/oldaplib/src/enums/sparql_result_format.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/enums/userdataclassattr.py` & `oldaplib-0.1.3/oldaplib/src/enums/userdataclassattr.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/enums/xsd_datatypes.py` & `oldaplib-0.1.3/oldaplib/src/enums/xsd_datatypes.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/Notify.py` & `oldaplib-0.1.3/oldaplib/src/helpers/Notify.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/context.py` & `oldaplib-0.1.3/oldaplib/src/helpers/context.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/langstring.py` & `oldaplib-0.1.3/oldaplib/src/helpers/langstring.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/observable_dict.py` & `oldaplib-0.1.3/oldaplib/src/helpers/observable_dict.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/observable_set.py` & `oldaplib-0.1.3/oldaplib/src/helpers/observable_set.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/oldaperror.py` & `oldaplib-0.1.3/oldaplib/src/helpers/oldaperror.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/propertyclass_singleton.py` & `oldaplib-0.1.3/oldaplib/src/helpers/propertyclass_singleton.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/query_processor.py` & `oldaplib-0.1.3/oldaplib/src/helpers/query_processor.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/semantic_version.py` & `oldaplib-0.1.3/oldaplib/src/helpers/semantic_version.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/serializer.py` & `oldaplib-0.1.3/oldaplib/src/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/helpers/tools.py` & `oldaplib-0.1.3/oldaplib/src/helpers/tools.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/iconnection.py` & `oldaplib-0.1.3/oldaplib/src/iconnection.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/in_project.py` & `oldaplib-0.1.3/oldaplib/src/in_project.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/model.py` & `oldaplib-0.1.3/oldaplib/src/model.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/oldaplist.py` & `oldaplib-0.1.3/oldaplib/src/oldaplist.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,25 @@
                  con: IConnection,
                  project: Project,
                  creator: Iri | None = None,
                  created: Xsd_dateTime | None = None,
                  contributor: Iri | None = None,
                  modified: Xsd_dateTime | None = None,
                  oldapListIri: Iri | str | None = None,
+                 inScheme: Iri | str,
+                 broaderTransitive: Iri | str | None = None,
+                 nextNode: Iri | str | None = None,
+                 leftIndex: int | None = None,
+                 rightIndex: int | None = None,
+                 notation: Xsd_string | str | None = None,
+                 note: LangString | str | None = None,
                  prefLabel: LangString | str | None = None,
-                 definition: LangString | str | None = None):
+                 altLabel: LangString | str | None = None,
+                 definition: LangString | str | None = None,
+                 changeNote: Xsd_string | str | None = None):
         super().__init__(con)
         if not isinstance(project, Project):
             raise OldapErrorValue('The project parameter must be a Project instance')
         self.__project = project
         context = Context(name=self._con.context_name)
         context[project.projectShortName] = project.namespaceIri
         context.use(project.projectShortName)
```

### Comparing `oldaplib-0.1.2/oldaplib/src/oldaplistnode.py` & `oldaplib-0.1.3/oldaplib/src/oldaplistnode.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from oldaplib.src.connection import Connection
 from oldaplib.src.helpers.langstring import LangString
 from oldaplib.src.iconnection import IConnection
 from oldaplib.src.model import Model
 from oldaplib.src.project import Project
 from oldaplib.src.resourceclass import ResourceClass
 from oldaplib.src.xsd.iri import Iri
+from oldaplib.src.xsd.xsd_datetime import Xsd_dateTime
 from oldaplib.src.xsd.xsd_string import Xsd_string
 
 
 @unique
 class OldapListNodeAttr(Enum):
     """
     This enum class represents the fields used in the project model
@@ -45,22 +46,21 @@
     }
 
     __system = None
     __listnodeclass = None
 
     def __init__(self, *,
                  con: IConnection,
-                 **kwargs):
-        super().__init__(connection=con)
-        if self.__system is None:
-            self.__system = Project.read(con, 'oldap')
-        if self.__listnodeclass is None:
-            self.__listnodeclass = ResourceClass.read(con, self.__system, Iri('oldap:OldapListNode'))
-        print(self.__system)
-        print(self.__listnodeclass)
+                 project: Project,
+                 creator: Iri | None = None,
+                 created: Xsd_dateTime | None = None,
+                 contributor: Iri | None = None,
+                 modified: Xsd_dateTime | None = None,
+                 oldapListIri: Iri | str | None = None,
+                 prefLabel: LangString | str | None = None,):
 
 if __name__ == '__main__':
     con = Connection(server='http://localhost:7200',
                      repo="oldap",
                      userId="rosenth",
                      credentials="RioGrande",
                      context_name="DEFAULT")
```

### Comparing `oldaplib-0.1.2/oldaplib/src/permissionset.py` & `oldaplib-0.1.3/oldaplib/src/permissionset.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/project.py` & `oldaplib-0.1.3/oldaplib/src/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,16 +204,14 @@
         self.__attributes[ProjectAttr.LABEL].set_notifier(self.notifier, Xsd_QName(ProjectAttr.LABEL.value))
         self.__attributes[ProjectAttr.COMMENT] = comment if isinstance(comment, LangString) else LangString(comment)
         self.__attributes[ProjectAttr.COMMENT].set_notifier(self.notifier, Xsd_QName(ProjectAttr.COMMENT.value))
         self.__attributes[ProjectAttr.PROJECT_SHORTNAME] = projectShortName if isinstance(projectShortName, Xsd_NCName) else Xsd_NCName(projectShortName)
         #
         # Consistency checks
         #
-        if not self.__attributes[ProjectAttr.LABEL]:
-            raise OldapErrorInconsistency(f'Project must have at least one rdfs:label, none given.')
         if projectStart is not None:
             self.__attributes[ProjectAttr.PROJECT_START] = projectStart if isinstance(projectStart, Xsd_date) else Xsd_date(projectStart)
         else:
             self.__attributes[ProjectAttr.PROJECT_START] = Xsd_date()
         if projectEnd is not None:
             self.__attributes[ProjectAttr.PROJECT_END] = projectEnd if isinstance(projectEnd, Xsd_date) else Xsd_date(projectEnd)
             if self.__attributes[ProjectAttr.PROJECT_END] < self.__attributes[ProjectAttr.PROJECT_START]:
```

### Comparing `oldaplib-0.1.2/oldaplib/src/propertyclass.py` & `oldaplib-0.1.3/oldaplib/src/propertyclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/resourceclass.py` & `oldaplib-0.1.3/oldaplib/src/resourceclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/user.py` & `oldaplib-0.1.3/oldaplib/src/user.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/user_dataclass.py` & `oldaplib-0.1.3/oldaplib/src/user_dataclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/floatingpoint.py` & `oldaplib-0.1.3/oldaplib/src/xsd/floatingpoint.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/iri.py` & `oldaplib-0.1.3/oldaplib/src/xsd/iri.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_anyuri.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_anyuri.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_base64binary.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_base64binary.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_boolean.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_boolean.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_byte.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_byte.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_date.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_date.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_datetime.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_datetime.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_datetimestamp.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_datetimestamp.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_decimal.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_decimal.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_double.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_double.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_duration.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_duration.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_float.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_float.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_gday.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_gday.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_gmonth.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_gmonth.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_gmonthday.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_gmonthday.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_gyear.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_gyear.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_gyearmonth.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_gyearmonth.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_hexbinary.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_hexbinary.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_id.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_id.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_idref.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_idref.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_int.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_int.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_integer.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_integer.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_language.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_language.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_long.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_long.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_name.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_name.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_ncname.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_ncname.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_negativeinteger.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_negativeinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_nmtoken.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_nmtoken.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_nonnegativeinteger.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_nonnegativeinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_nonpositiveinteger.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_nonpositiveinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_normalizedstring.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_normalizedstring.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_positiveinteger.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_positiveinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_qname.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_qname.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_short.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_short.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_string.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_string.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_time.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_time.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_token.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_token.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedbyte.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedbyte.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedint.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedint.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedlong.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedlong.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/src/xsd/xsd_unsignedshort.py` & `oldaplib-0.1.3/oldaplib/src/xsd/xsd_unsignedshort.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/gaga.trig` & `oldaplib-0.1.3/oldaplib/test/gaga.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/propclass_test.trig` & `oldaplib-0.1.3/oldaplib/test/propclass_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_connection.py` & `oldaplib-0.1.3/oldaplib/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_context.py` & `oldaplib-0.1.3/oldaplib/test/test_context.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_datamodel.py` & `oldaplib-0.1.3/oldaplib/test/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_dtypes.py` & `oldaplib-0.1.3/oldaplib/test/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_in_project.py` & `oldaplib-0.1.3/oldaplib/test/test_in_project.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_langstring.py` & `oldaplib-0.1.3/oldaplib/test/test_langstring.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_language_in.py` & `oldaplib-0.1.3/oldaplib/test/test_language_in.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_objectfactory.py` & `oldaplib-0.1.3/oldaplib/test/test_objectfactory.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_observable_set.py` & `oldaplib-0.1.3/oldaplib/test/test_observable_set.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_oldaplist.py` & `oldaplib-0.1.3/oldaplib/test/test_oldaplist.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_permissionset.py` & `oldaplib-0.1.3/oldaplib/test/test_permissionset.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_project.py` & `oldaplib-0.1.3/oldaplib/test/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,32 +222,14 @@
                           namespaceIri=NamespaceIRI("http://unitest.org/project/unittest#"),
                           projectStart=Xsd_date(2024, 1, 1),
                           projectEnd=Xsd_date(2025, 12, 31)
                           )
         self.assertIsNone(project.comment)
 
 
-    def test_project_empty_label(self):
-        with self.assertRaises(OldapErrorInconsistency):
-            project = Project(con=self._connection,
-                              projectShortName="updatetest",
-                              namespaceIri=NamespaceIRI("http://unitest.org/project/updatetest#"),
-                              projectStart=Xsd_date(2024, 1, 1),
-                              projectEnd=Xsd_date(2025, 12, 31)
-                              )
-        with self.assertRaises(OldapErrorInconsistency):
-            project = Project(con=self._connection,
-                              projectShortName="updatetest",
-                              label=LangString(),
-                              namespaceIri=NamespaceIRI("http://unitest.org/project/updatetest#"),
-                              projectStart=Xsd_date(2024, 1, 1),
-                              projectEnd=Xsd_date(2025, 12, 31)
-                              )
-
-
     # @unittest.skip('Work in progress')
     def test_project_modify(self):
         project = Project(con=self._connection,
                           projectShortName="updatetest",
                           label=LangString(["updatetest@en", "updatetest@de"]),
                           namespaceIri=NamespaceIRI("http://unitest.org/project/updatetest#"),
                           comment=LangString(["For testing@en", "Für Tests@de"]),
```

### Comparing `oldaplib-0.1.2/oldaplib/test/test_propertyclass.py` & `oldaplib-0.1.3/oldaplib/test/test_propertyclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_resourceclass.py` & `oldaplib-0.1.3/oldaplib/test/test_resourceclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_semantic_version.py` & `oldaplib-0.1.3/oldaplib/test/test_semantic_version.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_user.py` & `oldaplib-0.1.3/oldaplib/test/test_user.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/test/test_xsd_datatypes.py` & `oldaplib-0.1.3/oldaplib/test/test_xsd_datatypes.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/testdata/connection_test.trig` & `oldaplib-0.1.3/oldaplib/testdata/connection_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/testdata/datamodel_test.trig` & `oldaplib-0.1.3/oldaplib/testdata/datamodel_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/oldaplib/testdata/objectfactory_test.trig` & `oldaplib-0.1.3/oldaplib/testdata/objectfactory_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.2/pyproject.toml` & `oldaplib-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oldaplib"
-version = "0.1.2"
+version = "0.1.3"
 description = "Open Media Access Server Library (Linked Open Data middleware/RESTApi)"
 authors = ["Lukas Rosenthaler <lukas.rosenthaler@unibas.ch>"]
 license = "GNU Affero General Public License version 3"
 readme = "README.md"
 
 [tool.mkdocs]
 plugins = ["mkdocs-material", "mkdocstrings"]
```

### Comparing `oldaplib-0.1.2/PKG-INFO` & `oldaplib-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oldaplib
-Version: 0.1.2
+Version: 0.1.3
 Summary: Open Media Access Server Library (Linked Open Data middleware/RESTApi)
 License: GNU Affero General Public License version 3
 Author: Lukas Rosenthaler
 Author-email: lukas.rosenthaler@unibas.ch
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

