# Comparing `tmp/pydwca-0.1.1.tar.gz` & `tmp/pydwca-0.1.2.tar.gz`

## Comparing `pydwca-0.1.1.tar` & `pydwca-0.1.2.tar`

### file list

```diff
@@ -1,178 +1,179 @@
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 pydwca-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydwca-0.1.1/requirements-test.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pydwca-0.1.1/requirements.txt
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pydwca-0.1.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 pydwca-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/make.bat
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/dwca.classes.rst
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/dwca.rst
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/dwca.terms.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.resources.coverage.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.resources.distribution.rst
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.resources.rst
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.rst
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.types.rst
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/install.rst
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/modules.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/requirements.txt
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/usage.dwca.rst
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/usage.eml.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/usage.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/xml_common.rst
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/xml_common.utils.rst
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/_static/_js/pypi-icon.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/__init__.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/darwincore.py
--rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/darwincore_archive.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/simple_darwincore.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/chronometric_age.py
--rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/data_file.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/event.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/geological_context.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/identification.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/location.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/material_entity.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/material_sample.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/measurement_or_fact.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/occurrence.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/organism.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/outside_class.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/resource_relationship.py
--rw-r--r--   0        0        0    14149 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/taxon.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/__init__.py
--rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/chronometric_age.py
--rw-r--r--   0        0        0    10658 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/event.py
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/field.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/geological_context.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/identification.py
--rw-r--r--   0        0        0    29913 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/location.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/material_entity.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/material_sample.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/measurement_or_fact.py
--rw-r--r--   0        0        0    15474 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/occurrence.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/organism.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/outside_term.py
--rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/record_level.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/resource_relationship.py
--rw-r--r--   0        0        0    30795 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/taxon.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/__init__.py
--rw-r--r--   0        0        0    17942 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/eml.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/metadata.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/version.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/citation.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/dataset.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/keyword_set.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/licence.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/protocol.py
--rw-r--r--   0        0        0    18330 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/resource.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/resources.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/software.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/__init__.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/coverage.py
--rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/geo_coverage.py
--rw-r--r--   0        0        0    25361 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/taxa_coverage.py
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/time_coverage.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/__init__.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/distribution.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/inline.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/offline.py
--rw-r--r--   0        0        0    23149 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/online.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/__init__.py
--rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/access_type.py
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/address.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/eml_object.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/extension_string.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/extension_uri.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/i18n_string.py
--rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/individual_name.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/no_tag_object.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/organization_name.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/phone.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/position_name.py
--rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/responsible_party.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/section.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/semantic_annotation.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/text_type.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/__init__.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/xml_object.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/__init__.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/enum.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/establishment_means.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/gpolygon.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/iteratate.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/language.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/length_unit.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/type_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/__init__.py
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_dwca.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_dwca_no_pandas.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_meta.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_outside_term.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_identification.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_outside_class.py
--rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_taxon.py
--rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_taxon_no_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_any_field.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_datetime_field.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_float_field.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_int_field.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_list_str_field.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_outside_term.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_str_field.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_taxon.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_union_datetime_field.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_union_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_access_type.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_address.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_annotation.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_citation.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_dataset.py
--rw-r--r--   0        0        0    17788 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_eml.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_extension.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_extension_uri.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_i18n_string.py
--rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_individual_name.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_keyword_set.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_licence.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_metadata.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_organization_name.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_phone.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_position_name.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_protocol.py
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_responsible_party.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_section.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_semantic_annotation.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_software.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_text_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_coverage.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_geo_coverage.py
--rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_taxa_coverage.py
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_time_coverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_distribution.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_inline.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_offline.py
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_online.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/__init__.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/test_establishment_means.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/test_format.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/test_unformat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_xml/__init__.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_xml/test_simple_xml.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_xml/test_xml.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pydwca-0.1.1/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pydwca-0.1.1/LICENSE
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pydwca-0.1.1/README.md
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pydwca-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 pydwca-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 pydwca-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydwca-0.1.2/requirements-test.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pydwca-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pydwca-0.1.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pydwca-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/dwca.classes.rst
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/dwca.rst
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/dwca.terms.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/eml.resources.coverage.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/eml.resources.distribution.rst
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/eml.resources.rst
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/eml.rst
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/eml.types.rst
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/install.rst
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/modules.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/requirements.txt
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/usage.dwca.rst
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/usage.eml.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/usage.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/xml_common.rst
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/xml_common.utils.rst
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pydwca-0.1.2/docs/source/_static/_js/pypi-icon.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/base/__init__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/base/darwincore.py
+-rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/base/darwincore_archive.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/base/simple_darwincore.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/chronometric_age.py
+-rw-r--r--   0        0        0    14989 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/data_file.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/event.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/geological_context.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/identification.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/location.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/material_entity.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/material_sample.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/measurement_or_fact.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/occurrence.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/organism.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/outside_class.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/resource_relationship.py
+-rw-r--r--   0        0        0    14672 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/classes/taxon.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/__init__.py
+-rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/chronometric_age.py
+-rw-r--r--   0        0        0    10658 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/event.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/field.py
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/geological_context.py
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/identification.py
+-rw-r--r--   0        0        0    29913 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/location.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/material_entity.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/material_sample.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/measurement_or_fact.py
+-rw-r--r--   0        0        0    15474 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/occurrence.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/organism.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/outside_term.py
+-rw-r--r--   0        0        0    13316 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/record_level.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/resource_relationship.py
+-rw-r--r--   0        0        0    30795 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/dwca/terms/taxon.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/base/__init__.py
+-rw-r--r--   0        0        0    17942 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/base/eml.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/base/metadata.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/base/version.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/citation.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/dataset.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/keyword_set.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/licence.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/protocol.py
+-rw-r--r--   0        0        0    18330 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/resource.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/resources.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/software.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/coverage/__init__.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/coverage/coverage.py
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/coverage/geo_coverage.py
+-rw-r--r--   0        0        0    25361 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/coverage/taxa_coverage.py
+-rw-r--r--   0        0        0    14719 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/coverage/time_coverage.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/distribution/__init__.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/distribution/distribution.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/distribution/inline.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/distribution/offline.py
+-rw-r--r--   0        0        0    23149 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/resources/distribution/online.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/__init__.py
+-rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/access_type.py
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/address.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/eml_object.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/extension_string.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/extension_uri.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/i18n_string.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/individual_name.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/no_tag_object.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/organization_name.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/phone.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/position_name.py
+-rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/responsible_party.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/section.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/semantic_annotation.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/eml/types/text_type.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/__init__.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/xml_object.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/__init__.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/enum.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/establishment_means.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/gpolygon.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/iteratate.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/language.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/length_unit.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 pydwca-0.1.2/src/xml_common/utils/type_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca/__init__.py
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca/test_dwca.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca/test_dwca_no_pandas.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca/test_meta.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca/test_multiple_dataset.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca/test_outside_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_classes/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_classes/test_identification.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_classes/test_outside_class.py
+-rw-r--r--   0        0        0    19655 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_classes/test_taxon.py
+-rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_classes/test_taxon_no_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_any_field.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_datetime_field.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_float_field.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_int_field.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_list_str_field.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_outside_term.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_str_field.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_taxon.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_union_datetime_field.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_dwca_terms/test_union_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_access_type.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_address.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_annotation.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_citation.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_dataset.py
+-rw-r--r--   0        0        0    17788 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_eml.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_extension.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_extension_uri.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_i18n_string.py
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_individual_name.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_keyword_set.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_licence.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_metadata.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_organization_name.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_phone.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_position_name.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_protocol.py
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_responsible_party.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_section.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_semantic_annotation.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_software.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml/test_text_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_coverage/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_coverage/test_coverage.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_coverage/test_geo_coverage.py
+-rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_coverage/test_taxa_coverage.py
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_coverage/test_time_coverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_distribution/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_distribution/test_distribution.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_distribution/test_inline.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_distribution/test_offline.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_eml_distribution/test_online.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_util/__init__.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_util/test_establishment_means.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_util/test_format.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_util/test_unformat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_xml/__init__.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_xml/test_simple_xml.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pydwca-0.1.2/tests/test_xml/test_xml.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pydwca-0.1.2/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pydwca-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pydwca-0.1.2/README.md
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pydwca-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 pydwca-0.1.2/PKG-INFO
```

### Comparing `pydwca-0.1.1/.readthedocs.yaml` & `pydwca-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/.github/workflows/publish-pypi.yml` & `pydwca-0.1.2/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/Makefile` & `pydwca-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/make.bat` & `pydwca-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/conf.py` & `pydwca-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/dwca.classes.rst` & `pydwca-0.1.2/docs/source/dwca.classes.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/dwca.rst` & `pydwca-0.1.2/docs/source/dwca.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/dwca.terms.rst` & `pydwca-0.1.2/docs/source/dwca.terms.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/eml.resources.coverage.rst` & `pydwca-0.1.2/docs/source/eml.resources.coverage.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/eml.resources.distribution.rst` & `pydwca-0.1.2/docs/source/eml.resources.distribution.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/eml.resources.rst` & `pydwca-0.1.2/docs/source/eml.resources.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/eml.rst` & `pydwca-0.1.2/docs/source/eml.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/eml.types.rst` & `pydwca-0.1.2/docs/source/eml.types.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/index.rst` & `pydwca-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/usage.dwca.rst` & `pydwca-0.1.2/docs/source/usage.dwca.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/usage.eml.rst` & `pydwca-0.1.2/docs/source/usage.eml.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/xml_common.utils.rst` & `pydwca-0.1.2/docs/source/xml_common.utils.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/docs/source/_static/_js/pypi-icon.js` & `pydwca-0.1.2/docs/source/_static/_js/pypi-icon.js`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/base/darwincore.py` & `pydwca-0.1.2/src/dwca/base/darwincore.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/base/darwincore_archive.py` & `pydwca-0.1.2/src/dwca/base/darwincore_archive.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import io
+import os.path
 import zipfile
 from typing import List, Dict, Type
 from warnings import warn
 
 from lxml import etree as et
 
 from dwca.base import DarwinCore
@@ -122,14 +123,17 @@
             return element
 
     def __init__(self, _id: str = None) -> None:
         super().__init__()
         self.__id__ = _id
         self.__meta__ = DarwinCoreArchive.Metadata()
         self.__metadata__ = None
+        self.__dataset_meta__ = {
+            "metadata": self.__metadata__
+        }
         return
 
     @property
     def id(self) -> str:
         """str: A unique identifier for this DarwinCoreArchive."""
         return self.__id__
 
@@ -170,14 +174,21 @@
     def metadata(self) -> EML:
         """
         EML: Metadata instance, currently supported EML.
         """
         return self.__metadata__
 
     @property
+    def dataset_metadata(self) -> Dict[str, EML]:
+        """
+        Dict[str, EML]: Metadata instances for each dataset present on DWC-A.
+        """
+        return self.__dataset_meta__
+
+    @property
     def language(self) -> Language:
         """Language: Language of the Darwin Core Archive register on metadata."""
         return self.metadata.language
 
     def generate_eml(self, filename: str = "eml.xml") -> None:
         """
         Generate an EML file on the archive
@@ -222,30 +233,51 @@
         darwin_core.__metadata__ = eml
         core_file = archive.read(darwin_core.core.filename)
         darwin_core.__meta__.__core__.read_file(core_file.decode(encoding=metadata.__core__.__encoding__))
         darwin_core.__meta__.__core__._register_darwin_core_(0, darwin_core)
         for i, extension in enumerate(darwin_core.extensions):
             extension_file = archive.read(extension.filename)
             darwin_core.__meta__.__extensions__[i].read_file(extension_file.decode())
+        darwin_core.__dataset_meta__ = {
+            "metadata": darwin_core.__metadata__
+        }
+        for item in archive.namelist():
+            if item.startswith("dataset/"):
+                if item == "dataset/":
+                    continue
+                try:
+                    dataset_meta = EML.from_string(archive.read(item).decode(encoding="utf-8"))
+                except ValueError:
+                    dataset_meta = EML.from_string(archive.read(item))
+                darwin_core.__dataset_meta__[dataset_meta.package_id] = dataset_meta
         archive.close()
         return darwin_core
 
-    def to_file(self, path_to_archive: str, encoding: str = "utf-8") -> None:
+    def to_file(
+            self, path_to_archive: str,
+            encoding: str = "utf-8",
+            compression: int = zipfile.ZIP_DEFLATED,
+            compression_level: int = 6
+    ) -> None:
         """
         Generate a Darwin Core Archive file (`.zip` file) using the information of this instance.
 
         Parameters
         ----------
         path_to_archive : str
             Path of the archive to generate.
         encoding : str, optional
             Encoding of the corresponding files. Default `"utf-8"`.
+        compression : int, optional
+            The ZIP compression method to use. Default `zipfile.ZIP_DEFLATED`.
+        compression_level : int, optional
+            Compression level to use when writing files to the archive. Default `6`.
         """
         zip_buffer = io.BytesIO()
-        with zipfile.ZipFile(zip_buffer, 'a') as zip_file:
+        with zipfile.ZipFile(zip_buffer, 'a', compression=compression, compresslevel=compression_level) as zip_file:
             zip_file.writestr("meta.xml", self.__meta__.to_xml().encode(encoding))
             if self.metadata is not None:
                 zip_file.writestr(self.__meta__.__metadata__, self.__metadata__.to_xml().encode(encoding))
             if self.core is not None:
                 zip_file.writestr(self.core.filename, self.core.write_file())
             for extension in self.extensions:
                 zip_file.writestr(extension.filename, extension.write_file())
```

### Comparing `pydwca-0.1.1/src/dwca/classes/__init__.py` & `pydwca-0.1.2/src/dwca/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/chronometric_age.py` & `pydwca-0.1.2/src/dwca/classes/chronometric_age.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/data_file.py` & `pydwca-0.1.2/src/dwca/classes/data_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,39 @@
         return self.__files__
 
     @property
     def fields(self) -> List[str]:
         """List[str]: List of terms of this data file."""
         return [field.uri for field in self.__fields__]
 
+    def add_field(self, field: Field) -> None:
+        """
+        Add a field to this Data File.
+
+        Parameters
+        ----------
+        field : Field
+            A :class:`dwca.terms.field.Field` object.
+
+        Returns
+        -------
+        None
+        """
+        if field.index != len(self.__fields__):
+            warn(f"Field must be added at the end of current data, setting index to {len(self.__fields__)}")
+            field.index = len(self.__fields__)
+        field.__namespace__ = self.__namespace__
+        self.__fields__.append(field)
+        if len(self.__entries__) > 0:
+            self.__data__ = None
+            for entry in self.__entries__:
+                setattr(entry, field.name, None if field.default is None else field.format(field.default))
+        return
+
+
     @property
     def pandas(self) -> pd.DataFrame:
         """pandas.DataFrame: Data of this DataFile as pandas.DataFrame."""
         if self.__data__ is None:
             self.as_pandas()
         return self.__data__
 
@@ -278,14 +303,15 @@
             element_id = self.object_to_element("id")
         else:  # self.__type__ == DataFileType.EXTENSION:
             element_id = self.object_to_element("coreid")
         element_id.set("index", str(self.id))
         element.append(element_id)
         files = self.object_to_element("files")
         location = self.object_to_element("location")
+        location.text = self.filename
         files.append(location)
         element.append(files)
         for field in self.__fields__:
             if self.__type__ == DataFileType.EXTENSION and field.index == self.id:
                 continue
             field_element = field.to_element()
             element.append(field_element)
```

### Comparing `pydwca-0.1.1/src/dwca/classes/event.py` & `pydwca-0.1.2/src/dwca/classes/event.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/geological_context.py` & `pydwca-0.1.2/src/dwca/classes/geological_context.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/identification.py` & `pydwca-0.1.2/src/dwca/classes/identification.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/location.py` & `pydwca-0.1.2/src/dwca/classes/location.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/material_entity.py` & `pydwca-0.1.2/src/dwca/classes/material_entity.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/material_sample.py` & `pydwca-0.1.2/src/dwca/classes/material_sample.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/measurement_or_fact.py` & `pydwca-0.1.2/src/dwca/classes/measurement_or_fact.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/occurrence.py` & `pydwca-0.1.2/src/dwca/classes/occurrence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/organism.py` & `pydwca-0.1.2/src/dwca/classes/organism.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/outside_class.py` & `pydwca-0.1.2/src/dwca/classes/outside_class.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/resource_relationship.py` & `pydwca-0.1.2/src/dwca/classes/resource_relationship.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/classes/taxon.py` & `pydwca-0.1.2/src/dwca/classes/taxon.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,32 +120,42 @@
             tqdm.reset(total=100)
         tqdm.update(n=10)
         postfix = {"Exact match found": len(taxa_id)}
         tqdm.set_postfix(ordered_dict=postfix)
         tqdm.set_descriptor(desc="Getting synonyms")
         complete_taxa = self.all_synonyms(taxa_id, get_names=True)
         postfix["Synonyms found"] = len(complete_taxa) - len(taxa_id)
+        taxa_id = self.all_synonyms(taxa_id)
         tqdm.set_postfix(ordered_dict=postfix)
         tqdm.update(n=40)
         tqdm.set_descriptor(desc="Getting parents")
         parents = self.get_parents(taxa_id)
         parents.update(self.all_synonyms(parents))
         postfix["Parents found"] = len(parents)
         tqdm.set_postfix(ordered_dict=postfix)
         tqdm.update(n=40)
         tqdm.set_descriptor(desc=f"Filtering {taxa_name}")
         try:
             df = self.pandas
             name = taxa_field.name_cls()
-            df = df[df[name].isin(complete_taxa) | df[TaxonID.name_cls()].isin(parents)]
+            mask = df[TaxonID.name_cls()].isin(parents) | df[TaxonID.name_cls()].isin(taxa_id)
+            if filter_with_rank:
+                mask |= df[name].isin(complete_taxa)
+            df = df[mask]
             self.pandas = df
         except ImportError:
-            def filter_taxa(entry: DataFile.Entry) -> bool:
-                return (getattr(entry, taxa_field.name_cls()) in complete_taxa or
-                        getattr(entry, TaxonID.name_cls()) in parents)
+            if filter_with_rank:
+                def filter_taxa(entry: DataFile.Entry) -> bool:
+                    return (getattr(entry, taxa_field.name_cls()) in complete_taxa or
+                            getattr(entry, TaxonID.name_cls()) in parents or
+                            getattr(entry, TaxonID.name_cls()) in taxa_id)
+            else:
+                def filter_taxa(entry: DataFile.Entry) -> bool:
+                    return (getattr(entry, TaxonID.name_cls()) in parents or
+                            getattr(entry, TaxonID.name_cls()) in taxa_id)
             self.__entries__ = list(filter(filter_taxa, self.__entries__))
         postfix["Total filtered"] = len(self)
         tqdm.set_postfix(ordered_dict=postfix)
         tqdm.update(n=10)
         tqdm.close()
         return
 
@@ -300,15 +310,15 @@
         except ImportError:
             entries = self.__get_rows__(taxa_id)
             accepted_names = [getattr(entry, AcceptedNameUsageID.name_cls()) for entry in entries]
             synonyms = self.__get_entries__(**{f"{AcceptedNameUsageID.name_cls()}__isin": accepted_names})
             field = ScientificName.name_cls() if get_names else TaxonID.name_cls()
             return [getattr(synonymous, field) for synonymous in synonyms]
 
-    def __get_rows__(self, taxa_id: List[str]) -> Union[pd.DataFrame, List[DataFile.Entry]]:
+    def __get_rows__(self, taxa_id: Iterable[str]) -> Union[pd.DataFrame, List[DataFile.Entry]]:
         try:
             df = self.pandas
             current_taxa = df[df[TaxonID.name_cls()].isin(taxa_id)]
             if len(current_taxa) != len(taxa_id):
                 candidates = pd.Series(taxa_id)
                 not_present = candidates[~candidates.isin(df[TaxonID.name_cls()])]
                 warn(f"{', '.join(list(not_present))} not found in data file.")
```

### Comparing `pydwca-0.1.1/src/dwca/terms/__init__.py` & `pydwca-0.1.2/src/dwca/terms/__init__.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/chronometric_age.py` & `pydwca-0.1.2/src/dwca/terms/chronometric_age.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/event.py` & `pydwca-0.1.2/src/dwca/terms/event.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/field.py` & `pydwca-0.1.2/src/dwca/terms/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,19 @@
         return
 
     @property
     def index(self) -> int:
         """int: Specifies the position of the column in the row."""
         return self.__index__
 
+    @index.setter
+    def index(self, index: int) -> None:
+        self.__index__ = index
+        return
+
     @property
     def default(self) -> Any:
         """Any: Specifies a value to use if one is not supplied."""
         return self.__default__
 
     @property
     def vocabulary(self) -> str:
```

### Comparing `pydwca-0.1.1/src/dwca/terms/geological_context.py` & `pydwca-0.1.2/src/dwca/terms/geological_context.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/identification.py` & `pydwca-0.1.2/src/dwca/terms/identification.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/location.py` & `pydwca-0.1.2/src/dwca/terms/location.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/material_entity.py` & `pydwca-0.1.2/src/dwca/terms/material_entity.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/material_sample.py` & `pydwca-0.1.2/src/dwca/terms/material_sample.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/measurement_or_fact.py` & `pydwca-0.1.2/src/dwca/terms/measurement_or_fact.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/occurrence.py` & `pydwca-0.1.2/src/dwca/terms/occurrence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/organism.py` & `pydwca-0.1.2/src/dwca/terms/organism.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/outside_term.py` & `pydwca-0.1.2/src/dwca/terms/outside_term.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/record_level.py` & `pydwca-0.1.2/src/dwca/terms/record_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,30 @@
     URI = "http://purl.org/dc/elements/1.1/language"
     TYPE = Language
 
     def __init__(self, index: int | str, default: TYPE = None, vocabulary: str = None) -> None:
         super().__init__(index, default, vocabulary)
         return
 
+    def format(self, value: str) -> Language:
+        """
+        Format value to Language.
+
+        Parameters
+        ----------
+        value : str
+            Value to be formatted as a Language.
+
+        Returns
+        -------
+        Language
+            Value as a Language object.
+        """
+        return Language.get_language(value)
+
 
 class DWCLicense(Field):
     """
     A legal document giving official permission to do something with the resource.
 
     Parameters
     ----------
```

### Comparing `pydwca-0.1.1/src/dwca/terms/resource_relationship.py` & `pydwca-0.1.2/src/dwca/terms/resource_relationship.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/dwca/terms/taxon.py` & `pydwca-0.1.2/src/dwca/terms/taxon.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/base/eml.py` & `pydwca-0.1.2/src/eml/base/eml.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/base/metadata.py` & `pydwca-0.1.2/src/eml/base/metadata.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/base/version.py` & `pydwca-0.1.2/src/eml/base/version.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/citation.py` & `pydwca-0.1.2/src/eml/resources/citation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/dataset.py` & `pydwca-0.1.2/src/eml/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/keyword_set.py` & `pydwca-0.1.2/src/eml/resources/keyword_set.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/licence.py` & `pydwca-0.1.2/src/eml/resources/licence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/protocol.py` & `pydwca-0.1.2/src/eml/resources/protocol.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/resource.py` & `pydwca-0.1.2/src/eml/resources/resource.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/resources.py` & `pydwca-0.1.2/src/eml/resources/resources.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/software.py` & `pydwca-0.1.2/src/eml/resources/software.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/coverage/coverage.py` & `pydwca-0.1.2/src/eml/resources/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/coverage/geo_coverage.py` & `pydwca-0.1.2/src/eml/resources/coverage/geo_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/coverage/taxa_coverage.py` & `pydwca-0.1.2/src/eml/resources/coverage/taxa_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/coverage/time_coverage.py` & `pydwca-0.1.2/src/eml/resources/coverage/time_coverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
+import re
 from typing import Dict, List, Union, Tuple
 
 from lxml import etree as et
 import datetime as dt
 
 from xml_common import XMLObject
 from eml.types import EMLObject, Scope
+from xml_common.utils.type_functions import unformat_datetime, format_datetime
 
 
 class TemporalCoverage(EMLObject):
     """
     Temporal coverage information.
 
     Parameters
@@ -317,24 +319,23 @@
             Datetime in the corresponding format.
         """
         alternative_elem = element.find("alternativeTimeScale")
         if alternative_elem is not None:
             return TemporalCoverage.AlternativeTimeScale.parse(alternative_elem, nmap)
         time_elem = element.find("time")
         calendar_elem = element.find("calendarDate")
-        try:
-            calendar_date = dt.datetime.strptime(calendar_elem.text, "%Y-%m-%d").date()
-        except ValueError:
-            calendar_date = dt.datetime.strptime(calendar_elem.text, "%Y").date()
+        calendar_date = format_datetime(calendar_elem.text).date()
         if time_elem is not None:
             try:
-                return dt.datetime.strptime(
+                output_datetime = dt.datetime.strptime(
                     f"{calendar_date.strftime('%Y-%m-%d')} {time_elem.text}",
                     "%Y-%m-%d %H:%M:%SZ"
                 )
+                output_datetime = output_datetime.replace(tzinfo=dt.timezone.utc)
+                return output_datetime
             except ValueError:
                 return dt.datetime.strptime(
                     f"{calendar_date.strftime('%Y-%m-%d')} {time_elem.text}",
                     "%Y-%m-%d %H:%M:%S%z"
                 )
         else:
             return calendar_date
@@ -357,22 +358,26 @@
         Raises
         ------
         TypeError
             Not a valid datetime.
         """
         element = et.Element("placeholderDate")
         if isinstance(datetime, dt.datetime):
+            string_time = unformat_datetime(datetime)
+            string_time = re.sub(r"([+-])(\d{2})(\d{2})", r"\1\2:\3", string_time)
+            date_text, time_text = string_time.split("T")
             calendar_elem = et.Element("calendarDate")
-            calendar_elem.text = datetime.date().strftime("%Y-%m-%d")
+            calendar_elem.text = date_text
             element.append(calendar_elem)
             time_elem = et.Element("time")
-            time_elem.text = datetime.time().strftime("%H:%M:%S%z")
+            time_elem.text = time_text
             element.append(time_elem)
         elif isinstance(datetime, dt.date):
             calendar_elem = et.Element("calendarDate")
-            calendar_elem.text = datetime.strftime("%Y-%m-%d")
+            date_text = unformat_datetime(dt.datetime.combine(datetime, dt.time()))
+            calendar_elem.text = date_text
             element.append(calendar_elem)
         elif isinstance(datetime, TemporalCoverage.AlternativeTimeScale):
             element.append(datetime.to_element())
         else:
             raise TypeError("Not a valid datetime")
         return element
```

### Comparing `pydwca-0.1.1/src/eml/resources/distribution/distribution.py` & `pydwca-0.1.2/src/eml/resources/distribution/distribution.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/distribution/inline.py` & `pydwca-0.1.2/src/eml/resources/distribution/inline.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/resources/distribution/offline.py` & `pydwca-0.1.2/src/eml/resources/distribution/offline.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         offline_elem.append(name)
         if self.medium_density is not None:
             density_elem = self.object_to_element("mediumDensity")
             density_elem.text = self.medium_density
             offline_elem.append(density_elem)
         if self.medium_density_units is not None:
             units_elem = self.object_to_element("mediumDensityUnits")
-            units_elem.text = self.medium_density
+            units_elem.text = self.medium_density_units
             offline_elem.append(units_elem)
         if self.medium_volume is not None:
             volume_elem = self.object_to_element("mediumVolume")
             volume_elem.text = self.medium_volume
             offline_elem.append(volume_elem)
         for medium_format in self.medium_format:
             format_elem = self.object_to_element("mediumFormat")
```

### Comparing `pydwca-0.1.1/src/eml/resources/distribution/online.py` & `pydwca-0.1.2/src/eml/resources/distribution/online.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/__init__.py` & `pydwca-0.1.2/src/eml/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/access_type.py` & `pydwca-0.1.2/src/eml/types/access_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/address.py` & `pydwca-0.1.2/src/eml/types/address.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/eml_object.py` & `pydwca-0.1.2/src/eml/types/eml_object.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/extension_string.py` & `pydwca-0.1.2/src/eml/types/extension_string.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/extension_uri.py` & `pydwca-0.1.2/src/eml/types/extension_uri.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/i18n_string.py` & `pydwca-0.1.2/src/eml/types/i18n_string.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/individual_name.py` & `pydwca-0.1.2/src/eml/types/individual_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/no_tag_object.py` & `pydwca-0.1.2/src/eml/types/no_tag_object.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/organization_name.py` & `pydwca-0.1.2/src/eml/types/organization_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/phone.py` & `pydwca-0.1.2/src/eml/types/phone.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,8 +75,9 @@
         Returns
         -------
         lxml.tree.Element
             Object in the Element format.
         """
         phone_elem = super().to_element()
         phone_elem.set("phonetype", self.phone_type)
+        phone_elem.text = self.phone
         return phone_elem
```

### Comparing `pydwca-0.1.1/src/eml/types/position_name.py` & `pydwca-0.1.2/src/eml/types/position_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/responsible_party.py` & `pydwca-0.1.2/src/eml/types/responsible_party.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/section.py` & `pydwca-0.1.2/src/eml/types/section.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/semantic_annotation.py` & `pydwca-0.1.2/src/eml/types/semantic_annotation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/eml/types/text_type.py` & `pydwca-0.1.2/src/eml/types/text_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/xml_common/xml_object.py` & `pydwca-0.1.2/src/xml_common/xml_object.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/xml_common/utils/enum.py` & `pydwca-0.1.2/src/xml_common/utils/enum.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/xml_common/utils/establishment_means.py` & `pydwca-0.1.2/src/xml_common/utils/establishment_means.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/xml_common/utils/gpolygon.py` & `pydwca-0.1.2/src/xml_common/utils/gpolygon.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/xml_common/utils/iteratate.py` & `pydwca-0.1.2/src/xml_common/utils/iteratate.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/xml_common/utils/language.py` & `pydwca-0.1.2/src/xml_common/utils/language.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/src/xml_common/utils/length_unit.py` & `pydwca-0.1.2/src/xml_common/utils/length_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,8 +84,8 @@
         Generate the valid name of the unit.
 
         Returns
         -------
         str
             Name of the unit.
         """
-        return super().to_camel_case().capitalize()
+        return "_".join([word.lower().capitalize() for word in self.name.split("_")])
```

### Comparing `pydwca-0.1.1/src/xml_common/utils/type_functions.py` & `pydwca-0.1.2/src/xml_common/utils/type_functions.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca/test_dwca.py` & `pydwca-0.1.2/tests/test_dwca/test_dwca.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca/test_dwca_no_pandas.py` & `pydwca-0.1.2/tests/test_dwca/test_dwca_no_pandas.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca/test_meta.py` & `pydwca-0.1.2/tests/test_dwca/test_meta.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca/test_outside_term.py` & `pydwca-0.1.2/tests/test_dwca/test_outside_term.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_classes/test_identification.py` & `pydwca-0.1.2/tests/test_dwca_classes/test_identification.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_classes/test_outside_class.py` & `pydwca-0.1.2/tests/test_dwca_classes/test_outside_class.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_classes/test_taxon.py` & `pydwca-0.1.2/tests/test_dwca_classes/test_taxon.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,35 +2,84 @@
 import sys
 import unittest
 
 import pandas as pd
 from lxml import etree as et
 
 from dwca.classes import Taxon
+from dwca.terms import DWCLanguage
 from test_xml.test_xml import TestXML
+from xml_common.utils import Language
 
 PATH = os.path.abspath(os.path.dirname(__file__))
 
 
 class TestTaxon(TestXML):
     def setUp(self) -> None:
         with open(os.path.join(PATH, os.pardir, "example_data", "meta.xml"), "r", encoding="utf-8") as file:
             content = file.read()
         base_file = et.fromstring(content)
+        self.nmap = base_file.nsmap
         self.taxon_xml = base_file.find("core", namespaces=base_file.nsmap)
         self.text = et.tostring(self.taxon_xml, pretty_print=True).decode("utf-8")
         self.taxon = None
         return
 
     def read_pandas(self):
         self.taxon = Taxon.from_string(self.text)
         with open(os.path.join(PATH, os.pardir, "example_data", "taxon.txt"), "r", encoding="utf-8") as file:
             self.taxon.read_file(file.read())
         return
 
+    def test_add_field(self):
+        taxon = Taxon.from_string(self.text)
+        taxon.add_field(DWCLanguage(index=47, default="eng"))
+        self.assertEqual(48, len(taxon.__fields__), "Fields not set")
+        self.text = self.text.replace(
+            """<field index="46" default="EXAMPLE" term="http://rs.tdwg.org/dwc/terms/institutionCode"/>""",
+            """<field index="46" default="EXAMPLE" term="http://rs.tdwg.org/dwc/terms/institutionCode"/>
+    <field index="47" default="eng" term="http://purl.org/dc/elements/1.1/language"/>""")
+        self.assertEqualTree(et.fromstring(self.text), taxon.to_element(), "Error on element conversion with new field")
+
+    def test_add_field_incorrect_index(self):
+        taxon = Taxon.from_string(self.text)
+        with self.assertWarnsRegex(UserWarning, "index"):
+            taxon.add_field(DWCLanguage(index=3, default="eng"))
+        self.assertEqual(48, len(taxon.__fields__), "Fields not set")
+        self.text = self.text.replace(
+            """<field index="46" default="EXAMPLE" term="http://rs.tdwg.org/dwc/terms/institutionCode"/>""",
+            """<field index="46" default="EXAMPLE" term="http://rs.tdwg.org/dwc/terms/institutionCode"/>
+    <field index="47" default="eng" term="http://purl.org/dc/elements/1.1/language"/>""")
+        self.assertEqualTree(et.fromstring(self.text), taxon.to_element(), "Error on element conversion with new field")
+
+    def test_add_field_data(self):
+        self.read_pandas()
+        df = self.taxon.pandas
+        self.assertEqual(47, len(df.columns), "Wrong number of initial columns")
+        self.assertRaisesRegex(
+            AttributeError, "language",
+            getattr,
+            self.taxon.__entries__[0],
+            "language"
+        )
+        self.taxon.add_field(DWCLanguage(index=47, default="eng"))
+        self.assertEqual(
+            Language.ENG,
+            self.taxon.__entries__[0].language,
+            "Language not write on all entries"
+        )
+        df = self.taxon.pandas
+        self.assertEqual(48, len(df.columns), "Wrong number of columns after set")
+        self.assertEqual(48, len(self.taxon.fields), "Fields not set")
+        self.text = self.text.replace(
+            """<field index="46" default="EXAMPLE" term="http://rs.tdwg.org/dwc/terms/institutionCode"/>""",
+            """<field index="46" default="EXAMPLE" term="http://rs.tdwg.org/dwc/terms/institutionCode"/>
+    <field index="47" default="eng" term="http://purl.org/dc/elements/1.1/language"/>""")
+        self.assertEqualTree(et.fromstring(self.text), self.taxon.to_element(), "Error on element conversion with new field")
+
     def test_parse(self):
         taxon = Taxon.from_string(self.text)
         self.assertEqual("taxon.txt", taxon.filename, "Files parse incorrectly")
         self.assertEqual(0, taxon.id, "Files parse incorrectly")
         self.assertEqual("UTF-8", taxon.__encoding__, "Encoding parse incorrectly")
         self.assertEqual("\n", taxon.__lines_end__, "Lines end parse incorrectly")
         self.assertEqual("\t", taxon.__fields_end__, "Field end parse incorrectly")
```

### Comparing `pydwca-0.1.1/tests/test_dwca_classes/test_taxon_no_pandas.py` & `pydwca-0.1.2/tests/test_dwca_classes/test_taxon_no_pandas.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_any_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_any_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_datetime_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_datetime_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_float_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_float_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_int_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_int_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_list_str_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_list_str_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_outside_term.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_outside_term.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_str_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_str_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_taxon.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_taxon.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_union_datetime_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_union_datetime_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_dwca_terms/test_union_field.py` & `pydwca-0.1.2/tests/test_dwca_terms/test_union_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_access_type.py` & `pydwca-0.1.2/tests/test_eml/test_access_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_address.py` & `pydwca-0.1.2/tests/test_eml/test_address.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_annotation.py` & `pydwca-0.1.2/tests/test_eml/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_citation.py` & `pydwca-0.1.2/tests/test_eml/test_citation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_dataset.py` & `pydwca-0.1.2/tests/test_eml/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_eml.py` & `pydwca-0.1.2/tests/test_eml/test_eml.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_extension.py` & `pydwca-0.1.2/tests/test_eml/test_extension.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_extension_uri.py` & `pydwca-0.1.2/tests/test_eml/test_extension_uri.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_i18n_string.py` & `pydwca-0.1.2/tests/test_eml/test_i18n_string.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_individual_name.py` & `pydwca-0.1.2/tests/test_eml/test_individual_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_keyword_set.py` & `pydwca-0.1.2/tests/test_eml/test_keyword_set.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_licence.py` & `pydwca-0.1.2/tests/test_eml/test_licence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_metadata.py` & `pydwca-0.1.2/tests/test_eml/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_organization_name.py` & `pydwca-0.1.2/tests/test_eml/test_organization_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_phone.py` & `pydwca-0.1.2/tests/test_eml/test_phone.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_position_name.py` & `pydwca-0.1.2/tests/test_eml/test_position_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_responsible_party.py` & `pydwca-0.1.2/tests/test_eml/test_responsible_party.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_section.py` & `pydwca-0.1.2/tests/test_eml/test_section.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_semantic_annotation.py` & `pydwca-0.1.2/tests/test_eml/test_semantic_annotation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml/test_text_type.py` & `pydwca-0.1.2/tests/test_eml/test_text_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml_coverage/test_coverage.py` & `pydwca-0.1.2/tests/test_eml_coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml_coverage/test_geo_coverage.py` & `pydwca-0.1.2/tests/test_eml_coverage/test_geo_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     <geographicDescription>Manistee River watershed</geographicDescription>
     <boundingCoordinates>
         <westBoundingCoordinate>-118.25</westBoundingCoordinate>
         <eastBoundingCoordinate>-118.25</eastBoundingCoordinate>
         <northBoundingCoordinate>-18.25</northBoundingCoordinate>
         <southBoundingCoordinate>-118.25</southBoundingCoordinate>
         <boundingAltitudes>
-            <altitudeMinimum>-10</altitudeMinimum>
+            <altitudeMinimum>-10.0</altitudeMinimum>
             <altitudeMaximum>100.6</altitudeMaximum>
             <altitudeUnits>Yard_Indian</altitudeUnits>
         </boundingAltitudes>
     </boundingCoordinates>
     <datasetGPolygon>
         <datasetGPolygonOuterGRing>
-            <gRing>12, 2.0987 12, -7.5555 34.345,10.40</gRing>
+            <gRing>12.0, 2.0987 12.0, -7.5555 34.345, 10.4</gRing>
         </datasetGPolygonOuterGRing>
     </datasetGPolygon>
 </geographicCoverage>
         """
         geo_coverage = GeographicCoverage.from_string(text_xml)
         self.assertEqual(
             "Manistee River watershed",
@@ -232,15 +232,15 @@
                 <gRingLatitude>-18.25</gRingLatitude>
                 <gRingLongitude>+25</gRingLongitude>
             </gRingPoint>
             <gRingPoint>
                 <gRingLatitude>+78.25</gRingLatitude>
                 <gRingLongitude>45.24755</gRingLongitude>
             </gRingPoint>""", """
-<gRing>34.123, -118.25 -18.25, 25 78.25, 45.24755</gRing>
+<gRing>34.123, -118.25 -18.25, 25.0 78.25, 45.24755</gRing>
             """)
         self.assertEqualTree(
             et.fromstring(text_xml),
             geo_coverage.to_element(),
             "Error on to element"
         )
 
@@ -308,21 +308,21 @@
             "Error on equals implementation"
         )
 
     def test_polygon_to_xml(self):
         xml = """
 <datasetGPolygon>
     <datasetGPolygonOuterGRing>
-        <gRing>12, 2.0987 12, -7.5555 34.345, 10.40</gRing>
+        <gRing>12, 2.0987 12, -7.5555 34.345, 10.4</gRing>
     </datasetGPolygonOuterGRing>
     <datasetGPolygonExclusionGRing>
-        <gRing>12, 2.0987 12, -7.5555 34.345, 10.40</gRing>
+        <gRing>12, 2.0987 12, -7.5555 34.345, 10.4</gRing>
     </datasetGPolygonExclusionGRing>
     <datasetGPolygonExclusionGRing>
-        <gRing>12, 2.0987 12, -7.5555 34.345, 10.40</gRing>
+        <gRing>12, 2.0987 12, -7.5555 34.345, 10.4</gRing>
     </datasetGPolygonExclusionGRing>
 </datasetGPolygon>
         """
         polygon = GPolygon(
             outer=GRing((12, 2.0987), (12, -7.5555), (34.345, 10.40)),
             exclusion=[
                 GRing((12, 2.0987), (12, -7.5555), (34.345, 10.40)),
```

### Comparing `pydwca-0.1.1/tests/test_eml_coverage/test_taxa_coverage.py` & `pydwca-0.1.2/tests/test_eml_coverage/test_taxa_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml_coverage/test_time_coverage.py` & `pydwca-0.1.2/tests/test_eml_coverage/test_time_coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             coverage.single_datetime[0],
             "Error on parsing single date time"
         )
         self.assertEqual(
             dt.datetime(
                 2011, 12, 31,
                 8, 31, 22,
+                tzinfo=dt.timezone.utc
             ),
             coverage.single_datetime[1],
             "Error on parsing second single date time"
         )
         self.assertIsNone(coverage.range_datetime, "Range datetime from nowhere")
         self.assertEqualTree(et.fromstring(text_xml), coverage.to_element(), "Error on to element")
 
@@ -94,29 +95,30 @@
 <temporalCoverage id="1" scope="system" system="http://gbif.org">
     <rangeOfDates>
         <beginDate>
             <calendarDate>2001-01-01</calendarDate>
             <time>08:31:22Z</time>
         </beginDate>
         <endDate>
-            <calendarDate>2021-01-01</calendarDate>
+            <calendarDate>2021</calendarDate>
         </endDate>
     </rangeOfDates>
 </temporalCoverage>
         """
         coverage = TemporalCoverage.from_string(text_xml)
         self.assertEqual("1", coverage.id, "Error on parsing id")
         self.assertEqual(Scope.SYSTEM, coverage.scope, "Error on parsing scope")
         self.assertFalse(coverage.referencing, "Error on parsing")
         self.assertEqual("http://gbif.org", coverage.system, "Error on parsing system")
         self.assertEqual(0, len(coverage.single_datetime), "Single datetime from nowhere")
         self.assertEqual(
             dt.datetime(
                 2001, 1, 1,
                 8, 31, 22,
+                tzinfo=dt.timezone.utc
             ),
             coverage.range_datetime[0],
             "Error on parsing begin range date time"
         )
         self.assertEqual(
             dt.date(
                 2021, 1, 1
```

### Comparing `pydwca-0.1.1/tests/test_eml_distribution/test_distribution.py` & `pydwca-0.1.2/tests/test_eml_distribution/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml_distribution/test_inline.py` & `pydwca-0.1.2/tests/test_eml_distribution/test_inline.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml_distribution/test_offline.py` & `pydwca-0.1.2/tests/test_eml_distribution/test_offline.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_eml_distribution/test_online.py` & `pydwca-0.1.2/tests/test_eml_distribution/test_online.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_util/test_establishment_means.py` & `pydwca-0.1.2/tests/test_util/test_establishment_means.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_util/test_format.py` & `pydwca-0.1.2/tests/test_util/test_format.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_util/test_unformat.py` & `pydwca-0.1.2/tests/test_util/test_unformat.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_xml/test_simple_xml.py` & `pydwca-0.1.2/tests/test_xml/test_simple_xml.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/tests/test_xml/test_xml.py` & `pydwca-0.1.2/tests/test_xml/test_xml.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 class TestXML(unittest.TestCase):
     DEFAULT_TAGS = {}
 
     def assertEqualTree(self, expected: et.ElementTree, actual: et.ElementTree, msg: str) -> None:
         try:
             self.assertEqual(expected.tag, actual.tag, "Not same tag")
+            expected_text = expected.text.strip() if expected.text is not None else ""
+            actual_text = actual.text.strip() if actual.text is not None else ""
+            self.assertEqual(expected_text, actual_text, "Not same text")
             # Add default values:
             exp_attributes = deepcopy(expected.attrib)
             actual_attributes = deepcopy(actual.attrib)
             for key, value in self.DEFAULT_TAGS.items():
                 if key not in exp_attributes:
                     exp_attributes[key] = value
                 if key not in actual_attributes:
```

### Comparing `pydwca-0.1.1/.gitignore` & `pydwca-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/LICENSE` & `pydwca-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/README.md` & `pydwca-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.1/pyproject.toml` & `pydwca-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydwca"
-version = "0.1.1"
+version = "0.1.2"
 dynamic = ["dependencies"]
 description = 'Python library to read, parse and write Darwin Core Archive files'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MPL-2.0"
 license-files = { paths = ["LICENSE"] }
 keywords = []
```

### Comparing `pydwca-0.1.1/PKG-INFO` & `pydwca-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydwca
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library to read, parse and write Darwin Core Archive files
 Project-URL: Documentation, https://pydwca.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/IEB-BIODATA/pydwca/issues
 Project-URL: Source, https://github.com/IEB-BIODATA/pydwca
 Author-email: Juan Saez Hidalgo <jmsaez@ieb-chile.cl>
 License-Expression: MPL-2.0
 License-File: LICENSE
```

