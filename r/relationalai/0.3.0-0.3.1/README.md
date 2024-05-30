# Comparing `tmp/relationalai-0.3.0.tar.gz` & `tmp/relationalai-0.3.1.tar.gz`

## Comparing `relationalai-0.3.0.tar` & `relationalai-0.3.1.tar`

### file list

```diff
@@ -1,639 +1,639 @@
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.3.0/README.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/actions/benchmarks/action.yml
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/actions/snowflake-integration/action.yml
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/benchmarks.yml
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/ruff.yml
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/snowflake-integration.yml
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/README.md
--rw-r--r--   0        0        0    18616 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/getting_started.md
--rw-r--r--   0        0        0   184286 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/repair_priority_graph.png
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/README.md
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/config_check.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/config_explain.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/debugger.md
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_create.md
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_delete.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_get.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_list.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/exports_delete.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/exports_list.md
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_delete.md
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_list.md
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_snapshot.md
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_stream.md
--rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/init.md
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/profile_switch.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/transactions_cancel.md
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/transactions_get.md
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/transactions_list.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/version.md
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/add.md
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/choose.md
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/extend.md
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/in_.md
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/set.md
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/floordiv__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/mod__.md
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rfloordiv__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rmod__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/known_properties.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_clustering_coefficient.md
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/betweenness_centrality.md
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
--rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/diameter_range.md
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/distance.md
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_connected.md
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_reachable.md
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_triangle.md
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/local_clustering_coefficient.md
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_triangles.md
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/reachable_from.md
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/triangle_community.md
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/triangles.md
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/weighted.md
--rw-r--r--   0        0        0   103155 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/directed.png
--rw-r--r--   0        0        0   128981 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    95611 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/undirected.png
--rw-r--r--   0        0        0    93414 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/weighted.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/README.md
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/abs.md
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/acos.md
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/asin.md
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/atan.md
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/cbrt.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/ceil.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/cos.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/degrees.md
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/floor.md
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/isclose.md
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/log.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/radians.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/sign.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/sin.md
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/sqrt.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/tan.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/trunc_divide.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/like.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/regex_compile.md
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/regex_match.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/split.md
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/split_part.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/faq/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/faq/engines.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/cdc.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/cdc_simple.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/fraud.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/requirements.txt
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/simple_streamlit.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/snowflake_sql.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/imdb/imdb.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/power_transmission_network/edges.csv
--rw-r--r--   0        0        0    20669 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/power_transmission_network/nodes.csv
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/power_transmission_network/repair_priority.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/index.html
--rw-r--r--   0        0        0   495827 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/package.json
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/modernize.styl
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/theme.styl
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0    17251 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.styl
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.tsx
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/SystemStatus.styl
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/SystemStatus.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.styl
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.tsx
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/directives/sticky.ts
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/gradient-path.d.ts
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/fileUtils.test.ts
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/fileUtils.ts
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/format.ts
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/solid.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/emit.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/compiler.py
--rw-r--r--   0        0        0    13045 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/debugging.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/dependencies.py
--rw-r--r--   0        0        0    48537 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/dsl.py
--rw-r--r--   0        0        0    17340 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/metagen.py
--rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/rel.py
--rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0    14496 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/config.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/export_procedure.py.jinja
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/result_helpers.py
--rw-r--r--   0        0        0    46167 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/util.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    24073 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/math.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    57001 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/cli_helpers.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/constants.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/debugger_client.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/notes
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/constants.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/format.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/keys.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/snowflake_logger.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/span_format_test.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/tracing_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/testutil/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/testutil/snapshot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/util.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/conftest.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/test_snapshots.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/benchmarks/heap_snapshots.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/benchmarks/tastybytes.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query0.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query2.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query3.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query0.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query2.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query3.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query4.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query5.txt
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/README.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/conftest.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query1.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query2.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query0.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query1.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query10.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query11.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query12.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query13.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query14.txt
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query2.txt
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query3.txt
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query4.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query5.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query6.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query7.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query8.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query9.txt
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/effects/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query0.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query1.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query5.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__mixed_value_types/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query1.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query2.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query3.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query2.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query0.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/snowflake_only__cdc_smoke/query0.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query10.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query11.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query12.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query13.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query14.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query15.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query16.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query17.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query1.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query2.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/after_errors.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/demand_semantics.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/effects.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/hector.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/numeric_outputs.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/out_of_context.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/std_math.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/clustering.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/connectivity.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/distance.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/link_prediction.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/mixed_value_types.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/triangles.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/snowflake_integration/conftest.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/snowflake_integration/test_snapshots.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/snowflake_integration/test_cases/cdc_smoke.py
--rw-r--r--   0        0        0    16596 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_cli.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_config_store.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_dependencies.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_scrub_exceptions.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_configs/config_with_new_profile.toml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_configs/printed_config.txt
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_configs/raiconfig_example.toml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.3.0/.gitignore
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 relationalai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/pypi/README.md
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relationalai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.3.1/README.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/actions/benchmarks/action.yml
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/actions/snowflake-integration/action.yml
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/workflows/snowflake-integration.yml
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 relationalai-0.3.1/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/README.md
+-rw-r--r--   0        0        0    18616 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/getting_started.md
+-rw-r--r--   0        0        0   184286 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/repair_priority_graph.png
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/README.md
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/config_check.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/config_explain.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/debugger.md
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/engines_create.md
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/engines_delete.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/engines_get.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/engines_list.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/exports_delete.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/exports_list.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/imports_delete.md
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/imports_list.md
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/imports_snapshot.md
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/imports_stream.md
+-rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/init.md
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/profile_switch.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/transactions_cancel.md
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/transactions_get.md
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/transactions_list.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/cli/version.md
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/InstanceProperty/add.md
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/InstanceProperty/choose.md
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/InstanceProperty/extend.md
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/InstanceProperty/in_.md
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/InstanceProperty/set.md
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/floordiv__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/mod__.md
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/rfloordiv__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/rmod__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/known_properties.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_clustering_coefficient.md
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/betweenness_centrality.md
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/diameter_range.md
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/distance.md
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/is_connected.md
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/is_reachable.md
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/is_triangle.md
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/local_clustering_coefficient.md
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/num_triangles.md
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/reachable_from.md
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/triangle_community.md
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/triangles.md
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/weighted.md
+-rw-r--r--   0        0        0   103155 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/directed.png
+-rw-r--r--   0        0        0   128981 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    95611 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/undirected.png
+-rw-r--r--   0        0        0    93414 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/weighted.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/README.md
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/abs.md
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/acos.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/asin.md
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/atan.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/cbrt.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/ceil.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/cos.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/degrees.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/floor.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/isclose.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/log.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/radians.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/sign.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/sin.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/sqrt.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/tan.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/math/trunc_divide.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/like.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/regex_compile.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/regex_match.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/split.md
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/split_part.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/faq/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/cdc.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/cdc_simple.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/fraud.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/simple_streamlit.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/snowflake_sql.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/imdb/imdb.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/power_transmission_network/edges.csv
+-rw-r--r--   0        0        0    20669 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/power_transmission_network/nodes.csv
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/power_transmission_network/repair_priority.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 relationalai-0.3.1/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/index.html
+-rw-r--r--   0        0        0   495827 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/package.json
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/modernize.styl
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/theme.styl
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0    17251 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/FileDropZone.styl
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/FileDropZone.tsx
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/SystemStatus.styl
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/SystemStatus.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Breadcrumbs.styl
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Breadcrumbs.tsx
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/directives/sticky.ts
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/types/gradient-path.d.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/utils/fileUtils.test.ts
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/utils/fileUtils.ts
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/utils/format.ts
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 relationalai-0.3.1/frontend/debugger/src/utils/solid.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/emit.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    13045 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/debugging.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/dependencies.py
+-rw-r--r--   0        0        0    48537 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    17340 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/rel.py
+-rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    14496 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    18623 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/export_procedure.py.jinja
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/result_helpers.py
+-rw-r--r--   0        0        0    46080 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/clients/util.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    24073 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/std/math.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    57001 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/cli_helpers.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/constants.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/debugger_client.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/tools/notes
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/util/constants.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/util/format.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/util/keys.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/util/span_format_test.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/relationalai/util/tracing_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/testutil/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 relationalai-0.3.1/src/testutil/snapshot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/util.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/conftest.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/test_snapshots.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/benchmarks/heap_snapshots.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/benchmarks/tastybytes.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query0.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query2.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query3.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query0.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query2.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query3.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query4.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query5.txt
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/README.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query1.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query2.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query0.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query1.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query10.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query11.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query12.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query13.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query14.txt
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query2.txt
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query3.txt
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query4.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query5.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query6.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query7.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query8.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query9.txt
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/effects/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query0.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query1.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query5.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__mixed_value_types/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query1.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query2.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query3.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query2.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query0.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/snowflake_only__cdc_smoke/query0.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query10.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query11.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query12.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query13.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query14.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query15.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query16.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query17.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query1.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query2.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/after_errors.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/demand_semantics.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/effects.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/hector.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/numeric_outputs.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/out_of_context.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/std_math.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/clustering.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/connectivity.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/distance.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/mixed_value_types.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/end2end/test_cases/graphs/triangles.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/init-cli/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/snowflake_integration/conftest.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/snowflake_integration/test_snapshots.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/snowflake_integration/test_cases/cdc_smoke.py
+-rw-r--r--   0        0        0    16596 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/unit/test_config_store.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/unit/test_dependencies.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/unit/test_scrub_exceptions.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/unit/test_configs/config_with_new_profile.toml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/unit/test_configs/printed_config.txt
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 relationalai-0.3.1/tests/unit/test_configs/raiconfig_example.toml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 relationalai-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.3.1/docs/pypi/README.md
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relationalai-0.3.1/PKG-INFO
```

### Comparing `relationalai-0.3.0/README.md` & `relationalai-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/actions/benchmarks/action.yml` & `relationalai-0.3.1/.github/actions/benchmarks/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/actions/end-to-end/action.yml` & `relationalai-0.3.1/.github/actions/end-to-end/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/actions/snowflake-integration/action.yml` & `relationalai-0.3.1/.github/actions/snowflake-integration/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/workflows/benchmarks.yml` & `relationalai-0.3.1/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/workflows/end-to-end.yml` & `relationalai-0.3.1/.github/workflows/end-to-end.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/workflows/publish-to-pypi.yml` & `relationalai-0.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/workflows/ruff.yml` & `relationalai-0.3.1/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/workflows/snowflake-integration.yml` & `relationalai-0.3.1/.github/workflows/snowflake-integration.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/.github/workflows/unit-tests.yml` & `relationalai-0.3.1/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/getting_started.md` & `relationalai-0.3.1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/repair_priority_graph.png` & `relationalai-0.3.1/docs/repair_priority_graph.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.3.1/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/_old/metamodel.md` & `relationalai-0.3.1/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/_old/python_dsl.md` & `relationalai-0.3.1/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/_old/quickstart.md` & `relationalai-0.3.1/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/README.md` & `relationalai-0.3.1/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/config_check.md` & `relationalai-0.3.1/docs/api_reference/cli/config_check.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/config_explain.md` & `relationalai-0.3.1/docs/api_reference/cli/config_explain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/engines_create.md` & `relationalai-0.3.1/docs/api_reference/cli/engines_create.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/engines_delete.md` & `relationalai-0.3.1/docs/api_reference/cli/engines_delete.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/engines_get.md` & `relationalai-0.3.1/docs/api_reference/cli/engines_get.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/engines_list.md` & `relationalai-0.3.1/docs/api_reference/cli/engines_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/exports_delete.md` & `relationalai-0.3.1/docs/api_reference/cli/exports_delete.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/exports_list.md` & `relationalai-0.3.1/docs/api_reference/cli/exports_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/imports_delete.md` & `relationalai-0.3.1/docs/api_reference/cli/imports_delete.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/imports_list.md` & `relationalai-0.3.1/docs/api_reference/cli/imports_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/imports_snapshot.md` & `relationalai-0.3.1/docs/api_reference/cli/imports_snapshot.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/imports_stream.md` & `relationalai-0.3.1/docs/api_reference/cli/imports_stream.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/init.md` & `relationalai-0.3.1/docs/api_reference/cli/init.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/profile_switch.md` & `relationalai-0.3.1/docs/api_reference/cli/profile_switch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/transactions_cancel.md` & `relationalai-0.3.1/docs/api_reference/cli/transactions_cancel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/transactions_get.md` & `relationalai-0.3.1/docs/api_reference/cli/transactions_get.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/transactions_list.md` & `relationalai-0.3.1/docs/api_reference/cli/transactions_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/cli/version.md` & `relationalai-0.3.1/docs/api_reference/cli/version.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/configuration/README.md` & `relationalai-0.3.1/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Expression.md` & `relationalai-0.3.1/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Property.md` & `relationalai-0.3.1/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/README.md` & `relationalai-0.3.1/docs/api_reference/python/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Context/README.md` & `relationalai-0.3.1/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Context/enter__.md` & `relationalai-0.3.1/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Context/exit__.md` & `relationalai-0.3.1/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Context/iter__.md` & `relationalai-0.3.1/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Context/model.md` & `relationalai-0.3.1/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Context/results.md` & `relationalai-0.3.1/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.3.1/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.3.1/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.3.1/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.3.1/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Instance/README.md` & `relationalai-0.3.1/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Instance/set.md` & `relationalai-0.3.1/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.3.1/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/InstanceProperty/add.md` & `relationalai-0.3.1/docs/api_reference/python/InstanceProperty/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/InstanceProperty/choose.md` & `relationalai-0.3.1/docs/api_reference/python/InstanceProperty/choose.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/InstanceProperty/extend.md` & `relationalai-0.3.1/docs/api_reference/python/InstanceProperty/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/InstanceProperty/in_.md` & `relationalai-0.3.1/docs/api_reference/python/InstanceProperty/in_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.3.1/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/InstanceProperty/set.md` & `relationalai-0.3.1/docs/api_reference/python/InstanceProperty/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/README.md` & `relationalai-0.3.1/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/Type.md` & `relationalai-0.3.1/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/found.md` & `relationalai-0.3.1/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/not_found.md` & `relationalai-0.3.1/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.3.1/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/query.md` & `relationalai-0.3.1/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/read.md` & `relationalai-0.3.1/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/rule.md` & `relationalai-0.3.1/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/scope.md` & `relationalai-0.3.1/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Model/union.md` & `relationalai-0.3.1/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/README.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/add__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/floordiv__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/floordiv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/le__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/mod__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/mod__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.3.1/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Type/README.md` & `relationalai-0.3.1/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Type/add.md` & `relationalai-0.3.1/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Type/call__.md` & `relationalai-0.3.1/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Type/extend.md` & `relationalai-0.3.1/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Type/known_properties.md` & `relationalai-0.3.1/docs/api_reference/python/Type/known_properties.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/Type/or__.md` & `relationalai-0.3.1/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/README.md` & `relationalai-0.3.1/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.3.1/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.3.1/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.3.1/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.3.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/Vars.md` & `relationalai-0.3.1/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/alias.md` & `relationalai-0.3.1/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.3.1/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/adamic_adar.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/adamic_adar.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_clustering_coefficient.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_clustering_coefficient.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/betweenness_centrality.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/betweenness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/common_neighbor.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/common_neighbor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/diameter_range.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/diameter_range.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/distance.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_connected.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/is_connected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_reachable.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/is_reachable.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_triangle.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/is_triangle.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/local_clustering_coefficient.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/local_clustering_coefficient.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_indegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/max_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/max_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_degree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_indegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_outdegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_edges.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_nodes.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_triangles.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/num_triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/reachable_from.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/reachable_from.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/triangle_community.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/triangle_community.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/triangles.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_distance.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/add.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/set.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/to.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/Edge.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/weighted.md` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/weighted.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/directed.png` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/directed.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/undirected.png` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/undirected.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/weighted.png` & `relationalai-0.3.1/docs/api_reference/python/std/graphs/Graph/img/weighted.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/abs.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/abs.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/acos.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/acos.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/asin.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/asin.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/atan.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/atan.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/cbrt.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/cbrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/ceil.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/ceil.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/cos.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/cos.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/degrees.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/degrees.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/floor.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/floor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/isclose.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/isclose.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/log.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/log.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/radians.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/radians.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/sign.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/sign.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/sin.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/sin.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/sqrt.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/sqrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/tan.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/tan.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/math/trunc_divide.md` & `relationalai-0.3.1/docs/api_reference/python/std/math/trunc_divide.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/README.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/concat.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/contains.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/ends_with.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/join.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/length.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/like.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/like.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/regex_compile.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/regex_compile.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/regex_match.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/regex_match.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/replace.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/replace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/split.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/split.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/split_part.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/split_part.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/api_reference/python/std/strings/uppercase.md` & `relationalai-0.3.1/docs/api_reference/python/std/strings/uppercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/docs/faq/engines.md` & `relationalai-0.3.1/docs/faq/engines.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/README.md` & `relationalai-0.3.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/cdc.py` & `relationalai-0.3.1/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/cdc_simple.py` & `relationalai-0.3.1/examples/cdc_simple.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/custom_snowflake_connection.py` & `relationalai-0.3.1/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/emit_playground.py` & `relationalai-0.3.1/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/found.py` & `relationalai-0.3.1/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/fraud.ipynb` & `relationalai-0.3.1/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/fraud.py` & `relationalai-0.3.1/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/graph_algos.py` & `relationalai-0.3.1/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/nested.py` & `relationalai-0.3.1/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/or_types.py` & `relationalai-0.3.1/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/remote_load_csv.py` & `relationalai-0.3.1/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/simple_recursion.py` & `relationalai-0.3.1/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/simple_streamlit.py` & `relationalai-0.3.1/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/solver.py` & `relationalai-0.3.1/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/weighted_graph_algos.py` & `relationalai-0.3.1/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/articles_graph/README.md` & `relationalai-0.3.1/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/articles_graph/articles_graph.py` & `relationalai-0.3.1/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.3.1/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/articles_graph/utils.py` & `relationalai-0.3.1/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.3.1/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/data/people.csv` & `relationalai-0.3.1/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/data/transactions.csv` & `relationalai-0.3.1/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/ev_penetration/ev_penetration.py` & `relationalai-0.3.1/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.3.1/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/ev_penetration/state_stats.csv` & `relationalai-0.3.1/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/imdb/README.md` & `relationalai-0.3.1/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/imdb/imdb.csv` & `relationalai-0.3.1/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/imdb/imdb.py` & `relationalai-0.3.1/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/power_transmission_network/edges.csv` & `relationalai-0.3.1/examples/power_transmission_network/edges.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/power_transmission_network/nodes.csv` & `relationalai-0.3.1/examples/power_transmission_network/nodes.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/power_transmission_network/repair_priority.py` & `relationalai-0.3.1/examples/power_transmission_network/repair_priority.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/rel/solver.rel` & `relationalai-0.3.1/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.3.1/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.3.1/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.3.1/examples/social-money-network/snowflake_pagerank.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #--------------------------------------------------
 # Initialize Snowflake data
 #--------------------------------------------------
 
 Account = model.Type("Account", source="sandbox.public.accounts")
 
-Transaction = model.Type("Account", source="sandbox.public.transactions")
+Transaction = model.Type("Transaction", source="sandbox.public.transactions")
 Transaction.define(
     from_ = (Account, "from_account", "account_id"),
     to = (Account, "to_account", "account_id")
 )
 
 #--------------------------------------------------
 # Add types
```

### Comparing `relationalai-0.3.0/frontend/debugger/package-lock.json` & `relationalai-0.3.1/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/package.json` & `relationalai-0.3.1/frontend/debugger/package.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/tsconfig.json` & `relationalai-0.3.1/frontend/debugger/tsconfig.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/vite.config.ts` & `relationalai-0.3.1/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/.storybook/main.ts` & `relationalai-0.3.1/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/App.styl` & `relationalai-0.3.1/frontend/debugger/src/App.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/App.tsx` & `relationalai-0.3.1/frontend/debugger/src/App.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/Selection.tsx` & `relationalai-0.3.1/frontend/debugger/src/Selection.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/debugger_client.ts` & `relationalai-0.3.1/frontend/debugger/src/debugger_client.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/index.tsx` & `relationalai-0.3.1/frontend/debugger/src/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/logo.svg` & `relationalai-0.3.1/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/modernize.styl` & `relationalai-0.3.1/frontend/debugger/src/modernize.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/theme.styl` & `relationalai-0.3.1/frontend/debugger/src/theme.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/util.styl` & `relationalai-0.3.1/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/util.ts` & `relationalai-0.3.1/frontend/debugger/src/util.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/assets/favicon.png` & `relationalai-0.3.1/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/EventList.styl` & `relationalai-0.3.1/frontend/debugger/src/components/EventList.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/EventList.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/EventList.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.styl` & `relationalai-0.3.1/frontend/debugger/src/components/FileDropZone.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/FileDropZone.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.3.1/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/SystemStatus.styl` & `relationalai-0.3.1/frontend/debugger/src/components/SystemStatus.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/SystemStatus.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/SystemStatus.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Breadcrumbs.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Code.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Code.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.styl` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Collapsible.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.3.1/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/directives/sticky.ts` & `relationalai-0.3.1/frontend/debugger/src/directives/sticky.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.3.1/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.3.1/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.3.1/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.3.1/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.3.1/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/fixtures/union.json` & `relationalai-0.3.1/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.3.1/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/utils/fileUtils.test.ts` & `relationalai-0.3.1/frontend/debugger/src/utils/fileUtils.test.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/utils/fileUtils.ts` & `relationalai-0.3.1/frontend/debugger/src/utils/fileUtils.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/utils/format.ts` & `relationalai-0.3.1/frontend/debugger/src/utils/format.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/frontend/debugger/src/utils/solid.ts` & `relationalai-0.3.1/frontend/debugger/src/utils/solid.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/README.md` & `relationalai-0.3.1/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/emit.py` & `relationalai-0.3.1/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/fixtures.py` & `relationalai-0.3.1/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/patch.py` & `relationalai-0.3.1/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/util.py` & `relationalai-0.3.1/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/cli/__main__.py` & `relationalai-0.3.1/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/cli/collect_failures.py` & `relationalai-0.3.1/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/cli/collect_tests.py` & `relationalai-0.3.1/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/cli/repro.py` & `relationalai-0.3.1/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/cli/watch.py` & `relationalai-0.3.1/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/action.py` & `relationalai-0.3.1/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/context.py` & `relationalai-0.3.1/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/document.py` & `relationalai-0.3.1/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/group_limited.py` & `relationalai-0.3.1/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/ir.py` & `relationalai-0.3.1/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/scope.py` & `relationalai-0.3.1/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/task.py` & `relationalai-0.3.1/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/gen/test.py` & `relationalai-0.3.1/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/harness/database.py` & `relationalai-0.3.1/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/validate/diff.py` & `relationalai-0.3.1/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/validate/errors.py` & `relationalai-0.3.1/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/validate/mapping.py` & `relationalai-0.3.1/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/gentest/validate/roundtrip.py` & `relationalai-0.3.1/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/__init__.py` & `relationalai-0.3.1/src/relationalai/__init__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/compiler.py` & `relationalai-0.3.1/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/debugging.py` & `relationalai-0.3.1/src/relationalai/debugging.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/dependencies.py` & `relationalai-0.3.1/src/relationalai/dependencies.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/dsl.py` & `relationalai-0.3.1/src/relationalai/dsl.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/errors.py` & `relationalai-0.3.1/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/metagen.py` & `relationalai-0.3.1/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/metamodel.py` & `relationalai-0.3.1/src/relationalai/metamodel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/rel.py` & `relationalai-0.3.1/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/rel_emitter.py` & `relationalai-0.3.1/src/relationalai/rel_emitter.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/rel_utils.py` & `relationalai-0.3.1/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/analysis/mechanistic.py` & `relationalai-0.3.1/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/analysis/whynot.py` & `relationalai-0.3.1/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/clients/azure.py` & `relationalai-0.3.1/src/relationalai/clients/azure.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/clients/client.py` & `relationalai-0.3.1/src/relationalai/clients/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,22 +345,21 @@
             self.create_database(isolated=isolated, nowait_durable=nowait_durable)
 
     def create_database(self, isolated=True, nowait_durable=True):
         start = time.perf_counter()
         with debugging.span("create_database", source=self._source_database, target=self._database):
             database_exists = self.resources.get_graph(self._source_database)
             if isolated:
-                if database_exists:
-                    temp = self._database
-                    self._database = self._source_database
-                    self.exec_raw("", readonly=False, internal=True, nowait_durable=True)
-                    self._database = temp
-                    self.resources.clone_graph(self._database, self._source_database, nowait_durable=nowait_durable)
-                else:
-                    self.resources.create_graph(self._database)
+                if not database_exists:
+                    self.resources.create_graph(self._source_database)
+                temp = self._database
+                self._database = self._source_database
+                self.exec_raw("", readonly=False, internal=True, nowait_durable=True)
+                self._database = temp
+                self.resources.clone_graph(self._database, self._source_database, nowait_durable=nowait_durable)
             elif not database_exists:
                 self.resources.create_graph(self._database)
             if isolated and not self.keep_model:
                 atexit.register(self.delete_database)
             debugging.time("create_database", time.perf_counter() - start)
 
     def delete_database(self):
```

### Comparing `relationalai-0.3.0/src/relationalai/clients/config.py` & `relationalai-0.3.1/src/relationalai/clients/config.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/clients/export_procedure.py.jinja` & `relationalai-0.3.1/src/relationalai/clients/export_procedure.py.jinja`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/clients/result_helpers.py` & `relationalai-0.3.1/src/relationalai/clients/result_helpers.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/clients/snowflake.py` & `relationalai-0.3.1/src/relationalai/clients/snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,16 @@
     def create_import_stream(self, source:ImportSource, model:str, rate = 1, options: dict|None = None):
         assert isinstance(source, ImportSourceTable), "Snowflake integration only supports loading from SF Tables right now. Try loading your data as a table via the snowflake interface first."
         object = source.fqn
 
         if object.lower() in [x["name"].lower() for x in self.list_imports(model=model)]:
             return
 
-        info = self._exec(f"SHOW OBJECTS like ? in {source.database}.{source.schema}", [source.table])
+        query = f"SHOW OBJECTS LIKE '{source.table}' IN {source.database}.{source.schema}"
+        info = self._exec(query)
         if not info:
             raise ValueError(f"Object {source.table} not found in {source.database}.{source.schema}")
         else:
             data = info[0]
             if not data:
                 raise ValueError(f"Object {source.table} not found in {source.database}.{source.schema}")
             # (time, name, db_name, schema_name, kind, *rest)
@@ -685,48 +686,48 @@
         with debugging.span("transaction") as txn_span:
             with debugging.span("create_v2"):
                 response = self._exec(
                     f"CALL {APP_NAME}.api.exec_async_v2('{database}','{engine}', ?, {inputs}, {readonly}, {nowait_durable}, {headers});",
                     raw_code,
                 )
 
-                if not response:
-                    raise Exception("Failed to create transaction")
+            if not response:
+                raise Exception("Failed to create transaction")
+
+            artifact_urls = {}
+            rows = list(iter(response))
+
+            # process the first row since txn_id and state are the same for all rows
+            txn_id, state, filename, url = rows[0]
+            txn_span["txn_id"] = txn_id
+            debugging.event("transaction_created", txn_span, txn_id=txn_id)
 
-                artifact_urls = {}
-                rows = list(iter(response))
+            # fast path: transaction already finished
+            if state == "COMPLETED" or state == "ABORTED":
+                if txn_id in self._pending_transactions:
+                    self._pending_transactions.remove(txn_id)
+                artifact_urls[filename] = url
+
+                # Process rows to get the rest of the artifacts
+                for row in rows:
+                    _, _, filename, url = row
 
-                # process the first row since txn_id and state are the same for all rows
-                txn_id, state, filename, url = rows[0]
-                txn_span["txn_id"] = txn_id
-                debugging.event("transaction_created", txn_span, txn_id=txn_id)
-
-                # fast path: transaction already finished
-                if state == "COMPLETED" or state == "ABORTED":
-                    if txn_id in self._pending_transactions:
-                        self._pending_transactions.remove(txn_id)
                     artifact_urls[filename] = url
 
-                    # Process rows to get the rest of the artifacts
-                    for row in rows:
-                        _, _, filename, url = row
-
-                        artifact_urls[filename] = url
-
-                # Slow path: transaction not done yet; start polling
-                else:
-                    self._pending_transactions.append(txn_id)
-                    with debugging.span("wait", txn_id=txn_id):
-                        poll_with_specified_overhead(
-                            lambda: self._check_exec_async_status(txn_id), 1.0
-                        )
-                    artifact_urls = self._list_exec_async_artifacts(txn_id)
+            # Slow path: transaction not done yet; start polling
+            else:
+                self._pending_transactions.append(txn_id)
+                with debugging.span("wait", txn_id=txn_id):
+                    poll_with_specified_overhead(
+                        lambda: self._check_exec_async_status(txn_id), 1.0
+                    )
+                artifact_urls = self._list_exec_async_artifacts(txn_id)
 
-                with debugging.span("fetch"):
-                    return self._download_results(artifact_urls, txn_id, state)
+            with debugging.span("fetch"):
+                return self._download_results(artifact_urls, txn_id, state)
 
 
     #--------------------------------------------------
     # Exec
     #--------------------------------------------------
 
     def exec_raw(
```

### Comparing `relationalai-0.3.0/src/relationalai/clients/test.py` & `relationalai-0.3.1/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/clients/types.py` & `relationalai-0.3.1/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/clients/util.py` & `relationalai-0.3.1/src/relationalai/clients/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/loaders/csv.py` & `relationalai-0.3.1/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/loaders/loader.py` & `relationalai-0.3.1/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/loaders/types.py` & `relationalai-0.3.1/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/std/aggregates.py` & `relationalai-0.3.1/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/std/graphs.py` & `relationalai-0.3.1/src/relationalai/std/graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/std/math.py` & `relationalai-0.3.1/src/relationalai/std/math.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/std/strings.py` & `relationalai-0.3.1/src/relationalai/std/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/cli.py` & `relationalai-0.3.1/src/relationalai/tools/cli.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/cli_controls.py` & `relationalai-0.3.1/src/relationalai/tools/cli_controls.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/cli_helpers.py` & `relationalai-0.3.1/src/relationalai/tools/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/constants.py` & `relationalai-0.3.1/src/relationalai/tools/constants.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/debugger.py` & `relationalai-0.3.1/src/relationalai/tools/debugger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/debugger_client.py` & `relationalai-0.3.1/src/relationalai/tools/debugger_client.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/debugger_server.py` & `relationalai-0.3.1/src/relationalai/tools/debugger_server.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/tools/dev.py` & `relationalai-0.3.1/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/util/format.py` & `relationalai-0.3.1/src/relationalai/util/format.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/util/snowflake_logger.py` & `relationalai-0.3.1/src/relationalai/util/snowflake_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/util/span_format_test.py` & `relationalai-0.3.1/src/relationalai/util/span_format_test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/relationalai/util/tracing_logger.py` & `relationalai-0.3.1/src/relationalai/util/tracing_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/src/testutil/snapshot.py` & `relationalai-0.3.1/src/testutil/snapshot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/conftest.py` & `relationalai-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/util.py` & `relationalai-0.3.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/benchmarks/conftest.py` & `relationalai-0.3.1/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/benchmarks/benchmarks/heap_snapshots.py` & `relationalai-0.3.1/tests/benchmarks/benchmarks/heap_snapshots.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/benchmarks/benchmarks/tastybytes.py` & `relationalai-0.3.1/tests/benchmarks/benchmarks/tastybytes.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/README.md` & `relationalai-0.3.1/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/conftest.py` & `relationalai-0.3.1/tests/end2end/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_graph_visualize.py` & `relationalai-0.3.1/tests/end2end/test_graph_visualize.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query3.txt` & `relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query3.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.3.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/after_errors.py` & `relationalai-0.3.1/tests/end2end/test_cases/after_errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/agg_ordering.py` & `relationalai-0.3.1/tests/end2end/test_cases/agg_ordering.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/bool.py` & `relationalai-0.3.1/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/bottom.py` & `relationalai-0.3.1/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/demand_semantics.py` & `relationalai-0.3.1/tests/end2end/test_cases/demand_semantics.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/effects.py` & `relationalai-0.3.1/tests/end2end/test_cases/effects.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/export.py` & `relationalai-0.3.1/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/hector.py` & `relationalai-0.3.1/tests/end2end/test_cases/hector.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.3.1/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/not_found.py` & `relationalai-0.3.1/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/numeric_outputs.py` & `relationalai-0.3.1/tests/end2end/test_cases/numeric_outputs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/out_of_context.py` & `relationalai-0.3.1/tests/end2end/test_cases/out_of_context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/persist.py` & `relationalai-0.3.1/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/smoke.py` & `relationalai-0.3.1/tests/end2end/test_cases/smoke.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/std_math.py` & `relationalai-0.3.1/tests/end2end/test_cases/std_math.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/strings.py` & `relationalai-0.3.1/tests/end2end/test_cases/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/top.py` & `relationalai-0.3.1/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/union.py` & `relationalai-0.3.1/tests/end2end/test_cases/union.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.3.1/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/basics.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/basics.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/centrality.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/clustering.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/clustering.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/community.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/community.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/connectivity.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/connectivity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/degree.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/distance.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/distance.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/link_prediction.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/link_prediction.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/mixed_value_types.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/mixed_value_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/similarity.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/similarity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/end2end/test_cases/graphs/triangles.py` & `relationalai-0.3.1/tests/end2end/test_cases/graphs/triangles.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/init-cli/README.md` & `relationalai-0.3.1/tests/init-cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/init-cli/azure_basic.py` & `relationalai-0.3.1/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/init-cli/common.py` & `relationalai-0.3.1/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/roundtrip/test_document.py` & `relationalai-0.3.1/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/roundtrip/test_task.py` & `relationalai-0.3.1/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/snowflake_integration/conftest.py` & `relationalai-0.3.1/tests/snowflake_integration/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/snowflake_integration/test_cases/cdc_smoke.py` & `relationalai-0.3.1/tests/snowflake_integration/test_cases/cdc_smoke.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/unit/test_cli.py` & `relationalai-0.3.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/unit/test_config_store.py` & `relationalai-0.3.1/tests/unit/test_config_store.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/unit/test_dependencies.py` & `relationalai-0.3.1/tests/unit/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/unit/test_scrub_exceptions.py` & `relationalai-0.3.1/tests/unit/test_scrub_exceptions.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/unit/test_configs/config_with_new_profile.toml` & `relationalai-0.3.1/tests/unit/test_configs/config_with_new_profile.toml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/tests/unit/test_configs/raiconfig_example.toml` & `relationalai-0.3.1/tests/unit/test_configs/raiconfig_example.toml`

 * *Files identical despite different names*

### Comparing `relationalai-0.3.0/pyproject.toml` & `relationalai-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.3.0'
+version = '0.3.1'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.3.0/PKG-INFO` & `relationalai-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.3.0
+Version: 0.3.1
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: aiohttp
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
```

