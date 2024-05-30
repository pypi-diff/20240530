# Comparing `tmp/relationalai-0.2.9.tar.gz` & `tmp/relationalai-0.3.0.tar.gz`

## Comparing `relationalai-0.2.9.tar` & `relationalai-0.3.0.tar`

### file list

```diff
@@ -1,573 +1,639 @@
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.9/README.md
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/actions/benchmarks/action.yml
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/benchmarks.yml
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/README.md
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/README.md
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/config_check.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/config_explain.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/debugger.md
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_create.md
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_delete.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_get.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_list.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/exports_delete.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/exports_list.md
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_delete.md
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_list.md
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_snapshot.md
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_stream.md
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/init.md
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/profile_switch.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/transactions_cancel.md
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/transactions_get.md
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/transactions_list.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/version.md
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/floordiv__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rfloordiv__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/average_clustering_coefficient.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/diameter_range.md
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/distance.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_connected.md
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_reachable.md
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_triangle.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/local_lustering_coefficient.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_triangles.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/reachable_from.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/triangles.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/README.md
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/abs.md
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/acos.md
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/asin.md
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/atan.md
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/cbrt.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/ceil.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/cos.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/degrees.md
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/floor.md
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/isclose.md
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/log.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/radians.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/sign.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/sin.md
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/sqrt.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/tan.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/trunc_divide.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/like.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/regex_compile.md
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/regex_match.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/split.md
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/split_part.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/faq/README.md
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/faq/engines.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/cdc.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/fraud.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/requirements.txt
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/index.html
--rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/package.json
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventViewer.styl
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventViewer.tsx
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.styl
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.tsx
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.styl
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.tsx
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/utils/fileUtils.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/emit.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/compiler.py
--rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/debugging.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/dsl.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel2.py
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    39864 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    24099 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/math.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    59285 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/debugger_client.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/notes
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/constants.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/format.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/keys.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/snowflake_logger.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/tracing_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/__init__.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/conftest.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/util.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/benchmarks/conftest.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/benchmarks/test_heap_snapshots.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/benchmarks/test_tastybytes.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8133 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query0.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query5.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__mixed_value_types/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query0.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query10.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query11.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query12.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query13.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query14.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query15.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query16.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query17.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/after_errors.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/numeric_outputs.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/out_of_context.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/std_math.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/clustering.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/connectivity.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/distance.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/link_prediction.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/mixed_value_types.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/triangles.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_config_store.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_configs/config_with_new_profile.toml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_configs/printed_config.txt
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_configs/raiconfig_example.toml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.9/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 relationalai-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/pypi/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.3.0/README.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/actions/benchmarks/action.yml
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/actions/snowflake-integration/action.yml
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/snowflake-integration.yml
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 relationalai-0.3.0/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/README.md
+-rw-r--r--   0        0        0    18616 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/getting_started.md
+-rw-r--r--   0        0        0   184286 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/repair_priority_graph.png
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/README.md
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/config_check.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/config_explain.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/debugger.md
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_create.md
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_delete.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_get.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/engines_list.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/exports_delete.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/exports_list.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_delete.md
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_list.md
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_snapshot.md
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/imports_stream.md
+-rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/init.md
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/profile_switch.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/transactions_cancel.md
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/transactions_get.md
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/transactions_list.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/cli/version.md
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/add.md
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/choose.md
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/extend.md
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/in_.md
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/InstanceProperty/set.md
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/floordiv__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/mod__.md
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rfloordiv__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rmod__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/known_properties.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_clustering_coefficient.md
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/betweenness_centrality.md
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/diameter_range.md
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/distance.md
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_connected.md
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_reachable.md
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_triangle.md
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/local_clustering_coefficient.md
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_triangles.md
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/reachable_from.md
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/triangle_community.md
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/triangles.md
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/weighted.md
+-rw-r--r--   0        0        0   103155 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/directed.png
+-rw-r--r--   0        0        0   128981 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    95611 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/undirected.png
+-rw-r--r--   0        0        0    93414 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/weighted.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/README.md
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/abs.md
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/acos.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/asin.md
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/atan.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/cbrt.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/ceil.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/cos.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/degrees.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/floor.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/isclose.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/log.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/radians.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/sign.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/sin.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/sqrt.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/tan.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/math/trunc_divide.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/like.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/regex_compile.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/regex_match.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/split.md
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/split_part.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/faq/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/cdc.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/cdc_simple.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/fraud.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/simple_streamlit.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/snowflake_sql.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/imdb/imdb.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/power_transmission_network/edges.csv
+-rw-r--r--   0        0        0    20669 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/power_transmission_network/nodes.csv
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/power_transmission_network/repair_priority.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 relationalai-0.3.0/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/index.html
+-rw-r--r--   0        0        0   495827 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/package.json
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/modernize.styl
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/theme.styl
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0    17251 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.styl
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.tsx
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/SystemStatus.styl
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/SystemStatus.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.styl
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.tsx
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/directives/sticky.ts
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/gradient-path.d.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/fileUtils.test.ts
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/fileUtils.ts
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/format.ts
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 relationalai-0.3.0/frontend/debugger/src/utils/solid.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/emit.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    13045 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/debugging.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/dependencies.py
+-rw-r--r--   0        0        0    48537 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    17340 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/rel.py
+-rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    14496 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/export_procedure.py.jinja
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/result_helpers.py
+-rw-r--r--   0        0        0    46167 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/clients/util.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    24073 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/math.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    57001 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/cli_helpers.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/constants.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/debugger_client.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/tools/notes
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/constants.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/format.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/keys.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/span_format_test.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/relationalai/util/tracing_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/testutil/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 relationalai-0.3.0/src/testutil/snapshot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/util.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/conftest.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/test_snapshots.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/benchmarks/heap_snapshots.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/benchmarks/tastybytes.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query0.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query2.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/heap_snapshots/query3.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query0.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query2.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query3.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query4.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/benchmarks/snapshots/test_snapshots/test_snapshots/tastybytes/query5.txt
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/README.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query1.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query2.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query0.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query1.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query10.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query11.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query12.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query13.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query14.txt
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query2.txt
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query3.txt
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query4.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query5.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query6.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query7.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query8.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/demand_semantics/query9.txt
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/effects/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query0.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query1.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query5.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__mixed_value_types/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query1.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query2.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/hector/query3.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query2.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query0.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/snowflake_only__cdc_smoke/query0.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query10.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query11.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query12.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query13.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query14.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query15.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query16.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query17.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query1.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query2.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/after_errors.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/demand_semantics.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/effects.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/hector.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/numeric_outputs.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/out_of_context.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/std_math.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/clustering.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/connectivity.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/distance.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/mixed_value_types.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/end2end/test_cases/graphs/triangles.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/snowflake_integration/conftest.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/snowflake_integration/test_snapshots.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/snowflake_integration/test_cases/cdc_smoke.py
+-rw-r--r--   0        0        0    16596 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_config_store.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_dependencies.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_scrub_exceptions.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_configs/config_with_new_profile.toml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_configs/printed_config.txt
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 relationalai-0.3.0/tests/unit/test_configs/raiconfig_example.toml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 relationalai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.3.0/docs/pypi/README.md
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relationalai-0.3.0/PKG-INFO
```

### Comparing `relationalai-0.2.9/README.md` & `relationalai-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/.github/actions/benchmarks/action.yml` & `relationalai-0.3.0/.github/actions/benchmarks/action.yml`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,19 @@
   # Datadog
   datadog_api_key:
     required: false
     description: Datadog API key
   # Benchmark reporting
   sf_reporting_password:
     description: password for benchmark reporting
+    # Feature flag to use exec_async_v2
+  sf_use_exec_async_v2:
+    description: Feature flag to use exec_async_v2
+    required: false
+
 runs:
   using: "composite"
   steps:
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: ${{ inputs.python_version }}
@@ -86,14 +91,16 @@
         # TODO: use bucket instead of inserting directly to Snowflake
         SF_REPORTING_USER: pyrel_ci
         SF_REPORTING_PASSWORD: ${{ inputs.sf_reporting_password }}
         SF_REPORTING_ACCOUNT: ndsoebe-rai_snowservices
         SF_REPORTING_WAREHOUSE: DATA_ANALYTICS_WH
         SF_REPORTING_DATABASE: PYREL_BENCHMARKING
         SF_REPORTING_SCHEMA: public
+      
+        SF_USE_EXEC_ASYNC_V2: ${{ inputs.sf_use_exec_async_v2 }}
 
         ENABLE_TRACING_LOGGER: 'true'
 
         # datadog CI monitoring
         DD_SERVICE: pyrel-tests
         DD_ENV: ci
         DD_CIVISIBILITY_AGENTLESS_ENABLED: true
```

### Comparing `relationalai-0.2.9/.github/actions/end-to-end/action.yml` & `relationalai-0.3.0/.github/actions/snowflake-integration/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,18 @@
   datadog_api_key:
     required: false
     description: Datadog API key
   # Benchmark reporting
   sf_reporting_password:
     description: password for benchmark reporting
     required: false
-  
+  # Feature flag to use exec_async_v2
+  sf_use_exec_async_v2:
+    description: Feature flag to use exec_async_v2
+    required: false
 
 runs:
   using: "composite"
   steps:
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
@@ -69,40 +72,43 @@
         echo "ENGINE_NAME=pyrel_test_$(openssl rand -hex 5)" >> $GITHUB_ENV
         echo "Setting up ENGINE_NAME..."
       shell: bash
 
     - name: Run Create Engine
       run: |
         echo "Using ENGINE_NAME: $ENGINE_NAME"
-        .venv/bin/python -c "from tests.util import create_engine; create_engine('${{ env.ENGINE_NAME }}')"
+        # keep size in sync with tests/end2end/config.py
+        .venv/bin/python -c "from tests.util import create_engine; create_engine('${{ env.ENGINE_NAME }}', size='XS')"
 
       env: 
         RAI_CLIENT_ID: ${{ inputs.rai_client_id }}
         RAI_CLIENT_SECRET: ${{ inputs.rai_client_secret }}
         RAI_CLOUD_PROVIDER: ${{ inputs.rai_cloud_provider }}
         
         SF_TEST_ACCOUNT_NAME: ${{ inputs.sf_account }}
         SF_TEST_WAREHOUSE_NAME: ${{ inputs.sf_warehouse }}
         SF_TEST_APP_NAME: ${{ inputs.sf_rai_app_name }}
         SF_TEST_COMPUTE_POOL: ${{ inputs.sf_compute_pool }}
         SF_TEST_ACCOUNT_USERNAME: ${{ inputs.sf_username }}
         SF_TEST_ACCOUNT_PASSWORD: ${{ inputs.sf_password }}
 
+        SF_USE_EXEC_ASYNC_V2: ${{ inputs.sf_use_exec_async_v2 }}
+
         # datadog CI monitoring
         DD_SERVICE: pyrel-tests
         DD_ENV: ci
         DD_CIVISIBILITY_AGENTLESS_ENABLED: true
         DD_API_KEY: ${{ inputs.datadog_api_key }}
 
       shell: bash
     
     - name: Run Test
       run: |
         .venv/bin/pytest -s \
-          tests/end2end \
+          tests/snowflake_integration \
           --ddtrace \
           --ddtrace-patch-all \
           --cov=relationalai \
           --cov-report lcov:coverage/lcov.info \
           --cov-report html:coverage/html-report \
           --cov-report term
       env:
```

### Comparing `relationalai-0.2.9/.github/workflows/benchmarks.yml` & `relationalai-0.3.0/.github/workflows/end-to-end.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-name: Run Benchmarks
+name: Run End To End Tests
 
 on:
-  schedule:
-    - cron: '0 0 * * *'
+  push:
+    branches: [ main ]
+  pull_request:
   workflow_dispatch:
 
 concurrency:
   group:
     ${{ github.workflow }}-${{ (github.ref_name == 'main' || github.event_name == 'workflow_dispatch')
     && github.run_id
     || github.ref }}
-  cancel-in-progress: true 
+  cancel-in-progress: true
 
 jobs:
-  benchmark:
+  test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         include:
-          - python-version: '3.12'
+          - python-version: '3.11'
             cloud-provider: 'snowflake'
+          - python-version: '3.10'
+            cloud-provider: 'azure'
     steps:
 
-    - uses: actions/checkout@v4
-      name: Checkout repository
-
-    - uses: ./.github/actions/benchmarks
-      with:
-        python_version: ${{ matrix.python-version }}
-        rai_cloud_provider: ${{ matrix.cloud-provider }}
-        rai_client_id: ${{ secrets.RAI_CLIENT_ID }}
-        rai_client_secret: ${{ secrets.RAI_CLIENT_SECRET }}
-        sf_account: ndsoebe-rai_integration_aws_uswest_1_consumer
-        sf_warehouse: int_env_wh
-        sf_rai_app_name: rai_int_app
-        sf_compute_pool: int_env_benchmark_compute_xs
-        sf_username: team-prod-experience@relational.ai
-        sf_password: ${{ secrets.SF_TEST_ACCOUNT_PASSWORD }}
-        datadog_api_key: ${{ secrets.DD_API_KEY }}
-        sf_reporting_password: ${{ secrets.SF_REPORTING_PASSWORD }}
-    
-    - name: Upload Coverage Artifact
-      uses: actions/upload-artifact@v2
-      with:
-        name: coverage-artifact-${{ matrix.python-version }}
-        path: coverage/lcov.info
-
-    - name: Upload Coverage Report
-      uses: actions/upload-artifact@v2
-      with:
-        name: coverage-report-${{ matrix.python-version }}
-        path: coverage/html-report
+      - uses: actions/checkout@v4
+        name: Checkout repository
+        with:
+          ref: ${{ github.event_name == 'pull_request' && github.event.pull_request.head.sha || github.sha }}
+
+      - uses: ./.github/actions/end-to-end
+        with:
+          python_version: ${{ matrix.python-version }}
+          rai_cloud_provider: ${{ matrix.cloud-provider }}
+          rai_client_id: ${{ secrets.RAI_CLIENT_ID }}
+          rai_client_secret: ${{ secrets.RAI_CLIENT_SECRET }}
+          sf_account: ndsoebe-rai_integration_aws_uswest_1_consumer
+          sf_warehouse: int_env_wh
+          sf_rai_app_name: rai_int_app
+          sf_compute_pool: int_env_benchmark_compute_xs
+          sf_username: team-prod-experience@relational.ai
+          sf_password: ${{ secrets.SF_TEST_ACCOUNT_PASSWORD }}
+          datadog_api_key: ${{ secrets.DD_API_KEY }}
+          sf_reporting_password: ${{ secrets.SF_REPORTING_PASSWORD }}
+
+          sf_use_exec_async_v2: ${{ vars.SF_USE_EXEC_ASYNC_V2}}
+
+      - name: Upload Coverage Artifact
+        uses: actions/upload-artifact@v2
+        with:
+          name: coverage-artifact-${{ matrix.python-version }}
+          path: coverage/lcov.info
+
+      - name: Upload Coverage Report
+        uses: actions/upload-artifact@v2
+        with:
+          name: coverage-report-${{ matrix.python-version }}
+          path: coverage/html-report
```

### Comparing `relationalai-0.2.9/.github/workflows/end-to-end.yml` & `relationalai-0.3.0/.github/workflows/snowflake-integration.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-name: Run End To End Tests
+name: Run Snowflake Integration Tests
 
 on:
-  push:
-    branches: [ main ]
-  pull_request:
-    branches: [ main ]
+  schedule:
+    - cron: '0 0 * * *'
+  workflow_dispatch:
 
 concurrency:
   group:
     ${{ github.workflow }}-${{ (github.ref_name == 'main' || github.event_name == 'workflow_dispatch')
     && github.run_id
     || github.ref }}
   cancel-in-progress: true
@@ -16,44 +15,54 @@
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         include:
-          - python-version: '3.12'
+          - python-version: '3.11'
             cloud-provider: 'snowflake'
-          - python-version: '3.10'
-            cloud-provider: 'azure'
     steps:
 
       - uses: actions/checkout@v4
         name: Checkout repository
         with:
           ref: ${{ github.event_name == 'pull_request' && github.event.pull_request.head.sha || github.sha }}
 
-      - uses: ./.github/actions/end-to-end
+      - uses: ./.github/actions/snowflake-integration
         with:
           python_version: ${{ matrix.python-version }}
           rai_cloud_provider: ${{ matrix.cloud-provider }}
           rai_client_id: ${{ secrets.RAI_CLIENT_ID }}
           rai_client_secret: ${{ secrets.RAI_CLIENT_SECRET }}
           sf_account: ndsoebe-rai_integration_aws_uswest_1_consumer
           sf_warehouse: int_env_wh
           sf_rai_app_name: rai_int_app
           sf_compute_pool: int_env_benchmark_compute_xs
           sf_username: team-prod-experience@relational.ai
           sf_password: ${{ secrets.SF_TEST_ACCOUNT_PASSWORD }}
           datadog_api_key: ${{ secrets.DD_API_KEY }}
           sf_reporting_password: ${{ secrets.SF_REPORTING_PASSWORD }}
 
+          sf_use_exec_async_v2: ${{ vars.SF_USE_EXEC_ASYNC_V2}}
+
       - name: Upload Coverage Artifact
         uses: actions/upload-artifact@v2
         with:
           name: coverage-artifact-${{ matrix.python-version }}
           path: coverage/lcov.info
 
       - name: Upload Coverage Report
         uses: actions/upload-artifact@v2
         with:
           name: coverage-report-${{ matrix.python-version }}
           path: coverage/html-report
+
+      - name: Post to Slack
+        if: ${{ failure() }}
+        uses: slackapi/slack-github-action@v1.23.0
+        with:
+          channel-id: C066T0HBSTW # team-prod-experience-oncall
+          slack-message: |
+            Snowflake integration tests failed: https://github.com/${{ github.repository }}/actions/runs/${{ github.run_id }}
+        env:
+          SLACK_BOT_TOKEN: ${{ secrets.SLACK_BOT_TOKEN }}
```

### Comparing `relationalai-0.2.9/.github/workflows/publish-to-pypi.yml` & `relationalai-0.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/.github/workflows/ruff.yml` & `relationalai-0.3.0/.github/workflows/ruff.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 name: Python Ruff Lint
 
 on:
-  pull_request:
+  push:
     branches: [ main ]
+  pull_request:
+  workflow_dispatch:
 
 concurrency:
   group:
     ${{ github.workflow }}-${{ (github.ref_name == 'main' || github.event_name == 'workflow_dispatch')
     && github.run_id
     || github.ref }}
   cancel-in-progress: true
```

### Comparing `relationalai-0.2.9/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.3.0/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/_old/metamodel.md` & `relationalai-0.3.0/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/_old/python_dsl.md` & `relationalai-0.3.0/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/_old/quickstart.md` & `relationalai-0.3.0/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/README.md` & `relationalai-0.3.0/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/config_check.md` & `relationalai-0.3.0/docs/api_reference/cli/config_check.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/config_explain.md` & `relationalai-0.3.0/docs/api_reference/cli/config_explain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/engines_create.md` & `relationalai-0.3.0/docs/api_reference/cli/engines_create.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/engines_delete.md` & `relationalai-0.3.0/docs/api_reference/cli/engines_delete.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/engines_get.md` & `relationalai-0.3.0/docs/api_reference/cli/engines_get.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/engines_list.md` & `relationalai-0.3.0/docs/api_reference/cli/engines_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/exports_delete.md` & `relationalai-0.3.0/docs/api_reference/cli/exports_delete.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/exports_list.md` & `relationalai-0.3.0/docs/api_reference/cli/exports_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/imports_delete.md` & `relationalai-0.3.0/docs/api_reference/cli/imports_delete.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/imports_list.md` & `relationalai-0.3.0/docs/api_reference/cli/imports_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/imports_snapshot.md` & `relationalai-0.3.0/docs/api_reference/cli/imports_snapshot.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # `imports:snapshot`
 
 ```sh
 rai imports:snapshot [OPTIONS] [schema:<col_name>=<type>, ...] [syntax:<option>=<value>, ...]
 ```
 
 Load data from a CSV file into a RelationalAI model.
-The CSV file may be local or hosted publicly on Azure or S3.
+The CSV file may be local or hosted on Azure or S3.
+Pre-signed URLs are currently unsupported.
 
 > [!IMPORTANT]
 > `imports:snapshot` is only available for Azure-based models.
 
 ## Options
 
 | Option | Type | Description |
@@ -20,24 +21,27 @@
 | `--type` | Text | The file type. May be one of `"auto"` (default) or `"csv"`. |
 
 ## Arguments
 
 <!-- markdownlint-disable no-inline-html -->
 
 | Argument | Required | Description |
-| :--------- | :--- | :------------ |
-| `schema:<col_name>=<type>` | No | Set the type of the column named `<col_name>` to `<type>`.<br><br>`<type>` may be one of:<br><br>- `string`<br>- `boolean`<br>- `int`<br>- `float` |
+| :------------ | :--- | :--------------- |
+| `schema:<col_name>=<type>` | No | Set the type of the column named `<col_name>` to `<type>`.<br><br>`<type>` may be one of:<br><br>- `string`<br>- `boolean`<br>- `int`<br>- `float`<br>- `date`<br>- `datetime` |
 | `syntax:header_row=<line_number>` | No | Set the line number of the header row in the CSV file. Defaults to `1`. The values `-1` and `0` indicate that the file has no header row. |
 | `syntax:datarow=<line_number>` | No | Set the line number from which to begin parsing data from the CSV file. If missing, defaults to the first line after the header row. |
 | `syntax:missingstrings=<string1>` | No | Set the string that represents missing (null) values in the CSV file. Defaults to `""`.  |
 | `syntax:delim=<delimiter>` | No | Set the delimiter used in the CSV file. Defaults to `","`. |
 | `syntax:quotechar=<char>` | No | Set the character used to quote fields in the CSV file. Defaults to `"`. |
 | `syntax:escapechar=<char>` | No | Set the character used to escape the quote characters in the CSV file. Defaults to a backslash (`\`). |
 | `syntax:decimalchar=<char>` | No | Set the character used to represent the decimal point in the CSV file. Defaults to a period (`.`). |
 | `syntax:groupmark=<char>` | No | Set the character used to group digits in numbers. By default, group marks are not permitted in numbers. Set the group mark to the comma (`,`) to parse numbers such as `1,000.0`. |
+| `integration:provider=<provider>` | No | Set the cloud provider that hosts the file. May be one of `"azure"` or `"s3"`. Required for importing privately hosted files. Ignored when importing local files. |
+| `integration:region=<region>` | No | Set the region of S3 bucket containing the file. Required for importing privately hosted files from AWS S3. Ignored when importing local files or when `provider` is set to `"azure"`. |
+| `integration:credentials:<key>=<value>` | No | Set the credentials for the cloud provider.<br><br>Required keys for Azure:<br><br>- `azure_sas_token`<br><br>Required keys for AWS S3:<br><br>- `access_key_id`<br>- `secret_access_key`<br><br>Required for importing privately hosted cloud files. Ignored when importing local files. |
 
 <!-- markdownlint-enable no-inline-html -->
 
 ## Example
 
 Run `rai imports:snapshot` without any arguments to use the built-in CLI prompts to select and upload a file.
 After you select the model to use and the file to upload, you are asked to provide a resource name,
@@ -87,14 +91,30 @@
 
 ? Use this schema for transactions: Yes
 ▰▰▰▰ Snapshot for transactions created
 
 ---------------------------------------------------
 ```
 
+Pass a URL to the `--source` flag to import a remote file.
+The file _must_ be hosted with Azure or AWS S3.
+Note that pre-signed URLs are currently not supported.
+If the file is hosted privately, you must provide the `integration:provider` and `integration:credentials` arguments:
+
+```sh
+# Import a file hosted on Azure.
+$ rai imports:snapshot --source https://example.blob.core.windows.net/data/transactions.csv --model myModel --name transactions integration:provider=azure integration:credentials:azure_sas_token=<AZURE_SAS_TOKEN>
+
+# Import a file hosted on AWS S3.
+# Note that the integration:region argument is required.
+$ rai imports:snapshot --source https://example.s3.amazonaws.com/data/transactions.csv --model myModel --name transactions integration:provider=s3 integration:region=us-west-2 integration:credentials:access_key_id=<AWS_SECRET_KEY_ID> integration:credentials:secret_access_key=<AWS_SECRET_KEY>
+```
+
+If the file is hosted publicly, the `integration:*` arguments are not required.
+
 To change the default schema, pass additional command-line arguments of the form `schema:<column_name>=<type>`.
 For example, to use `string` for the `amount` column, pass the arg `schema:amount=string`.
 As usual, you are asked to verify the schema before the snapshot is uploaded:
 
 ```sh
 $ rai imports:snapshot --source data/transactions.csv --model myModel --name transactions schema:amount=string
 
@@ -114,14 +134,21 @@
 ▰▰▰▰ Snapshot for transactions created
 
 ---------------------------------------------------
 ```
 
 You may provide multiple `schema:*` arguments to customize the schema as needed.
 
+To specify the delimeter, quote character, and other parsing options, pass additional `syntax:*` arguments.
+For example, to use a tab character as the delimiter, pass the argument `syntax:delim=\t`:
+
+```sh
+$ rai imports:snapshot --source data/transactions.csv --model myModel --name transactions syntax:delim=\t
+```
+
 Once you create the snapshot, you may add objects from the file to your model in
 a [`model.read()`](../python/Model/read.md) context:
 
 ```python
 import relationalai as rai
 
 model = rai.Model("myModel")
```

### Comparing `relationalai-0.2.9/docs/api_reference/cli/imports_stream.md` & `relationalai-0.3.0/docs/api_reference/cli/imports_stream.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/profile_switch.md` & `relationalai-0.3.0/docs/api_reference/cli/profile_switch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/transactions_cancel.md` & `relationalai-0.3.0/docs/api_reference/cli/transactions_cancel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/transactions_get.md` & `relationalai-0.3.0/docs/api_reference/cli/transactions_get.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/transactions_list.md` & `relationalai-0.3.0/docs/api_reference/cli/transactions_list.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/cli/version.md` & `relationalai-0.3.0/docs/api_reference/cli/version.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```sh
 $ rai version
 
 ---------------------------------------------------
  
                                           
   RelationalAI   0.2.5 → 0.2.7      
-  Rai-sdk        0.7.4              
+  Rai-sdk        0.7.5              
   Python         3.12.1             
   App            2024.5.8-a1b26cea  
                                     
 
 ---------------------------------------------------
 ```
```

### Comparing `relationalai-0.2.9/docs/api_reference/configuration/README.md` & `relationalai-0.3.0/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Expression.md` & `relationalai-0.3.0/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Property.md` & `relationalai-0.3.0/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/README.md` & `relationalai-0.3.0/docs/api_reference/python/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # RelationalAI Python API Reference
 
-This document outlines all of the functions, classes, and methods
-in the public RelationalAI Python API.
+This document outlines all of the functions, classes, and methods in the public RelationalAI Python API.
 
 ## `relationalai`
 
 The `relationalai` namespace contains classes for fundamental concepts, including the
 [`Model`](./Model/README.md), [`Type`](./Type/README.md), [`Context`](./Context/README.md), and [`Producer`](./Producer/README.md) classes.
 
 - [`Context`](./Context/README.md)
@@ -16,19 +15,22 @@
   - [`Context.results`](./Context/results.md)
 - [`ContextSelect`](./ContextSelect/README.md)
   - [`ContextSelect.__call__()`](./ContextSelect/call__.md)
   - [`ContextSelect.__getattribute__()`](./ContextSelect/getattribute__.md)
   - [`ContextSelect.add()`](./ContextSelect/add.md)
 - [`Expression`](./Expression.md)
 - [`Instance`](./Instance/README.md)
-  - [`Instance.persist()`](./Instance/persist.md)
   - [`Instance.set()`](./Instance/set.md)
-  - [`Instance.unpersist()`](./Instance/unpersist.md)
 - [`InstanceProperty`](./InstanceProperty/README.md)
+  - [`InstanceProperty.add()`](./InstanceProperty/add.md)
+  - [`InstanceProperty.choose()`](./InstanceProperty/choose.md)
+  - [`InstanceProperty.extend()`](./InstanceProperty/extend.md)
+  - [`InstanceProperty.in_()`](./InstanceProperty/in_.md)
   - [`InstanceProperty.or_()`](./InstanceProperty/or_.md)
+  - [`InstanceProperty.set()`](./InstanceProperty/set.md)
 - [`Model`](./Model/README.md)
   - [`Model.found()`](./Model/found.md)
   - [`Model.name`](./Model/name.md)
   - [`Model.not_found()`](./Model/not_found.md)
   - [`Model.ordered_choice()`](./Model/ordered_choice.md)
   - [`Model.query()`](./Model/query.md)
   - [`Model.read()`](./Model/read.md)
@@ -43,29 +45,32 @@
   - [`Producer.__exit__()`](./Producer/exit__.md)
   - [`Producer.__floordiv__()`](./Producer/floordiv__.md)
   - [`Producer.__ge__()`](./Producer/ge__.md)
   - [`Producer.__getattribute__()`](./Producer/getattribute__.md)
   - [`Producer.__gt__()`](./Producer/gt__.md)
   - [`Producer.__le__()`](./Producer/le__.md)
   - [`Producer.__lt__()`](./Producer/lt__.md)
+  - [`Producer.__mod__()`](./Producer/mod__.md)
   - [`Producer.__mul__()`](./Producer/mul__.md)
   - [`Producer.__ne__()`](./Producer/ne__.md)
   - [`Producer.__radd__()`](./Producer/radd__.md)
   - [`Producer.__rfloordiv__()`](./Producer/rfloordiv__.md)
+  - [`Producer.__rmod__()`](./Producer/rmod__.md)
   - [`Producer.__rmul__()`](./Producer/rmul__.md)
   - [`Producer.__rsub__()`](./Producer/rsub__.md)
   - [`Producer.__rtruediv__()`](./Producer/rtruediv__.md)
   - [`Producer.__sub__()`](./Producer/sub__.md)
   - [`Producer.__truediv__()`](./Producer/truediv__.md)
 - [`Property`](./Property.md)
 - [`Type`](./Type/README.md)
   - [`Type.__call__()`](./Type/call__.md)
   - [`Type.__or__()`](./Type/or__.md)
   - [`Type.add()`](./Type/add.md)
   - [`Type.extend()`](./Type/extend.md)
+  - [`Type.known_properties()`](./Type/known_properties.md)
   - [`Type.model`](./Type/model.md)
   - [`Type.name`](./Type/name.md)
 
 ## [`relationalai.std`](./std/README.md)
 
 The `relationalai.std` namespace contains the RelationalAI Query Builder Standard Library.
 This includes functions for performing [aggregations](./std/aggregates/)
@@ -88,15 +93,15 @@
 
 - [`graphs.Compute`](./std/graphs/Compute/README.md)
   - [`graphs.Compute.adamic_adar()`](./std/graphs/Compute/adamic_adar.md)
   - [`graphs.Compute.avg_clustering_coefficient()`](./std/graphs/Compute/avg_clustering_coefficient.md)
   - [`graphs.Compute.avg_degree()`](./std/graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./std/graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./std/graphs/Compute/avg_outdegree.md)
-  - [`graphs.Compute.betweenness_centrality()`](./std/graphs/Compute/betweeness_centrality.md)
+  - [`graphs.Compute.betweenness_centrality()`](./std/graphs/Compute/betweenness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./std/graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./std/graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.degree_centrality()`](./std/graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.degree()`](./std/graphs/Compute/degree.md)
   - [`graphs.Compute.diameter_range()`](./std/graphs/Compute/diameter_range.md)
   - [`graphs.Compute.distance()`](./std/graphs/Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./std/graphs/Compute/eigenvector_centrality.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Context/README.md` & `relationalai-0.3.0/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Context/enter__.md` & `relationalai-0.3.0/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Context/exit__.md` & `relationalai-0.3.0/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Context/iter__.md` & `relationalai-0.3.0/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Context/model.md` & `relationalai-0.3.0/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Context/results.md` & `relationalai-0.3.0/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.3.0/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.3.0/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.3.0/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.3.0/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Instance/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/max.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,79 @@
-<!-- markdownlint-disable MD024 -->
-
-# `relationalai.Instance`
-
-Instances are [producers](../Producer/README.md) that produce the internal IDs of objects in a model.
-You create instances by calling a [`Type`](../Type/README.md) object or the [`relationalai.std.Vars()`](../std/Vars.md) method,
-which both return an instance of the `Instance` class.
+# `relationalai.std.aggregates.max()`
 
 ```python
-class relationalai.Instance(model: Model)
+relationalai.std.aggregates.max(*args: Producer, per: Optional[List[Producer]]) -> Expression
 ```
 
-`Instance` is a subclass of [`Producer`](../Producer/README.md).
+Creates an [`Expression`](../../Expression.md) object that produces the maximum of
+the values produced by one or more [`Producer`](../../Producer/README.md) objects.
+Pass a list of `Producer` objects to the optional `per` parameter to group values and compute the maximum value per group.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `model` | [`Model`](../Model/README.md) | The model in which the instance is created. |
+| `*args` | [`Producer`](../../Producer/README.md) | One or more [`Producer`](../../Producer/README.md) objects. |
 
-## Methods
+## Returns
 
-- [`Instance.persist()`](./persist.md)
-- [`Instance.set()`](./set.md)
-- [`Instance.unpersist()`](./unpersist.md)
+An [`Expression`](../../Expression.md) object.
 
 ## Example
 
-Use [`Type`](../Type/README.md) objects and [`Model`](../Model/README.md) methods to create an `Instance` object
-rather than constructing one directly:
-
 ```python
 import relationalai as rai
+from relationalai.std import aggregates
 
 model = rai.Model("people")
 Person = model.Type("Person")
 
 with model.rule():
-    # The `Type.add()` method returns an `Instance` object.
-    kermit = Person.add(name="Kermit")
-    # `Instance` objects have a `.set()` method for setting properties.
-    kermit.set(favorite_color="green")
+    Person.add(name="Joe", age=39)
+    Person.add(name="Jane", age=40)
+
+with model.query() as select:
+    person = Person()
+    max_age = aggregates.max(person.age)
+    response = select(max_age)
+
+print(response.results)
+# Output:
+#    result
+# 0      40
+```
+
+To group values and compute the maximum for each group,
+pass one or more `Producer` objects to the optional `per` parameter as a list.
+In the following example, the `person` object is passed to `per` to compute the maximum age of a person's friends:
+
+```python
+import relationalai as rai
+from relationalai.std import aggregates
+
+model = rai.Model("friends")
+Person = model.Type("Person")
+
+with model.rule():
+    joe = Person.add(name="Joe", age=39)
+    jane = Person.add(name="Jane", age=40)
+    john = Person.add(name="John", age=41)
+    joe.set(friend=jane).set(friend=john)
+    jane.set(friend=joe)
+    john.set(friend=joe)
 
 with model.query() as select:
-    # Calling a `Type` object returns an `Instance` object.
     person = Person()
-    response = select(person.name)
+    max_friend_age = aggregates.max(person.friend.age, per=[person])
+    response = select(person.name, max_friend_age)
 
 print(response.results)
 # Output:
-#      name
-# 0  Kermit
+#    name  result
+# 0  Jane      39
+# 1   Joe      41
+# 2  John      39
 ```
 
-The following all return `Instance` objects:
+## See Also
 
-- [`relationalai.Type.add()`](../Type/add.md)
-- [`relationalai.Type.__call__()`](../Type/call__.md)
-- [`relationalal.std.Vars()`](../std/Vars.md)
+[`avg()`](./avg.md) and [`min()`](./min.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/lt__.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-# `relationalai.InstanceProperty.or_()`
+# `relationalai.Producer.__lt__()`
 
 ```python
-relationalai.InstanceProperty.or_(other: Any) -> InstanceProperty
+relationalai.Producer.__lt__(other: Any) -> Expression
 ```
 
-Returns an [`InstanceProperty`](./README.md) that produces the same values as the original `InstanceProperty` as well
-the default value `other` for objects on which the property is not set.
+Returns an [`Expression`](../Expression.md) that restricts [`Producer`](./README.md) to values strictly less than `other`.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `other` | `Any` | The default property value. |
+| `other` | `Any` | A numeric value or another `Producer` object. |
 
 ## Returns
 
-An [`InstanceProperty`](./README.md) object.
+An [`Expression`](../Expression.md) object.
 
 ## Example
 
+The `Producer.__lt__()` method is called when you use the `<` operator with a `Producer` object:
 
 ```python
 import relationalai as rai
 
 model = rai.Model("people")
 Person = model.Type("Person")
 
 with model.rule():
     Person.add(name="Fred", age=39)
-    Person.add(name="Wilma")
+    Person.add(name="Wilma", age=36)
 
 with model.query() as select:
     person = Person()
-    age = person.age.or_(-1)  # Produce -1 if the person has no age property.
-    response = select(person.name, age)
+    # Restrict `person.age` to values that are strictly less
+    # than 39. `person.age` returns an `InstanceProperty` object,
+    # which is also a `Producer` object.
+    person.age < 39
+    response = select(person.name, person.age)
 
 print(response.results)
 # Output:
 #     name  age
-# 0   Fred   39
-# 1  Wilma   -1
-```
-
-Note that you may put the call to `.or_()` inside of `select` if you wish:
-
-```python
-with model.query() as select:
-    person = Person()
-    response = select(person.name, person.age.or_(-1))
+# 0  Wilma   36
 ```
 
-Contrast that to the same query without `.or_()`, which does not return a row for Wilma:
+You may use `<` with two `Producer` objects:
 
 ```python
 with model.query() as select:
-    person = Person()
-    response = select(person.name, person.age)
+    person1, person2 = Person(), Person()
+    person1.age < person2.age
+    response = select(person1.name, person2.name)
 
 print(response.results)
 # Output:
-#     name  age
-# 0   Fred   39
+#     name  name2
+# 0  Wilma  Fred
 ```
+
+## See Also
+
+[`Producer.__gt__()`](./gt__.md),
+[`Producer.__ge__()`](./ge__.md),
+and [`Producer.__le__()`](./le__.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/Type.md` & `relationalai-0.3.0/docs/api_reference/python/Model/Type.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 Creates a new [Type](../Type/README.md) in the model.
 
 #### Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `name` | `str` | The name of the type. Type names must begin with a Unicode letter or an underscore followed by one or more Unicode letters, underscores, or numbers. |
+| `name` | `str` | The name of the type. Must begin with a Unicode letter or an underscore followed by one or more Unicode letters, underscores, or numbers. |
 
 #### Returns
 
 A [`Type`](../Type/README.md) object.
 
 #### Example
 
 ```python
 import relationalai as rai
 
+# Create a model named "people" with a Person type.
 model = rai.Model("people")
-
 Person = model.Type("Person")
 ```
 
 #### See Also
 
 [`Type`](../Type/README.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/found.md` & `relationalai-0.3.0/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/not_found.md` & `relationalai-0.3.0/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.3.0/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/query.md` & `relationalai-0.3.0/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/read.md` & `relationalai-0.3.0/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/rule.md` & `relationalai-0.3.0/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/scope.md` & `relationalai-0.3.0/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Model/union.md` & `relationalai-0.3.0/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/README.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/pow__.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,79 @@
-<!-- markdownlint-disable MD024 -->
-
-# Producer
-
-`Producer` objects represent an unknown value in a context.
-When a [query](../Model/query.md) context is evaluated,
-the values matching the context's constraints are produced.
-The `Producer` class is the base class for different types of producers,
-such as [`Instance`](../Instance/README.md) objects, which produce the IDs of objects in your model,
-or [`InstanceProperty`](../InstanceProperty/README.md) objects, which produce object property values.
+# `relationalai.Producer.__pow__()`
 
 ```python
-class Producer(model: Model)
+Producer.__pow__(exp: Any) -> Expression
 ```
 
+Returns an [`Expression`](../Expression.md) the produces the values of the [`Producer`](./README.md) to the power of `exp`.
+
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `model` | [`Model`](../Model/README.md) | The model in which the producer is created. |
+| `exp` | `Any` | A numeric value or another `Producer` object. |
 
-## Methods
+## Returns
 
-- [`Producer.__add__()`](./add__.md)
-- [`Producer.__enter__()`](./enter__.md)
-- [`Producer.__eq__()`](./eq__.md)
-- [`Producer.__exit__()`](./exit__.md)
-- [`Producer.__floordiv__()`](./floordiv__.md)
-- [`Producer.__ge__()`](./ge__.md)
-- [`Producer.__getattribute__()`](./getattribute__.md)
-- [`Producer.__gt__()`](./gt__.md)
-- [`Producer.__le__()`](./le__.md)
-- [`Producer.__lt__()`](./lt__.md)
-- [`Producer.__mul__()`](./mul__.md)
-- [`Producer.__ne__()`](./ne__.md)
-- [`Producer.__pow__()`](./pow__.md),
-- [`Producer.__radd__()`](./radd__.md)
-- [`Producer.__rfloordiv__()`](./rfloordiv__.md)
-- [`Producer.__rmul__()`](./rmul__.md)
-- [`Producer.__rpow__()`](./rpow__.md),
-- [`Producer.__rsub__()`](./rsub__.md)
-- [`Producer.__rtruediv__()`](./rtruediv__.md)
-- [`Producer.__sub__()`](./sub__.md)
-- [`Producer.__truediv__()`](./truediv__.md)
+An [`Expression`](../Expression.md) object.
 
 ## Example
 
-`Producer` objects show up all over the place:
+You may raise a `Producer` object by a number literal:
 
 ```python
 import relationalai as rai
 
 model = rai.Model("people")
 Person = model.Type("Person")
 
 with model.rule():
-    # `Type.add()` returns an `Instance` object, which is a `Producer`.
-    fred = Person.add(name="Fred", age=39)
-    fred.set(favorite_color="green")
+    Person.add(name="Fred", age=39)
+    Person.add(name="Wilma", age=36)
 
 with model.query() as select:
-    # Calling a Type returns an `Instance`.
     person = Person()
+    # `person.age` returns an `InstanceProperty` object,
+    # which is also a `Producer` object.
+    square_age = person.age ** 2
+    response = select(person.name, square_age)
 
-    # Accessing a property returns an `InstanceProperty` object,
-    # which is a `Producer`.
-    name = person.name
-    age = person.age
+print(response.results)
+# Output:
+#     name  result
+# 0   Fred    1521
+# 1  Wilma    1296
+```
 
-    # Operators return an `Expression` object, which is a `Producer`.
-    age > 30
+You may also use a `Producer` as the exponent:
 
-    response = select(name, age)
+```python
+import relationalai as rai
+
+model = rai.Model("people")
+Person = model.Type("Person")
+
+with model.rule():
+    Person.add(name="Fred", age=39)
+    Person.add(name="Wilma", age=36)
+
+with model.query() as select:
+    person = Person()
+    val = 1.01 ** person.age  # A producer can be the exponent.
+    response = select(person.name, val)
 
 print(response.results)
 # Output:
-#    name  age
-# 0  Fred   39
+#     name    result
+# 0   Fred  1.474123
+# 1  Wilma  1.430769
 ```
 
-The following classes are all subclasses of `Producer`:
+## See Also
+
+[`Producer.__add__()`](./add__.md),
+[`Producer.__sub__()`](./sub__.md),
+[`Producer.__mul__()`](./mul__.md),
+[`Producer.__truediv__()`](./truediv__.md),
+[`Producer.__floordiv__()`](./floordiv__.md),
+and [`Producer.__mod__()`](./mod__.md).
 
-- [`Instance`](../Instance/README.md)
-- [`InstanceProperty`](../InstanceProperty/README.md)
-- [`Expression`](../Expression.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/add__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/add__.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,11 +68,13 @@
 #     name      v
 # 0   Fred  300.0
 # 1  Wilma  400.0
 ```
 
 ## See Also
 
+[`Producer.__sub__()`](./sub__.md),
 [`Producer.__mul__()`](./mul__.md),
+[`Producer.__truediv__()`](./truediv__.md),
+[`Producer.__floordiv__()`](./floordiv__.md),
 [`Producer.__pow__()`](./pow__.md),
-[`Producer.__sub__()`](./sub__.md),
-and [`Producer.__truediv__()`](./truediv__.md).
+and [`Producer.__mod__()`](./mod__.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/floordiv__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/floordiv__.md`

 * *Files 16% similar despite different names*

```diff
@@ -57,8 +57,13 @@
 #    result
 # 0   -62.0
 # 1    61.0
 ```
 
 ## See Also
 
-[`__truediv__()`](./truediv__.md) and [`std.math.trunc_divide`](../std/math/trunc_divide.md).
+[`Producer.__add__()`](./add__.md),
+[`Producer.__sub__()`](./sub__.md),
+[`Producer.__mul__()`](./mul__.md),
+[`Producer.__truediv__()`](./truediv__.md),
+[`Producer.__pow__()`](./pow__.md),
+and [`Producer.__mod__()`](./mod__.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/le__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/ne__.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# `relationalai.Producer.__lt__()`
+# `relationalai.Producer.__ne__()`
 
 ```python
-relationalai.Producer.__lt__(other: Any) -> Expression
+relationalai.Producer.__ne__(other: Any) -> Expression
 ```
 
-Returns an [`Expression`](../Expression.md) that restricts [`Producer`](./README.md) to values strictly less than `other`.
+Returns an [`Expression`](../Expression.md) that restricts [`Producer`](./README.md) to values not equal to `other`.
 
-## Parameters
+#### Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
 | `other` | `Any` | A numeric value or another `Producer` object. |
 
-## Returns
+#### Returns
 
 An [`Expression`](../Expression.md) object.
 
-## Example
+#### Example
 
-The `Producer.__lt__()` method is called when you use the `<` operator with a `Producer` object:
+The `Producer.__ne__()` method is called when you use the `!=` operator with a `Producer` object:
 
 ```python
 import relationalai as rai
 
 model = rai.Model("people")
 Person = model.Type("Person")
 
 with model.rule():
     Person.add(name="Fred", age=39)
     Person.add(name="Wilma", age=36)
 
 with model.query() as select:
     person = Person()
-    # Restrict `person.age` to values that are strictly less
-    # than 39. `person.age` returns an `InstanceProperty` object,
+    # Restrict `person.age` to values that are equal to 36.
+    # `person.age` returns an `InstanceProperty` object,
     # which is also a `Producer` object.
-    person.age < 39
+    person.age != 36
     response = select(person.name, person.age)
 
 print(response.results)
 # Output:
-#     name  age
-# 0  Wilma   36
+#    name  age
+# 0  Fred   39
 ```
 
-You may use `<` with two `Producer` objects:
+You may use `!=` with two `Producer` objects:
 
 ```python
 with model.query() as select:
     person1, person2 = Person(), Person()
-    person1.age < person2.age
+    person1.age != person2.age
     response = select(person1.name, person2.name)
 
 print(response.results)
 # Output:
 #     name  name2
-# 0  Wilma  Fred
+#     name  name2
+# 0   Fred  Wilma
+# 1  Wilma   Fred
 ```
 
-## See Also
+#### See Also
 
-[`Producer.__gt__()`](./gt__.md),
-[`Producer.__ge__()`](./ge__.md),
-and [`Producer.__le__()`](./le__.md).
+[`Producer.__eq__()`](./eq__.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/mul__.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,10 +68,12 @@
 # 0   Fred   600.0
 # 1  Wilma  1200.0
 ```
 
 ## See Also
 
 [`Producer.__add__()`](./add__.md),
-[`Producer.__pow__()`](./pow__.md),
 [`Producer.__sub__()`](./sub__.md),
-and [`Producer.__truediv__()`](./truediv__.md).
+[`Producer.__truediv__()`](./truediv__.md),
+[`Producer.__floordiv__()`](./floordiv__.md),
+[`Producer.__pow__()`](./pow__.md),
+and [`Producer.__mod__()`](./mod__.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/asin.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,75 @@
-# `relationalai.Producer.__ne__()`
+# `relationalai.std.math.asin()`
 
 ```python
-relationalai.Producer.__ne__(other: Any) -> Expression
+relationalai.std.math.asin(number: Number | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../Expression.md) that restricts [`Producer`](./README.md) to values not equal to `other`.
+Returns an [`Expression`](../../Expression.md) object that produces the arcsine of `number` radians.
 
-#### Parameters
+## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :------ |
-| `other` | `Any` | A numeric value or another `Producer` object. |
+| :--- | :--- | :--------- |
+| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the arcsine of. |
 
-#### Returns
+## Returns
 
-An [`Expression`](../Expression.md) object.
+An [`Expression`](../../Expression.md) object that produces `float` values.
 
-#### Example
+## Example
 
-The `Producer.__ne__()` method is called when you use the `!=` operator with a `Producer` object:
+`asin()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
 
 ```python
 import relationalai as rai
+from relationalai.std import alias
+from relationalai.std.math import asin
 
+# Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
+# Add a person to the model.
 with model.rule():
-    Person.add(name="Fred", age=39)
-    Person.add(name="Wilma", age=36)
+    Person.add(name="Alice", age=3, height_m=0.95)
 
+# asin() works with numeric producers, such as a person's height property.
+# Inputs are assumed to be in radians.
 with model.query() as select:
     person = Person()
-    # Restrict `person.age` to values that are equal to 36.
-    # `person.age` returns an `InstanceProperty` object,
-    # which is also a `Producer` object.
-    person.age != 36
-    response = select(person.name, person.age)
+    response = select(person.name, alias(asin(person.height_m), "asin_height"))
 
 print(response.results)
 # Output:
-#    name  age
-# 0  Fred   39
+#     name  asin_height
+# 0  Alice     1.253236
+
+# asin() also works with Python number objects.
+with model.query() as select:
+    response = select(asin(0))
+
+print(response.results)
+# Output:
+#           v
+# 0  1.570796
 ```
 
-You may use `!=` with two `Producer` objects:
+The input to `asin()` must be in the range -1 to 1, inclusive.
+If the input is outside this range,
+the [query](../../Model/query.md) or [rule](../../Model/rule.md) will be impossible to satisfy:
 
 ```python
 with model.query() as select:
-    person1, person2 = Person(), Person()
-    person1.age != person2.age
-    response = select(person1.name, person2.name)
+    person = Person()
+    response = select(person.name, alias(asin(person.age), "asin_age"))
 
 print(response.results)
 # Output:
-#     name  name2
-#     name  name2
-# 0   Fred  Wilma
-# 1  Wilma   Fred
+# Empty DataFrame
+# Columns: []
+# Index: []
 ```
 
-#### See Also
+## See Also
 
-[`Producer.__eq__()`](./eq__.md)
+[`sin()`](./sin.md), [`acos()`](./acos.md), and [`atan()`](./atan.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/cos.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,59 @@
-# `relationalai.Producer.__pow__()`
+# `relationalai.std.math.cos()`
 
 ```python
-Producer.__pow__(exp: Any) -> Expression
+relationalai.std.math.cos(number: Number | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../Expression.md) the produces the values of the [`Producer`](./README.md) to the power of `exp`.
+Returns an [`Expression`](../../Expression.md) object that produces the cosine of `number` radians.
 
 ## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :------ |
-| `exp` | `Any` | A numeric value or another `Producer` object. |
+| :--- | :--- | :--------- |
+| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the cosine of. |
 
 ## Returns
 
-An [`Expression`](../Expression.md) object.
+An [`Expression`](../../Expression.md) object that produces `float` values.
 
 ## Example
 
-You may raise a `Producer` object by a number literal:
+`cos()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
 
 ```python
 import relationalai as rai
+from relationalai.std import alias
+from relationalai.std.math import cos
 
+# Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
+# Add a person to the model.
 with model.rule():
-    Person.add(name="Fred", age=39)
-    Person.add(name="Wilma", age=36)
+    Person.add(name="Alice", age=30)
 
+# cos() works with numeric producers, such as a person's age property.
+# Inputs are assumed to be in radians.
 with model.query() as select:
     person = Person()
-    # `person.age` returns an `InstanceProperty` object,
-    # which is also a `Producer` object.
-    square_age = person.age ** 2
-    response = select(person.name, square_age)
+    response = select(person.name, alias(cos(person.age), "cos_age"))
 
 print(response.results)
 # Output:
-#     name  result
-# 0   Fred    1521
-# 1  Wilma    1296
-```
-
-You may also use a `Producer` as the exponent:
-
-```python
-import relationalai as rai
-
-model = rai.Model("people")
-Person = model.Type("Person")
-
-with model.rule():
-    Person.add(name="Fred", age=39)
-    Person.add(name="Wilma", age=36)
+#     name   cos_age
+# 0  Alice  0.154251
 
+# cos() also works with Python number objects.
 with model.query() as select:
-    person = Person()
-    val = 1.01 ** person.age  # A producer can be the exponent.
-    response = select(person.name, val)
+    response = select(cos(0))
 
 print(response.results)
 # Output:
-#     name    result
-# 0   Fred  1.474123
-# 1  Wilma  1.430769
+#      v
+# 0  1.0
 ```
 
 ## See Also
 
-[`Producer.__add__()`](./add__.md),
-[`Producer.__mul__()`](./mul__.md),
-[`Producer.__sub__()`](./sub__.md),
-and [`Producer.__truediv__()`](./truediv__.md).
+[`acos()`](./acos.md), [`sin()`](./sin.md), and [`tan()`](./tan.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/sub__.md`

 * *Files 6% similar despite different names*

```diff
@@ -69,9 +69,11 @@
 # 1  Wilma  26
 ```
 
 ## See Also
 
 [`Producer.__add__()`](./add__.md),
 [`Producer.__mul__()`](./mul__.md),
+[`Producer.__truediv__()`](./truediv__.md),
+[`Producer.__floordiv__()`](./floordiv__.md),
 [`Producer.__pow__()`](./pow__.md),
-and [`Producer.__truediv__()`](./truediv__.md).
+and [`Producer.__mod__()`](./mod__.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.3.0/docs/api_reference/python/Producer/truediv__.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,10 +69,12 @@
 # 0   Fred  0.2
 # 1  Wilma  0.6
 ```
 
 ## See Also
 
 [`Producer.__add__()`](./add__.md),
+[`Producer.__sub__()`](./sub__.md),
 [`Producer.__mul__()`](./mul__.md),
+[`Producer.__floordiv__()`](./floordiv__.md),
 [`Producer.__pow__()`](./pow__.md),
-and [`Producer.__sub__()`](./sub__.md).
+and [`Producer.__mod__()`](./mod__.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/Type/add.md` & `relationalai-0.3.0/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Type/call__.md` & `relationalai-0.3.0/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Type/extend.md` & `relationalai-0.3.0/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/Type/or__.md` & `relationalai-0.3.0/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/README.md` & `relationalai-0.3.0/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # `relationalai.clients.Snowflake.SnowflakeTable`
 
-The `SnowflakeTable` class represents an existing table in your Snowflake account.
-You create `SnowflakeTable` instances using a [`Snowflake`](../Snowflake.md) object.
+The `SnowflakeTable` class is a subclass of [`Type`](../../../Type/README.md)
+that represents objects imported from a Snowflake table.
 
 ```python
-class relationalai.clients.snowflake.SnowflakeTable()
+class relationalai.clients.snowflake.SnowflakeTable(Type)
 ```
 
+`SnowflakeTable` objects are not created directly.
+You create `SnowflakeTable` instances using a [`Snowflake`](../Snowflake.md) object.
+See the [Example](#example) section for details.
+
 > [!IMPORTANT]
-> You must stream the contents of a Snowflake table to your [model](../../../Model/README.md)
-> before you can access the table with RelationalAI.
-> Snowflake admins can set up streams using the [SQL library](../../../../sql/README.md)
-> or the CLI's [`imports:stream`](../../../../cli/README.md#importsstream) command.
+> Before you can access a Snowflake table in a model,
+> you must import the table using the [`rai imports:stream`](../../cli/imports_stream.md) CLI command
+> or the [RelationalAI SQL Library](../../../../sql/README.md).
+> Your Snowflake user must have the correct priveledges to create a stream on the table.
+> Contact your Snowflake administrator if you need help importing a Snowflake table.
 
 ## Parameters
 
 None.
 
 ## Methods
 
 - [`SnowflakeTable.describe()`](./describe.md)
+- [`SnowflakeTable.fqname()`](./fqname.md)
+- [`SnowflakeTable.namespace()`](./namespace.md)
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.clients.snowflake import Snowflake
 
@@ -39,24 +46,28 @@
 # For instance, this query gets the names and ages of all people.
 with model.query() as select:
     person = Person()
     response = (person.name, person.age)
 ```
 
 The `Person` object returned by `sf.sandbox.public.people` is a [`SnowflakeTable`](./SnowflakeTable.md) instance.
-The table is presumed to be in [third normal form](https://en.wikipedia.org/wiki/Third_normal_form).
-
-Think of `SnowflakeTable` as a read-only [`Type`](../../Type/call__.md).
-Although you may query a `SnowflakeTable` as if it were a `Type` object,
-you can't add objects to a table like you can using [`Type.add()`](../../Type/add.md).
-
 Property names, such as `age`, come from the table's column names and are case-insensitive.
 For example, if the column in the table is named `AGE` in all caps,
 then `person.AGE` and `person.age` both refer to the same column.
 
+You can view all of the known properties of a `SnowflakeTable` object,
+including properties derived from the table's columns,
+using the [`.known_properties()`](../../../Type/known_properties.md) method:
+
+```python
+print(Person.known_properties())
+# Output:
+# ['id', 'name', 'age']
+```
+
 Use the [`SnowflakeTable.describe()`](./SnowflakeTable/describe.md) method to describe table columns,
 such as which column serves as the [primary key](./PrimaryKey.md):
 
 ```python
 import relationalai as rai
 from relationalai.clients.snowflake import Snowflake, PrimaryKey
 
@@ -65,13 +76,20 @@
 
 Person = sf.sandbox.public.people
 # Set the `id` column as the primary key.
 Person.describe(id=PrimaryKey)
 ```
 
 Multiple primary key columns are supported.
+
+Primary keys are automatically detected from the table's Schema in Snowflake,
+provided the table has a primary key constraint.
+If the table does not have a primary key constraint,
+then `.describe()` may be used to manually designate a primary key for the model to use.
+Calling describe does not alter the table's schema in Snowflake.
+
 You may also define foreign key relationships.
 See [`SnowflakeTable.describe()`](./SnowflakeTable/describe.md) for more details.
 
 ## See Also
 
 [`PrimaryKey`](./PrimaryKey.md) and [`Snowflake`](../Snowflake.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # `relationalai.clients.snowflake.SnowflakeTable.fqname()`
 
 ```python
-relationalai.clients.snowflake.SnowflakeTable.namespace() -> str
+relationalai.clients.snowflake.SnowflakeTable.fqname() -> str
 ```
 
 Returns the [fully-qualified](https://docs.snowflake.com/en/sql-reference/name-resolution) Snowflake table name
 as a string of the form `"<db_name>.<schema_name>.<table_name>"`.
 
 ## Parameters
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.3.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 - [`graphs.Compute`](./graphs/Compute/README.md)
   - [`graphs.Compute.adamic_adar()`](./graphs/Compute/adamic_adar.md)
   - [`graphs.Compute.avg_clustering_coefficient()`](./graphs/Compute/avg_clustering_coefficient.md)
   - [`graphs.Compute.avg_degree()`](./graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./graphs/Compute/avg_outdegree.md)
-  - [`graphs.Compute.betweenness_centrality()`](./graphs/Compute/betweeness_centrality.md)
+  - [`graphs.Compute.betweenness_centrality()`](./graphs/Compute/betweenness_centrality.md)
   - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.degree_centrality()`](./graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.degree()`](./graphs/Compute/degree.md)
   - [`graphs.Compute.diameter_range()`](./graphs/Compute/diameter_range.md)
   - [`graphs.Compute.distance()`](./graphs/Compute/distance.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/Vars.md` & `relationalai-0.3.0/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/alias.md` & `relationalai-0.3.0/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/min.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# `relationalai.std.aggregates.max()`
+# `relationalai.std.aggregates.min()`
 
 ```python
-relationalai.std.aggregates.max(*args: Producer, per: Optional[List[Producer]]) -> Expression
+relationalai.std.aggregates.min(*args: Producer, per: Optional[List[Producer]]) -> Expression
 ```
 
-Creates an [`Expression`](../../Expression.md) object that produces the maximum of
+Creates an [`Expression`](../../Expression.md) object that produces the minimum of
 the values produced by one or more [`Producer`](../../Producer/README.md) objects.
-Pass a list of `Producer` objects to the optional `per` parameter to group values and compute the maximum value per group.
+Pass a list of `Producer` objects to the optional `per` parameter to group values and compute the minimum value per group.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
 | `*args` | [`Producer`](../../Producer/README.md) | One or more [`Producer`](../../Producer/README.md) objects. |
 
@@ -29,26 +29,26 @@
 
 with model.rule():
     Person.add(name="Joe", age=39)
     Person.add(name="Jane", age=40)
 
 with model.query() as select:
     person = Person()
-    max_age = aggregates.max(person.age)
-    response = select(max_age)
+    min_age = aggregates.min(person.age)
+    response = select(min_age)
 
 print(response.results)
 # Output:
 #    result
-# 0      40
+# 0      39
 ```
 
-To group values and compute the maximum for each group,
+To group values and compute the minimum for each group,
 pass one or more `Producer` objects to the optional `per` parameter as a list.
-In the following example, the `person` object is passed to `per` to compute the maximum age of a person's friends:
+In the following example, the `person` object is passed to `per` to compute the minimum age of a person's friends:
 
 ```python
 import relationalai as rai
 from relationalai.std import aggregates
 
 model = rai.Model("friends")
 Person = model.Type("Person")
@@ -59,21 +59,21 @@
     john = Person.add(name="John", age=41)
     joe.set(friend=jane).set(friend=john)
     jane.set(friend=joe)
     john.set(friend=joe)
 
 with model.query() as select:
     person = Person()
-    max_friend_age = aggregates.max(person.friend.age, per=[person])
-    response = select(person.name, max_friend_age)
+    min_friend_age = aggregates.min(person.friend.age, per=[person])
+    response = select(person.name, min_friend_age)
 
 print(response.results)
 # Output:
 #    name  result
 # 0  Jane      39
-# 1   Joe      41
+# 1   Joe      40
 # 2  John      39
 ```
 
 ## See Also
 
-[`avg()`](./avg.md) and [`min()`](./min.md).
+[`avg()`](./avg.md) and [`max()`](./max.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/sum.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# `relationalai.std.aggregates.min()`
+# `relationalai.std.aggregates.sum()`
 
 ```python
-relationalai.std.aggregates.min(*args: Producer, per: Optional[List[Producer]]) -> Expression
+relationalai.std.aggregates.sum(*args: Producer, per: Optional[List[Producer]]) -> Expression
 ```
 
-Creates an [`Expression`](../../Expression.md) object that produces the minimum of
-the values produced by one or more [`Producer`](../../Producer/README.md) objects.
-Pass a list of `Producer` objects to the optional `per` parameter to group values and compute the minimum value per group.
+Creates an [`Expression`](../../Expression.md) object that produces the sum of the values produced by a [`Producer`](../../Producer/README.md).
+Pass a list of one or more `Producer` objects to the optional `per` parameter to group values and compute the sum per group.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
 | `*args` | [`Producer`](../../Producer/README.md) | One or more [`Producer`](../../Producer/README.md) objects. |
 
@@ -24,56 +23,88 @@
 import relationalai as rai
 from relationalai.std import aggregates
 
 model = rai.Model("people")
 Person = model.Type("Person")
 
 with model.rule():
-    Person.add(name="Joe", age=39)
-    Person.add(name="Jane", age=40)
+    Person.add(name="Joe", age=41)
+    Person.add(name="Jane", age=39)
 
 with model.query() as select:
     person = Person()
-    min_age = aggregates.min(person.age)
-    response = select(min_age)
+    age_sum = aggregates.sum(person.age)
+    response = select(age_sum)
 
 print(response.results)
 # Output:
-#    result
-# 0      39
+#     v
+# 0  80
 ```
 
-To group values and compute the minimum for each group,
+`person.age` represents the _set_ of all ages in the model.
+If two people have the same age, you must pass the `person` instance,
+in addition to `person.age`, to `sum()` so that each person contributes to the sum:
+
+```python
+import relationalai as rai
+from relationalai.std import aggregates
+
+model = rai.Model("people")
+Person = model.Type("Person")
+
+with model.rule():
+    Person.add(name="Joe", age=41)
+    Person.add(name="Jane", age=39)
+    Person.add(name="John", age=41)
+
+with model.query() as select:
+    person = Person()
+    age_sum = aggregates.sum(person, person.age)
+    response = select(age_sum)
+
+print(response.results)
+# Output:
+#      v
+# 0  121
+```
+
+When the [query](../../Model/query.md) is evaluated,
+all pairs of `person` objects and their `age` properties are formed, and the sum of the age values is computed.
+You may pass any number of [`Producer`](../../Producer/README.md) objects to `sum()`.
+The aggregation occurs over the values produced by the last argument.
+
+To group values and compute the sum for each group,
 pass one or more `Producer` objects to the optional `per` parameter as a list.
-In the following example, the `person` object is passed to `per` to compute the minimum age of a person's friends:
+In the following example, the `person` object is passed to `per` to compute the sum of the ages of a person's friends:
 
 ```python
 import relationalai as rai
 from relationalai.std import aggregates
 
 model = rai.Model("friends")
 Person = model.Type("Person")
 
 with model.rule():
-    joe = Person.add(name="Joe", age=39)
-    jane = Person.add(name="Jane", age=40)
+    joe = Person.add(name="Joe", age=41)
+    jane = Person.add(name="Jane", age=39)
     john = Person.add(name="John", age=41)
     joe.set(friend=jane).set(friend=john)
     jane.set(friend=joe)
     john.set(friend=joe)
 
 with model.query() as select:
     person = Person()
-    min_friend_age = aggregates.min(person.friend.age, per=[person])
-    response = select(person.name, min_friend_age)
+    friend_age_sum = aggregates.sum(person.friend, person.friend.age, per=[person])
+    response = select(person.name, friend_age_sum)
 
 print(response.results)
 # Output:
-#    name  result
-# 0  Jane      39
-# 1   Joe      40
-# 2  John      39
+#    name   v
+# 0  Jane  41
+# 1   Joe  80
+# 2  John  41
 ```
 
 ## See Also
 
-[`avg()`](./avg.md) and [`max()`](./max.md).
+[`avg()`]() and [`count()`]().
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.3.0/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/acos.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,75 @@
-# `relationalai.std.aggregates.sum()`
+# `relationalai.std.math.acos()`
 
 ```python
-relationalai.std.aggregates.sum(*args: Producer, per: Optional[List[Producer]]) -> Expression
+relationalai.std.math.acos(number: Number | Producer) -> Expression
 ```
 
-Creates an [`Expression`](../../Expression.md) object that produces the sum of the values produced by a [`Producer`](../../Producer/README.md).
-Pass a list of one or more `Producer` objects to the optional `per` parameter to group values and compute the sum per group.
+Returns an [`Expression`](../../Expression.md) object that produces the arccosine of `number` radians.
 
 ## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :------ |
-| `*args` | [`Producer`](../../Producer/README.md) | One or more [`Producer`](../../Producer/README.md) objects. |
+| :--- | :--- | :--------- |
+| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the arccosine of. |
 
 ## Returns
 
-An [`Expression`](../../Expression.md) object.
+An [`Expression`](../../Expression.md) object that produces `float` values.
 
 ## Example
 
+`acos()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
+
 ```python
 import relationalai as rai
-from relationalai.std import aggregates
+from relationalai.std import alias
+from relationalai.std.math import acos
 
+# Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
+# Add a person to the model.
 with model.rule():
-    Person.add(name="Joe", age=41)
-    Person.add(name="Jane", age=39)
+    Person.add(name="Alice", age=3, height_m=0.95)
 
+# acos() works with numeric producers, such as a person's height property.
+# Inputs are assumed to be in radians.
 with model.query() as select:
     person = Person()
-    age_sum = aggregates.sum(person.age)
-    response = select(age_sum)
+    response = select(person.name, alias(acos(person.height_m), "acos_height"))
 
 print(response.results)
 # Output:
-#     v
-# 0  80
-```
-
-`person.age` represents the _set_ of all ages in the model.
-If two people have the same age, you must pass the `person` instance,
-in addition to `person.age`, to `sum()` so that each person contributes to the sum:
-
-```python
-import relationalai as rai
-from relationalai.std import aggregates
-
-model = rai.Model("people")
-Person = model.Type("Person")
-
-with model.rule():
-    Person.add(name="Joe", age=41)
-    Person.add(name="Jane", age=39)
-    Person.add(name="John", age=41)
+#     name  acos_height
+# 0  Alice      0.31756
 
+# acos() also works with Python number objects.
 with model.query() as select:
-    person = Person()
-    age_sum = aggregates.sum(person, person.age)
-    response = select(age_sum)
+    response = select(acos(0))
 
 print(response.results)
 # Output:
-#      v
-# 0  121
+#           v
+# 0  1.570796
 ```
 
-When the [query](../../Model/query.md) is evaluated,
-all pairs of `person` objects and their `age` properties are formed, and the sum of the age values is computed.
-You may pass any number of [`Producer`](../../Producer/README.md) objects to `sum()`.
-The aggregation occurs over the values produced by the last argument.
-
-To group values and compute the sum for each group,
-pass one or more `Producer` objects to the optional `per` parameter as a list.
-In the following example, the `person` object is passed to `per` to compute the sum of the ages of a person's friends:
+The input to `acos()` must be in the range -1 to 1, inclusive.
+If the input is outside this range,
+the [query](../../Model/query.md) or [rule](../../Model/rule.md) will be impossible to satisfy:
 
 ```python
-import relationalai as rai
-from relationalai.std import aggregates
-
-model = rai.Model("friends")
-Person = model.Type("Person")
-
-with model.rule():
-    joe = Person.add(name="Joe", age=41)
-    jane = Person.add(name="Jane", age=39)
-    john = Person.add(name="John", age=41)
-    joe.set(friend=jane).set(friend=john)
-    jane.set(friend=joe)
-    john.set(friend=joe)
-
 with model.query() as select:
     person = Person()
-    friend_age_sum = aggregates.sum(person.friend, person.friend.age, per=[person])
-    response = select(person.name, friend_age_sum)
+    response = select(person.name, alias(acos(person.age), "acos_age"))
 
 print(response.results)
 # Output:
-#    name   v
-# 0  Jane  41
-# 1   Joe  80
-# 2  John  41
+# Empty DataFrame
+# Columns: []
+# Index: []
 ```
 
 ## See Also
 
-[`avg()`]() and [`count()`]().
+[`cos()`](./cos.md), [`asin()`](./asin.md), and [`atan()`](./atan.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # `relationalai.std.graphs`
 
-The `relationalai.std.graphs` namespace contains functions and classes for building
-[graphs](./Graph/README.md) from objects in a [model](../../Model/README.md) and doing graph analytics.
+Graphs are comprised of nodes, which are entities from a [model](../../Model/README.md),
+and edges representing relationships between nodes.
+The `relationalai.std.graphs` namespace contains tools constructing and analyzing graphs.
 
+- [`graphs.Graph`](./Graph/README.md)
+  - [`graphs.Graph.compute`](./Graph/compute.md)
+  - [`graphs.Graph.Edge`](./Graph/Edge.md)
+  - [`graphs.Graph.fetch()`](./Graph/fetch.md)
+  - [`graphs.Graph.id`](./Graph/id.md)
+  - [`graphs.Graph.model`](./Graph/model.md)
+  - [`graphs.Graph.Node`](./Graph/Node.md)
+  - [`graphs.Graph.undirected`](./Graph/undirected.md)
+  - [`graphs.Graph.visualize()`](./Graph/visualize.md)
+- [`graphs.Edge`](./Edge/README.md)
+  - [`graphs.Edge.__call__()`](./Edge/call__.md)
+  - [`graphs.Edge.add()`](./Edge/add.md)
+  - [`graphs.Edge.extend()`](./Edge/extend.md)
+- [`graphs.EdgeInstance`](./EdgeInstance/README.md)
+  - [`graphs.EdgeInstance.from_`](./EdgeInstance/from_.md)
+  - [`graphs.EdgeInstance.to`](./EdgeInstance/to.md)
+  - [`graphs.EdgeInstance.set()`](./EdgeInstance/set.md)
 - [`graphs.Compute`](./Compute/README.md)
   - [`graphs.Compute.adamic_adar()`](./Compute/adamic_adar.md)
   - [`graphs.compute.avg_clustering_coefficient()`](./Compute/avg_clustering_coefficient.md)
   - [`graphs.Compute.avg_degree()`](./Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./Compute/avg_outdegree.md)
-  - [`graphs.Compute.betweenness_centrality()`](./Compute/betweeness_centrality.md)
+  - [`graphs.Compute.betweenness_centrality()`](./Compute/betweenness_centrality.md)
   - [`graphs.Compute.common_neighbor()`](./Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./Compute/cosine_similarity.md)
   - [`graphs.Compute.degree_centrality()`](./Compute/degree_centrality.md)
   - [`graphs.Compute.degree()`](./Compute/degree.md)
   - [`graphs.Compute.diameter_range()`](./Compute/diameter_range.md)
   - [`graphs.Compute.distance()`](./Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./Compute/eigenvector_centrality.md)
-  - [`graph.Compute.indegree()`](./Compute/indegree.md)
+  - [`graphs.Compute.indegree()`](./Compute/indegree.md)
   - [`graphs.Compute.is_connected()`](./Compute/is_connected.md)
   - [`graphs.Compute.is_reachable()`](./Compute/is_reachable.md)
   - [`graphs.Compute.is_triangle()`](./Compute/is_triangle.md)
   - [`graphs.Compute.label_propagation()`](./Compute/label_propagation.md)
   - [`graphs.Compute.local_clustering_coefficient()`](./Compute/local_clustering_coefficient.md)
   - [`graphs.Compute.louvain()`](./Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./Compute/max_degree.md)
@@ -32,31 +50,14 @@
   - [`graphs.Compute.min_outdegree()`](./Compute/min_outdegree.md)
   - [`graphs.Compute.num_edges()`](./Compute/num_edges.md)
   - [`graphs.Compute.num_nodes()`](./Compute/num_nodes.md)
   - [`graphs.Compute.num_triangles()`](./Compute/num_triangles.md)
   - [`graphs.Compute.outdegree()`](./Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./Compute/pagerank.md)
   - [`graphs.Compute.preferential_attachment()`](./Compute/preferential_attachment.md)
-  - [`graphs.Compute.reachable_from()`](./Compute/reachable_from.md
+  - [`graphs.Compute.reachable_from()`](./Compute/reachable_from.md)
   - [`graphs.Compute.triangles()`](./Compute/triangles.md)
   - [`graphs.Compute.weakly_connected_component()`](./Compute/weakly_connected_component.md)
   - [`graphs.Compute.weighted_distance()`](./Compute/weighted_distance.md)
   - [`graphs.Compute.weighted_cosine_similarity()`](./Compute/weighted_cosine_similarity.md)
   - [`graphs.Compute.weighted_degree_centrality()`](./Compute/weighted_degree_centrality.md)
   - [`graphs.Compute.weighted_jaccard_similarity()`](./Compute/weighted_jaccard_similarity.md)
-- [`graphs.Edge`](./Edge/README.md)
-  - [`graphs.Edge.__call__()`](./Edge/call__.md)
-  - [`graphs.Edge.add()`](./Edge/add.md)
-  - [`graphs.Edge.extend()`](./Edge/extend.md)
-- [`graphs.EdgeInstance`](./EdgeInstance/README.md)
-  - [`graphs.EdgeInstance.from_`](./EdgeInstance/from_.md)
-  - [`graphs.EdgeInstance.to`](./EdgeInstance/to.md)
-  - [`graphs.EdgeInstance.set()`](./EdgeInstance/set.md)
-- [`graphs.Graph`](./Graph/README.md)
-  - [`graphs.Graph.compute`](./Graph/compute.md)
-  - [`graphs.Graph.Edge`](./Graph/Edge.md)
-  - [`graphs.Graph.fetch()`](./Graph/fetch.md)
-  - [`graphs.Graph.id`](./Graph/id.md)
-  - [`graphs.Graph.model`](./Graph/model.md)
-  - [`graphs.Graph.Node`](./Graph/Node.md)
-  - [`graphs.Graph.undirected`](./Graph/undirected.md)
-  - [`graphs.Graph.visualize()`](./Graph/visualize.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/average_clustering_coefficient.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_clustering_coefficient.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 # `relationalai.std.graphs.Compute.avg_clustering_coefficient()`
 
 ```python
-relationalai.std.graphs.Compute.avg_clustering_coefficient(node: Producer) -> Expression
+relationalai.std.graphs.Compute.avg_clustering_coefficient() -> Expression
 ```
 
-An [Expression](docs/api_reference/python/Expression.md) object that produces
-the average of all local clustering coefficents of nodes in the graph.
-Only undirected graphs are supported.
+Compute the average clustering coefficient of all nodes in an undirected graph.
+The average clustering coefficient is the average of the
+[local clustering coefficients](./local_clustering_coefficient.md) for each node in the graph.
+Values range from `0` to `1`.
+Higher average clustering coefficients indicate nodes' increased tendency to form triangles with neighbors.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
+
+Directed graphs are not supported.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | No |   |
 | Undirected | Yes |   |
 | Weighted | Yes | Weights are ignored. |
 | Unweighted | Yes |   |
 
-## Parameters
-
-None.
-
 ## Returns
 
-An [Expression](docs/api_reference/python/Expression.md) object that produces `float` values.
+Returns an [Expression](../../../Expression.md) object that produces
+the average clustering coefficient of all nodes in the graph as a floating-point value.
 
 ## Example
 
+Use `.avg_clustering_coefficient()` to compute the average clustering coefficient of all nodes in an undirected graph.
+You access the `.avg_clustering_coefficient()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with Person and Friendship types.
+# Create a model named "socialNetwork" with a Person type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
-Friendship = model.Type("Friendship")
 
-# Add some people and friendships to the model.
+# Add some people to the model and connect them with a multi-valued `friend` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    charlie = Person.add(name="Charlie")
-    diana = Person.add(name="Diana")
-    Friendship.add(person1=alice, person2=bob)
-    Friendship.add(person1=alice, person2=charlie)
-    Friendship.add(person1=alice, person2=diana)
-    Friendship.add(person1=bob, person2=charlie)
-    
-# Create an undirected graph with nodes from the Person type and edges from the Friendship type.
+    carol = Person.add(name="Carol")
+    daniel = Person.add(name="Daniel")
+    alice.friends.extend([bob, carol])
+    bob.friends.extend([alice, carol, daniel])
+
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has four edges: Alice, Bob, and Carol form a triangle, and Daniel is only connected to Bob.
 graph = Graph(model, undirected=True)
 graph.Node.extend(Person)
-with model.rule():
-    friendship = Friendship()
-    graph.Edge.add(friendship.person1, friendship.person2)
+graph.Edge.extend(Person.friends)
 
 # Compute the average clustering coefficient of the graph.
 with model.query() as select:
-    clustering_coeff = graph.compute.avg_clustering_coefficient()
-    response = select(alias(clustering_coeff, "clustering_coefficient"))
+    acc = graph.compute.avg_clustering_coefficient()
+    response = select(alias(acc, "avg_clustering_coefficient"))
 
 print(response.results)
 # Output:
-#    clustering_coefficient
-# 0                0.583333
+#    avg_clustering_coefficient
+# 0                    0.583333
 ```
 
 ## See Also
 
-[`local_clustering_coefficient()`](./local_lustering_coefficient.md)
+[`local_clustering_coefficient()`](./local_clustering_coefficient.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,70 @@
-# `relationalai.std.graphs.Compute.avg_degree()`
+# `relationalai.std.graphs.Compute.avg_indegree()`
 
 ```python
-relationalai.std.graphs.Compute.avg_degree() -> Expression
+relationalai.std.graphs.Compute.avg_indegree() -> Expression
 ```
 
-An [Expression](docs/api_reference/python/Expression.md) object that produces the average degree of the graph.
-For directed graphs, the degree of a node is the sum of the [indegree](./indegree.md) and [outdegree](./outdegree.md) of the node.
+Compute the average indegree of all nodes in a graph.
+In a directed graph, the indegree of a node is the number of edges that point to the node.
+For an undirected graph, `.avg_indegree()` is an alias of [`.avg_degree()`](./avg_degree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
 | Weighted | Yes | Weights are ignored. |
-
-## Parameters
-
-No parameters are needed.
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [Expression](docs/api_reference/python/Expression.md) object.
+Returns an [Expression](../../../Expression.md) object that
+produces the average indegree of the graph as a floating-point value.
 
 ## Example
 
+Use `.avg_indegree()` to compute the average indegree of a node in a graph.
+You access the `.avg_indegree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 # Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the graph and connect them with a `follows` property
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    carol = Person.add(name="Carol")
+    alice.friends.extend([bob, carol])
+    bob.friends.add(alice)
+    carol.friends.add(alice)
     
-# Create an undirected graph and add all Person objects to the set of nodes
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one between Alice and Bob and one between Alice and Carol.
 graph = Graph(model, undirected=True)
-graph.Node.extend(Person, label=Person.name)
-graph.Edge.extend(Person.follows)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.friends)
 
-# Compute the minimum degree of the graph
+# Compute the average indegree of the graph.
 with model.query() as select:
-    avg_degree = graph.compute.avg_degree()
-    response = select(avg_degree)
+    avg_indegree = graph.compute.avg_indegree()
+    response = select(avg_indegree)
     
 print(response.results)
 # Output:
-#      v
-# 0  1.0
+#    v
+# 0  1
 ```
+
+In undirected graphs, `.avg_indegree()` is the same as [`.avg_degree()`](./max_degree.md).
+
+## See Also
+
+[`.indegree()`](./indegree.md), [`.min_indegree()`](./max_indegree.md), and [`.max_indegree()`](./max_indegree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,42 @@
-# `relationalai.std.graphs.Compute.avg_indegree()`
+# `relationalai.std.graphs.Graph.compute`
 
-```python
-relationalai.std.graphs.Compute.avg_indegree() -> Expression
-```
-
-An [Expression](docs/api_reference/python/Expression.md) object that produces
-the average [indegree](./indegree.md) of the graph.
-
-## Supported Graph Types
-
-| Graph Type | Supported | Notes |
-| :--- | :--- | :------ |
-| Directed | Yes |   |
-| Undirected | Yes |   |
-| Weighted | Yes | Weights are ignored. |
-
-## Parameters
-
-No parameters are needed.
-
-## Returns
-
-An [Expression](docs/api_reference/python/Expression.md) object.
+Returns a `Compute` object for computing graph analytical methods on the graph.
+See the [`Compute`](../Compute/README.md) class docs for a full list of available methods.
 
 ## Example
 
 ```python
 import relationalai as rai
+from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the graph and connect them with a `follows` property
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
-    
-# Create an undirected graph and add all Person objects to the set of nodes
-graph = Graph(model, undirected=True)
-graph.Node.extend(Person, label=Person.name)
+    alice.follows.add(bob)
+
+# Create a directed graph with 'Person' nodes and 'follows' edges.
+graph = Graph(model)
 graph.Edge.extend(Person.follows)
 
-# Compute the minimum degree of the graph
+# Compute the PageRank of each person in the graph.
 with model.query() as select:
-    avg_indegree = graph.compute.avg_indegree()
-    response = select(avg_indegree)
-    
+    person = Person()
+    pagerank = graph.compute.pagerank(person)
+    response = select(person.name, alias(pagerank, "pagerank"))
+
 print(response.results)
 # Output:
-#      v
-# 0  0.5
+#     name         v
+# 0  Alice  0.350877
+# 1    Bob  0.649123
 ```
+
+## See Also
+
+[`Compute`](../Compute/README.md) and [`Graph`](./README.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,64 @@
-# `relationalai.std.graphs.Compute.avg_outdegree()`
+# `relationalai.std.graphs.Compute.num_edges()`
 
 ```python
-relationalai.std.graphs.Compute.avg_outdegree() -> Expression
+relationalai.std.graphs.Compute.num_edges() -> Expression
 ```
 
-An [Expression](docs/api_reference/python/Expression.md) object that produces
-the average [outdegree](./outdegree.md) of the graph.
+Get the number of edges in the graph.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
 | Weighted | Yes | Weights are ignored. |
-
-## Parameters
-
-No parameters are needed.
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [Expression](docs/api_reference/python/Expression.md) object.
+Returns an [Expression](docs/api_reference/python/Expression.md) that
+produces the number of edges in the graph as an integer value.
 
 ## Example
 
+Use `.num_edges()` to get the number of edges in a graph.
+You access the `.num_edges()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
+from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
 # Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the graph and connect them with a `follows` property
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    alice.friends.add(bob)
+    bob.friends.add(alice)
     
-# Create an undirected graph and add all Person objects to the set of nodes
+# Create an undirected graph with Person nodes and edges between friends.
 graph = Graph(model, undirected=True)
-graph.Node.extend(Person, label=Person.name)
-graph.Edge.extend(Person.follows)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.friends)
 
-# Compute the minimum degree of the graph
+# Get the number of edges in the graph.
 with model.query() as select:
-    avg_outdegree = graph.compute.avg_outdegree()
-    response = select(avg_outdegree)
+    num_edges = graph.compute.num_edges()
+    response = select(alias(num_edges, "num_edges")
     
 print(response.results)
 # Output:
-#      v
-# 0  0.5
+#    v
+# 0  1
 ```
+
+## See Also
+
+[`.num_nodes()`](./num_nodes.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,87 @@
-# `relationalai.std.graphs.Compute.betweenness_centrality()`
+# `relationalai.std.graphs.Compute.avg_degree()`
 
 ```python
-relationalai.std.graphs.Compute.betweenness_centrality(node: Producer) -> Expression
+relationalai.std.graphs.Compute.avg_degree() -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[betweenness centrality](https://en.wikipedia.org/wiki/Betweenness_centrality) values
-for the producer passed to `node`.
+Get the average degree of all nodes the graph.
+For an undirected graph, the degree of a node is the number of neighbors it has in the graph.
+In a directed graph, the degree of a node is the sum of its [indegree](./indegree.md) and [outdegree](./outdegree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `float` values.
+Returns an [Expression](../../../Expression.md) object
+that produces the average degree of the graph as a floating-point value.
 
 ## Example
 
+Use `.avg_degree()` to compute the average degree of a graph:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
-
-# Create a graph and add all Person objects to the set of nodes
-# and the Person.follows property to the set of edges.
-graph = Graph(model)
+    alice.friends.extend([bob, carol])
+    bob.friends.add(alice)
+    carol.friends.add(alice)
+    
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one between Alice and Bob and one between Alice and Carol.
+graph = Graph(model, undirected=True)
 graph.Node.extend(Person)
-graph.Edge.extend(Person.follows)
+graph.Edge.extend(Person.friends)
 
-# Compute the betweenness centrality of each person in the graph.
+# Compute the average degree of the graph.
 with model.query() as select:
-    person = Person()
-    centrality = graph.compute.betweenness_centrality(person)
-    response = select(person.name, centrality)
+    avg_degree = graph.compute.avg_degree()
+    response = select(avg_degree)
+    
+print(response.results)
+# Output:
+#           v
+# 0  1.333333
+```
+
+In directed graphs, the degree of a node is the sum of its [indegree](./indegree.md) and [outdegree](./outdegree.md):
 
+```python
+# Create a directed graph with Person  nodes and edges between friends.
+# Note that graphs are directed by default.
+# This graph has four edges: two between Alice and Bob and two between Alice and Carol.
+directed_graph = Graph(model)
+directed_graph.Node.extend(Person)
+directed_graph.Edge.extend(Person.friends)
+
+# Compute the average degree of the directed graph.
+with model.query() as select:
+    avg_degree = directed_graph.compute.avg_degree()
+    response = select(avg_degree)
+    
 print(response.results)
 # Output:
-#     name    v
-# 0  Alice  1.0
-# 1    Bob  0.0
-# 2  Carol  1.0
+#           v
+# 0  2.666667
 ```
 
 ## See Also
 
-[`Compute.degree_centrality`](./degree_centrality.md) and [`Compute.pagerank`](./pagerank.md).
+[`.degree()`](./degree.md), [`.max_degree()`](./max_degree.md), and [`.avg_degree()`](./avg_degree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,63 @@
-# `relationalai.std.graphs.Compute.cosine_similarity()`
+# `relationalai.std.graphs.Compute.num_nodes()`
 
 ```python
-relationalai.std.graphs.Compute.cosine_similarity(node1: Producer, node2: Producer) -> Expression
+relationalai.std.graphs.Compute.num_nodes() -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[cosine similarity](https://en.wikipedia.org/wiki/Cosine_similarity) values
-between the producers passed to `node1` and `node2`.
+Get the number of nodes in the graph.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
-| Directed | No |   |
+| Directed | Yes |   |
 | Undirected | Yes |   |
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node1` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
-| `node2` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `float` values.
+Returns an [Expression](docs/api_reference/python/Expression.md) that
+produces the number of nodes in the graph as an integer value.
 
 ## Example
 
+Use `.num_nodes()` to get the number of nodes in a graph.
+You access the `.num_nodes()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `friend` property.
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(friend=bob)
-    bob.set(friend=carol)
-
-# Create a graph and add all `Person` objects to the set of nodes
-# and the `Person.friend` property to the set of edges.
-# Note that `cosine_similarity` is only defined for undirected graphs.
+    alice.friends.add(bob)
+    bob.friends.add(alice)
+    
+# Create an undirected graph with Person nodes and edges between friends.
 graph = Graph(model, undirected=True)
 graph.Node.extend(Person)
-graph.Edge.extend(Person.friend)
+graph.Edge.extend(Person.friends)
 
-# Compute the cosine similarity between each pair of distinct people.
+# Get the number of nodes in the graph.
 with model.query() as select:
-    person1 = Person()
-    person2 = Person()
-    person1 != person2
-    similarity = graph.compute.cosine_similarity(person1, person2)
-    response = select(person1.name, person2.name, similarity)
-
+    avg_degree = graph.compute.num_nodes()
+    response = select(avg_degree)
+    
 print(response.results)
 # Output:
-#     name  name2    v
-# 0  Alice  Carol  1.0
-# 1  Carol  Alice  1.0
+#    v
+# 0  2
 ```
 
-> [!NOTE]
-> Pairs of nodes for which the cosine similarity is `0.0` are excluded from results.
+## See Also
+
+[`.num_edges()`](./num_edges.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,88 @@
-# `relational.std.graphs.Compute.degree()`
+# `relationalai.std.graphs.Compute.min_degree()`
 
 ```python
-relationalai.std.graphs.Compute.degree(node: Producer) -> Expression
+relationalai.std.graphs.Compute.min_degree() -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[degree](https://en.wikipedia.org/wiki/Degree_(graph_theory)) values for the producer passed to `node`.
-For a directed graph, the degree of a node is the sum of its [indegree](./indegree.md) and [outdegree](./outdegree.md).
+Compute the minimum degree of all nodes a graph.
+For an undirected graph, the degree of a node is the number of neighbors it has in the graph.
+In a directed graph, the degree of a node is the sum of its [indegree](./indegree.md) and [outdegree](./outdegree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `int` values.
+Returns an [Expression](../../../Expression.md) object that produces the minimum degree of the graph as an integer value.
 
 ## Example
 
+Use `.min_degree()` to compute the minimum degree of a node in a graph.
+You access the `.min_degree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
-
-# Create an undirected graph and add all Person objects to the set of nodes
-# and the Person.follows property to the set of edges.
+    alice.friends.extend([bob, carol])
+    bob.friends.add(alice)
+    carol.friends.add(alice)
+    
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one between Alice and Bob and one between Alice and Carol.
 graph = Graph(model, undirected=True)
 graph.Node.extend(Person)
-graph.Edge.extend(Person.follows)
+graph.Edge.extend(Person.friends)
 
-# Compute the degree of each person in the graph.
+# Compute the minimum degree of the graph.
 with model.query() as select:
-    person = Person()
-    degree = graph.compute.degree(person)
-    response = select(person.name, degree)
-
+    min_degree = graph.compute.min_degree()
+    response = select(min_degree)
+    
 print(response.results)
 # Output:
-#     name  v
-# 0  Alice  2
-# 1    Bob  2
-# 2  Carol  2
+#    v
+# 0  1
+```
 
-# In a directed graph, the degree of a node is the sum of its indegree and outdegrees.
-graph = Graph(model)
-graph.Node.extend(Person)
-graph.Edge.exted(Person.follows)
+In directed graphs, the degree of a node is the sum of its [indegree](./indegree.md) and [outdegree](./outdegree.md):
 
-with model.query() as select:
-    person = Person()
-    degree = graph.compute.degree(person)
-    response = select(person.name, degree)
+```python
+# Create a directed graph with Person  nodes and edges between friends.
+# Note that graphs are directed by default.
+# This graph has four edges: two between Alice and Bob and two between Alice and Carol.
+directed_graph = Graph(model)
+directed_graph.Node.extend(Person)
+directed_graph.Edge.extend(Person.friends)
 
+# Compute the minimum degree of the directed graph.
+with model.query() as select:
+    min_degree = directed_graph.compute.min_degree()
+    response = select(min_degree)
+    
 print(response.results)
 # Output:
-#     name  v
-# 0  Alice  3
-# 1    Bob  2
-# 2  Carol  3
+#    v
+# 0  2
 ```
 
 ## See Also
 
-[`Compute.indegree()`](./indegree.md) and [`Compute.outdegree()`](./outdegree.md).
+[`.degree()`](./degree.md), [`.max_degree()`](./max_degree.md), and [`.avg_degree()`](./avg_degree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,88 @@
-# `relationalai.std.graphs.Compute.degree_centrality()`
+# `relationalai.std.graphs.Compute.max_degree()`
 
 ```python
-relationalai.std.graphs.Compute.degree_centrality(node: Producer) -> Expression
+relationalai.std.graphs.Compute.max_degree() -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[degree centrality](https://en.wikipedia.org/wiki/Centrality#Degree_centrality) values
-for the producer passed to `node`.
+Compute the maximum degree of all nodes a graph.
+For an undirected graph, the degree of a node is the number of neighbors it has in the graph.
+In a directed graph, the degree of a node is the sum of its [indegree](./indegree.md) and [outdegree](./outdegree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `float` values.
+Returns an [Expression](../../../Expression.md) object that produces the maximum degree of the graph as an integer value.
 
 ## Example
 
+Use `.max_degree()` to compute the maximum degree of a node in a graph.
+You access the `.max_degree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
-
-# Create a graph and add all Person objects to the set of nodes
-# and the Person.follows property to the set of edges.
-graph = Graph(model)
+    alice.friends.extend([bob, carol])
+    bob.friends.add(alice)
+    carol.friends.add(alice)
+    
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one between Alice and Bob and one between Alice and Carol.
+graph = Graph(model, undirected=True)
 graph.Node.extend(Person)
-graph.Edge.extend(Person.follows)
+graph.Edge.extend(Person.friends)
 
-# Compute the degree centrality of each person in the graph.
+# Compute the maximum degree of the graph.
 with model.query() as select:
-    person = Person()
-    centrality = graph.compute.degree_centrality(person)
-    response = select(person.name, centrality)
+    max_dgree = graph.compute.max_degree()
+    response = select(max_dgree)
+    
+print(response.results)
+# Output:
+#    v
+# 0  2
+```
+
+In directed graphs, the degree of a node is the sum of its [indegree](./indegree.md) and [outdegree](./outdegree.md):
 
+```python
+# Create a directed graph with Person  nodes and edges between friends.
+# Note that graphs are directed by default.
+# This graph has four edges: two between Alice and Bob and two between Alice and Carol.
+directed_graph = Graph(model)
+directed_graph.Node.extend(Person)
+directed_graph.Edge.extend(Person.friends)
+
+# Compute the maximum degree of the directed graph.
+with model.query() as select:
+    max_degree = directed_graph.compute.max_degree()
+    response = select(max_degree)
+    
 print(response.results)
 # Output:
-#     name    v
-# 0  Alice  1.5
-# 1    Bob  1.0
-# 2  Carol  1.5
+#    v
+# 0  4
 ```
 
 ## See Also
 
-[`Compute.betweenness_centrality`](./betweenness_centrality.md) and [`Compute.pagerank`](./pagerank.md).
+[`.degree()`](./degree.md), [`.min_degree()`](./min_degree.md), and [`.avg_degree()`](./avg_degree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/distance.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/distance.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,98 @@
 # `relationalai.std.graphs.Compute.distance()`
 
 ```python
 relationalai.std.graphs.Compute.distance(node1: Producer, node2: Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that computes the
-the shortest path length from `node1` and `node2`.
-Note: Be careful using `distance` on the entire graph, since for large graphs, this may be infeasible. 
+Compute the shortest path length between two nodes in the graph.
+Edge weights are ignored in weighted graphs.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
+
+> [!NOTE]
+> Be careful using `distance` on the entire graph, since for large graphs, this may be infeasible.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :--- |
 | Undirected | Yes |   |
 | Directed | Yes |   |
-| Weighted | Yes | Weights are ignored.   |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node1` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
-| `node2` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| `node1` | [`Producer`](../../../Producer.md) | A node in the graph. |
+| `node2` | [`Producer`](../../../Producer.md) | A node in the graph. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `int` values.
+Returns an [Expression](../../../Expression.md) object that produces
+the shortest path length between `node1` and `node2` as an integer value.
 
 ## Example
+
+Use `.distance()` to compute the shortest path length between two nodes in a graph.
+You access the `.distance()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "transportationNetwork" with City and Road types.
-model = rai.Model("transportationNetwork")
-City = model.Type("City")
-Road = model.Type("Road")
+# Create a model named "socialNetwork" with a Person type.
+model = rai.Model("socialNetwork")
+Person = model.Type("Person")
 
-# Add cities and roads to the model.
+# Add some people to the model and connect them with a multi-valued `follows` property.
 with model.rule():
-    new_york = City.add(name="New York")
-    los_angeles = City.add(name="Los Angeles")
-    chicago = City.add(name="Chicago")
-    houston = City.add(name="Houston")
-    Road.add(city1=new_york, city2=chicago)
-    Road.add(city1=new_york, city2=houston)
-    Road.add(city1=chicago, city2=los_angeles)
-    Road.add(city1=houston, city2=los_angeles)
-
-# Create a graph with nodes from City and edges from Road.
-graph = Graph(model, undirected=True) 
-graph.Node.extend(City)
-with model.rule():
-    road = Road()
-    graph.Edge.add(road.city1, road.city2)
+    alice = Person.add(name="Alice")
+    bob = Person.add(name="Bob")
+    carol = Person.add(name="Carol")
+    daniel = Person.add(name="Daniel")
+    alice.follows.add(bob)
+    bob.follows.add(carol)
+    carol.follows.add(daniel)
+
+# Create a directed graph with Person nodes and edges between followers.
+# Note that graphs are directed by default.
+# This graph has three edges: one from Alice to Bob, Bob to Carol, and Carol to Daniel.
+graph = Graph(model)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.follows)
 
-# Compute smallest number of roads you must take to get from Los Angeles and New York.
+# Find the distance between Alice and Daniel.
 with model.query() as select:
-    los_angeles = City(name="Los Angeles")
-    new_york = City(name="New York")
-    distance = graph.compute.distance(los_angeles, new_york)
-    response = select(alias(distance, "distance"))
+    dist = graph.compute.distance(Person(name="Alice"), Person(name="Daniel"))
+    response = select(alias(dist, "distance"))
 
 print(response.results)
 # Output:
 #    distance
-# 0         2
+# 0         3
+
+# Find all nodes at distance at most two from Alice.
+with model.query() as select:
+    node = Person()
+    dist = graph.compute.distance(Person(name="Alice"), node)
+    dist <= 2
+    response = select(node.name, alias(dist, "distance"))
+
+print(response.results)
+# Output:
+#     name  distance
+# 0  Alice         0
+# 1    Bob         1
+# 2  Carol         2
 ```
 
+Note that the distance between a node and itself is `0`.
+
 ## See Also
 
-[`weighted_distance()`](./weighted_distance.md)
+[`.is_reachable()`](./is_reachable.md),
+[`.reachable_from()`](./reachable_from.md),
+and [`weighted_distance()`](./weighted_distance.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-# `relationalai.std.graphs.Compute.eigenvector_centrality()`
+# `relationalai.std.graphs.Compute.avg_outdegree()`
 
 ```python
-relationalai.std.graphs.Compute.eigenvector_centrality(node: Producer) -> Expression
+relationalai.std.graphs.Compute.avg_outdegree() -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[eigenvector centrality](https://en.wikipedia.org/wiki/Eigenvector_centrality) values
-for the producer passed to `node`.
+Compute the average outdegree of all nodes in a graph.
+In a directed graph, the outdegree of a node is the number of edges that point away from the node.
+For an undirected graph, `.avg_outdegree()` is an alias of [`.avg_degree()`](./avg_degree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
-| Directed | No |   |
+| Directed | Yes |   |
 | Undirected | Yes |   |
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `float` values.
+Returns an [Expression](../../../Expression.md) object that
+produces the average outdegree of the graph as a floating-point value.
 
 ## Example
 
+Use `.avg_outdegree()` to compute the average outdegree of a node in a graph.
+You access the `.avg_outdegree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `friend` property.
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
-    alice.set(friend=carol)
-    bob.set(friend=carol)
-
-# Create a graph and add all Person objects to the set of nodes
-# and the Person.friend property to the set of edges.
+    alice.friends.extend([bob, carol])
+    bob.friends.add(alice)
+    carol.friends.add(alice)
+    
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one between Alice and Bob and one between Alice and Carol.
 graph = Graph(model, undirected=True)
-graph.Edge.extend(Person.friend)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.friends)
 
-# Compute the eigenvector centrality of each person in the graph.
+# Compute the average outdegree of the graph.
 with model.query() as select:
-    person = Person()
-    centrality = graph.compute.eigenvector_centrality(person)
-    response = select(person.name, centrality)
-
+    avg_outdegree = graph.compute.avg_outdegree()
+    response = select(avg_outdegree)
+    
 print(response.results)
 # Output:
-#     name        v
-# 0  Alice  0.57735
-# 1    Bob  0.57735
-# 2  Carol  0.57735
+#    v
+# 0  1
 ```
 
+In undirected graphs, `.avg_outdegree()` is the same as [`.avg_degree()`](./max_degree.md).
+
 ## See Also
 
-[`Compute.betweenness_centrality()`](./betweenness_centrality.md),
-[`Compute.degree_centrality()`](./degree_centrality.md),
-and [`Compute.pagerank()`](./pagerank.md).
+[`.outdegree()`](./outdegree.md), [`.min_outdegree()`](./max_outdegree.md), and [`.max_outdegree()`](./max_outdegree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 # `relational.std.graphs.Compute.indegree()`
 
 ```python
 relationalai.std.graphs.Compute.indegree(node: Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[indegree](https://en.wikipedia.org/wiki/Directed_graph#Indegree_and_outdegree) values for the producer passed to `node`.
-For an undirected graph, the indegree of a node is the same as its [degree](./degree.md).
+Compute the indegree of a node.
+In a directed graph, the indegree of a node is the number of edges that point to the node.
+For an undirected graph, `.indegree()` is an alias of [`.degree()`](./degree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| node | [Producer](../../../Producer.md) | A node in the graph. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `int` values.
+Returns an [Expression](../../../Expression.md) object that produces the indegree of the node as an integer value.
 
 ## Example
 
+Use `.indegree()` to compute the indegree of a node in a graph.
+You access the `.indegree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(follows=bob).set(follows=carol)
-    bob.set(follows=carol)
-
-# Create a directed graph and add all edges from the Person.follows property.
-directed_graph = Graph(model)
-directed_graph.Edge.extend(Person.follows)
+    alice.friends.add(bob)
+    bob.friends.add(alice)
+    
+# Create a directed graph with Person nodes and edges between friends.
+# Note that graphs are directed by default.
+# This graphs has two edges: one from Alice to Bob and one from Bob to Alice.
+graph = Graph(model)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.friends)
 
-# Compute the indegree of each person in the graph.
+# Get the number of nodes in the graph.
 with model.query() as select:
+    # Get all Person objects.
     person = Person()
-    indegree = directed_graph.compute.indegree(person)
+    # Compute the indegree of each person.
+    indegree = graph.compute.indegree(person)
+    # Select the name of each person and their indegree.
     response = select(person.name, indegree)
-
+    
 print(response.results)
 # Output:
 #     name  v
-# 0  Alice  0
+# 0  Alice  1
 # 1    Bob  1
-# 2  Carol  2
-
-# In an undirected graph, the indegree of a node is the same as its degree.
-undirected_graph = Graph(model, undirected=True)
-undirected_graph.Edge.extend(Person.follows)
-
-with model.query() as select:
-    person = Person()
-    indegree = undirected_graph.compute.indegree(person)
-    degree = undirected_graph.compute.degree(person)
-    response = select(person.name, indegree, degree)
-
-print(response.results)
-# Output:
-#     name  v  v2
-# 0  Alice  2   2
-# 1    Bob  2   2
-# 2  Carol  2   2
 ```
 
+For an undirected graph, `.indegree()` is same as [`.degree()`](./degree.md).
+
 ## See Also
 
-[`Compute.degree()`](./degree.md) and [`Compute.outdegree()`](./outdegree.md).
+[`min_indegree()`](./min_indegree.md),
+[`max_indegree()`](./max_indegree.md),
+[`avg_indegree()`](./avg_indegree.md),
+[`.degree()`](./degree.md),
+and [`.outdegree()`](./outdegree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,86 @@
-# `relationalai.std.graphs.Compute.infomap()`
+<!-- markdownlint-disable MD024 -->
+
+# `relationalai.std.graphs.EdgeInstance`
 
 ```python
-relationalai.std.graphs.Compute.infomap(node: Producer) -> Expression
+class relationalai.std.graphs.EdgeInstance
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces community IDs for nodes using the
-[Infomap algorithm](https://www.mapequation.org/assets/publications/EurPhysJ2010Rosvall.pdf).
-
-## Supported Graph Types
-
-| Graph Type | Supported | Notes |
-| :--- | :--- | :------ |
-| Directed | Yes |   |
-| Undirected | Yes |   |
-| Weighted | Yes |   |
+`EdgeInstance` is a subclass of [`Producer`](../Producer/README.md) that produces edges in a graph.
+They are created by called a graph's [`Edge`](../Graph/Edge.md) object or the [`Edge.add()`](../Graph/Edge/add.md) method.
+An `EdgeInstance` is similar to an [`Instance`](../Instance/README.md),
+but rather than representing an object, it represents a pairs of objects.
+As a result, you can't add `EdgeInstance` objects to a [`Type`](../../../Type/README.md).
 
-## Parameters
+## Attributes
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces node objects. |
+| [`.from_`](./from_.md) | [`Producer`](../../Producer.md) | The node at the start of the edge. |
+| [`.to`](./to.md) | [`Producer`](../../Producer.md) | The node at the end of the edge. |
 
-## Returns
+## Methods
 
-An [`Expression`](../../../Expression.md) object that produces `int` community IDs.
+| Name | Description | Returns |
+| :--- | :------ | :------ |
+| [`.set()`](./set.md) | Set properties on an edge. | [`EdgeInstance`](./README.md) |
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    dan = Person.add(name="Dan")
-    edgar = Person.add(name="Edgar")
-    alice.set(follows=bob)
-    carol.set(follows=dan)
+    alice.follows.add(bob)
 
-# Create a graph and add all `Person` objects to the set of nodes
-# and the `Person.follows` property to the set of edges.
+# Create a directed graph.
 graph = Graph(model)
-graph.Edge.extend(Person.follows)
-graph.Node.extend(Person)  # Ensures isolated nodes like `edgar` are included.
 
-# Detect communities of nodes using `infomap()`.
+# Add edges to the graph from the 'Person.follows' property.
+graph.Edge.extend(Person.follows, type="follows")
+
+# Query the edges in the graph.
 with model.query() as select:
-    person = Person()
-    community = graph.compute.infomap(person)
-    response = select(person.name, community)
+    # 'edge' is an EdgeInstance object.
+    edge = graph.Edge()
+    # Use the '.from_' and '.to' attributes to access the nodes
+    # connected by the edge, and the '.type' attribute to access
+    # the edge's 'type' property.
+    response = select(edge.from_.name, edge.to.name, edge.type)
 
 print(response.results)
 # Output:
-#     name  v
-# 0  Alice  2
-# 1    Bob  2
-# 2  Carol  1
-# 3    Dan  1
+#     name name2        v
+# 0  Alice   Bob  follows
+
+# Use the '.set()' method to set properties on an edge.
+with model.rule():
+    edge = graph.Edge()
+    # Set the 'weight' property of all edges to 1.0.
+    edge.set(weight=1.0)
+    # NOTE: Setting the 'weight' property does not turn the graph
+    # into a weighted graph. You can only create a weighted graph
+    # by passing 'weighted=True' to the 'Graph' constructor.
+
+# Query the edges in the graph.
+with model.query() as select:
+    edge = graph.Edge()
+    response = select(edge.from_.name, edge.to.name, edge.weight)
+
+print(response.results)
+# Output:
+#     name name2    v
+# 0  Alice   Bob  1.0
 ```
 
-> [!NOTE]
-> Isolated nodes are not assigned community IDs and are excluded from the results.
+## See Also
+
+[`Graph`](../Graph/README.md) and [`Edge`](../Edge/README.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_connected.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/is_connected.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 # `relationalai.std.graphs.Compute.is_connected()`
 
 ```python
 relationalai.std.graphs.Compute.is_connected() -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces `True` if the graph is connected
-and `False` otherwise.
+Check if the graph is connected.
+A graph is connected if every node is reachable from every other node in the undirected version of the graph.
+For directed graphs, connected is the same as weakly connected.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
-| Weighted | Yes |   |
-
-## Parameters
-
-None.
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `bool` values.
+Returns an [Expression](../../../Expression.md) object that filters connected graphs.
 
 ## Example
 
+Use `.is_connected()` to check if a graph is connected.
+You access the `.is_connected()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
 # Create a model named "socialNetwork" with a Person type.
-model = rai.Model("socialNetwork")
+model = rai.Model("socialNetwork1000")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the model and connect them with a multi-valued `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
-    alice.set(follows=bob)
+    alice.follows.add(bob)
 
-# Create a graph and add nodes and edges from the `follows` property.
-graph = Graph(model)
+# Create a directed graph with Person nodes and edges between followers.
+# Note that graphs are directed by default.
+# This graph has one edge from Alice to Bob. Carol is not connected to anyone.
+graph = Graph(model, with_isolated_nodes=True)
 graph.Node.extend(Person)
 graph.Edge.extend(Person.follows)
 
-# Is the graph conected? No, because Edgar is not connected to anyone else.
+# Is the graph connected?
 with model.query() as select:
-    connected = graph.compute.is_connected()
-    response = select(alias(connected, "connected"))
+    with model.match() as connected:
+        with graph.compute.is_connected():
+            connected.add(True)
+        with model.case():
+            connected.add(False)
+    response = select(alias(connected, "is_connected"))
 
 print(response.results)
 # Output:
-#    connected
-# 0      False
+#    is_connected
+# 0         False
 ```
+
+In the example above, the graph is not connected because Carol is not connected to anyone.
+
+## See Also
+
+[`.weakly_connected_component()`](weakly_connected_component.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_triangle.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/triangles.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,94 @@
-# `relationalai.std.graphs.Compute.is_triangle()`
+# `relationalai.std.graphs.Compute.triangles()`
 
 ```python
-relationalai.std.graphs.Compute.is_triangle(node1: Producer, node2: Producer, node3: Producer) -> Expression
+relationalai.std.graphs.Compute.triangles(node: Producer | None = None) -> tuple[Expression, Expression, Expression]
 ```
 
-Returns an [Expression](docs/api_reference/python/Expression.md) object that produces `bool` values indicating whether `node1`, `node2`, and `node3` form a triangle in the graph.
+Find all unique triangles in the graph.
+A triangle is a set of three nodes `x`, `y`, and `z` such that
+there is an edge between `x` and `y`, `y` and `z`, and `z` and `x`.
+If `node` is not `None`, the unique triangles that `node` is part of are computed.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
 | Weighted | Yes | Weights are ignored. |
 | Unweighted | Yes |   |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node1` | [`Producer`](docs/api_reference/python/Producer.md) | The first node in the triangle. |
-| `node2` | [`Producer`](docs/api_reference/python/Producer.md) | The second node in the triangle. |
-| `node3` | [`Producer`](docs/api_reference/python/Producer.md) | The third node in the triangle. |
+| `node` | [`Producer`](../../../Producer.md) or `None` | A node in the graph. If not `None`, the unique triangles that `node` is part of are computed. Otherwise, the total number of unique triangles in the graph is computed. Default is `None`. |
 
 ## Returns
 
-Returns an [Expression](docs/api_reference/python/Expression.md) object that produces `bool` values.
+Returns a tuple `(node1, node2, node3)` of three [Expression](../../../Expression.md) objects that produce
+triples of nodes that form unique triangles in the graph.
+
+For undirected graphs, triples are produced so that the nodes are ordered in ascending order by their internal identifiers.
+In directed graphs, `.triangles()` produces triples of nodes such that `node1 < node2`, `node1 < node3`, and `node2 != node3`.
+This ensures that each triangle is unique based on the ordering of nodes and edge directions.
+For instance, `(1, 2, 3)` and `(1, 3, 2)` denote distinct directed triangles.
 
 ## Example
 
+Use `.triangles()` to find all unique triangles in a graph.
+You access the `.triangles()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type
+# Create a model named "socialNetwork" with a Person type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to and 
+# Add some people to the model and connect them with a multi-valued `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     charlie = Person.add(name="Charlie")
     diana = Person.add(name="Diana")
-    alice.set(follows=bob)
-    bob.set(follows=charlie)
-    charlie.set(follows=alice).set(follows=diana)
-    
-# Create a directed graph with edges from the Person.follows property
+    alice.follows.add(bob)
+    bob.follows.add(charlie)
+    charlie.follows.extend([alice, diana])
+    diana.follows.add(bob)
+
+# Create a directed graph with Person nodes and edges between followers.
+# Note that graphs are directed by default.
 graph = Graph(model)
 graph.Edge.extend(Person.follows)
 
-# Do Alice, Bob, and Charlie form a triangle?
+# Compute the unique triangles in the graph.
 with model.query() as select:
-    is_triangle = graph.compute.is_triangle(
-        Person(name="Alice"), Person(name="Bob"), Person(name="Charlie")
-    )
-    response = select(is_triangle)
+    person1, person2, person3 = graph.compute.triangles()
+    response = select(person1.name, person2.name, person3.name)
     
 print(response.results)
 # Output:
-#       v
-# 0  True
+#       name  name2 name3
+# 0  Charlie  Alice   Bob
+# 1  Charlie  Diana   Bob
 
-# Do Alice, Bob, and Diana form a triangle?
+# Compute the unique triangles that include Alice.
 with model.query() as select:
-    is_triangle = graph.compute.is_triangle(
-        Person(name="Alice"), Person(name="Bob"), Person(name="Diana")
-    )
-    response = select(is_triangle)
+    alice = Person(name="Alice")
+    person1, person2, person3 = graph.compute.triangles(alice)
+    response = select(person1.name, person2.name, person3.name)
 
 print(response.results)
 # Output:
-#        v
-# 0  False
+#       name  name2 name3
+# 0  Charlie  Alice   Bob
 ```
 
 ## See Also
 
-[`num_triangles()`](./num_triangles.md) and [`triangles`](./triangles.md).
+[`.is_triangle()`](./is_triangle.md) and [`.num_triangles()`](./num_triangles.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,86 @@
-# `relationalai.std.graphs.Compute.jaccard_similarity()`
+# `relationalai.std.graphs.Compute.weighted_degree_centrality()`
 
 ```python
-relationalai.std.graphs.Compute.jaccard_similarity(node1: Producer, node2: Producer) -> Expression
+relationalai.std.graphs.Compute.weighted_degree_centrality(node: Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[Jaccard similarity](https://en.wikipedia.org/wiki/Jaccard_index) values
-between the producers passed to `node1` and `node2`.
+Compute the weighted degree centrality of a node in a graph.
+The weighted degree centrality of a node is the sum of the weights of the edges incident to the node
+divided by one less than the number of nodes in the graph.
+In unweighted graphs, `.weighted_degree_centrality()` is an alias of [`.degree_centrality()`](./degree_centrality.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
+| Weighted | Yes |   |
+| Unweighted | Yes | Edge weights default to `1.0`. |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node1` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
-| `node2` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| `node` | [`Producer`](../../../Producer.md) | A node in the graph. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `float` values.
+Returns an [`Expression`](../../../Expression.md) object that produces
+the weighted degree centrality of the node as a floating-point value, calculated according to the formula:
+
+```
+weighted_degree_centrality = sum(weight of edges incident to node) / (number of nodes - 1)
+```
 
 ## Example
 
+Use `.weighted_degree_centrality()` to compute the weighted degree centrality of a node in a graph.
+You access the `.weighted_degree_centrality()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
+from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with Person and Friendship types.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
+Friendship = model.Type("Friendship")
 
-# Add some people to the model and connect them with a `friend` property.
+# Add some people to the model and connect them with friendships.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
-    alice.set(friend=bob)
-    bob.set(friend=carol)
+    Friendship.add(person1=alice, person2=bob, strength=100)
+    Friendship.add(person1=bob, person2=carol, strength=10)
 
-# Create a graph and add all `Person` objects to the set of nodes
-# and the `Person.friend` property to the set of edges.
-# Note that `cosine_similarity` is only defined for undirected graphs.
-graph = Graph(model, undirected=True)
+# Create an weighted, undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one from Alice and Bob and one from Bob and Carol.
+# The edges are weighted by the strength of each friendship.
+graph = Graph(model, undirected=True, weighted=True)
 graph.Node.extend(Person)
-graph.Edge.extend(Person.friend)
+with model.rule():
+    friendship = Friendship()
+    graph.Edge.add(friendship.person1, friendship.person2, weight=friendship.strength)
 
-# Compute the cosine similarity between each pair of distinct people.
+# Compute the weighted degree centrality of each person in the graph.
 with model.query() as select:
-    person1 = Person()
-    person2 = Person()
-    person1 != person2
-    similarity = graph.compute.jaccard_similarity(person1, person2)
-    response = select(person1.name, person2.name, similarity)
+    person = Person()
+    centrality = graph.compute.weighted_degree_centrality(person)
+    response = select(person.name, alias(centrality, "weighted_degree_centrality"))
 
 print(response.results)
 # Output:
-#     name  name2    v
-# 0  Alice  Carol  1.0
-# 1  Carol  Alice  1.0
+#     name  weighted_degree_centrality
+# 0  Alice                        50.0
+# 1    Bob                        55.0
+# 2  Carol                         5.0
 ```
 
-> [!NOTE]
-> Pairs of nodes for which the Jaccard similarity is `0.0` are excluded from results.
+## See Also
+
+[`.degree_centrality()`](./degree_centrality.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/trunc_divide.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,52 @@
-# `relationalai.std.graphs.Compute.label_propagation()`
+# `relationalai.std.math.trunc_divide()`
 
 ```python
-relationalai.std.graphs.Compute.label_propagation(node: Producer) -> Expression
+relationalai.std.math.trunc_divide(numerator: Number | Producer, denominator: Number | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces integer community labels for the producer passed to `node` using the
-[label propagation](https://en.wikipedia.org/wiki/Label_propagation_algorithm) algorithm.
-
-## Supported Graph Types
-
-| Graph Type | Supported | Notes |
-| :--- | :--- | :------ |
-| Directed | Yes |   |
-| Undirected | Yes |   |
+Returns an [`Expression`](../../Expression.md) that produces the result of the division of `numerator` by `denominator`, rounded towards zero.
+The type of the result is the same as the type of the `numerator`.
 
 ## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| :--- | :--- | :--------- |
+| `numerator` | `Number` or [`Producer`](../../Producer/README.md) | The numerator of the division. |
+| `denominator` | `Number` or [`Producer`](../../Producer/README.md) | The denominator of the division. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `int` values.
+An [`Expression`](../../Expression.md) object.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std.graphs import Graph
+from relationalai.std import alias
+from relationalai.std.math import trunc_divide
 
-# Create a model named "socialNetwork" with a Person type.
-model = rai.Model("socialNetwork")
+# Create a model with a `Person` type.
+model = rai.Model("people")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the model.
 with model.rule():
-    alice = Person.add(name="Alice")
-    bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
-
-# Create a graph and add all Person objects to the set of nodes
-# and the Person.follows property to the set of edges.
-graph = Graph(model)
-graph.Node.extend(Person)
-graph.Edge.extend(Person.follows)
+    Person.add(name="Alice", height_cm=170.1)
+    Person.add(name="Bob", height_cm=180)
 
-# Compute the PageRank of each person in the graph.
+# What is each person's height rounded down to the nearest whole number?
 with model.query() as select:
-    person = Person()
-    community = graph.compute.label_propagation(person)
-    response = select(person.name, community)
+    p = Person()
+    half_height = trunc_divide(p.height_cm, 2)
+    response = select(p.name, alias(half_height, "half_height"))
 
 print(response.results)
 # Output:
-#     name  v
-# 0  Alice  3
-# 1    Bob  3
-# 2  Carol  3
+#     name  half_height
+# 0  Alice         85.0
+# 1    Bob         90.0
 ```
 
 ## See Also
 
-[`Compute.weakly_connected_component`](./weakly_connected_component.md)
+[`//`](../../Producer/floordiv__.md) (floor division) and [`/`](../../Producer/truediv__.md) (true division).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,69 @@
-# `relationalai.std.graphs.Compute.max_degree()`
+# `relationalai.std.graphs.Compute.min_indegree()`
 
 ```python
-relationalai.std.graphs.Compute.max_degree() -> Expression
+relationalai.std.graphs.Compute.min_indegree() -> Expression
 ```
 
-An [Expression](docs/api_reference/python/Expression.md) object that produces the maximum degree of the graph.
-For directed graphs, the degree of a node is the sum of the [indegree](./indegree.md) and [outdegree](./outdegree.md) of the node.
+Compute the minimum indegree of all nodes in a graph.
+In a directed graph, the indegree of a node is the number of edges that point to the node.
+For an undirected graph, `.min_indegree()` is an alias of [`.min_degree()`](./min_degree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
 | Weighted | Yes | Weights are ignored. |
-
-## Parameters
-
-No parameters are needed.
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [Expression](docs/api_reference/python/Expression.md) object.
+Returns an [Expression](../../../Expression.md) object that produces the minimum indegree of the graph as an integer value.
 
 ## Example
 
+Use `.min_indegree()` to compute the minimum indegree of a graph.
+You access the `.min_indegree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 # Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the graph and connect them with a `follows` property
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    carol = Person.add(name="Carol")
+    alice.friends.extend([bob, carol])
+    bob.friends.add(alice)
+    carol.friends.add(alice)
     
-# Create an undirected graph and add all Person objects to the set of nodes
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one between Alice and Bob and one between Alice and Carol.
 graph = Graph(model, undirected=True)
-graph.Node.extend(Person, label=Person.name)
-graph.Edge.extend(Person.follows)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.friends)
 
-# Compute the minimum degree of the graph
+# Compute the minimum indegree of the graph.
 with model.query() as select:
-    max_degree = graph.compute.max_degree()
-    response = select(max_degree)
+    min_indegree = graph.compute.min_indegree()
+    response = select(min_indegree)
     
 print(response.results)
 # Output:
 #    v
 # 0  1
 ```
+
+In undirected graphs, `.min_indegree()` is the same as [`.min_degree()`](./min_degree.md).
+
+## See Also
+
+[`.indegree()`](./indegree.md), [`.max_indegree()`](./max_indegree.md), and [`.avg_indegree()`](./avg_indegree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,70 @@
-# `relationalai.std.graphs.Compute.max_outdegree()`
+# `relationalai.std.graphs.Compute.min_outdegree()`
 
 ```python
-relationalai.std.graphs.Compute.max_outdegree() -> Expression
+relationalai.std.graphs.Compute.min_outdegree() -> Expression
 ```
 
-An [Expression](docs/api_reference/python/Expression.md) object that produces
-the maximum [outdegree](./outdegree.md) of the graph.
+Compute the minimum outdegree of all nodes in a graph.
+In a directed graph, the outdegree of a node is the number of edges that point away from the node.
+For an undirected graph, `.min_outdegree()` is an alias of [`.min_degree()`](./min_degree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
 | Weighted | Yes | Weights are ignored. |
-
-## Parameters
-
-No parameters are needed.
+| Unweighted | Yes |   |
 
 ## Returns
 
-An [Expression](docs/api_reference/python/Expression.md) object.
+Returns an [Expression](../../../Expression.md) object that produces
+the minimum outdegree of the graph as an integer value.
 
 ## Example
 
+Use `.min_outdegree()` to compute the minimum outdegree of a graph.
+You access the `.min_outdegree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 # Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the graph and connect them with a `follows` property
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    carol = Person.add(name="Carol")
+    alice.friends.extend([bob, carol])
+    bob.friends.add(alice)
+    carol.friends.add(alice)
     
-# Create an undirected graph and add all Person objects to the set of nodes
+# Create an undirected graph with Person nodes and edges between friends.
+# This graph has two edges: one between Alice and Bob and one between Alice and Carol.
 graph = Graph(model, undirected=True)
-graph.Node.extend(Person, label=Person.name)
-graph.Edge.extend(Person.follows)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.friends)
 
-# Compute the minimum degree of the graph
+# Compute the minimum outdegree of the graph.
 with model.query() as select:
-    max_outdegree = graph.compute.max_outdegree()
-    response = select(max_outdegree)
+    min_outdegree = graph.compute.min_outdegree()
+    response = select(min_outdegree)
     
 print(response.results)
 # Output:
 #    v
 # 0  1
 ```
+
+In directed graphs, `.min_outdegree()` is the same as [`.min_degree()`](./min_degree.md).
+
+## See Also
+
+[`.outdegree()`](./outdegree.md), [`.max_outdegree()`](./max_outdegree.md), and [`.avg_outdegree()`](./avg_outdegree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_triangles.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/num_triangles.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 # `relationalai.std.graphs.Compute.num_triangles()`
 
 ```python
 relationalai.std.graphs.Compute.num_triangles(node: Producer | None = None) -> Expression
 ```
 
-Returns an [Expression](docs/api_reference/python/Expression.md) object that produces the number of unique triangles in the graph.
+Compute the number of unique triangles in the graph.
+A triangle is a set of three nodes `x`, `y`, and `z` such that
+there is an edge between `x` and `y`, `y` and `z`, and `z` and `x`.
+If `node` is not `None`, the number of unique triangles that `node` is part of is computed.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
 | Weighted | Yes | Weights are ignored. |
 | Unweighted | Yes |   |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node` | [`Producer`](docs/api_reference/python/Producer.md) | Optional node for which to compute the number of unique triangles. If `None`, the number of unique triangles in the whole graph is computed. |
+| `node` | [`Producer`](../../../Producer.md) or `None` | A node in the graph. If not `None`, the number of unique triangles that `node` is part of is computed. Otherwise, the total number of unique triangles in the graph is computed. Default is `None`. |
 
 ## Returns
 
-Returns an [Expression](docs/api_reference/python/Expression.md) object that producers `int` values.
+Returns an [Expression](../../../Expression.md) object that produces
+the number of unique triangles in the graph as an integer value, if `node` is `None`,
+or the number of unique triangles that `node` is part of as an integer value, if `node` is not `None`.
 
 ## Example
 
+Use `.num_triangles()` to compute the number of unique triangles in a graph.
+You access the `.num_triangles()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type
+# Create a model named "socialNetwork" with a Person type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to and 
+# Add some people to the model and connect them with a multi-valued `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     charlie = Person.add(name="Charlie")
     diana = Person.add(name="Diana")
-    alice.set(follows=bob)
-    bob.set(follows=charlie)
-    charlie.set(follows=alice).set(follows=diana)
-    
-# Create a directed graph with edges from the Person.follows property
+    alice.follows.add(bob)
+    bob.follows.add(charlie)
+    charlie.follows.extend([alice, diana])
+
+# Create a directed graph with Person nodes and edges between followers.
+# Note that graphs are directed by default.
 graph = Graph(model)
+graph.Node.extend(Person)
 graph.Edge.extend(Person.follows)
 
 # Compute the number of unique triangles in the graph.
 with model.query() as select:
     num_triangles = graph.compute.num_triangles()
     response = select(alias(num_triangles, "num_triangles"))
     
@@ -73,8 +85,8 @@
 # 1      Bob              1
 # 2  Charlie              1
 # 3    Diana              0
 ```
 
 ## See Also
 
-[`is_triangle()`](./is_triangle.md) and [`triangles`](./triangles.md).
+[`.is_triangle()`](./is_triangle.md) and [`.triangles()`](./triangles.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 # `relational.std.graphs.Compute.outdegree()`
 
 ```python
 relationalai.std.graphs.Compute.outdegree(node: Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the
-[outdegree](https://en.wikipedia.org/wiki/Directed_graph#Indegree_and_outdegree) values for the producer passed to `node`.
-For an undirected graph, the outdegree of a node is the same as its [degree](./degree.md).
+Compute the outdegree of a node in the graph.
+In a directed graph, the outdegree of a node is the number of edges that point away from the node.
+For an undirected graph, `.outdegree()` is an alias of [`.degree()`](./degree.md).
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| node | [Producer](../../../Producer.md) | A node in the graph. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `int` values.
+Returns an [Expression](../../../Expression.md) object that produces the outdegree of the node as an integer value.
 
 ## Example
 
+Use `.outdegree()` to compute the outdegree of a node in a graph.
+You access the `.outdegree()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the graph and connect them with a 'friends' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(follows=bob).set(follows=carol)
-    bob.set(follows=carol)
-
-# Create a directed graph and add all edges from the Person.follows property.
-directed_graph = Graph(model)
-directed_graph.Edge.extend(Person.follows)
+    alice.friends.add(bob)
+    bob.friends.add(alice)
+    
+# Create a directed graph with Person nodes and edges between friends.
+# Note that graphs are directed by default.
+# This graphs has two edges: one from Alice to Bob and one from Bob to Alice.
+graph = Graph(model)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.friends)
 
-# Compute the outdegree of each person in the graph.
+# Get the number of nodes in the graph.
 with model.query() as select:
+    # Get all Person objects.
     person = Person()
-    outdegree = directed_graph.compute.outdegree(person)
+    # Compute the outdegree of each person.
+    outdegree = graph.compute.outdegree(person)
+    # Select the name of each person and their outdegree.
     response = select(person.name, outdegree)
-
+    
 print(response.results)
 # Output:
 #     name  v
-# 0  Alice  2
+# 0  Alice  1
 # 1    Bob  1
-# 2  Carol  0
-
-# In an undirected graph, the outdegree of a node is the same as its degree.
-undirected_graph = Graph(model, undirected=True)
-undirected_graph.Edge.extend(Person.follows)
-
-with model.query() as select:
-    person = Person()
-    outdegree = undirected_graph.compute.outdegree(person)
-    degree = undirected_graph.compute.degree(person)
-    response = select(person.name, outdegree, degree)
-
-print(response.results)
-# Output:
-#     name  v  v2
-# 0  Alice  2   2
-# 1    Bob  2   2
-# 2  Carol  2   2
 ```
 
+In undirected graphs, [`.outdegree()`](./outdegree.md) is same as [`.degree()`](./degree.md).
+
 ## See Also
 
-[`Compute.degree()`](./degree.md) and [`Compute.indegree()`](./indegree.md).
+[`min_outdegree()`](./min_outdegree.md),
+[`max_outdegree()`](./max_outdegree.md),
+[`avg_outdegree()`](./avg_outdegree.md),
+[`.degree()`](./degree.md),
+and [`.outdegree()`](./outdegree.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,64 @@
-# `relationalai.std.graphs.Compute.pagerank()`
+# `relationalai.std.graphs.Graph.Edge`
 
-```python
-relationalai.std.graphs.Compute.pagerank(
-    node: Producer,
-    damping_factor: float = 0.85,
-    tolerance: float = 1e-6,
-    max_iter: int = 20
-) -> Expression
-```
-
-Returns an [`Expression`](../../../Expression.md) that produces the
-[PageRank](https://en.wikipedia.org/wiki/PageRank) values for the producer passed to `node`.
-
-## Supported Graph Types
-
-| Graph Type | Supported | Notes |
-| :--- | :--- | :------ |
-| Directed | Yes |   |
-| Undirected | Yes |   |
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
-| `damping_factor` | `float` | The PageRank damping factor. Must be between 0 and 1, inclusive. Default is 0.85. |
-| `tolerance` | `float` | The convergence tolerance for the PageRank algorithm. Default is 1e-6. |
-| `max_iter` | `int` | The maximum number of iterations allowed in the PageRank algorithm. Default is 20. |
-
-## Returns
-
-An [`Expression`](../../../Expression.md) object that produces `float` values.
+An [`Edge`](../Edge/README.md) object that can be used to add and query edges in a graph.
 
 ## Example
 
+`Graph.Edge` is an [`Edge`](../Edge/README.md) object.
+Use its [`.add()`](../Edge/add.md) and [`.extend()`](../Edge/extend.md) methods to add edges to the graph:
+
 ```python
 import relationalai as rai
+from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model with a 'Person' and 'Message' types.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
+Message = model.Type("Message")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add people and messages to the model.
+# People are connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
-
-# Create a graph and add all Person objects to the set of nodes
-# and the Person.follows property to the set of edges.
-graph = Graph(model)
-graph.Node.extend(Person)
-graph.Edge.extend(Person.follows)
+    alice.follows.add(bob)
+    Message.add(sender=alice, recipient=bob, text="Hey Bob!")
+
+# Create a weighted, directed graph.
+# Graphs are directed by default, so only the 'weighted' parameter is needed.
+graph = Graph(model, weighted=True)
+
+# Add edges using the 'Person.follows'. Person nodes are automatically added
+# to the graph. The 'label' parameter is optional and sets the edge's label
+# in the graph visualization.
+graph.Edge.extend(Person.follows, label="follows")
 
-# Compute the PageRank of each person in the graph.
+# Alternatively, you can add specific edges in a rule using 'Edge.add()'.
+# For example, this rule adds edges of type "message" between all senders and recipients.
+with model.rule():
+    message = Message()
+    graph.Edge.add(from_=message.sender, to=message.recipient, label="message")
+
+# You can query edges using `Graph.Edge`, which behaves like a 'Type' object.
+# It returns an 'EdgeInstance' object that can be used to access the edge's
+# properties. Use the 'from_' and 'to' properties to access the nodes at
+# either end of the edge.
 with model.query() as select:
-    person = Person()
-    centrality = graph.compute.pagerank(person)
-    response = select(person.name, centrality)
+    edge = graph.Edge()
+    response = select(edge.from_.name, edge.to.name, alias(edge.label, "label"))
 
 print(response.results)
 # Output:
-#     name         v
-# 0  Alice  0.397402
-# 1    Bob  0.214806
-# 2  Carol  0.387792
+#     name name2        v
+# 0  Alice   Bob  follows
+# 1  Alice   Bob  message
 ```
 
+
 ## See Also
 
-[`Compute.betweenness_centrality`](./betweenness_centrality.md)
-and [`Compute.degree_centrality`](./degree_centrality.md).
+[`graphs.Edge`](../Edge/README.md),
+[`graphs.EdgeInstance`](../EdgeInstance/README.md),
+[`Graph`](./README.md),
+and [`Node`](./Node.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/reachable_from.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/reachable_from.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 # `relationalai.std.graphs.Compute.reachable_from()`
 
 ```python
 relationalai.std.graphs.Compute.reachable_from(node: Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces object IDs of all nodes reachable from `node` in the transitive closure of the graph.
-Self-loops are only included in the transitive closure if they exist in the graph.
+Find all nodes reachable from `node` in a graph.
+One node is reachable from another if there is a path from the first node to the second.
+Nodes with self-loops are considered to be reachable from themselves.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
-| Weighted | Yes |   |
+| Weighted | Yes | Weights are ignored. |
+| Unweighted | Yes |   |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :---------- |
-| node | [`Producer`](../../Producer.md) | The node from which to compute the transitive closure. |
+| `node` | [`Producer`](../../../Producer.md) | A node in the graph. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces object IDs of all nodes reachable from `node`.
+Returns an [Expression](../../../Expression.md) object that produces
+[model](../../../Model/README.md) objects that are reachable from `node`.
 
 ## Example
 
+Use `.reachable_from()` to find all nodes reachable from a node in a graph.
+You access the `.reachable_from()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
-from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
 # Create a model named "socialNetwork" with a Person type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the model and connect them with a multi-valued `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
-    alice.set(follows=bob)
-    bob.set(follows=carol)
+    alice.follows.add(bob)
+    bob.follows.add(carol)
 
-# Create a graph and add nodes and edges from the `follows` property.
+# Create a directed graph with Person nodes and edges between followers.
+# Note that graphs are directed by default.
+# This graph has edges from Alice to Bob and Bob to Carol.
 graph = Graph(model)
+graph.Node.extend(Person)
 graph.Edge.extend(Person.follows)
 
-# Who is "reachable" from Alice, following a chain of `follows` edges?
+# Who is reachable from Alice?
 with model.query() as select:
-    alice = Person(name="Alice")
-    reachable_from_alice = graph.compute.reachable_from(node=alice)
-    response = select(reachable_from_alice.name)
+    reachable = graph.compute.reachable_from(Person(name="Alice"))
+    response = select(reachable.name)
 
 print(response.results)
 # Output:
 #     name
 # 0    Bob
 # 1  Carol
 ```
 
-Alice is not reported as reachable from herself because there is no edge from Alice to herself in the graph.
+In the example above, both Bob and Carol are reachable from Alice
+because there is a path from Alice to Bob and a path from Alice to Carol that passes through Bob.
+Alice is not reachable from herself because her node has no self-loop.
+
+To check if one node is reachable from another, use [`.is_reachable()`](./is_reachable.md).
+Use [`.distance()`](./distance.md) to find the shortest path length between two nodes.
+
+## See Also
+
+[`.is_reachable()`](./is_reachable.md) and [`.distance()`](./distance.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/triangles.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/diameter_range.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,76 @@
-# `relationalai.std.graphs.Compute.triangles()`
+# `relationalai.std.graphs.Compute.diameter_range()`
 
 ```python
-relationalai.std.graphs.Compute.triangles(node: Producer | None = None) -> tuple[Expression]
+relationalai.std.graphs.Compute.diameter_range() -> tuple[Expression, Expression]
 ```
 
-Returns a tiple of [Expression](docs/api_reference/python/Expression.md) objects that produce
-all nodes that form unique triangles in the graph.
-If the optional `node` parameter is provided, the all unique triangles that include the node are produced.
+Compute lower and upper bounds for the diameter of a graph.
+The diameter is the length of the longest shortest path between any two nodes in the graph.
+Edge weights are ignored in weighted graphs.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
-| :--- | :--- | :------ |
-| Directed | Yes |   |
+| :--- | :--- | :--- |
 | Undirected | Yes |   |
+| Directed | Yes |   |
 | Weighted | Yes | Weights are ignored. |
 | Unweighted | Yes |   |
 
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](docs/api_reference/python/Producer.md) | Optional node for which to compute the unique triangles. If `None`, all unique triangles in the graph are computed. |
-
 ## Returns
 
-Returns a tuple of three [Expression](docs/api_reference/python/Expression.md) objects.
+Returns a tuple of two [Expression](../../../Expression.md) objects that produce
+the lower and upper bounds for the diameter of the graph.
+
+The diameter range is computed by selecting a subset highest [degree](./degree.md) nodes
+and, for each node, finding the length of the longest shortest path from that node to the rest of the graph.
+The minimum and maximum of these lengths are returned as the lower and upper bounds of the diameter, respectively.
 
 ## Example
 
+Use `.diameter_range()` to compute the range of possible diameters in a graph.
+You access the `.diameter_range()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
 from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type
+# Create a model named "socialNetwork" with a Person type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to and 
+# Add some people to the model and connect them with a multi-valued `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    charlie = Person.add(name="Charlie")
-    diana = Person.add(name="Diana")
-    alice.set(follows=bob)
-    bob.set(follows=charlie)
-    charlie.set(follows=alice).set(follows=diana)
-    diana.set(follows=bob)
-    
-# Create a directed graph with edges from the Person.follows property
+    carol = Person.add(name="Carol")
+    alice.follows.add(bob)
+    bob.follows.add(carol)
+
+# Create a directed graph with Person nodes and edges between followers.
+# Note that graphs are directed by default.
+# This graph has edges from Alice to Bob and Bob to Carol.
 graph = Graph(model)
+graph.Node.extend(Person)
 graph.Edge.extend(Person.follows)
 
-# Compute the unique triangles in the graph.
+# Compute the diameter range of the graph.
 with model.query() as select:
-    person1, person2, person3 = graph.compute.triangles()
-    response = select(person1.name, person2.name, person3.name)
-    
-print(response.results)
-# Output:
-#       name  name2 name3
-# 0  Charlie  Alice   Bob
-# 1  Charlie  Diana   Bob
-
-# Compute the unique triangles that include Alice.
-with model.query() as select:
-    alice = Person(name="Alice")
-    person1, person2, person3 = graph.compute.triangles(alice)
-    response = select(person1.name, person2.name, person3.name)
+    diam_min, diam_max = graph.compute.diameter_range()
+    response = select(alias(diam_min, "min"), alias(diam_max, "max"))
 
 print(response.results)
 # Output:
-#       name  name2 name3
-# 0  Charlie  Alice   Bob
+#    min  max
+# 0    2    2
 ```
 
+In cases like this where the lower and upper bounds are the same, the diameter of the graph is known exactly.
+This may not always be the case, especially for larger and more complex graphs.
+
 ## See Also
 
-[`is_triangle()`](./is_triangle.md) and [`num_triangles`](./num_triangles.md).
+[`.distance()`](./distance.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,53 @@
-# `relationalai.std.graphs.Compute.weakly_connected_component()`
+# `relationalai.std.graphs.Graph.fetch()`
 
 ```python
-relationalai.std.graphs.Compute.weakly_connected_component(node: Producer) -> Expression
+relationalai.std.graphs.Graph.fetch() -> dict
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the component IDs of the
-[weakly connected components](https://en.wikipedia.org/wiki/Weak_component)
-to which the nodes produced by the `node` producer belong.
-
-## Supported Graph Types
-
-| Graph Type | Supported | Notes |
-| :--- | :--- | :------ |
-| Directed | Yes |   |
-| Undirected | Yes |   |
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+Returns a dictionary with two keys, `"nodes"` and `"edges"`, containing the graph's data.
+`.fetch()` is a blocking operation that queries the model and returns the data locally.
+It may be slow and consume a lot of memory for large graphs.
+Use `.fetch()` to pass graph data to external libraries, such as alternative visualization tools.
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `string` values.
+A `dict` object.
 
 ## Example
 
 ```python
+from pprint import pprint
+
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
+    alice.follows.add(bob)
 
-# Create a graph and add all Person objects to the set of nodes
-# and the Person.follows property to the set of edges.
+# Create a directed graph with 'Person' nodes and 'follows' edges.
 graph = Graph(model)
-graph.Node.extend(Person)
-graph.Edge.extend(Person.follows)
-
-# Compute the weakly connected component for each person in the graph.
-with model.query() as select:
-    person = Person()
-    component = graph.compute.weakly_connected_component(person)
-    response = select(person.name, component)
+graph.Node.extend(Person, label=Person.name)
+graph.Edge.extend(Person.follows, label="follows")
 
-print(response.results)
+# Fetch the graph.
+# NOTE: Fetching the graph queries the model and returns the data locally.
+# If the graph is large, fetching it may be slow and consume a lot of memory.
+pprint(graph.fetch())
 # Output:
-#     name                       v
-# 0  Alice  JCOgZI0tb1qNRTyXYhDFOw
-# 1    Bob  JCOgZI0tb1qNRTyXYhDFOw
-# 2  Carol  JCOgZI0tb1qNRTyXYhDFOw
+# {'edges': defaultdict(<class 'dict'>,
+#                       {('+0JKlsJxRGKBYFiMq/o/Sg', 'ru89MBnrLAPLQFVtoYdnfQ'): {'label': 'follows'}}),
+#  'nodes': defaultdict(<class 'dict'>,
+#                       {'+0JKlsJxRGKBYFiMq/o/Sg': {'label': 'Alice'},
+#                        'ru89MBnrLAPLQFVtoYdnfQ': {'label': 'Bob'}})}
 ```
 
-Component IDs are the object IDs of the objects chosen to represent the components.
-In the preceding example, all three nodes are in the same component.
-
 ## See Also
 
-[`Compute.label_propagation`](./label_propagation.md)
+[`.visualize()`](./visualize.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_distance.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Compute/weighted_distance.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,97 @@
 # `relationalai.std.graphs.Compute.weighted_distance()`
 
 ```python
 relationalai.std.graphs.Compute.weighted_distance(node1: Producer, node2: Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that computes the weighted distance between `node1` and `node2`.
-`weighted_distance` is the counterpart of [`distance`](./distance.md) that uses edge weights for computing the shortest path length between nodes.
-All edge weights must be non-negative, otherwise no results are returned.
+Compute the shortest path length between `node1` and `node2` in a weighted graph.
+Must be called in a [rule](../../../Model/rule.md) or [query](../../../Model/query.md) context.
+Alias for [`.distance()`](./distance.md) in unweighted graphs.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :--- |
-| Undirected | Yes | Edge weights default to `1.0` |
-| Directed | Yes | Edge weights default to `1.0` |
-| Weighted | Yes |   |
+| Undirected | Yes |   |
+| Directed | Yes |   |
+| Weighted | Yes | Only positive edge weights are supported. |
+| Unweighted | Yes | Edge weights default to `1.0`.  |
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `node1` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
-| `node2` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+| `node1` | [`Producer`](../../../Producer.md) | A node in the graph. |
+| `node2` | [`Producer`](../../../Producer.md) | A node in the graph. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `int` values.
+Returns an [Expression](../../../Expression.md) object that produces
+the shortest path length between `node1` and `node2` as a float value.
 
 ## Example
+
+Use `.weighted_distance()` to compute the shortest path length between two nodes in a weighted graph.
+You access the `.weighted_distance()` method from a [`Graph`](../Graph.md) object's
+[`.compute`](../Graph/compute.md) attribute:
+
 ```python
 import relationalai as rai
+from relationalai.std import alias
 from relationalai.std.graphs import Graph
 
-# Create a model named "weightedTransportationNetwork" with City and Road types.
-model = rai.Model("weightedTransportationNetwork")
-City = model.Type("City")
-Road = model.Type("Road")
+# Create a model named "socialNetwork" with Person and Friendship types.
+model = rai.Model("socialNetwork")
+Person = model.Type("Person")
+Friendship = model.Type("Friendship")
 
-# Add cities and roads to the model.
+# Add some people to the model and connect them with the Friendship type.
 with model.rule():
-    new_york = City.add(name="New York")
-    los_angeles = City.add(name="Los Angeles")
-    chicago = City.add(name="Chicago")
-    houston = City.add(name="Houston")
-    Road.add(from_=new_york, to=los_angeles, distance=2500)
-    Road.add(from_=new_york, to=chicago, distance=800)
-    Road.add(from_=new_york, to=houston, distance=1600)
-    Road.add(from_=los_angeles, to=chicago, distance=1100)
-    Road.add(from_=los_angeles, to=houston, distance=1400)
-
-# Create a graph with weighted edges.
+    alice = Person.add(name="Alice")
+    bob = Person.add(name="Bob")
+    carol = Person.add(name="Carol")
+    daniel = Person.add(name="Daniel")
+    Friendship.add(person1=alice, person2=bob, strength=1.0)
+    Friendship.add(person1=bob, person2=carol, strength=0.5)
+    Friendship.add(person1=carol, person2=daniel, strength=0.75)
+
+# Create a directed graph with Person nodes and edges between friends.
+# Note that graphs are directed by default.
+# This graph has three edges: one from Alice to Bob, Bob to Carol, and Carol to Daniel.
+# The edges are weighted by the strength of each friendship.
 graph = Graph(model, weighted=True)
-graph.Node.extend(City)
-
-# Add the roads to the graph as weighted edges.
+graph.Node.extend(Person)
 with model.rule():
-    r = Road()
-    graph.Edge.add(r.from_, r.to, weight=r.distance)
+    friendship = Friendship()
+    graph.Edge.add(friendship.person1, friendship.person2, weight=friendship.strength)
+
+# Find the weighted distance between Alice and Daniel.
+with model.query() as select:
+    dist = graph.compute.weighted_distance(Person(name="Alice"), Person(name="Daniel"))
+    response = select(alias(dist, "distance"))
+
+print(response.results)
+# Output:
+#    distance
+# 0      2.25
 
-# Compute the weighted distance between each pair of distinct locations.
+# Find all nodes with weighted distance at most two from Alice.
 with model.query() as select:
-    r = Road()
-    weighted_distance = graph.compute.weighted_distance(r.from_, r.to)
-    response = select(r.from_.name, r.to.name, weighted_distance)
+    node = Person()
+    dist = graph.compute.weighted_distance(Person(name="Alice"), node)
+    dist <= 2.0
+    response = select(node.name, alias(dist, "distance"))
 
 print(response.results)
-# Output: 
-#           name        name2       v
-# 0  Los Angeles      Chicago  1100.0
-# 1  Los Angeles      Houston  1400.0
-# 2     New York      Chicago   800.0
-# 3     New York      Houston  1600.0
-# 4     New York  Los Angeles  2500.0
+# Output:
+#     name  distance
+# 0  Alice       0.0
+# 1    Bob       1.0
+# 2  Carol       1.5
 ```
 
 ## See Also
 
-[`distance()`](./distance.md)
+[`distance()`](./distance.md),
+[`.is_reachable()`](./is_reachable.md),
+and [`.reachable_from()`](./reachable_from.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,60 @@
-# `relationalai.std.graphs.Edge`
-
-The `Edge` class is used to represent the edge set of a graph.
-You do not need to create an `Edge` instance directly.
-Each `Graph` object has an `Edge` instance that you can access via [`Graph.Edge`](../Graph/Edge.md),
-which returns an instance of the `Edge` class.
-
-`Edge` objects behave similarly to [`Type`](../../../Type/README.md) objects,
-except that instead of returning [`Instance`](../../../Instance/README.md) objects,
-they return [`EdgeInstance`](../EdgeInstance/README.md) objects.
+# `relationalai.std.graphs.EdgeInstance.set()`
 
 ```python
-class relationalai.std.graphs.Edge(graph: Graph)
+EdgeInstance.set(**kwargs) -> EdgeInstance
 ```
 
+Sets properties on an [`EdgeInstance`](./README.md) object and returns the `EdgeInstance`.
+Note that unlike [`Instance.set()`](../../../Instance/set.md),
+you can't set a [`Type`](../../../Type/README.md) on an edge.
+Must be called in a [rule](../../Model/rule.md) or [query](../../Model/query.md) context.
+
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `graph` | [`Graph`](../Graph/README.md) | The graph on which the `Edges` object is instantiated. |
+| `*kwargs` | `Any` | Properties and values to set on the `EdgeInstance`. |
 
-## Methods
+## Returns
 
-- [`Edge.__call__()`](./call__.md)
-- [`Edge.add()`](./add.md)
-- [`Edge.extend()`](./extend.md)
+An [`EdgeInstance`](./README.md) object.
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named `socialNetwork` with a `Person` type.
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    alice.follows.add(bob)
 
-# Create a directed graph.
+# Create a directed graph with 'Person' nodes and 'follows' edges.
 graph = Graph(model)
-
-# Add edges to the graph based on the `follows` property.
-# Note that nodes are automatically added to the graph when edges are added.
 graph.Edge.extend(Person.follows)
 
-# You may add specific edges to a graph using the `Edge.add()` method inside of a rule.
+# Set the 'color' property of all edges to 'red'.
 with model.rule():
-    p = Person(name="Alice")
-    graph.Edge.add(from_=p, to=p.follows)
+    edge = graph.Edge()
+    edge.set(color="red")
 
-# To query edges, call the `Edge` object and select the desired properties.
+# Query the edges in the graph.
 with model.query() as select:
     edge = graph.Edge()
-    response = select(edge.from_.name, edge.to.name)
+    response = select(edge.from_.name, edge.to.name, edge.color)
 
 print(response.results)
 # Output:
-#   name  name2
-# 0  Bob  Alice
+#     name name2    v
+# 0  Alice   Bob  red
 ```
 
 ## See Also
 
-[`Graph.Edge`](../Graph/Edge.md) and [`Graph.Node`](../Graph/Node.md).
+[`Edge.add()`](../Edge/add.md) and [`Edge.extend()`](../Edge/extend.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,69 @@
-# `relationalai.std.graphs.Edge.__call__()`
+# `relationalai.std.graphs.Edge.add()`
 
 ```python
-relationalai.std.graphs.Edge.__call__(self, from_: Producer = None, to: Prodcuer = None, **kwargs) -> EdgeInstance
+relationalai.std.graphs.Edge.add(from_: Producer, to: Producer, **kwargs: Any) -> EdgeInstance
 ```
 
-Returns an [`EdgeInstance`](../EdgeInstance/README.md) object that produces
-edges matching that optional `from_` and `to` arguments with properties set to the provided keyword arguments.
-You must call an `Edge` instance from within a [rule](../Model/rule.md) or [query](../Model/query.md) context.
+Adds edges to the graph from objects produced by `from_` to objects produced by `to`.
+Edge properties may be passed as keyword arguments to `**kwargs`.
+Objects produced by `from_` and `to` are automatically added to the graph's [nodes](../Graph/Node.md).
+Must be called in a [rule](../Model/rule.md) or [query](../Model/query.md) context.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `from_` | [`Producer`](../../../Producer/README.md) | The node(s) that matched edges must have in the `from_` position. |
-| `to` | [`Producer`](../../../Producer/README.md) | The node(s) that matched edges must have in the `to` position. |
-| `*kwargs` | `Any` | Properties that matched edges must have set. |
+| `from_` | [`Producer`](../../Producer.md) | The node at the start of the edge. |
+| `to` | [`Producer`](../../Producer.md) | The node at the end of the edge. |
+| `**kwargs` | `Any` | Keyword arguments to set the edge's properties. |
 
 ## Returns
 
 An [`EdgeInstance`](../EdgeInstance/README.md) object.
 
 ## Example
 
-When you call an `Edge` object without any arguments it returns an [`EdgeInstance`](../Instance/README.md)
-that produces every edge in a graph:
+Use `Edge.add()` to add edges to the graph:
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model with `Person` and `Transaction` types.
-model = rai.Model("transactions2")
+# Create a model with 'Person' and 'Transaction' types.
+model = rai.Model("transactions")
 Person = model.Type("Person")
 Transaction = model.Type("Transaction")
 
 # Add some people and transactions to the model.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     Transaction.add(sender=bob, receiver=alice, amount=100.0)
 
-# Create a graph.
+# Create a directed graph.
 graph = Graph(model)
-graph.Node.extend(Person)
 
 # Add transactions to the graph as edges.
+# The 'weight' parameter sets the weight property of each edge.
 with model.rule():
     transaction = Transaction()
     graph.Edge.add(
         from_=transaction.sender,
         to=transaction.receiver,
         weight=transaction.amount
     )
 
-# Display all edges in the graph.
+# Query the edges in the graph.
 with model.query() as select:
     edge = graph.Edge()
     response = select(edge.from_.name, edge.to.name, edge.weight)
 
 print(response.results)
 # Output:
 #   name  name2      v
 # 0  Bob  Alice  100.0
 ```
 
-Pass property values as keyword arguments when you call a type to
-get an `EdgeInstance` that produces objects with those properties:
-
-```python
-with model.query() as select:
-    edge = graph.Edge(weight=100.0)
-
-print(response.results)
-# Output:
-#   name  name2      v
-# 0  Bob  Alice  100.0
-```
-
 ## See Also
 
-[`EdgeInstance`](../EdgeInstance/README.md)
+[`.extend()`](./extend.md) and [`Graph.Edge`](../Graph/Edge.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 # `relationalai.std.graphs.Edge.extend()`
 
 ```python
-relationalai.std.graph.Edge.extend(prop: Property, **kwargs: Any) -> None
+relationalai.std.graphs.Edge.extend(prop: Property, **kwargs: Any) -> None
 ```
 
 Add pairs of objects from a [`Property`](../../../Property.md) to a graph's edges.
 Edge properties may be passed as keyword arguments to `**kwargs`.
-You can use and display these properties in graph visualizations.
-Objects produced by the `prop` producer are automatically added to the graph's nodes.
+Objects produced by the property are automatically added to the graph's [nodes](../Graph/Node.md).
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `prop` | [`Property`](../../../Property.md) | The property from which edges are to be added. |
-| `**kwargs` | `Any` | Keyword arguments representing property name and value pairs. Values may be literals or `Producer` objects. |
+| `prop` | `Property` | The property to extend the graph's edges with. |
+| `**kwargs` | `Any` | Keyword arguments to set the edge's properties. |
 
 ## Returns
 
 `None`.
 
 ## Example
 
+Use `Edge.extend()` to add edges to the graph from a property.
+You do not need to call `.extend()` in a [rule](../Model/rule.md) or [query](../Model/query.md) context.
+
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model with a `Person` type.
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows="Bob")
+    alice.follows.add(bob)
 
-# Create a graph and extend the edges with the `Person.follows` property.
+# Create a directed graph.
 graph = Graph(model)
-graph.Node.extend(Person)
+
+# Extend the graph's edges with the 'Person.follows' property.
 graph.Edge.extend(Person.follows)
+
+# Query the edges in the graph.
+with model.query() as select:
+    edge = graph.Edge()
+    response = select(edge.from_.name, edge.to.name)
+
+print(response.results)
+# Output:
+#     name name2
+# 0  Alice   Bob
 ```
 
 ## See Also
 
-[`Edges.add()`](./add.md)
+[`.add()`](./add.md) and [`Graph.Edge`](../Graph/Edge.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/split_part.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,58 @@
-<!-- markdownlint-disable MD024 -->
-
-# `relationalai.std.graphs.EdgeInstance`
-
-`EdgeInstance` objects produce edges in graphs.
-They behave similarly to [`Instance`](../Instance/README.md) objects,
-but rather than representing a single object in a model,
-they represent a pair of objects in an edge relationship in a graph.
-As a result, you can't add `EdgeInstance` objects to `Type` objects.
-
-You create `EdgeInstance` objects by calling a graph's [`Edge`](../Graph/Edge.md) object.
+# `relational.std.strings.split_part()`
 
 ```python
-class relationalai.std.graphs.EdgeInstance(edge: Edge, from_: Producer, to: Producer, **kwargs)
+relationalai.std.strings.split_part(string: str | Producer, separator: str | Producer, index: int | Producer) -> Expression
 ```
 
+Returns an [`Expression`](../../Expression.md) object that produces the substring of `string` that is separated by `separator` at the given `index`.
+
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `edge` | [`Edge`](../Graph/Edge.md) | The `Edge` object from which the `EdgeInstance` is created. |
-| `from_` | [`Producer`](../Producer/README.md) | The source node(s) of the edge(s). |
-| `to` | [`Producer`](../Producer/README.md) | The `target node(s) or the edge(s). |
-| `**kwargs` | `Dict[str, Any]` | The properties of the edge(s). |
-
-## Attributes
+| `string` | `str` or [`Producer`](../../../Producer/README.md) | The string to split. |
+| `separator` | `str` or [`Producer`](../../../Producer/README.md) | The separator to split the string by. |
+| `index` | `int` or [`Producer`](../../../Producer/README.md) | The zero-based index of the substring to return. |
 
-- [`EdgeInstance.from_`](./from_.md)
-- [`EdgeInstance.to`](./to.md)
+## Returns
 
-## Methods
-
-- [`EdgeInstance.set()`](./set.md)
+An [`Expression`](../../Expression.md) object that producer `string` values.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std.graphs import Graph
+from relationalai.std.strings import split_part
 
-# Create a model with `Person` and `Transaction` types.
-model = rai.Model("socialNetwork")
+# Create a model named "people" with a Person type.
+model = rai.Model("people")
 Person = model.Type("Person")
 
-# Add some people and transactions to the model.
+# Add some people to the model.
+with model.rule():
+    alice = Person.add(name="Alice Smith")
+    bob = Person.add(name="Bob Jones")
+
+# Create 'first' and 'last' properties by splitting the 'name' property.
 with model.rule():
-    alice = Person.add(name="Alice")
-    bob = Person.add(name="Bob")
-    alice.set(follows=bob)
-
-# Create a graph and add edges to it.
-graph = Graph(model)
-graph.Edge.extend(Person.follows)
+    person = Person()
+    person.set(
+        first=split_part(person.name, " ", 0),
+        last=split_part(person.name, " ", 1)
+    )
 
-# Display the edges of the graph.
+# Query the 'first' and 'last' properties.
 with model.query() as select:
-    edge = graph.Edge()  # `edge` is an EdgeInstance object
-    response = select(edge.from_.name, edge.to.name)
+    person = Person()
+    response = select(person.first, person.last)
 
 print(response.results)
 # Output:
-#   name  name2
-# 0  Bob  Alice
+#    first   last
+# 0  Alice  Smith
+# 1    Bob  Jones
 ```
+
+## See Also
+
+[`split`](./split.md), [`join`](./join.md), and [`concat`](./concat.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-# `relationalai.std.graphs.EdgeInstance.from_`
+# `relationalai.std.graphs.EdgeInstance.to`
 
-Returns a `Producer` object that produces the source node(s) of the [`EdgeInstance`](./README.md).
+Returns a [`Producer`](../../../Producer/README.md) object that produces
+the terminal node of an edge.
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model with a `Person` type.
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a 'follows' property.
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    alice.follows.add(bob)
 
-# Create a graph and add edges to it.
+# Create a directed graph with 'Person' nodes and 'follows' edges.
 graph = Graph(model)
 graph.Edge.extend(Person.follows)
 
-# Display the source nodes of the edges.
+# Get the names of all people Alice follows.
 with model.query() as select:
-    edge = graph.Edge()
-    source_node = edge.from_
-    response = select(source_node.name)
+    edge = graph.Edge(from_=Person(name="Alice"))
+    follows = edge.to
+    response = select(follows.name)
 
 print(response.results)
 # Output:
-#     name
-# 0  Alice
+#   name
+# 0  Bob
 ```
 
 ## See Also
 
-- [`EdgeInstance.to`](./to.md)
+[`.from_`](./from_.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,40 @@
-# `relationalai.std.graphs.Graph.Node`
+# `relationalai.std.graphs.EdgeInstance.from_`
 
-A [`Type`](../../../Type/README.md) object representing the set of nodes in a graph.
-
-## Returns
-
-A [`Type`](../../../Type/README.md) object.
+Returns a [`Producer`](../../../Producer/README.md) object that produces
+the node at the start of an edge.
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model with a `Person` type.
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    alice.follows.add(bob)
 
-# Create a graph.
+# Create a directed graph with 'Person' nodes and 'follows' edges.
 graph = Graph(model)
+graph.Edge.extend(Person.follows)
 
-# Add all of the people in the model to the graph's nodes using `Node.extend()`.
-graph.Node.extend(Person, label=Person.name)
-
-# Alternatively, you can add specific nodes in a rule using `Node.add()`.
-with model.rule():
-    p = Person(name="Alice")
-    graph.Node.add(p, label=p.name)
-
-# You can query the nodes the same way you query any other `Type` object.
+# Get the names of all people following Bob.
 with model.query() as select:
-    node = graph.Node()
-    response = select(node.label)
+    edge = graph.Edge(to=Person(name="Bob"))
+    follower = edge.from_
+    response = select(follower.name)
 
 print(response.results)
 # Output:
-#    label
+#     name
 # 0  Alice
-# 1    Bob
 ```
 
 ## See Also
 
-[`Type`](../../../Type/README.md)
+[`.to`](./to.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/sin.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,59 @@
-# `relationalai.std.graphs.Graph.compute`
+# `relationalai.std.math.sin()`
 
-An attribute assigned to the graph's [`Compute`](../Compute/README.md) object.
+```python
+relationalai.std.math.sin(number: Number | Producer) -> Expression
+```
+
+Returns an [`Expression`](../../Expression.md) object that produces the sine of `number` radians.
+
+## Parameters
+
+| Name | Type | Description |
+| :--- | :--- | :--------- |
+| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the sine of. |
 
 ## Returns
 
-A [`Compute`](../Compute/README.md) object.
+An [`Expression`](../../Expression.md) object that produces `float` values.
 
 ## Example
 
-A graph's `.compute` object contains methods for computing graph analytical functions on graphs, such as PageRank:
+`sin()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
 
 ```python
 import relationalai as rai
-from relationalai.std.graphs import Graph
+from relationalai.std import alias
+from relationalai.std.math import sin
 
-# Create a model with a `Person` type.
-model = rai.Model("socialNetwork")
+# Create a model named "people" with a Person type.
+model = rai.Model("people")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add a person to the model.
 with model.rule():
-    alice = Person.add(name="Alice")
-    bob = Person.add(name="Bob")
-    alice.set(follows=bob)
-
-# Create a graph from the model add edges from the `Person.follows` property.
-graph = Graph(model)
-graph.Edge.extend(Person.follows)
+    Person.add(name="Alice", age=30)
 
-# Compute the PageRank of each person in the graph.
+# sin() works with numeric producers, such as a person's age property.
+# Inputs are assumed to be in radians.
 with model.query() as select:
     person = Person()
-    pagerank = graph.compute.pagerank(person)
-    response = select(person.name, pagerank)
+    response = select(person.name, alias(sin(person.age), "sin_age"))
 
 print(response.results)
 # Output:
-#     name         v
-# 0  Alice  0.350877
-# 1    Bob  0.649123
+#     name   sin_age
+# 0  Alice -0.988032
+
+# sin() also works with Python number objects.
+with model.query() as select:
+    response = select(sin(0))
+
+print(response.results)
+# Output:
+#      v
+# 0  0.0
 ```
 
-See [`Compute`](../Compute/README.md) for more information.
+## See Also
+
+[`asin()`](./asin.md), [`cos()`](./cos.md), and [`tan()`](./tan.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,82 @@
 # `relationalai.std.graphs.Graph.visualize()`
 
 ```python
-relationalai.std.graphs.Graph.visualize(three: bool = False, style: dict = {}, **kwargs) ->
+relationalai.std.graphs.Graph.visualize(three: bool = False, style: dict = {}, **kwargs) -> Figure
 ```
 
 Visualize a graph.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
 | `three` | `bool` | Whether or not to use the `three.js` 3D render engine. Defaults to `False`. |
-| `style` | `dict` | A dictionary with a `"nodes"` key and an `"edges"` key that defines the visual style of the graph.
+| `style` | `dict` | A dictionary of visual properties for nodes and edges. |
 | `**kwargs` | `Any` | Additional keyword arguments to pass to the gravis visualization library. See the [gravis docs](https://robert-haas.github.io/gravis-docs/index.html) for full details. |
 
 ## Returns
 
 A gravis [`Figure`](https://robert-haas.github.io/gravis-docs/rst/api/figure.html) object.
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model with a `Person` type.
+# Create a model with a 'Person' type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add people to the model connected by a multi-valued 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    alice.set(follows=bob)
+    alice.follows.add(bob)
 
 # Create a graph with edges from the `Person.follows` property.
 graph = Graph(model)
 graph.Node.extend(Person)
 graph.Edge.extend(Person.follows)
 
 # Visualize the graph.
 fig = graph.visualize()
+
+# In Jupyter notebooks, the figure is displayed inline.
+# For other environments, use the `.display()` method to open the figure in a new browser window.
 fig.display()
 ```
 
-The figure opens in a new web browser window.
-
 ![A graph with two nodes and one edge.](./img/graph-viz.png)
 
-> [!TIP]
-> In a Jupyter Notebook, `graph.visualize()` will display the figure.
-> You do not need to assign the figure to a variable and call the `.display()` method.
-
 You may change the label, color, and size of nodes and edges:
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model with a `Person` type.
+# Create a model with 'Person' and 'Brand' types.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 Brand = model.Type("Brand")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the model and connect them with a multi-valued `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     acme = Brand.add(name="Acme")
-    alice.set(follows=bob).set(follows=acme)
-    bob.set(follows=acme)
+    alice.follows.extend([bob, acme])
+    bob.follows.add(acme)
 
-# Create a graph with edges from the `Person.follows` property.
+# Create a directed graph with 'Person' and 'Brand' nodes and 'follows' edges.
 graph = Graph(model)
 graph.Node.extend(Person, label=Person.name, color="blue")
 graph.Node.extend(Brand, label=Brand.name, color="red")
-graph.Edge.extend(Person.follows)
+graph.Edge.extend(Person.follows, label="follows")
 
 # Compute the PageRank of people in the graph and use it for the node's size.
 with model.rule():
     person = Person()
     rank = graph.compute.pagerank(person)
     graph.Node.add(person, size=rank * 50)
 
@@ -92,44 +89,44 @@
 You can also describe the visual properties of nodes and edges by passing a dictionary to the `style` parameter.
 The following example produces the same visualization as the preceding example:
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model with a `Person` type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 Brand = model.Type("Brand")
 
-# Add some people to the model and connect them with a `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     acme = Brand.add(name="Acme")
-    alice.set(follows=bob).set(follows=acme)
-    bob.set(follows=acme)
+    alice.follows.extend([bob, acme])
+    bob.follows.add(acme)
 
-# Create a graph with edges from the `Person.follows` property.
 graph = Graph(model)
 graph.Node.extend(Person, kind="person")
 graph.Node.extend(Brand, kind="brand")
 graph.Edge.extend(Person.follows)
 
-# Compute the PageRank of people in the graph and use it for the node's size.
+
 with model.rule():
     person = Person()
     rank = graph.compute.pagerank(person)
     graph.Node.add(person)
 
 graph.visualize(style={
     "nodes": {
+        # Color nodes by their 'kind' property.
         "color": lambda n: {"person": "blue", "brand": "red"}.get(n["kind"]),
+        # Size nodes by their 'rank' property and scale them.
         "size": lambda n: n.get("rank", 1.0) * 50,
     },
-    "edges": {}
+    # Label edges as "follows."
+    "edges": {"label": "follows"}
 })
 ```
 
 ## See Also
 
-[`Graph.visualize()`](./visualize.md)
+[`.fetch()`](./fetch.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.3.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/abs.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/abs.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/acos.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/tan.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,59 @@
-# `relationalai.std.math.acos()`
+# `relationalai.std.math.tan()`
 
 ```python
-relationalai.std.math.acos(number: Number | Producer) -> Expression
+relationalai.std.math.tan(number: Number | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) object that produces the arccosine of `number` radians.
+Returns an [`Expression`](../../Expression.md) object that produces the tangent of `number` radians.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :--------- |
-| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the arccosine of. |
+| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the tangent of. |
 
 ## Returns
 
 An [`Expression`](../../Expression.md) object that produces `float` values.
 
 ## Example
 
-`acos()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
+`tan()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
 
 ```python
 import relationalai as rai
 from relationalai.std import alias
-from relationalai.std.math import acos
+from relationalai.std.math import tan
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add a person to the model.
 with model.rule():
-    Person.add(name="Alice", age=3, height_m=0.95)
+    Person.add(name="Alice", age=30)
 
-# acos() works with numeric producers, such as a person's height property.
+# tan() works with numeric producers, such as a person's age property.
 # Inputs are assumed to be in radians.
 with model.query() as select:
     person = Person()
-    response = select(person.name, alias(acos(person.height_m), "acos_height"))
+    response = select(person.name, alias(tan(person.age), "tan_age"))
 
 print(response.results)
 # Output:
-#     name  acos_height
-# 0  Alice      0.31756
+#     name   tan_age
+# 0  Alice -6.405331
 
-# acos() also works with Python number objects.
+# tan() also works with Python number objects.
 with model.query() as select:
-    response = select(acos(0))
+    response = select(tan(0))
 
 print(response.results)
 # Output:
-#           v
-# 0  1.570796
-```
-
-The input to `acos()` must be in the range -1 to 1, inclusive.
-If the input is outside this range,
-the [query](../../Model/query.md) or [rule](../../Model/rule.md) will be impossible to satisfy:
-
-```python
-with model.query() as select:
-    person = Person()
-    response = select(person.name, alias(acos(person.age), "acos_age"))
-
-print(response.results)
-# Output:
-# Empty DataFrame
-# Columns: []
-# Index: []
+#      v
+# 0  0.0
 ```
 
 ## See Also
 
-[`cos()`](./cos.md), [`asin()`](./asin.md), and [`atan()`](./atan.md).
+[`atan()`](./atan.md), [`cos()`](./cos.md), and [`sin()`](./sin.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/asin.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/atan.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,59 @@
-# `relationalai.std.math.asin()`
+# `relationalai.std.math.atan()`
 
 ```python
-relationalai.std.math.asin(number: Number | Producer) -> Expression
+relationalai.std.math.atan(number: Number | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) object that produces the arcsine of `number` radians.
+Returns an [`Expression`](../../Expression.md) object that produces the arctangent of `number` radians.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :--------- |
-| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the arcsine of. |
+| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the arctangent of. |
 
 ## Returns
 
 An [`Expression`](../../Expression.md) object that produces `float` values.
 
 ## Example
 
-`asin()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
+`atan()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
 
 ```python
 import relationalai as rai
 from relationalai.std import alias
-from relationalai.std.math import asin
+from relationalai.std.math import atan
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add a person to the model.
 with model.rule():
     Person.add(name="Alice", age=3, height_m=0.95)
 
-# asin() works with numeric producers, such as a person's height property.
+# atan() works with numeric producers, such as a person's height property.
 # Inputs are assumed to be in radians.
 with model.query() as select:
     person = Person()
-    response = select(person.name, alias(asin(person.height_m), "asin_height"))
+    response = select(person.name, alias(atan(person.height_m), "atan_height"))
 
 print(response.results)
 # Output:
-#     name  asin_height
-# 0  Alice     1.253236
+#     name  atan_height
+# 0  Alice     0.759763
 
-# asin() also works with Python number objects.
+# atan() also works with Python number objects.
 with model.query() as select:
-    response = select(asin(0))
+    response = select(atan(0))
 
 print(response.results)
 # Output:
-#           v
-# 0  1.570796
-```
-
-The input to `asin()` must be in the range -1 to 1, inclusive.
-If the input is outside this range,
-the [query](../../Model/query.md) or [rule](../../Model/rule.md) will be impossible to satisfy:
-
-```python
-with model.query() as select:
-    person = Person()
-    response = select(person.name, alias(asin(person.age), "asin_age"))
-
-print(response.results)
-# Output:
-# Empty DataFrame
-# Columns: []
-# Index: []
+#      v
+# 0  0.0
 ```
 
 ## See Also
 
-[`sin()`](./sin.md), [`acos()`](./acos.md), and [`atan()`](./atan.md).
+[`tan()`](./sin.md), [`acos()`](./acos.md), and [`asin()`](./asin.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/atan.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/radians.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-# `relationalai.std.math.atan()`
+# `relationalai.std.math.radians()`
 
 ```python
-relationalai.std.math.atan(number: Number | Producer) -> Expression
+relationalai.std.math.radians(degrees: Number | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) object that produces the arctangent of `number` radians.
+Returns an [`Expression`](../../Expression.md) object that produces the equivalent number of `degrees` in radians.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :--------- |
-| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the arctangent of. |
+| `degrees` | `Number` or [`Producer`](../../Producer/README.md) | The number of degrees to convert to radians. |
 
 ## Returns
 
 An [`Expression`](../../Expression.md) object that produces `float` values.
 
 ## Example
 
-`atan()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
+`radians()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
 
 ```python
 import relationalai as rai
 from relationalai.std import alias
-from relationalai.std.math import atan
+from relationalai.std.math import radians
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add a person to the model.
 with model.rule():
-    Person.add(name="Alice", age=3, height_m=0.95)
+    Person.add(name="Alice", age=30)
 
-# atan() works with numeric producers, such as a person's height property.
-# Inputs are assumed to be in radians.
+# radians() works with numeric producers, such as a person's age property.
 with model.query() as select:
     person = Person()
-    response = select(person.name, alias(atan(person.height_m), "atan_height"))
+    response = select(person.name, alias(radians(person.age), "radians_age"))
 
 print(response.results)
 # Output:
-#     name  atan_height
-# 0  Alice     0.759763
+#     name  radians_age
+# 0  Alice     0.523599
 
-# atan() also works with Python number objects.
+# radians() also works with Python number objects.
 with model.query() as select:
-    response = select(atan(0))
+    response = select(radians(180))
 
 print(response.results)
 # Output:
-#      v
-# 0  0.0
+#           v
+# 0  3.141593
 ```
 
 ## See Also
 
-[`tan()`](./sin.md), [`acos()`](./acos.md), and [`asin()`](./asin.md).
+[`degrees()`](./degrees.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/cbrt.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/cbrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/ceil.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/ceil.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/cos.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/concat.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,68 @@
-# `relationalai.std.math.cos()`
+# `relational.std.strings.concat()`
 
 ```python
-relationalai.std.math.cos(number: Number | Producer) -> Expression
+relationalai.std.strings.concat(string1: str | Producer, string2: str | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) object that produces the cosine of `number` radians.
+Returns an [`Expression`](../../Expression.md) that produces strings by concatenating `string1` and `string2`.
 
 ## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :--------- |
-| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the cosine of. |
+| :--- | :--- | :------ |
+| `string1` | `str` or [`Producer`](../../../Producer/README.md) | A string or a producer that produces string values. |
+| `string2` | `str` or [`Producer`](../../../Producer/README.md) | A string or a producer that produces string values. |
 
 ## Returns
 
-An [`Expression`](../../Expression.md) object that produces `float` values.
+An [`Expression`](../../../Expression.md) object.
 
 ## Example
 
-`cos()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
-
 ```python
 import relationalai as rai
-from relationalai.std import alias
-from relationalai.std.math import cos
+from relationalai.std.strings import concat
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
-# Add a person to the model.
+# Add some people to the model.
 with model.rule():
-    Person.add(name="Alice", age=30)
+    alice = Person.add(first="Alice", last="Smith")
+    bob = Person.add(first="Bob", last="Jones")
 
-# cos() works with numeric producers, such as a person's age property.
-# Inputs are assumed to be in radians.
+# Concatenate the first and last names of all people.
 with model.query() as select:
     person = Person()
-    response = select(person.name, alias(cos(person.age), "cos_age"))
+    full_name = concat(person.first, person.last)
+    response = select(full_name)
 
 print(response.results)
 # Output:
-#     name   cos_age
-# 0  Alice  0.154251
+#             v
+# 0  AliceSmith
+# 1    BobJones
+```
+
+To add a space between the first and last names, you can concatenate a space string with last name:
 
-# cos() also works with Python number objects.
+```python
+concat = std.strings.concat
 with model.query() as select:
-    response = select(cos(0))
+    person = Person()
+    full_name = concat(person.first, concat(" ", person.last))
+    # Alternatively, you could use std.strings.join:
+    # full_name = join([person.first, person.last], " ")
+    response = select(full_name)
 
 print(response.results)
 # Output:
-#      v
-# 0  1.0
+#              v
+# 0  Alice Smith
+# 1    Bob Jones
 ```
 
 ## See Also
 
-[`acos()`](./acos.md), [`sin()`](./sin.md), and [`tan()`](./tan.md).
+[`join`](./join.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/degrees.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/degrees.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/floor.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/floor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/isclose.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/isclose.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/log.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/log.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/radians.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/contains.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-# `relationalai.std.math.radians()`
+# `relational.std.strings.contains()`
 
 ```python
-relationalai.std.math.radians(degrees: Number | Producer) -> Expression
+relationalai.std.strings.contains(string: str | Producer, substring: str | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) object that produces the equivalent number of `degrees` in radians.
+Adds a constraint to a [rule](../../Model/rule.md) or [query](../../Model/query.md) that
+`string` must contain the substring `substring`.
 
 ## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :--------- |
-| `degrees` | `Number` or [`Producer`](../../Producer/README.md) | The number of degrees to convert to radians. |
+| :--- | :--- | :------ |
+| `string` | [`Producer`](../../../Producer/README.md) | The string to check. |
+| `substring` | `str` or [`Producer`](../../../Producer/README.md) | The substring to check for. |
 
 ## Returns
 
-An [`Expression`](../../Expression.md) object that produces `float` values.
+An [`Expression`](../../../Expression.md) object.
 
 ## Example
 
-`radians()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
-
 ```python
 import relationalai as rai
-from relationalai.std import alias
-from relationalai.std.math import radians
+from relationalai.std.strings import contains
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
-# Add a person to the model.
+# Add some people to the model.
 with model.rule():
-    Person.add(name="Alice", age=30)
+    alice = Person.add(name="Alice")
+    bob = Person.add(name="Bob")
 
-# radians() works with numeric producers, such as a person's age property.
+# Get all people whose name contains "Ali".
 with model.query() as select:
     person = Person()
-    response = select(person.name, alias(radians(person.age), "radians_age"))
+    contains(person.name, "Ali")
+    response = select(person.name)
 
 print(response.results)
 # Output:
-#     name  radians_age
-# 0  Alice     0.523599
+#     name
+# 0  Alice
 
-# radians() also works with Python number objects.
+# The `substring` argument can also be a Producer.
 with model.query() as select:
-    response = select(radians(180))
+    sub = Person(name="Bob").name
+    person = Person()
+    contains(person.name, sub)
+    response = select(person.name)
 
 print(response.results)
 # Output:
-#           v
-# 0  3.141593
+#    name
+# 0   Bob
 ```
 
 ## See Also
 
-[`degrees()`](./degrees.md)
+[`ends_with`](./ends_with.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/sign.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/sign.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/sin.md` & `relationalai-0.3.0/docs/api_reference/python/std/math/sqrt.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-# `relationalai.std.math.sin()`
+# `relationalai.std.math.sqrt()`
 
 ```python
-relationalai.std.math.sin(number: Number | Producer) -> Expression
+relationalai.std.math.sqrt(number: Number | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) object that produces the sine of `number` radians.
+Returns an [`Expression`](../../Expression.md) that produces the square root of `number`.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :--------- |
-| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the sine of. |
+| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the square root of. |
 
 ## Returns
 
-An [`Expression`](../../Expression.md) object that produces `float` values.
+An [`Expression`](../../Expression.md) object.
 
 ## Example
 
-`sin()` works with both numeric [producers](../../Producer/README.md) and Python number objects:
-
 ```python
 import relationalai as rai
 from relationalai.std import alias
-from relationalai.std.math import sin
+from relationalai.std.math import sqrt
 
-# Create a model named "people" with a Person type.
+# Create a model with a `Person` type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
-# Add a person to the model.
+# Add some people to the model.
 with model.rule():
-    Person.add(name="Alice", age=30)
-
-# sin() works with numeric producers, such as a person's age property.
-# Inputs are assumed to be in radians.
-with model.query() as select:
-    person = Person()
-    response = select(person.name, alias(sin(person.age), "sin_age"))
-
-print(response.results)
-# Output:
-#     name   sin_age
-# 0  Alice -0.988032
+    Person.add(name="Alice", age=9)
+    Person.add(name="Bob", age=16)
+    Person.add(name="Charlie", age=25)
 
-# sin() also works with Python number objects.
+# What is the square root of each person's age?
 with model.query() as select:
-    response = select(sin(0))
+    p = Person()
+    age_sqrt = sqrt(p.age)
+    response = select(p.name, alias(age_sqrt, "age_sqrt"))
 
 print(response.results)
 # Output:
-#      v
-# 0  0.0
+#       name  age_cbrt
+# 0    Alice       3.0
+# 1      Bob       4.0
+# 2  Charlie       5.0
 ```
 
 ## See Also
 
-[`asin()`](./asin.md), [`cos()`](./cos.md), and [`tan()`](./tan.md).
+[`cbrt()`](./cbrt.md) and [`**`](../../Producer/pow__.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/sqrt.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/regex_match.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-# `relationalai.std.math.sqrt()`
+# `relational.std.strings.regex_match()`
 
 ```python
-relationalai.std.math.sqrt(number: Number | Producer) -> Expression
+relationalai.std.strings.regex_match(string: str | Producer, regex: str | Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) that produces the square root of `number`.
+Adds a constraint to a [rule](../../Model/rule.md) or [query](../../Model/query.md) that
+`string` must match the regular expression `regex`.
 
 ## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :--------- |
-| `number` | `Number` or [`Producer`](../../Producer/README.md) | The number to take the square root of. |
+| :--- | :--- | :------ |
+| `string` | `str` or [`Producer`](../../../Producer/README.md) | The string to match against. |
+| `regex` | `str` or [`Producer`](../../../Producer/README.md) | A string containing a regular expression. |
 
 ## Returns
 
-An [`Expression`](../../Expression.md) object.
+An [`Expression`](../../../Expression.md) object.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std import alias
-from relationalai.std.math import sqrt
+from relationalai.std.strings import like
 
-# Create a model with a `Person` type.
+# Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add some people to the model.
 with model.rule():
-    Person.add(name="Alice", age=9)
-    Person.add(name="Bob", age=16)
-    Person.add(name="Charlie", age=25)
+    alice = Person.add(name="Alice")
+    bob = Person.add(name="Bob")
 
-# What is the square root of each person's age?
+# Get all people whose name ends with "ice".
 with model.query() as select:
-    p = Person()
-    age_sqrt = sqrt(p.age)
-    response = select(p.name, alias(age_sqrt, "age_sqrt"))
+    person = Person()
+    regex_match(person.name, r"Ali.*")
+    response = select(person.name)
 
 print(response.results)
 # Output:
-#       name  age_cbrt
-# 0    Alice       3.0
-# 1      Bob       4.0
-# 2  Charlie       5.0
+#     name
+# 0  Alice
 ```
 
 ## See Also
 
-[`cbrt()`](./cbrt.md) and [`**`](../../Producer/pow__.md).
+[`regex_compile`](./regex_compile.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/math/trunc_divide.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/split.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-# `relationalai.std.math.trunc_divide()`
+# `relational.std.strings.split()`
 
 ```python
-relationalai.std.math.trunc_divide(numerator: Number | Producer, denominator: Number | Producer) -> Expression
+relationalai.std.strings.split(string: str | Producer, separator: str | Producer) -> tuple[Expression]
 ```
 
-Returns an [`Expression`](../../Expression.md) that produces the result of the division of `numerator` by `denominator`, rounded towards zero.
-The type of the result is the same as the type of the `numerator`.
+Returns a tuple of [`Expression`](../../Expression.md) objects
+where the first element produces the zero-based indices of each substring in `string` that is separated by `separator`
+and the second element produces the substrings themselves.
 
 ## Parameters
 
 | Name | Type | Description |
-| :--- | :--- | :--------- |
-| `numerator` | `Number` or [`Producer`](../../Producer/README.md) | The numerator of the division. |
-| `denominator` | `Number` or [`Producer`](../../Producer/README.md) | The denominator of the division. |
+| :--- | :--- | :------ |
+| `string` | `str` or [`Producer`](../../../Producer/README.md) | A string or a producer that produces string values. |
+| `separator` | `str` or [`Producer`](../../../Producer/README.md) | A string or a producer that produces string values. |
 
 ## Returns
 
-An [`Expression`](../../Expression.md) object.
+A tuple of two [`Expression`](../../Expression.md) objects.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std import alias
-from relationalai.std.math import trunc_divide
+from relationalai.std.strings import split
 
-# Create a model with a `Person` type.
+# Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add some people to the model.
 with model.rule():
-    Person.add(name="Alice", height_cm=170.1)
-    Person.add(name="Bob", height_cm=180)
+    alice = Person.add(name="Alice Smith")
+    bob = Person.add(name="Bob Jones")
 
-# What is each person's height rounded down to the nearest whole number?
+# Create 'first' and 'last' properties by splitting the 'name' property.
+with model.rule():
+    person = Person()
+    index, substring = split(person.name, " ")
+    with index == 0:
+        person.set(first=substring)
+    with index == 1:
+        person.set(last=substring)
+
+# Query the 'first' and 'last' properties.
 with model.query() as select:
-    p = Person()
-    half_height = trunc_divide(p.height_cm, 2)
-    response = select(p.name, alias(half_height, "half_height"))
+    person = Person()
+    response = select(person.first, person.last)
 
 print(response.results)
 # Output:
-#     name  half_height
-# 0  Alice         85.0
-# 1    Bob         90.0
+#    first   last
+# 0  Alice  Smith
+# 1    Bob  Jones
 ```
 
 ## See Also
 
-[`//`](../../Producer/floordiv__.md) (floor division) and [`/`](../../Producer/truediv__.md) (true division).
+[`split_part`](./split_part.md), [`join`](./join.md), and [`concat`](./concat.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/README.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/uppercase.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,50 @@
-# `relational.std.strings.concat()`
+# `relational.std.strings.uppercase()`
 
 ```python
-relationalai.std.strings.concat(string1: str | Producer, string2: str | Producer) -> Expression
+relationalai.std.strings.uppercase(string: Producer) -> Expression
 ```
 
-Returns an [`Expression`](../../Expression.md) that produces strings by concatenating `string1` and `string2`.
+Returns an [`Expression`](../../Expression.md) that produces the uppercase version
+of the strings produced by the `string` producer.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `string1` | `str` or [`Producer`](../../../Producer/README.md) | A string or a producer that produces string values. |
-| `string2` | `str` or [`Producer`](../../../Producer/README.md) | A string or a producer that produces string values. |
+| `string` | [`Producer`](../../../Producer/README.md) | A producer that produces string values. |
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object.
+An [`Expression`](../../../Expression.md) object that produce uppercase strings.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std.strings import concat
+from relationalai.std.strings import uppercase
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add some people to the model.
 with model.rule():
-    alice = Person.add(first="Alice", last="Smith")
-    bob = Person.add(first="Bob", last="Jones")
+    alice = Person.add(name="Alice")
+    bob = Person.add(name="Bob")
 
-# Concatenate the first and last names of all people.
+# Get all people whose name ends with "ice".
 with model.query() as select:
     person = Person()
-    full_name = concat(person.first, person.last)
-    response = select(full_name)
+    name_upper = uppercase(person.name)
+    response = select(person.name, name_upper)
 
 print(response.results)
 # Output:
-#             v
-# 0  AliceSmith
-# 1    BobJones
-```
-
-To add a space between the first and last names, you can concatenate a space string with last name:
-
-```python
-concat = std.strings.concat
-with model.query() as select:
-    person = Person()
-    full_name = concat(person.first, concat(" ", person.last))
-    # Alternatively, you could use std.strings.join:
-    # full_name = join([person.first, person.last], " ")
-    response = select(full_name)
-
-print(response.results)
-# Output:
-#              v
-# 0  Alice Smith
-# 1    Bob Jones
+#     name      v
+# 0  Alice  ALICE
+# 1    Bob    BOB
 ```
 
 ## See Also
 
-[`join`](./join.md)
+[`lowercase`](./lowercase.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/ends_with.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-# `relational.std.strings.contains()`
+# `relational.std.strings.ends_with()`
 
 ```python
-relationalai.std.strings.contains(string: str | Producer, substring: str | Producer) -> Expression
+relationalai.std.strings.ends_with(string: Producer, suffix: str | Producer) -> Expression
 ```
 
-Adds a constraint to a [rule](../../Model/rule.md) or [query](../../Model/query.md) that
-`string` must contain the substring `substring`.
+Constrains the `string` Producer to only values that end in `suffix`.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `string` | [`Producer`](../../../Producer/README.md) | The string to check. |
-| `substring` | `str` or [`Producer`](../../../Producer/README.md) | The substring to check for. |
+| `string` | [`Producer`](../../../Producer/README.md) | A producer that produces string values. |
+| `suffix` | `str` or [`Producer`](../../../Producer/README.md) | The substring to check for. |
 
 ## Returns
 
 An [`Expression`](../../../Expression.md) object.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std.strings import contains
+from relationalai.std.strings import ends_with
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add some people to the model.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
 
-# Get all people whose name contains "Ali".
+# Get all people whose name ends with "ice".
 with model.query() as select:
     person = Person()
-    contains(person.name, "Ali")
+    ends_with(person.name, "Ali")
     response = select(person.name)
 
 print(response.results)
 # Output:
 #     name
 # 0  Alice
 
 # The `substring` argument can also be a Producer.
 with model.query() as select:
     sub = Person(name="Bob").name
     person = Person()
-    contains(person.name, sub)
+    ends_with(person.name, sub)
     response = select(person.name)
 
 print(response.results)
 # Output:
 #    name
 # 0   Bob
 ```
 
 ## See Also
 
-[`ends_with`](./ends_with.md)
+[`contains`](./contains.md)
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/like.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,54 @@
-# `relational.std.strings.ends_with()`
+# `relational.std.strings.like()`
 
 ```python
-relationalai.std.strings.ends_with(string: Producer, suffix: str | Producer) -> Expression
+relationalai.std.strings.like(string: str | Producer, pattern: str | Producer) -> Expression
 ```
 
-Constrains the `string` Producer to only values that end in `suffix`.
+Adds a constraint to a [rule](../../Model/rule.md) or [query](../../Model/query.md) that
+`string` must match the SQL LIKE pattern `pattern`.
+The `%` character acts as a wildcard, matching any sequence of characters.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `string` | [`Producer`](../../../Producer/README.md) | A producer that produces string values. |
-| `suffix` | `str` or [`Producer`](../../../Producer/README.md) | The substring to check for. |
+| `string` | `str` or [`Producer`](../../../Producer/README.md) | The string to match against. |
+| `pattern` | `str` or [`Producer`](../../../Producer/README.md) | A SQL LIKE pattern. |
 
 ## Returns
 
 An [`Expression`](../../../Expression.md) object.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std.strings import ends_with
+from relationalai.std.strings import like
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add some people to the model.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
 
-# Get all people whose name ends with "ice".
+# Get all people whose name contains 'li'.
 with model.query() as select:
     person = Person()
-    ends_with(person.name, "Ali")
+    like(person.name, "%li%")
     response = select(person.name)
 
 print(response.results)
 # Output:
 #     name
 # 0  Alice
-
-# The `substring` argument can also be a Producer.
-with model.query() as select:
-    sub = Person(name="Bob").name
-    person = Person()
-    ends_with(person.name, sub)
-    response = select(person.name)
-
-print(response.results)
-# Output:
-#    name
-# 0   Bob
 ```
 
 ## See Also
 
-[`contains`](./contains.md)
+[`contains`](./contains.md),
+[`ends_with`](./ends_with.md),
+[`regex_match`](./regex_match.md),
+and [`starts_with`](./starts_with.md).
```

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/join.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/length.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/regex_compile.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/regex_compile.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/docs/api_reference/python/std/strings/regex_match.md` & `relationalai-0.3.0/docs/api_reference/python/std/strings/replace.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-# `relational.std.strings.regex_match()`
+# `relational.std.strings.replace()
 
 ```python
-relationalai.std.strings.regex_match(string: str | Producer, regex: str | Producer) -> Expression
+relationalai.std.strings.replace(string: Producer, old: str | Producer, new: str | Producer) -> Expression
 ```
 
-Adds a constraint to a [rule](../../Model/rule.md) or [query](../../Model/query.md) that
-`string` must match the regular expression `regex`.
+Returns an [`Expression`](../../Expression.md) that produces strings by replacing all occurrences of the substring `old` in strings from the `string` Producer with the substring `new`.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `string` | `str` or [`Producer`](../../../Producer/README.md) | The string to match against. |
-| `regex` | `str` or [`Producer`](../../../Producer/README.md) | A string containing a regular expression. |
+| `string` | `str` or [`Producer`](../../../Producer/README.md) | A string or a producer that produces string values. |
+| `old` | `str` or [`Producer`](../../../Producer/README.md) | The substring to replace. |
+| `new` | `str` or [`Producer`](../../../Producer/README.md) | The substring to replace `old` with. |
 
 ## Returns
 
 An [`Expression`](../../../Expression.md) object.
 
 ## Example
 
 ```python
 import relationalai as rai
-from relationalai.std.strings import like
+from relationalai.std.strings import replace
 
 # Create a model named "people" with a Person type.
 model = rai.Model("people")
 Person = model.Type("Person")
 
 # Add some people to the model.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
 
-# Get all people whose name ends with "ice".
+# Replace all occurrences of "ice" with "icia".
 with model.query() as select:
     person = Person()
-    regex_match(person.name, r"Ali.*")
-    response = select(person.name)
+    replaced_name = replace(person.name, "ice", "icia")
+    response = select(replaced_name)
 
 print(response.results)
 # Output:
-#     name
-# 0  Alice
+#     name       v
+# 0  Alice  Alicia
+# 1    Bob     Bob
 ```
-
-## See Also
-
-[`regex_compile`](./regex_compile.md).
```

### Comparing `relationalai-0.2.9/docs/faq/engines.md` & `relationalai-0.3.0/docs/faq/engines.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,7 +48,17 @@
 
 For large inputs, graph algorithms generally aim to utilize all resources on an engine.
 Run at most one large scale graph algorithm per engine at a time.
 
 Each active Snowflake schema requires memory on an engine.
 Avoid interacting with more than two or three schemas through a single engine at a time.
 Always prefer working with the same engine on the same schema and avoid mixing, as juggling too many active schemas will degrade engine performance.
+
+Billing is based on engine run-time, not usage.
+To minimize costs, shut down your engine when not in use.
+However, frequent restarts incur warm-up costs, both financial and in terms of performance.
+You may want to keep an engine running if you expect to use it again soon.
+In the future, policies for automated cost management will be provided.
+
+Engines responsible for maintaining streams from Snowflake to RelationalAI should be kept running
+to ensure that changes to your Snowflake tables are available right away.
+If you do shut down a stream's engine, changes to the data are synced when the engine is restarted.
```

### Comparing `relationalai-0.2.9/examples/README.md` & `relationalai-0.3.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/cdc.py` & `relationalai-0.3.0/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/custom_snowflake_connection.py` & `relationalai-0.3.0/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/emit_playground.py` & `relationalai-0.3.0/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/found.py` & `relationalai-0.3.0/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/fraud.ipynb` & `relationalai-0.3.0/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/fraud.py` & `relationalai-0.3.0/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/graph_algos.py` & `relationalai-0.3.0/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/nested.py` & `relationalai-0.3.0/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/or_types.py` & `relationalai-0.3.0/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/remote_load_csv.py` & `relationalai-0.3.0/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/simple_recursion.py` & `relationalai-0.3.0/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/simple_streamlit.py` & `relationalai-0.3.0/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/solver.py` & `relationalai-0.3.0/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/weighted_graph_algos.py` & `relationalai-0.3.0/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/articles_graph/README.md` & `relationalai-0.3.0/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/articles_graph/articles_graph.py` & `relationalai-0.3.0/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.3.0/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/articles_graph/utils.py` & `relationalai-0.3.0/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.3.0/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/data/people.csv` & `relationalai-0.3.0/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/data/transactions.csv` & `relationalai-0.3.0/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/ev_penetration/ev_penetration.py` & `relationalai-0.3.0/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.3.0/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/ev_penetration/state_stats.csv` & `relationalai-0.3.0/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/imdb/README.md` & `relationalai-0.3.0/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/imdb/imdb.csv` & `relationalai-0.3.0/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/imdb/imdb.py` & `relationalai-0.3.0/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/rel/solver.rel` & `relationalai-0.3.0/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.3.0/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.3.0/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.3.0/examples/social-money-network/snowflake_pagerank.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 #pyright: reportUnusedExpression=false
 from typing import Tuple
 import rich
 import relationalai as rai
 from relationalai.std import aggregates
 from relationalai.std.graphs import Graph
-from relationalai.clients.snowflake import Snowflake, PrimaryKey
 
-model = rai.Model("SFPagerank", dry_run=False)
+model = rai.Model("SFPagerank")
 
 #--------------------------------------------------
 # Initialize Snowflake data
 #--------------------------------------------------
 
-sf = Snowflake(model)
-Account = sf.sandbox.public.accounts
-Account.describe(
-    account_id=PrimaryKey,
-)
+Account = model.Type("Account", source="sandbox.public.accounts")
 
-Transaction = sf.sandbox.public.transactions
-Transaction.describe(
-    id=PrimaryKey,
-    from_account=(Account, "from_"),
-    to_account=(Account, "to")
+Transaction = model.Type("Account", source="sandbox.public.transactions")
+Transaction.define(
+    from_ = (Account, "from_account", "account_id"),
+    to = (Account, "to_account", "account_id")
 )
 
 #--------------------------------------------------
 # Add types
 #--------------------------------------------------
 
 Merchant = model.Type("Merchant")
@@ -95,14 +89,7 @@
     t = Transaction(to=m)
     total = aggregates.sum(t, t.amount, per=[m])
     return m.name, m.rank, total #type: ignore
 
 print("\nCalling merchant rank from Snowflake!\n")
 for row in model.resources._exec("call sandbox.public.merchant_rank(0.04);"):
     rich.print(row)
-
-
-
-
-
-
-
```

### Comparing `relationalai-0.2.9/frontend/debugger/package-lock.json` & `relationalai-0.3.0/frontend/debugger/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916772000025983%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'@solid-primitives/date': '^2.0.21', "*

 * *               "'@solid-primitives/timer': '^1.3.9', 'gradient-path': '^2.3.0', 'vitest': "*

 * *               "'^1.6.0'}, 'devDependencies': {'jsdom': '^24.0.0'}, 'engines': "*

 * *               "OrderedDict([('node', '22.1.0'), ('npm', '10.7.0')])}, "*

 * *               "'node_modules/@adobe/css-tools': {'devOptional': True, delete: ['dev']}, "*

 * *               "'node_modules/@esbuild/aix-ppc64': {delete: ['dev']}, "*

 * *               "'node_mod […]*

```diff
@@ -1,44 +1,53 @@
 {
     "lockfileVersion": 3,
     "name": "relationalai-debugger-ui",
     "packages": {
         "": {
             "dependencies": {
                 "@kobalte/core": "^0.12.6",
+                "@solid-primitives/date": "^2.0.21",
+                "@solid-primitives/timer": "^1.3.9",
                 "@tabler/icons": "^3.1.0",
+                "gradient-path": "^2.3.0",
                 "prismjs": "^1.29.0",
-                "solid-js": "^1.8.11"
+                "solid-js": "^1.8.11",
+                "vitest": "^1.6.0"
             },
             "devDependencies": {
                 "@chromatic-com/storybook": "^1.2.25",
                 "@storybook/addon-essentials": "^8.0.4",
                 "@storybook/addon-interactions": "^8.0.4",
                 "@storybook/addon-links": "^8.0.4",
                 "@storybook/blocks": "^8.0.4",
                 "@storybook/preview-api": "^8.0.4",
                 "@storybook/testing-library": "^0.2.2",
                 "@types/prismjs": "^1.26.3",
+                "jsdom": "^24.0.0",
                 "solid-devtools": "^0.29.2",
                 "storybook": "^8.0.4",
                 "storybook-solidjs": "^1.0.0-beta.2",
                 "storybook-solidjs-vite": "^1.0.0-beta.2",
                 "stylus": "^0.63.0",
                 "typescript": "^5.3.3",
                 "vite": "^5.0.11",
                 "vite-plugin-prismjs": "^0.0.11",
                 "vite-plugin-solid": "^2.8.2",
                 "vite-plugin-solid-svg": "^0.8.1"
             },
+            "engines": {
+                "node": "22.1.0",
+                "npm": "10.7.0"
+            },
             "license": "UNLICENSED",
             "name": "relationalai-debugger-ui",
             "version": "0.0.0"
         },
         "node_modules/@adobe/css-tools": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-rE0Pygv0sEZ4vBWHlAgJLGDU7Pm8xoO6p3wsEceb7GYAjScrOHpEo8KK/eVkAcnSM+slAEtXjA2JpdjLp4fJQQ==",
             "resolved": "https://registry.npmjs.org/@adobe/css-tools/-/css-tools-4.3.3.tgz",
             "version": "4.3.3"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.5",
@@ -2014,15 +2023,14 @@
             "resolved": "https://registry.npmjs.org/@emotion/use-insertion-effect-with-fallbacks/-/use-insertion-effect-with-fallbacks-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/@esbuild/aix-ppc64": {
             "cpu": [
                 "ppc64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-D+EBOJHXdNZcLJRBkhENNG8Wji2kgc9AZ9KiPr1JuZjsNtyHzrsfLRrY0tk2H2aoFu6RANO1y1iPPUCDYWkb5g==",
             "optional": true,
             "os": [
                 "aix"
@@ -2030,15 +2038,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/aix-ppc64/-/aix-ppc64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/android-arm": {
             "cpu": [
                 "arm"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-t98Ra6pw2VaDhqNWO2Oph2LXbz/EJcnLmKLGBJwEwXX/JAN83Fym1rU8l0JUWK6HkIbWONCSSatf4sf2NBRx/w==",
             "optional": true,
             "os": [
                 "android"
@@ -2046,15 +2053,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/android-arm/-/android-arm-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/android-arm64": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-mRzjLacRtl/tWU0SvD8lUEwb61yP9cqQo6noDZP/O8VkwafSYwZ4yWy24kan8jE/IMERpYncRt2dw438LP3Xmg==",
             "optional": true,
             "os": [
                 "android"
@@ -2062,15 +2068,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/android-arm64/-/android-arm64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/android-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-btzExgV+/lMGDDa194CcUQm53ncxzeBrWJcncOBxuC6ndBkKxnHdFJn86mCIgTELsooUmwUm9FkhSp5HYu00Rg==",
             "optional": true,
             "os": [
                 "android"
@@ -2078,15 +2083,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/android-x64/-/android-x64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/darwin-arm64": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-4J6IRT+10J3aJH3l1yzEg9y3wkTDgDk7TSDFX+wKFiWjqWp/iCfLIYzGyasx9l0SAFPT1HwSCR+0w/h1ES/MjA==",
             "optional": true,
             "os": [
                 "darwin"
@@ -2094,15 +2098,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/darwin-arm64/-/darwin-arm64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/darwin-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-tBcXp9KNphnNH0dfhv8KYkZhjc+H3XBkF5DKtswJblV7KlT9EI2+jeA8DgBjp908WEuYll6pF+UStUCfEpdysA==",
             "optional": true,
             "os": [
                 "darwin"
@@ -2110,15 +2113,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/darwin-x64/-/darwin-x64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/freebsd-arm64": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-d3qI41G4SuLiCGCFGUrKsSeTXyWG6yem1KcGZVS+3FYlYhtNoNgYrWcvkOoaqMhwXSMrZRl69ArHsGJ9mYdbbw==",
             "optional": true,
             "os": [
                 "freebsd"
@@ -2126,15 +2128,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/freebsd-arm64/-/freebsd-arm64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/freebsd-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-d+DipyvHRuqEeM5zDivKV1KuXn9WeRX6vqSqIDgwIfPQtwMP4jaDsQsDncjTDDsExT4lR/91OLjRo8bmC1e+Cw==",
             "optional": true,
             "os": [
                 "freebsd"
@@ -2142,15 +2143,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/freebsd-x64/-/freebsd-x64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-arm": {
             "cpu": [
                 "arm"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-VhLPeR8HTMPccbuWWcEUD1Az68TqaTYyj6nfE4QByZIQEQVWBB8vup8PpR7y1QHL3CpcF6xd5WVBU/+SBEvGTg==",
             "optional": true,
             "os": [
                 "linux"
@@ -2158,15 +2158,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-arm/-/linux-arm-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-arm64": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-9pb6rBjGvTFNira2FLIWqDk/uaf42sSyLE8j1rnUpuzsODBq7FvpwHYZxQ/It/8b+QOS1RYfqgGFNLRI+qlq2A==",
             "optional": true,
             "os": [
                 "linux"
@@ -2174,15 +2173,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-arm64/-/linux-arm64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-ia32": {
             "cpu": [
                 "ia32"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-o10utieEkNPFDZFQm9CoP7Tvb33UutoJqg3qKf1PWVeeJhJw0Q347PxMvBgVVFgouYLGIhFYG0UGdBumROyiig==",
             "optional": true,
             "os": [
                 "linux"
@@ -2190,15 +2188,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-ia32/-/linux-ia32-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-loong64": {
             "cpu": [
                 "loong64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-PR7sp6R/UC4CFVomVINKJ80pMFlfDfMQMYynX7t1tNTeivQ6XdX5r2XovMmha/VjR1YN/HgHWsVcTRIMkymrgQ==",
             "optional": true,
             "os": [
                 "linux"
@@ -2206,15 +2203,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-loong64/-/linux-loong64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-mips64el": {
             "cpu": [
                 "mips64el"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-4BlTqeutE/KnOiTG5Y6Sb/Hw6hsBOZapOVF6njAESHInhlQAghVVZL1ZpIctBOoTFbQyGW+LsVYZ8lSSB3wkjA==",
             "optional": true,
             "os": [
                 "linux"
@@ -2222,15 +2218,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-mips64el/-/linux-mips64el-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-ppc64": {
             "cpu": [
                 "ppc64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-rD3KsaDprDcfajSKdn25ooz5J5/fWBylaaXkuotBDGnMnDP1Uv5DLAN/45qfnf3JDYyJv/ytGHQaziHUdyzaAg==",
             "optional": true,
             "os": [
                 "linux"
@@ -2238,15 +2233,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-ppc64/-/linux-ppc64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-riscv64": {
             "cpu": [
                 "riscv64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-snwmBKacKmwTMmhLlz/3aH1Q9T8v45bKYGE3j26TsaOVtjIag4wLfWSiZykXzXuE1kbCE+zJRmwp+ZbIHinnVg==",
             "optional": true,
             "os": [
                 "linux"
@@ -2254,15 +2248,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-riscv64/-/linux-riscv64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-s390x": {
             "cpu": [
                 "s390x"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-wcWISOobRWNm3cezm5HOZcYz1sKoHLd8VL1dl309DiixxVFoFe/o8HnwuIwn6sXre88Nwj+VwZUvJf4AFxkyrQ==",
             "optional": true,
             "os": [
                 "linux"
@@ -2270,15 +2263,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-s390x/-/linux-s390x-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/linux-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-1MdwI6OOTsfQfek8sLwgyjOXAu+wKhLEoaOLTjbijk6E2WONYpH9ZU2mNtR+lZ2B4uwr+usqGuVfFT9tMtGvGw==",
             "optional": true,
             "os": [
                 "linux"
@@ -2286,15 +2278,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/linux-x64/-/linux-x64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/netbsd-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-K8/DhBxcVQkzYc43yJXDSyjlFeHQJBiowJ0uVL6Tor3jGQfSGHNNJcWxNbOI8v5k82prYqzPuwkzHt3J1T1iZQ==",
             "optional": true,
             "os": [
                 "netbsd"
@@ -2302,15 +2293,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/netbsd-x64/-/netbsd-x64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/openbsd-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-eMpKlV0SThJmmJgiVyN9jTPJ2VBPquf6Kt/nAoo6DgHAoN57K15ZghiHaMvqjCye/uU4X5u3YSMgVBI1h3vKrQ==",
             "optional": true,
             "os": [
                 "openbsd"
@@ -2318,15 +2308,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/openbsd-x64/-/openbsd-x64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/sunos-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-2UyFtRC6cXLyejf/YEld4Hajo7UHILetzE1vsRcGL3earZEW77JxrFjH4Ez2qaTiEfMgAXxfAZCm1fvM/G/o8w==",
             "optional": true,
             "os": [
                 "sunos"
@@ -2334,15 +2323,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/sunos-x64/-/sunos-x64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/win32-arm64": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-GRibxoawM9ZCnDxnP3usoUDO9vUkpAxIIZ6GQI+IlVmr5kP3zUq+l17xELTHMWTWzjxa2guPNyrpq1GWmPvcGQ==",
             "optional": true,
             "os": [
                 "win32"
@@ -2350,15 +2338,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/win32-arm64/-/win32-arm64-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/win32-ia32": {
             "cpu": [
                 "ia32"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-HfLOfn9YWmkSKRQqovpnITazdtquEW8/SoHW7pWpuEeguaZI4QnCRW6b+oZTztdBnZOS2hqJ6im/D5cPzBTTlQ==",
             "optional": true,
             "os": [
                 "win32"
@@ -2366,15 +2353,14 @@
             "resolved": "https://registry.npmjs.org/@esbuild/win32-ia32/-/win32-ia32-0.20.2.tgz",
             "version": "0.20.2"
         },
         "node_modules/@esbuild/win32-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-N49X4lJX27+l9jbLKSqZ6bKNjzQvHaT8IIFUy+YIqmXQdjYCToGWwOItDrfby14c78aDd5NHQl29xingXfCdLQ==",
             "optional": true,
             "os": [
                 "win32"
@@ -2466,15 +2452,14 @@
             "resolved": "https://registry.npmjs.org/string-width/-/string-width-5.1.2.tgz",
             "version": "5.1.2"
         },
         "node_modules/@jest/schemas": {
             "dependencies": {
                 "@sinclair/typebox": "^0.27.8"
             },
-            "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
             "integrity": "sha512-mo5j5X+jIZmJQveBKeS/clAueipV7KgiX1vMgCxam1RNYiqE1w62n0/tJJnHtjW8ZHcQco5gY85jA3mi0L+nSA==",
             "resolved": "https://registry.npmjs.org/@jest/schemas/-/schemas-29.6.3.tgz",
             "version": "29.6.3"
         },
@@ -2507,15 +2492,14 @@
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-R8gLRTZeyp03ymzP/6Lil/28tGeGEzhx1q2k703KGWRAI1VdvPIXdG70VJc2pAMw3NA6JKL5hhFu1sJX0Mnn/A==",
             "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.2.1.tgz",
             "version": "1.2.1"
         },
         "node_modules/@jridgewell/sourcemap-codec": {
-            "dev": true,
             "integrity": "sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==",
             "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz",
             "version": "1.4.15"
         },
         "node_modules/@jridgewell/trace-mapping": {
             "dependencies": {
                 "@jridgewell/resolve-uri": "^3.1.0",
@@ -2674,181 +2658,167 @@
             "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/@rollup/rollup-android-arm-eabi": {
             "cpu": [
                 "arm"
             ],
-            "dev": true,
             "integrity": "sha512-5ZYPOuaAqEH/W3gYsRkxQATBW3Ii1MfaT4EQstTnLKViLi2gLSQmlmtTpGucNP3sXEpOiI5tdGhjdE111ekyEg==",
             "optional": true,
             "os": [
                 "android"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm-eabi/-/rollup-android-arm-eabi-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-android-arm64": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "integrity": "sha512-BSbaCmn8ZadK3UAQdlauSvtaJjhlDEjS5hEVVIN3A4bbl3X+otyf/kOJV08bYiRxfejP3DXFzO2jz3G20107+Q==",
             "optional": true,
             "os": [
                 "android"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm64/-/rollup-android-arm64-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-darwin-arm64": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "integrity": "sha512-Ovf2evVaP6sW5Ut0GHyUSOqA6tVKfrTHddtmxGQc1CTQa1Cw3/KMCDEEICZBbyppcwnhMwcDce9ZRxdWRpVd6g==",
             "optional": true,
             "os": [
                 "darwin"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-arm64/-/rollup-darwin-arm64-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-darwin-x64": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "integrity": "sha512-U+Jcxm89UTK592vZ2J9st9ajRv/hrwHdnvyuJpa5A2ngGSVHypigidkQJP+YiGL6JODiUeMzkqQzbCG3At81Gg==",
             "optional": true,
             "os": [
                 "darwin"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-x64/-/rollup-darwin-x64-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-linux-arm-gnueabihf": {
             "cpu": [
                 "arm"
             ],
-            "dev": true,
             "integrity": "sha512-8wZidaUJUTIR5T4vRS22VkSMOVooG0F4N+JSwQXWSRiC6yfEsFMLTYRFHvby5mFFuExHa/yAp9juSphQQJAijQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm-gnueabihf/-/rollup-linux-arm-gnueabihf-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-linux-arm64-gnu": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "integrity": "sha512-Iu0Kno1vrD7zHQDxOmvweqLkAzjxEVqNhUIXBsZ8hu8Oak7/5VTPrxOEZXYC1nmrBVJp0ZcL2E7lSuuOVaE3+w==",
             "optional": true,
             "os": [
                 "linux"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-gnu/-/rollup-linux-arm64-gnu-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-linux-arm64-musl": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "integrity": "sha512-C31QrW47llgVyrRjIwiOwsHFcaIwmkKi3PCroQY5aVq4H0A5v/vVVAtFsI1nfBngtoRpeREvZOkIhmRwUKkAdw==",
             "optional": true,
             "os": [
                 "linux"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-musl/-/rollup-linux-arm64-musl-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-linux-riscv64-gnu": {
             "cpu": [
                 "riscv64"
             ],
-            "dev": true,
             "integrity": "sha512-Oq90dtMHvthFOPMl7pt7KmxzX7E71AfyIhh+cPhLY9oko97Zf2C9tt/XJD4RgxhaGeAraAXDtqxvKE1y/j35lA==",
             "optional": true,
             "os": [
                 "linux"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-riscv64-gnu/-/rollup-linux-riscv64-gnu-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-linux-x64-gnu": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "integrity": "sha512-yUD/8wMffnTKuiIsl6xU+4IA8UNhQ/f1sAnQebmE/lyQ8abjsVyDkyRkWop0kdMhKMprpNIhPmYlCxgHrPoXoA==",
             "optional": true,
             "os": [
                 "linux"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-gnu/-/rollup-linux-x64-gnu-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-linux-x64-musl": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "integrity": "sha512-9RyNqoFNdF0vu/qqX63fKotBh43fJQeYC98hCaf89DYQpv+xu0D8QFSOS0biA7cGuqJFOc1bJ+m2rhhsKcw1hw==",
             "optional": true,
             "os": [
                 "linux"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-musl/-/rollup-linux-x64-musl-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-win32-arm64-msvc": {
             "cpu": [
                 "arm64"
             ],
-            "dev": true,
             "integrity": "sha512-46ue8ymtm/5PUU6pCvjlic0z82qWkxv54GTJZgHrQUuZnVH+tvvSP0LsozIDsCBFO4VjJ13N68wqrKSeScUKdA==",
             "optional": true,
             "os": [
                 "win32"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-arm64-msvc/-/rollup-win32-arm64-msvc-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-win32-ia32-msvc": {
             "cpu": [
                 "ia32"
             ],
-            "dev": true,
             "integrity": "sha512-P5/MqLdLSlqxbeuJ3YDeX37srC8mCflSyTrUsgbU1c/U9j6l2g2GiIdYaGD9QjdMQPMSgYm7hgg0551wHyIluw==",
             "optional": true,
             "os": [
                 "win32"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-ia32-msvc/-/rollup-win32-ia32-msvc-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@rollup/rollup-win32-x64-msvc": {
             "cpu": [
                 "x64"
             ],
-            "dev": true,
             "integrity": "sha512-UKXUQNbO3DOhzLRwHSpa0HnhhCgNODvfoPWv2FCXme8N/ANFfhIPMGuOT+QuKd16+B5yxZ0HdpNlqPvTMS1qfw==",
             "optional": true,
             "os": [
                 "win32"
             ],
             "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-x64-msvc/-/rollup-win32-x64-msvc-4.13.0.tgz",
             "version": "4.13.0"
         },
         "node_modules/@sinclair/typebox": {
-            "dev": true,
             "integrity": "sha512-+Fj43pSMwJs4KRrH/938Uf+uAELIgVBmQzg/q1YG10djyfA3TnrU8N8XzqCh/okZdszqBQTZf96idMfE5lnwTA==",
             "resolved": "https://registry.npmjs.org/@sinclair/typebox/-/typebox-0.27.8.tgz",
             "version": "0.27.8"
         },
         "node_modules/@solid-devtools/debugger": {
             "dependencies": {
                 "@nothing-but/utils": "~0.12.0",
@@ -2915,14 +2885,27 @@
             "integrity": "sha512-TAtU7qD7ipSLSXHnq8FhhosAPVX+dnOCb/ITcGcLlj8e/C9YKcxDhgBHJ3R/d1xDRb5/vO/szJtEz6fnQD311Q==",
             "peerDependencies": {
                 "solid-js": "^1.6.12"
             },
             "resolved": "https://registry.npmjs.org/@solid-primitives/cursor/-/cursor-0.0.112.tgz",
             "version": "0.0.112"
         },
+        "node_modules/@solid-primitives/date": {
+            "dependencies": {
+                "@solid-primitives/memo": "^1.3.8",
+                "@solid-primitives/timer": "^1.3.9",
+                "@solid-primitives/utils": "^6.2.3"
+            },
+            "integrity": "sha512-DZSmILY9YZarO0IVRzac8gQ6aMgC9QKzKJEgZnv7cF5K4QdkzhdkYud3HC/pfacZ7x1elopZrS0HbCkQllCrYg==",
+            "peerDependencies": {
+                "solid-js": "^1.6.12"
+            },
+            "resolved": "https://registry.npmjs.org/@solid-primitives/date/-/date-2.0.21.tgz",
+            "version": "2.0.21"
+        },
         "node_modules/@solid-primitives/event-bus": {
             "dependencies": {
                 "@solid-primitives/utils": "^6.2.3"
             },
             "dev": true,
             "integrity": "sha512-bSwVA4aI2aNHomSbEroUnisMSyDDXJbrw4U8kFEvrcYdlLrJX5i6QeCFx+vj/zdQQw62KAllrEIyWP8KMpPVnQ==",
             "peerDependencies": {
@@ -2996,14 +2979,26 @@
             "integrity": "sha512-ZecE4BqY0oBk0YG00nzaAWO5Mjcny8Fc06CdbXadH9T9lzq/9GefqcSe/5AtdXqjvY/DtJ5C6CkcjPZO0o/eqg==",
             "peerDependencies": {
                 "solid-js": "^1.6.12"
             },
             "resolved": "https://registry.npmjs.org/@solid-primitives/static-store/-/static-store-0.0.8.tgz",
             "version": "0.0.8"
         },
+        "node_modules/@solid-primitives/memo": {
+            "dependencies": {
+                "@solid-primitives/scheduled": "^1.4.3",
+                "@solid-primitives/utils": "^6.2.3"
+            },
+            "integrity": "sha512-U75pfLFSxFmM2xbx1+2XPPyWbaXrnUFF10spbFuOUgJ7azrC+4y+FnrVi4RKqHw9gftd8aKQuTiyMQq468YLQw==",
+            "peerDependencies": {
+                "solid-js": "^1.6.12"
+            },
+            "resolved": "https://registry.npmjs.org/@solid-primitives/memo/-/memo-1.3.8.tgz",
+            "version": "1.3.8"
+        },
         "node_modules/@solid-primitives/platform": {
             "dev": true,
             "integrity": "sha512-sSxcZfuUrtxcwV0vdjmGnZQcflACzMfLriVeIIWXKp8hzaS3Or3tO6EFQkTd3L8T5dTq+kTtLvPscXIpL0Wzdg==",
             "peerDependencies": {
                 "solid-js": "^1.6.12"
             },
             "resolved": "https://registry.npmjs.org/@solid-primitives/platform/-/platform-0.1.2.tgz",
@@ -3066,15 +3061,14 @@
             "peerDependencies": {
                 "solid-js": "^1.6.12"
             },
             "resolved": "https://registry.npmjs.org/@solid-primitives/rootless/-/rootless-1.4.5.tgz",
             "version": "1.4.5"
         },
         "node_modules/@solid-primitives/scheduled": {
-            "dev": true,
             "integrity": "sha512-HfWN5w7b7FEc6VPLBKnnE302h90jsLMuR28Fcf7neRGGf8jBj6wm6/UFQ00VlKexHFMR6KQ2u4VBh5a1ZcqM8g==",
             "peerDependencies": {
                 "solid-js": "^1.6.12"
             },
             "resolved": "https://registry.npmjs.org/@solid-primitives/scheduled/-/scheduled-1.4.3.tgz",
             "version": "1.4.3"
         },
@@ -3099,14 +3093,22 @@
             "integrity": "sha512-1mBxOGAPXmfD5oYCvqjKBDN7SuNjz2qz7RdH7KtsuNLQh6lpuSKadtHnLvru0Y8Vz1InqTJisBIy/6P5kyDmPw==",
             "peerDependencies": {
                 "solid-js": "^1.6.12"
             },
             "resolved": "https://registry.npmjs.org/@solid-primitives/styles/-/styles-0.0.111.tgz",
             "version": "0.0.111"
         },
+        "node_modules/@solid-primitives/timer": {
+            "integrity": "sha512-uD+4+boV7k+5W+hL5d30eodUXSwOfOQz8AfbMPVmLOHaTmd0mdfpw0NkYhyn1rgcx1bSn/nHTd8lraHiMhO/6w==",
+            "peerDependencies": {
+                "solid-js": "^1.6.12"
+            },
+            "resolved": "https://registry.npmjs.org/@solid-primitives/timer/-/timer-1.3.9.tgz",
+            "version": "1.3.9"
+        },
         "node_modules/@solid-primitives/trigger": {
             "dependencies": {
                 "@solid-primitives/utils": "^6.2.3"
             },
             "integrity": "sha512-4oc8grBzBit7ByXgE1aZ0QXfhdlhXaiFjDKYsOhRyUJa8fN4hdr2IgsYqjmHwxyjK+Dm2OUwkCI1bGkaLgtgXg==",
             "peerDependencies": {
                 "solid-js": "^1.6.12"
@@ -5128,15 +5130,14 @@
         "node_modules/@types/emscripten": {
             "dev": true,
             "integrity": "sha512-TB/6hBkYQJxsZHSqyeuO1Jt0AB/bW6G7rHt9g7lML7SOF6lbgcHvw/Lr+69iqN0qxgXLhWKScAon73JNnptuDw==",
             "resolved": "https://registry.npmjs.org/@types/emscripten/-/emscripten-1.39.10.tgz",
             "version": "1.39.10"
         },
         "node_modules/@types/estree": {
-            "dev": true,
             "integrity": "sha512-/kYRxGDLWzHOB7q+wtSUQlFrtcdUccpfy+X+9iMBpHK8QLLhx2wIPYuS5DYtR9Wa/YlZAbIovy7qVdB1Aq6Lyw==",
             "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.5.tgz",
             "version": "1.0.5"
         },
         "node_modules/@types/express": {
             "dependencies": {
                 "@types/body-parser": "*",
@@ -5200,15 +5201,15 @@
             "resolved": "https://registry.npmjs.org/@types/mime/-/mime-1.3.5.tgz",
             "version": "1.3.5"
         },
         "node_modules/@types/node": {
             "dependencies": {
                 "undici-types": "~5.26.4"
             },
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-dHM6ZxwlmuZaRmUPfv1p+KrdD1Dci04FbdEm/9wEMouFqxYoFl5aMkt0VMAUtYRQDyYvD41WJLukhq/ha3YuTw==",
             "resolved": "https://registry.npmjs.org/@types/node/-/node-20.11.30.tgz",
             "version": "20.11.30"
         },
         "node_modules/@types/normalize-package-data": {
             "dev": true,
             "integrity": "sha512-37i+OaWTh9qeK4LSHPsyRC7NahnGotNuZvjLSgcPzblpHB3rrCJxAOgI5gCdKm7coonsaX1Of0ILiTcnZjbfxA==",
@@ -5278,14 +5279,19 @@
                 "@types/node": "*"
             },
             "dev": true,
             "integrity": "sha512-PDRk21MnK70hja/YF8AHfC7yIsiQHn1rcXx7ijCFBX/k+XQJhQT/gw3xekXKJvx+5SXaMMS8oqQy09Mzvz2TuQ==",
             "resolved": "https://registry.npmjs.org/@types/serve-static/-/serve-static-1.15.5.tgz",
             "version": "1.15.5"
         },
+        "node_modules/@types/tinycolor2": {
+            "integrity": "sha512-iEN8J0BoMnsWBqjVbWH/c0G0Hh7O21lpR2/+PrvAVgWdzL7eexIFm4JN/Wn10PTcmNdtS6U67r499mlWMXOxNw==",
+            "resolved": "https://registry.npmjs.org/@types/tinycolor2/-/tinycolor2-1.4.6.tgz",
+            "version": "1.4.6"
+        },
         "node_modules/@types/unist": {
             "dev": true,
             "integrity": "sha512-dqId9J8K/vGi5Zr7oo212BGii5m3q5Hxlkwy3WpYuKPklmBEvsbMYYyLxAQpSffdLl/gdW0XUpKWFvYmyoWCoQ==",
             "resolved": "https://registry.npmjs.org/@types/unist/-/unist-3.0.2.tgz",
             "version": "3.0.2"
         },
         "node_modules/@types/uuid": {
@@ -5369,43 +5375,120 @@
         },
         "node_modules/@vitest/expect/node_modules/react-is": {
             "dev": true,
             "integrity": "sha512-xWGDIW6x921xtzPkhiULtthJHoJvBbF3q26fzloPCK0hsvxtPVelvftw3zjbHWSkR2km9Z+4uxbDDK/6Zw9B8w==",
             "resolved": "https://registry.npmjs.org/react-is/-/react-is-18.2.0.tgz",
             "version": "18.2.0"
         },
+        "node_modules/@vitest/runner": {
+            "dependencies": {
+                "@vitest/utils": "1.6.0",
+                "p-limit": "^5.0.0",
+                "pathe": "^1.1.1"
+            },
+            "funding": {
+                "url": "https://opencollective.com/vitest"
+            },
+            "integrity": "sha512-P4xgwPjwesuBiHisAVz/LSSZtDjOTPYZVmNAnpHHSR6ONrf8eCJOFRvUwdHn30F5M1fxhqtl7QZQUk2dprIXAg==",
+            "resolved": "https://registry.npmjs.org/@vitest/runner/-/runner-1.6.0.tgz",
+            "version": "1.6.0"
+        },
+        "node_modules/@vitest/runner/node_modules/p-limit": {
+            "dependencies": {
+                "yocto-queue": "^1.0.0"
+            },
+            "engines": {
+                "node": ">=18"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-/Eaoq+QyLSiXQ4lyYV23f14mZRQcXnxfHrN0vCai+ak9G0pp9iEQukIIZq5NccEvwRB8PUnZT0KsOoDCINS1qQ==",
+            "resolved": "https://registry.npmjs.org/p-limit/-/p-limit-5.0.0.tgz",
+            "version": "5.0.0"
+        },
+        "node_modules/@vitest/runner/node_modules/yocto-queue": {
+            "engines": {
+                "node": ">=12.20"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-9bnSc/HEW2uRy67wc+T8UwauLuPJVn28jb+GtJY16iiKWyvmYJRXVT4UamsAEGQfPohgr2q4Tq0sQbQlxTfi1g==",
+            "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-1.0.0.tgz",
+            "version": "1.0.0"
+        },
+        "node_modules/@vitest/snapshot": {
+            "dependencies": {
+                "magic-string": "^0.30.5",
+                "pathe": "^1.1.1",
+                "pretty-format": "^29.7.0"
+            },
+            "funding": {
+                "url": "https://opencollective.com/vitest"
+            },
+            "integrity": "sha512-+Hx43f8Chus+DCmygqqfetcAZrDJwvTj0ymqjQq4CvmpKFSTVteEOBzCusu1x2tt4OJcvBflyHUE0DZSLgEMtQ==",
+            "resolved": "https://registry.npmjs.org/@vitest/snapshot/-/snapshot-1.6.0.tgz",
+            "version": "1.6.0"
+        },
+        "node_modules/@vitest/snapshot/node_modules/ansi-styles": {
+            "engines": {
+                "node": ">=10"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/ansi-styles?sponsor=1"
+            },
+            "integrity": "sha512-Cxwpt2SfTzTtXcfOlzGEee8O+c+MmUgGrNiBcXnuWxuFJHe6a5Hz7qwhwe5OgaSYI0IJvkLqWX1ASG+cJOkEiA==",
+            "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-5.2.0.tgz",
+            "version": "5.2.0"
+        },
+        "node_modules/@vitest/snapshot/node_modules/pretty-format": {
+            "dependencies": {
+                "@jest/schemas": "^29.6.3",
+                "ansi-styles": "^5.0.0",
+                "react-is": "^18.0.0"
+            },
+            "engines": {
+                "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
+            },
+            "integrity": "sha512-Pdlw/oPxN+aXdmM9R00JVC9WVFoCLTKJvDVLgmJ+qAffBMxsV85l/Lu7sNx4zSzPyoL2euImuEwHhOXdEgNFZQ==",
+            "resolved": "https://registry.npmjs.org/pretty-format/-/pretty-format-29.7.0.tgz",
+            "version": "29.7.0"
+        },
+        "node_modules/@vitest/snapshot/node_modules/react-is": {
+            "integrity": "sha512-/LLMVyas0ljjAtoYiPqYiL8VWXzUUdThrmU5+n20DZv+a+ClRoevUzw5JxU+Ieh5/c87ytoTBV9G1FiKfNJdmg==",
+            "resolved": "https://registry.npmjs.org/react-is/-/react-is-18.3.1.tgz",
+            "version": "18.3.1"
+        },
         "node_modules/@vitest/spy": {
             "dependencies": {
                 "tinyspy": "^2.2.0"
             },
-            "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-Ywau/Qs1DzM/8Uc+yA77CwSegizMlcgTJuYGAi0jujOteJOUf1ujunHThYo243KG9nAyWT3L9ifPYZ5+As/+6Q==",
-            "resolved": "https://registry.npmjs.org/@vitest/spy/-/spy-1.4.0.tgz",
-            "version": "1.4.0"
+            "integrity": "sha512-leUTap6B/cqi/bQkXUu6bQV5TZPx7pmMBKBQiI0rJA8c3pB56ZsaTbREnF7CJfmvAS4V2cXIBAh/3rVwrrCYgw==",
+            "resolved": "https://registry.npmjs.org/@vitest/spy/-/spy-1.6.0.tgz",
+            "version": "1.6.0"
         },
         "node_modules/@vitest/utils": {
             "dependencies": {
                 "diff-sequences": "^29.6.3",
                 "estree-walker": "^3.0.3",
                 "loupe": "^2.3.7",
                 "pretty-format": "^29.7.0"
             },
-            "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-mx3Yd1/6e2Vt/PUC98DcqTirtfxUyAZ32uK82r8rZzbtBeBo+nqgnjx/LvqQdWsrvNtm14VmurNgcf4nqY5gJg==",
-            "resolved": "https://registry.npmjs.org/@vitest/utils/-/utils-1.4.0.tgz",
-            "version": "1.4.0"
+            "integrity": "sha512-21cPiuGMoMZwiOHa2i4LXkMkMkCGzA+MVFV70jRwHo95dL4x/ts5GZhML1QWuy7yfp3WzK3lRvZi3JnXTYqrBw==",
+            "resolved": "https://registry.npmjs.org/@vitest/utils/-/utils-1.6.0.tgz",
+            "version": "1.6.0"
         },
         "node_modules/@vitest/utils/node_modules/ansi-styles": {
-            "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "funding": {
                 "url": "https://github.com/chalk/ansi-styles?sponsor=1"
             },
             "integrity": "sha512-Cxwpt2SfTzTtXcfOlzGEee8O+c+MmUgGrNiBcXnuWxuFJHe6a5Hz7qwhwe5OgaSYI0IJvkLqWX1ASG+cJOkEiA==",
@@ -5414,24 +5497,22 @@
         },
         "node_modules/@vitest/utils/node_modules/pretty-format": {
             "dependencies": {
                 "@jest/schemas": "^29.6.3",
                 "ansi-styles": "^5.0.0",
                 "react-is": "^18.0.0"
             },
-            "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
             "integrity": "sha512-Pdlw/oPxN+aXdmM9R00JVC9WVFoCLTKJvDVLgmJ+qAffBMxsV85l/Lu7sNx4zSzPyoL2euImuEwHhOXdEgNFZQ==",
             "resolved": "https://registry.npmjs.org/pretty-format/-/pretty-format-29.7.0.tgz",
             "version": "29.7.0"
         },
         "node_modules/@vitest/utils/node_modules/react-is": {
-            "dev": true,
             "integrity": "sha512-xWGDIW6x921xtzPkhiULtthJHoJvBbF3q26fzloPCK0hsvxtPVelvftw3zjbHWSkR2km9Z+4uxbDDK/6Zw9B8w==",
             "resolved": "https://registry.npmjs.org/react-is/-/react-is-18.2.0.tgz",
             "version": "18.2.0"
         },
         "node_modules/@yarnpkg/esbuild-plugin-pnp": {
             "dependencies": {
                 "tslib": "^2.4.0"
@@ -5492,31 +5573,50 @@
             "resolved": "https://registry.npmjs.org/accepts/-/accepts-1.3.8.tgz",
             "version": "1.3.8"
         },
         "node_modules/acorn": {
             "bin": {
                 "acorn": "bin/acorn"
             },
-            "dev": true,
             "engines": {
                 "node": ">=0.4.0"
             },
             "integrity": "sha512-Y9rRfJG5jcKOE0CLisYbojUjIrIEE7AGMzA/Sm4BslANhbS+cDMpgBdcPT91oJ7OuJ9hYJBx59RjbhxVnrF8Xg==",
             "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.11.3.tgz",
             "version": "8.11.3"
         },
+        "node_modules/acorn-walk": {
+            "engines": {
+                "node": ">=0.4.0"
+            },
+            "integrity": "sha512-cjkyv4OtNCIeqhHrfS81QWXoCBPExR/J62oyEqepVw8WaQeSqpW2uhuLPh1m9eWhDuOo/jUXVTlifvesOWp/4A==",
+            "resolved": "https://registry.npmjs.org/acorn-walk/-/acorn-walk-8.3.2.tgz",
+            "version": "8.3.2"
+        },
         "node_modules/address": {
             "dev": true,
             "engines": {
                 "node": ">= 10.0.0"
             },
             "integrity": "sha512-4B/qKCfeE/ODUaAUpSwfzazo5x29WD4r3vXiWsB7I2mSDAihwEqKO+g8GELZUQSSAo5e1XTYh3ZVfLyxBc12nA==",
             "resolved": "https://registry.npmjs.org/address/-/address-1.2.2.tgz",
             "version": "1.2.2"
         },
+        "node_modules/agent-base": {
+            "dependencies": {
+                "debug": "^4.3.4"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">= 14"
+            },
+            "integrity": "sha512-H0TSyFNDMomMNJQBn8wFV5YC/2eJ+VXECwOadZJT554xP6cODZHPX3H9QMQECxvrgiSOP1pHjy1sMWQVYJOUOA==",
+            "resolved": "https://registry.npmjs.org/agent-base/-/agent-base-7.1.1.tgz",
+            "version": "7.1.1"
+        },
         "node_modules/aggregate-error": {
             "dependencies": {
                 "clean-stack": "^2.0.0",
                 "indent-string": "^4.0.0"
             },
             "dev": true,
             "engines": {
@@ -5616,15 +5716,14 @@
             },
             "dev": true,
             "integrity": "sha512-eLHpSK/Y4nhMJ07gDaAzoX/XAKS8PSaojml3M0DM4JpV1LAi5JOJ/p6H/XWrl8L+DzVEvVCW1z3vWAaB9oTsQw==",
             "resolved": "https://registry.npmjs.org/assert/-/assert-2.1.0.tgz",
             "version": "2.1.0"
         },
         "node_modules/assertion-error": {
-            "dev": true,
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-jgsaNduz+ndvGyFt3uSuWqvy4lCnIJiovtouQN5JZHOKCS2QuhEdbcQHFhVksz2N2U9hXJo8odG7ETyWlEeuDw==",
             "resolved": "https://registry.npmjs.org/assertion-error/-/assertion-error-1.1.0.tgz",
             "version": "1.1.0"
         },
@@ -5648,14 +5747,20 @@
         },
         "node_modules/async": {
             "dev": true,
             "integrity": "sha512-baNZyqaaLhyLVKm/DlvdW051MSgO6b8eVfIezl9E5PqWxFgzLm/wQntEW4zOytVburDEr0JlALEpdOFwvErLsg==",
             "resolved": "https://registry.npmjs.org/async/-/async-3.2.5.tgz",
             "version": "3.2.5"
         },
+        "node_modules/asynckit": {
+            "devOptional": true,
+            "integrity": "sha512-Oei9OH4tRh0YqU3GxhX79dM/mwVgvbZJaSNaRk+bshkj0S5cfHcgYakreBjrHwatXKbz+IoIdYLxrKim2MjW0Q==",
+            "resolved": "https://registry.npmjs.org/asynckit/-/asynckit-0.4.0.tgz",
+            "version": "0.4.0"
+        },
         "node_modules/available-typed-arrays": {
             "dependencies": {
                 "possible-typed-array-names": "^1.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
@@ -5761,15 +5866,15 @@
             "peerDependencies": {
                 "@babel/core": "^7.0.0"
             },
             "resolved": "https://registry.npmjs.org/babel-preset-solid/-/babel-preset-solid-1.8.16.tgz",
             "version": "1.8.16"
         },
         "node_modules/balanced-match": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==",
             "resolved": "https://registry.npmjs.org/balanced-match/-/balanced-match-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/base64-js": {
             "dev": true,
             "funding": [
@@ -5916,15 +6021,15 @@
             "version": "0.2.0"
         },
         "node_modules/brace-expansion": {
             "dependencies": {
                 "balanced-match": "^1.0.0",
                 "concat-map": "0.0.1"
             },
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==",
             "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-1.1.11.tgz",
             "version": "1.1.11"
         },
         "node_modules/braces": {
             "dependencies": {
                 "fill-range": "^7.0.1"
@@ -6019,14 +6124,22 @@
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-pMhOfFDPiv9t5jjIXkHosWmkSyQbvsgEVNkz0ERHbuLh2T/7j4Mqqpz523Fe8MVY89KC6Sh/QfS2sM+SjgFDcw==",
             "resolved": "https://registry.npmjs.org/bytes/-/bytes-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "node_modules/cac": {
+            "engines": {
+                "node": ">=8"
+            },
+            "integrity": "sha512-b6Ilus+c3RrdDk+JhLKUAQfzzgLEPy6wcXqS7f/xe1EETvsDP6GORG7SFuOs6cID5YkqchW/LXZbX5bc8j7ZcQ==",
+            "resolved": "https://registry.npmjs.org/cac/-/cac-6.7.14.tgz",
+            "version": "6.7.14"
+        },
         "node_modules/call-bind": {
             "dependencies": {
                 "es-define-property": "^1.0.0",
                 "es-errors": "^1.3.0",
                 "function-bind": "^1.1.2",
                 "get-intrinsic": "^1.2.4",
                 "set-function-length": "^1.2.1"
@@ -6068,15 +6181,14 @@
                 "check-error": "^1.0.3",
                 "deep-eql": "^4.1.3",
                 "get-func-name": "^2.0.2",
                 "loupe": "^2.3.6",
                 "pathval": "^1.1.1",
                 "type-detect": "^4.0.8"
             },
-            "dev": true,
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-13sOfMv2+DWduEU+/xbun3LScLoqN17nBeTLUsmDfKdoiC1fr0n9PU4guu4AhRcOVFk/sW8LyZWHuhWtQZiF+g==",
             "resolved": "https://registry.npmjs.org/chai/-/chai-4.4.1.tgz",
             "version": "4.4.1"
         },
@@ -6094,15 +6206,14 @@
             "resolved": "https://registry.npmjs.org/chalk/-/chalk-2.4.2.tgz",
             "version": "2.4.2"
         },
         "node_modules/check-error": {
             "dependencies": {
                 "get-func-name": "^2.0.2"
             },
-            "dev": true,
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-iKEoDYaRmd1mxM90a2OEfWhjsjPpYPuQ+lMYsoxB126+t8fw7ySEO48nmDg5COTjxDI65/Y2OWpeEHk3ZOe8zg==",
             "resolved": "https://registry.npmjs.org/check-error/-/check-error-1.0.3.tgz",
             "version": "1.0.3"
         },
@@ -6253,14 +6364,26 @@
         },
         "node_modules/color-name": {
             "dev": true,
             "integrity": "sha512-72fSenhMw2HZMTVHeCA9KCmpEIbzWiQsjN+BHcBbS9vr1mtt+vJjPdksIBNUmKAW8TFUDPJK5SUU3QhE9NEXDw==",
             "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.3.tgz",
             "version": "1.1.3"
         },
+        "node_modules/combined-stream": {
+            "dependencies": {
+                "delayed-stream": "~1.0.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">= 0.8"
+            },
+            "integrity": "sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==",
+            "resolved": "https://registry.npmjs.org/combined-stream/-/combined-stream-1.0.8.tgz",
+            "version": "1.0.8"
+        },
         "node_modules/commander": {
             "dev": true,
             "engines": {
                 "node": ">= 6"
             },
             "integrity": "sha512-U7VdrJFnJgo4xjrHpTzu0yrHPGImdsmD95ZlgYSEajAn2JKzDhDTPG9kBTefmObL2w/ngeZnilk+OV9CG3d7UA==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-6.2.1.tgz",
@@ -6314,19 +6437,24 @@
         "node_modules/compression/node_modules/ms": {
             "dev": true,
             "integrity": "sha512-Tpp60P6IUJDTuOq/5Z8cdskzJujfwqfOTkrwIwj7IRISpnkJnT6SyJ4PCPnGMoFjC9ddhal5KVIYtAt97ix05A==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/concat-map": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==",
             "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
             "version": "0.0.1"
         },
+        "node_modules/confbox": {
+            "integrity": "sha512-uJcB/FKZtBMCJpK8MQji6bJHgu1tixKPxRLeGkNzBoOZzpnZUJm0jm2/sBDWcuBx1dYgxV4JU+g5hmNxCyAmdA==",
+            "resolved": "https://registry.npmjs.org/confbox/-/confbox-0.1.7.tgz",
+            "version": "0.1.7"
+        },
         "node_modules/consola": {
             "dev": true,
             "engines": {
                 "node": "^14.18.0 || >=16.10.0"
             },
             "integrity": "sha512-I5qxpzLv+sJhTVEoLYNcTW+bThDCPsit0vLNKShZx6rLtpilNpmmeTPaeqJb9ZE9dV3DGaeby6Vuhrw38WjeyQ==",
             "resolved": "https://registry.npmjs.org/consola/-/consola-3.2.3.tgz",
@@ -6415,15 +6543,14 @@
         },
         "node_modules/cross-spawn": {
             "dependencies": {
                 "path-key": "^3.1.0",
                 "shebang-command": "^2.0.0",
                 "which": "^2.0.1"
             },
-            "dev": true,
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==",
             "resolved": "https://registry.npmjs.org/cross-spawn/-/cross-spawn-7.0.3.tgz",
             "version": "7.0.3"
         },
@@ -6512,41 +6639,104 @@
         },
         "node_modules/csso/node_modules/mdn-data": {
             "dev": true,
             "integrity": "sha512-aylIc7Z9y4yzHYAJNuESG3hfhC+0Ibp/MAMiaOZgNv4pmEdFyfZhhhny4MNiAfWdBQ1RQ2mfDWmM1x8SvGyp8g==",
             "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.28.tgz",
             "version": "2.0.28"
         },
+        "node_modules/cssstyle": {
+            "dependencies": {
+                "rrweb-cssom": "^0.6.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-8ZYiJ3A/3OkDd093CBT/0UKDWry7ak4BdPTFP2+QEP7cmhouyq/Up709ASSj2cK02BbZiMgk7kYjZNS4QP5qrQ==",
+            "resolved": "https://registry.npmjs.org/cssstyle/-/cssstyle-4.0.1.tgz",
+            "version": "4.0.1"
+        },
         "node_modules/csstype": {
             "integrity": "sha512-M1uQkMl8rQK/szD0LNhtqxIPLpimGm8sOBwU7lLnCpSbTyY3yeU1Vc7l4KT5zT4s/yOxHH5O7tIuuLOCnLADRw==",
             "resolved": "https://registry.npmjs.org/csstype/-/csstype-3.1.3.tgz",
             "version": "3.1.3"
         },
+        "node_modules/data-urls": {
+            "dependencies": {
+                "whatwg-mimetype": "^4.0.0",
+                "whatwg-url": "^14.0.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-ZYP5VBHshaDAiVZxjbRVcFJpc+4xGgT0bK3vzy1HLN8jTO975HEbuYzZJcHoQEY5K1a0z8YayJkyVETa08eNTg==",
+            "resolved": "https://registry.npmjs.org/data-urls/-/data-urls-5.0.0.tgz",
+            "version": "5.0.0"
+        },
+        "node_modules/data-urls/node_modules/tr46": {
+            "dependencies": {
+                "punycode": "^2.3.1"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-tk2G5R2KRwBd+ZN0zaEXpmzdKyOYksXwywulIX95MBODjSzMIuQnQ3m8JxgbhnL1LeVo7lqQKsYa1O3Htl7K5g==",
+            "resolved": "https://registry.npmjs.org/tr46/-/tr46-5.0.0.tgz",
+            "version": "5.0.0"
+        },
+        "node_modules/data-urls/node_modules/webidl-conversions": {
+            "devOptional": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "integrity": "sha512-VwddBukDzu71offAQR975unBIGqfKZpM+8ZX6ySk8nYhVoo5CYaZyzt3YBvYtRtO+aoGlqxPg/B87NGVZ/fu6g==",
+            "resolved": "https://registry.npmjs.org/webidl-conversions/-/webidl-conversions-7.0.0.tgz",
+            "version": "7.0.0"
+        },
+        "node_modules/data-urls/node_modules/whatwg-url": {
+            "dependencies": {
+                "tr46": "^5.0.0",
+                "webidl-conversions": "^7.0.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-1lfMEm2IEr7RIV+f4lUNPOqfFL+pO+Xw3fJSqmjX9AbXcXcYOkCe1P6+9VBZB6n94af16NfZf+sSk0JCBZC9aw==",
+            "resolved": "https://registry.npmjs.org/whatwg-url/-/whatwg-url-14.0.0.tgz",
+            "version": "14.0.0"
+        },
         "node_modules/debug": {
             "dependencies": {
                 "ms": "2.1.2"
             },
-            "dev": true,
             "engines": {
                 "node": ">=6.0"
             },
             "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
             "peerDependenciesMeta": {
                 "supports-color": {
                     "optional": true
                 }
             },
             "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
             "version": "4.3.4"
         },
+        "node_modules/decimal.js": {
+            "devOptional": true,
+            "integrity": "sha512-VBBaLc1MgL5XpzgIP7ny5Z6Nx3UrRkIViUkPUdtl9aya5amy3De1gsUUSB1g3+3sExYNjCAsAznmukyxCb1GRA==",
+            "resolved": "https://registry.npmjs.org/decimal.js/-/decimal.js-10.4.3.tgz",
+            "version": "10.4.3"
+        },
         "node_modules/deep-eql": {
             "dependencies": {
                 "type-detect": "^4.0.0"
             },
-            "dev": true,
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-WaEtAOpRA1MQ0eohqZjpGD8zdI0Ovsm8mmFhaDN8dvDZzyoUMcYDnf5Y6iu7HTXxf8JDS23qWa4a+hKCDyOPzw==",
             "resolved": "https://registry.npmjs.org/deep-eql/-/deep-eql-4.1.3.tgz",
             "version": "4.1.3"
         },
@@ -6692,14 +6882,23 @@
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==",
             "resolved": "https://registry.npmjs.org/rimraf/-/rimraf-3.0.2.tgz",
             "version": "3.0.2"
         },
+        "node_modules/delayed-stream": {
+            "devOptional": true,
+            "engines": {
+                "node": ">=0.4.0"
+            },
+            "integrity": "sha512-ZySD7Nf91aLB0RxL4KGrKHBXl7Eds1DAmEdcoVawXnLD7SDhpNgtuII2aAkg7a7QS41jxPSZ17p4VdGnMHk3MQ==",
+            "resolved": "https://registry.npmjs.org/delayed-stream/-/delayed-stream-1.0.0.tgz",
+            "version": "1.0.0"
+        },
         "node_modules/depd": {
             "dev": true,
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-g7nH6P6dyDioJogAAGprGpCtVImJhpPk/roCzdb3fIh61/s/nPsfR6onyMwkCAR/OlC3yBC0lESvUoQEAssIrw==",
             "resolved": "https://registry.npmjs.org/depd/-/depd-2.0.0.tgz",
@@ -6756,15 +6955,14 @@
             },
             "dev": true,
             "integrity": "sha512-aBzdj76lueB6uUst5iAs7+0H/oOjqI5D16XUWxlWMIMROhcM0rfsNVk93zTngq1dDNpoXRr++Sus7ETAExppAQ==",
             "resolved": "https://registry.npmjs.org/detect-port/-/detect-port-1.5.1.tgz",
             "version": "1.5.1"
         },
         "node_modules/diff-sequences": {
-            "dev": true,
             "engines": {
                 "node": "^14.15.0 || ^16.10.0 || >=18.0.0"
             },
             "integrity": "sha512-EjePK1srD3P08o2j4f0ExnylqRs5B9tJjcp9t1krH2qRi8CCdsYfwe9JgSLurFBWwq4uOlipzfk5fHNvwFKr8Q==",
             "resolved": "https://registry.npmjs.org/diff-sequences/-/diff-sequences-29.6.3.tgz",
             "version": "29.6.3"
         },
@@ -6935,17 +7133,17 @@
             "dependencies": {
                 "jake": "^10.8.5"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
-            "integrity": "sha512-rC+QVNMJWv+MtPgkt0y+0rVEIdbtxVADApW9JXrUVlzHetgcyczP/E7DJmWJ4fJCZF2cPcBk0laWO9ZHMG3DmQ==",
-            "resolved": "https://registry.npmjs.org/ejs/-/ejs-3.1.9.tgz",
-            "version": "3.1.9"
+            "integrity": "sha512-UeJmFfOrAQS8OJWPZ4qtgHyWExa088/MtK5UEyoJGFH67cDEXkZSviOiKRCZ4Xij0zxI3JECgYs3oKx+AizQBA==",
+            "resolved": "https://registry.npmjs.org/ejs/-/ejs-3.1.10.tgz",
+            "version": "3.1.10"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
             "integrity": "sha512-XzWNH4ZSa9BwVUQSDorPWAUQ5WGuYz7zJUNpNif40zFCiCl20t8zgylmreNmn26h5kiyw2lg7RfTmeMBsDklqg==",
             "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.715.tgz",
             "version": "1.4.715"
         },
@@ -6970,15 +7168,15 @@
             },
             "dev": true,
             "integrity": "sha512-+uw1inIHVPQoaVuHzRyXd21icM+cnt4CzD5rW+NC1wjOUSTOs+Te7FOv7AhN7vS9x/oIyhLP5PR1H+phQAHu5Q==",
             "resolved": "https://registry.npmjs.org/end-of-stream/-/end-of-stream-1.4.4.tgz",
             "version": "1.4.4"
         },
         "node_modules/entities": {
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": ">=0.12"
             },
             "funding": {
                 "url": "https://github.com/fb55/entities?sponsor=1"
             },
             "integrity": "sha512-V0hjH4dGPh9Ao5p0MoRY6BVqtwCjhz6vI5LT8AJ55H+4g9/4vbHx1I54fS0XuclLhDHArPQCiMjDxjaL8fPxhw==",
@@ -7053,15 +7251,14 @@
             "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
             "version": "0.9.3"
         },
         "node_modules/esbuild": {
             "bin": {
                 "esbuild": "bin/esbuild"
             },
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "hasInstallScript": true,
             "integrity": "sha512-WdOOppmUNU+IbZ0PaDiTst80zjnrOkyJNHoKupIcVyU8Lvla3Ugx94VzkQ32Ijqd7UhHJy75gNWDMUekcrSJ6g==",
             "optionalDependencies": {
                 "@esbuild/aix-ppc64": "0.20.2",
@@ -7146,15 +7343,14 @@
             "resolved": "https://registry.npmjs.org/esprima/-/esprima-4.0.1.tgz",
             "version": "4.0.1"
         },
         "node_modules/estree-walker": {
             "dependencies": {
                 "@types/estree": "^1.0.0"
             },
-            "dev": true,
             "integrity": "sha512-7RUKfXgSMMkzt6ZuXmqapOurLGPPfgj6l9uRZ7lRGolvk0y2yocc35LdcxKC5PQZdn2DMqioAQ2NoWcrTKmm6g==",
             "resolved": "https://registry.npmjs.org/estree-walker/-/estree-walker-3.0.3.tgz",
             "version": "3.0.3"
         },
         "node_modules/esutils": {
             "dev": true,
             "engines": {
@@ -7566,14 +7762,28 @@
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-bzyZ1e88w9O1iNJbKnOlvYTrWPDl46O1bG0D3XInv+9tkPrxrN8jUUTiFlDkkmKWgn1M6CfIA13SuGqOa9Korw==",
             "resolved": "https://registry.npmjs.org/signal-exit/-/signal-exit-4.1.0.tgz",
             "version": "4.1.0"
         },
+        "node_modules/form-data": {
+            "dependencies": {
+                "asynckit": "^0.4.0",
+                "combined-stream": "^1.0.8",
+                "mime-types": "^2.1.12"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">= 6"
+            },
+            "integrity": "sha512-ETEklSGi5t0QMZuiXoA/Q6vcnxcLQP5vdugSpuAyi6SVGi2clPPp+xgEhuMaHC+zGgn31Kd235W35f7Hykkaww==",
+            "resolved": "https://registry.npmjs.org/form-data/-/form-data-4.0.0.tgz",
+            "version": "4.0.0"
+        },
         "node_modules/forwarded": {
             "dev": true,
             "engines": {
                 "node": ">= 0.6"
             },
             "integrity": "sha512-buRG0fpBtRHSTCOASe6hD258tEubFoRLb4ZNA6NxMVHNw2gOcwHo9wyablzMzOA5z9xA9L1KNjk/Nt6MT9aYow==",
             "resolved": "https://registry.npmjs.org/forwarded/-/forwarded-0.2.0.tgz",
@@ -7635,21 +7845,20 @@
         "node_modules/fs-minipass/node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/fs.realpath": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/fsevents": {
-            "dev": true,
             "engines": {
                 "node": "^8.16.0 || ^10.6.0 || >=11.0.0"
             },
             "hasInstallScript": true,
             "integrity": "sha512-5xoDfX+fL7faATnagmWPpbFtwh/R77WmMMqqHGS65C3vvB0YHrgF+B1YmZ3441tMj5n63k0212XNoJwzlhffQw==",
             "optional": true,
             "os": [
@@ -7682,15 +7891,14 @@
                 "node": ">=6.9.0"
             },
             "integrity": "sha512-3hN7NaskYvMDLQY55gnW3NQ+mesEAepTqlg+VEbj7zzqEMBVNhzcGYYeqFo/TlYz6eQiFcp1HcsCZO+nGgS8zg==",
             "resolved": "https://registry.npmjs.org/gensync/-/gensync-1.0.0-beta.2.tgz",
             "version": "1.0.0-beta.2"
         },
         "node_modules/get-func-name": {
-            "dev": true,
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-8vXOvuE167CtIc3OyItco7N/dpRtBbYOsPsXCz7X/PMnlGjYjSGuZJgM1Y7mmew7BKf9BqvLX2tnOVy1BBUsxQ==",
             "resolved": "https://registry.npmjs.org/get-func-name/-/get-func-name-2.0.2.tgz",
             "version": "2.0.2"
         },
@@ -7764,15 +7972,15 @@
                 "fs.realpath": "^1.0.0",
                 "inflight": "^1.0.4",
                 "inherits": "2",
                 "minimatch": "^3.1.1",
                 "once": "^1.3.0",
                 "path-is-absolute": "^1.0.0"
             },
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": "*"
             },
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==",
@@ -7840,14 +8048,22 @@
         },
         "node_modules/graceful-fs": {
             "dev": true,
             "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
             "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
             "version": "4.2.11"
         },
+        "node_modules/gradient-path": {
+            "dependencies": {
+                "tinygradient": "^1.0.0"
+            },
+            "integrity": "sha512-vZdF/Z0EpqUztzWXFjFC16lqcialHacYoRonslk/bC6CuujkuIrqx7etlzdYHY4SnUU94LRWESamZKfkGh7yYQ==",
+            "resolved": "https://registry.npmjs.org/gradient-path/-/gradient-path-2.3.0.tgz",
+            "version": "2.3.0"
+        },
         "node_modules/gunzip-maybe": {
             "bin": {
                 "gunzip-maybe": "bin.js"
             },
             "dependencies": {
                 "browserify-zlib": "^0.1.4",
                 "is-deflate": "^1.0.0",
@@ -8013,14 +8229,26 @@
         },
         "node_modules/hosted-git-info": {
             "dev": true,
             "integrity": "sha512-mxIDAb9Lsm6DoOJ7xH+5+X4y1LU/4Hi50L9C5sIswK3JzULS4bwk1FvjdBgvYR4bzT4tuUQiC15FE2f5HbLvYw==",
             "resolved": "https://registry.npmjs.org/hosted-git-info/-/hosted-git-info-2.8.9.tgz",
             "version": "2.8.9"
         },
+        "node_modules/html-encoding-sniffer": {
+            "dependencies": {
+                "whatwg-encoding": "^3.1.1"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-Y22oTqIU4uuPgEemfz7NDJz6OeKf12Lsu+QC+s3BVpda64lTiMYCyGwg5ki4vFxkMwQdeZDl2adZoqUgdFuTgQ==",
+            "resolved": "https://registry.npmjs.org/html-encoding-sniffer/-/html-encoding-sniffer-4.0.0.tgz",
+            "version": "4.0.0"
+        },
         "node_modules/html-entities": {
             "dev": true,
             "integrity": "sha512-DV5Ln36z34NNTDgnz0EWGBLZENelNAtkiFA4kyNOG2tDI6Mz1uSWiq1wAKdyjnJwyDiDO7Fa2SO1CTxPXL8VxA==",
             "resolved": "https://registry.npmjs.org/html-entities/-/html-entities-2.3.3.tgz",
             "version": "2.3.3"
         },
         "node_modules/http-errors": {
@@ -8035,14 +8263,40 @@
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-FtwrG/euBzaEjYeRqOgly7G0qviiXoJWnvEH2Z1plBdXgbyjv34pHTSb9zoeHMyDy33+DWy5Wt9Wo+TURtOYSQ==",
             "resolved": "https://registry.npmjs.org/http-errors/-/http-errors-2.0.0.tgz",
             "version": "2.0.0"
         },
+        "node_modules/http-proxy-agent": {
+            "dependencies": {
+                "agent-base": "^7.1.0",
+                "debug": "^4.3.4"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">= 14"
+            },
+            "integrity": "sha512-T1gkAiYYDWYx3V5Bmyu7HcfcvL7mUrTWiM6yOfa3PIphViJ/gFPbvidQ+veqSOHci/PxBcDabeUNCzpOODJZig==",
+            "resolved": "https://registry.npmjs.org/http-proxy-agent/-/http-proxy-agent-7.0.2.tgz",
+            "version": "7.0.2"
+        },
+        "node_modules/https-proxy-agent": {
+            "dependencies": {
+                "agent-base": "^7.0.2",
+                "debug": "4"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">= 14"
+            },
+            "integrity": "sha512-wlwpilI7YdjSkWaQ/7omYBMTliDcmCN8OLihO6I9B86g06lMyAoqgoDpV0XqoaPOKj+0DIdAvnsWfyAAhmimcg==",
+            "resolved": "https://registry.npmjs.org/https-proxy-agent/-/https-proxy-agent-7.0.4.tgz",
+            "version": "7.0.4"
+        },
         "node_modules/human-signals": {
             "dev": true,
             "engines": {
                 "node": ">=10.17.0"
             },
             "integrity": "sha512-B4FFZ6q/T2jhhksgkbEW3HBvWIfDW85snkQgawt07S7J5QXTk6BkNV+0yAeZrM5QpMAdYlocGoljn0sJ/WQkFw==",
             "resolved": "https://registry.npmjs.org/human-signals/-/human-signals-2.1.0.tgz",
@@ -8108,21 +8362,21 @@
             "version": "4.0.0"
         },
         "node_modules/inflight": {
             "dependencies": {
                 "once": "^1.3.0",
                 "wrappy": "1"
             },
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
             "resolved": "https://registry.npmjs.org/inflight/-/inflight-1.0.6.tgz",
             "version": "1.0.6"
         },
         "node_modules/inherits": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
             "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
             "version": "2.0.4"
         },
         "node_modules/internal-slot": {
             "dependencies": {
                 "es-errors": "^1.3.0",
@@ -8443,14 +8697,20 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-h5PpgXkWitc38BBMYawTYMWJHFZJVnBquFE57xFpjB8pJFiF6gZ+bU+WyI/yqXiFR5mdLsgYNaPe8uao6Uv9Og==",
             "resolved": "https://registry.npmjs.org/is-plain-object/-/is-plain-object-2.0.4.tgz",
             "version": "2.0.4"
         },
+        "node_modules/is-potential-custom-element-name": {
+            "devOptional": true,
+            "integrity": "sha512-bCYeRA2rVibKZd+s2625gGnGF/t7DSqDs4dP7CrLA1m7jKWz6pps0LpYLJN8Q64HtmPKJ1hrN3nzPNKFEKOUiQ==",
+            "resolved": "https://registry.npmjs.org/is-potential-custom-element-name/-/is-potential-custom-element-name-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "node_modules/is-regex": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "has-tostringtag": "^1.0.0"
             },
             "dev": true,
             "engines": {
@@ -8614,15 +8874,14 @@
         "node_modules/isarray": {
             "dev": true,
             "integrity": "sha512-xHjhDr3cNBK0BzdUJSPXZntQUx/mwMS5Rw4A7lPJ90XGAO6ISP/ePDNuo0vhqOZU+UD5JoodwCAAoZQd3FeAKw==",
             "resolved": "https://registry.npmjs.org/isarray/-/isarray-2.0.5.tgz",
             "version": "2.0.5"
         },
         "node_modules/isexe": {
-            "dev": true,
             "integrity": "sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==",
             "resolved": "https://registry.npmjs.org/isexe/-/isexe-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/isobject": {
             "dev": true,
             "engines": {
@@ -8849,14 +9108,88 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
+        "node_modules/jsdom": {
+            "dependencies": {
+                "cssstyle": "^4.0.1",
+                "data-urls": "^5.0.0",
+                "decimal.js": "^10.4.3",
+                "form-data": "^4.0.0",
+                "html-encoding-sniffer": "^4.0.0",
+                "http-proxy-agent": "^7.0.0",
+                "https-proxy-agent": "^7.0.2",
+                "is-potential-custom-element-name": "^1.0.1",
+                "nwsapi": "^2.2.7",
+                "parse5": "^7.1.2",
+                "rrweb-cssom": "^0.6.0",
+                "saxes": "^6.0.0",
+                "symbol-tree": "^3.2.4",
+                "tough-cookie": "^4.1.3",
+                "w3c-xmlserializer": "^5.0.0",
+                "webidl-conversions": "^7.0.0",
+                "whatwg-encoding": "^3.1.1",
+                "whatwg-mimetype": "^4.0.0",
+                "whatwg-url": "^14.0.0",
+                "ws": "^8.16.0",
+                "xml-name-validator": "^5.0.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-UDS2NayCvmXSXVP6mpTj+73JnNQadZlr9N68189xib2tx5Mls7swlTNao26IoHv46BZJFvXygyRtyXd1feAk1A==",
+            "peerDependencies": {
+                "canvas": "^2.11.2"
+            },
+            "peerDependenciesMeta": {
+                "canvas": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/jsdom/-/jsdom-24.0.0.tgz",
+            "version": "24.0.0"
+        },
+        "node_modules/jsdom/node_modules/tr46": {
+            "dependencies": {
+                "punycode": "^2.3.1"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-tk2G5R2KRwBd+ZN0zaEXpmzdKyOYksXwywulIX95MBODjSzMIuQnQ3m8JxgbhnL1LeVo7lqQKsYa1O3Htl7K5g==",
+            "resolved": "https://registry.npmjs.org/tr46/-/tr46-5.0.0.tgz",
+            "version": "5.0.0"
+        },
+        "node_modules/jsdom/node_modules/webidl-conversions": {
+            "devOptional": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "integrity": "sha512-VwddBukDzu71offAQR975unBIGqfKZpM+8ZX6ySk8nYhVoo5CYaZyzt3YBvYtRtO+aoGlqxPg/B87NGVZ/fu6g==",
+            "resolved": "https://registry.npmjs.org/webidl-conversions/-/webidl-conversions-7.0.0.tgz",
+            "version": "7.0.0"
+        },
+        "node_modules/jsdom/node_modules/whatwg-url": {
+            "dependencies": {
+                "tr46": "^5.0.0",
+                "webidl-conversions": "^7.0.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-1lfMEm2IEr7RIV+f4lUNPOqfFL+pO+Xw3fJSqmjX9AbXcXcYOkCe1P6+9VBZB6n94af16NfZf+sSk0JCBZC9aw==",
+            "resolved": "https://registry.npmjs.org/whatwg-url/-/whatwg-url-14.0.0.tgz",
+            "version": "14.0.0"
+        },
         "node_modules/jsesc": {
             "bin": {
                 "jsesc": "bin/jsesc"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
@@ -8938,14 +9271,29 @@
         },
         "node_modules/lines-and-columns": {
             "dev": true,
             "integrity": "sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==",
             "resolved": "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz",
             "version": "1.2.4"
         },
+        "node_modules/local-pkg": {
+            "dependencies": {
+                "mlly": "^1.4.2",
+                "pkg-types": "^1.0.3"
+            },
+            "engines": {
+                "node": ">=14"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/antfu"
+            },
+            "integrity": "sha512-ok6z3qlYyCDS4ZEU27HaU6x/xZa9Whf8jD4ptH5UZTQYZVYeb9bnZ3ojVhiJNLiXK1Hfc0GNbLXcmZ5plLDDBg==",
+            "resolved": "https://registry.npmjs.org/local-pkg/-/local-pkg-0.5.0.tgz",
+            "version": "0.5.0"
+        },
         "node_modules/locate-path": {
             "dependencies": {
                 "p-locate": "^5.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
@@ -9067,15 +9415,14 @@
             "resolved": "https://registry.npmjs.org/loose-envify/-/loose-envify-1.4.0.tgz",
             "version": "1.4.0"
         },
         "node_modules/loupe": {
             "dependencies": {
                 "get-func-name": "^2.0.1"
             },
-            "dev": true,
             "integrity": "sha512-zSMINGVYkdpYSOBmLi0D1Uo7JU9nVdQKrHxC8eYlV+9YKK9WePqAlL7lSlorG/U2Fw1w0hTBmaa/jrQ3UbPHtA==",
             "resolved": "https://registry.npmjs.org/loupe/-/loupe-2.3.7.tgz",
             "version": "2.3.7"
         },
         "node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^3.0.2"
@@ -9094,15 +9441,14 @@
             "resolved": "https://registry.npmjs.org/lz-string/-/lz-string-1.5.0.tgz",
             "version": "1.5.0"
         },
         "node_modules/magic-string": {
             "dependencies": {
                 "@jridgewell/sourcemap-codec": "^1.4.15"
             },
-            "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-ISQTe55T2ao7XtlAStud6qwYPZjE4GK1S/BeVPus4jrq6JuOnQ00YKQC581RWhR122W7msZV263KzVeLoqidyQ==",
             "resolved": "https://registry.npmjs.org/magic-string/-/magic-string-0.30.8.tgz",
             "version": "0.30.8"
         },
@@ -9181,15 +9527,14 @@
         "node_modules/merge-descriptors": {
             "dev": true,
             "integrity": "sha512-cCi6g3/Zr1iqQi6ySbseM1Xvooa98N0w31jzUYrXPX2xqObmFGHJ0tQ5u74H3mVh7wLouTseZyYIq39g8cNp1w==",
             "resolved": "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/merge-stream": {
-            "dev": true,
             "integrity": "sha512-abv/qOcuPfk3URPfDzmZU1LKmuw8kT+0nIHvKrKgFrwifol/doWcdA4ZqsWQ8ENrFKkd67Mfpo/LovbIUsbt3w==",
             "resolved": "https://registry.npmjs.org/merge-stream/-/merge-stream-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/merge2": {
             "dev": true,
             "engines": {
@@ -9230,27 +9575,27 @@
                 "node": ">=4"
             },
             "integrity": "sha512-x0Vn8spI+wuJ1O6S7gnbaQg8Pxh4NNHb7KSINmEWKiPE4RKOplvijn+NkmYmmRgP68mc70j2EbeTFRsrswaQeg==",
             "resolved": "https://registry.npmjs.org/mime/-/mime-1.6.0.tgz",
             "version": "1.6.0"
         },
         "node_modules/mime-db": {
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": ">= 0.6"
             },
             "integrity": "sha512-sPU4uV7dYlvtWJxwwxHD0PuihVNiE7TyAbQ5SWxDCB9mUYvOgroQOwYQQOKPJ8CIbE+1ETVlOoK1UC2nU3gYvg==",
             "resolved": "https://registry.npmjs.org/mime-db/-/mime-db-1.52.0.tgz",
             "version": "1.52.0"
         },
         "node_modules/mime-types": {
             "dependencies": {
                 "mime-db": "1.52.0"
             },
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": ">= 0.6"
             },
             "integrity": "sha512-ZDY+bPm5zTTF+YpCrAU9nK0UgICYPT0QtT1NZWFv4s++TNkcgVaT0g6+4R2uI4MjQjzysHB1zxuWL50hzaeXiw==",
             "resolved": "https://registry.npmjs.org/mime-types/-/mime-types-2.1.35.tgz",
             "version": "2.1.35"
         },
@@ -9272,15 +9617,15 @@
             "resolved": "https://registry.npmjs.org/min-indent/-/min-indent-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^1.1.7"
             },
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==",
             "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.1.2.tgz",
             "version": "3.1.2"
         },
@@ -9347,25 +9692,34 @@
         },
         "node_modules/mkdirp-classic": {
             "dev": true,
             "integrity": "sha512-gKLcREMhtuZRwRAfqP3RFW+TK4JqApVBtOIftVgjuABpAtpxhPGaDcfvbhNvD0B8iD1oUr/txX35NjcaY6Ns/A==",
             "resolved": "https://registry.npmjs.org/mkdirp-classic/-/mkdirp-classic-0.5.3.tgz",
             "version": "0.5.3"
         },
+        "node_modules/mlly": {
+            "dependencies": {
+                "acorn": "^8.11.3",
+                "pathe": "^1.1.2",
+                "pkg-types": "^1.1.0",
+                "ufo": "^1.5.3"
+            },
+            "integrity": "sha512-U9SDaXGEREBYQgfejV97coK0UL1r+qnF2SyO9A3qcI8MzKnsIFKHNVEkrDyNncQTKQQumsasmeq84eNMdBfsNQ==",
+            "resolved": "https://registry.npmjs.org/mlly/-/mlly-1.7.0.tgz",
+            "version": "1.7.0"
+        },
         "node_modules/ms": {
-            "dev": true,
             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
         "node_modules/nanoid": {
             "bin": {
                 "nanoid": "bin/nanoid.cjs"
             },
-            "dev": true,
             "engines": {
                 "node": "^10 || ^12 || ^13.7 || ^14 || >=15.0.1"
             },
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
@@ -9484,14 +9838,20 @@
             "funding": {
                 "url": "https://github.com/fb55/nth-check?sponsor=1"
             },
             "integrity": "sha512-lqjrjmaOoAnWfMmBPL+XNnynZh2+swxiX3WUE0s4yEHI6m+AwrK2UZOimIRl3X/4QctVqS8AiZjFqyOGrMXb/w==",
             "resolved": "https://registry.npmjs.org/nth-check/-/nth-check-2.1.1.tgz",
             "version": "2.1.1"
         },
+        "node_modules/nwsapi": {
+            "devOptional": true,
+            "integrity": "sha512-QK0sRs7MKv0tKe1+5uZIQk/C8XGza4DAnztJG8iD+TpJIORARrCxczA738awHrZoHeTjSSoHqao2teO0dC/gFQ==",
+            "resolved": "https://registry.npmjs.org/nwsapi/-/nwsapi-2.2.10.tgz",
+            "version": "2.2.10"
+        },
         "node_modules/nypm": {
             "bin": {
                 "nypm": "dist/cli.mjs"
             },
             "dependencies": {
                 "citty": "^0.1.6",
                 "consola": "^3.2.3",
@@ -9720,15 +10080,15 @@
             "resolved": "https://registry.npmjs.org/on-headers/-/on-headers-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/once": {
             "dependencies": {
                 "wrappy": "1"
             },
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==",
             "resolved": "https://registry.npmjs.org/once/-/once-1.4.0.tgz",
             "version": "1.4.0"
         },
         "node_modules/onetime": {
             "dependencies": {
                 "mimic-fn": "^2.1.0"
@@ -9940,14 +10300,26 @@
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "integrity": "sha512-ayCKvm/phCGxOkYRSCM82iDwct8/EonSEgCSxWxD7ve6jHggsFl4fZVQBPRNgQoKiuV/odhFrGzQXZwbifC8Rg==",
             "resolved": "https://registry.npmjs.org/parse-json/-/parse-json-5.2.0.tgz",
             "version": "5.2.0"
         },
+        "node_modules/parse5": {
+            "dependencies": {
+                "entities": "^4.4.0"
+            },
+            "devOptional": true,
+            "funding": {
+                "url": "https://github.com/inikulin/parse5?sponsor=1"
+            },
+            "integrity": "sha512-Czj1WaSVpaoj0wbhMzLmWD69anp2WH7FXMB9n1Sy8/ZFF9jolSQVMu1Ij5WIyGmcBmhk7EOndpO4mIpihVqAXw==",
+            "resolved": "https://registry.npmjs.org/parse5/-/parse5-7.1.2.tgz",
+            "version": "7.1.2"
+        },
         "node_modules/parseurl": {
             "dev": true,
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-CiyeOxFT/JZyN5m0z9PfXw4SCBJ6Sygz1Dpl0wqjlhDEGGBP1GnsUVEL0p63hoG1fcj3fHynXi9NYO4nWOL+qQ==",
             "resolved": "https://registry.npmjs.org/parseurl/-/parseurl-1.3.3.tgz",
@@ -9959,24 +10331,23 @@
                 "node": ">=8"
             },
             "integrity": "sha512-ak9Qy5Q7jYb2Wwcey5Fpvg2KoAc/ZIhLSLOSBmRmygPsGwkVVt0fZa0qrtMz+m6tJTAHfZQ8FnmB4MG4LWy7/w==",
             "resolved": "https://registry.npmjs.org/path-exists/-/path-exists-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/path-is-absolute": {
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-AVbw3UJ2e9bq64vSaS9Am0fje1Pa8pbGqTTsmXfaIiMpnr5DlDhfJOuLj9Sf95ZPVDAUerDfEk88MPmPe7UCQg==",
             "resolved": "https://registry.npmjs.org/path-is-absolute/-/path-is-absolute-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/path-key": {
-            "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-ojmeN0qd+y0jszEtoY48r0Peq5dwMEkIlCOu6Q5f41lfkswXuKtYrhgoTpLnyIcHm24Uhqx+5Tqm2InSwLhE6Q==",
             "resolved": "https://registry.npmjs.org/path-key/-/path-key-3.1.1.tgz",
             "version": "3.1.1"
         },
@@ -10023,21 +10394,19 @@
                 "node": ">=8"
             },
             "integrity": "sha512-gDKb8aZMDeD/tZWs9P6+q0J9Mwkdl6xMV8TjnGP3qJVJ06bdMgkbBlLU8IdfOsIsFz2BW1rNVT3XuNEl8zPAvw==",
             "resolved": "https://registry.npmjs.org/path-type/-/path-type-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/pathe": {
-            "dev": true,
             "integrity": "sha512-whLdWMYL2TwI08hn8/ZqAbrVemu0LNaNNJZX73O6qaIdCTfXutsLhMkjdENX0qhsQ9uIimo4/aQOmXkoon2nDQ==",
             "resolved": "https://registry.npmjs.org/pathe/-/pathe-1.1.2.tgz",
             "version": "1.1.2"
         },
         "node_modules/pathval": {
-            "dev": true,
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-Dp6zGqpTdETdR63lehJYPeIOqpiNBNtc7BpWSLrOje7UaIsE5aY92r/AunQA7rsXvet3lrJ3JnZX29UPTKXyKQ==",
             "resolved": "https://registry.npmjs.org/pathval/-/pathval-1.1.1.tgz",
             "version": "1.1.1"
         },
@@ -10049,15 +10418,14 @@
             },
             "dev": true,
             "integrity": "sha512-FhJ+YbOSBb9/rIl2ZeE/QHEsWn7PqNYt8ARAY3kIgNGOk13g9FGyIY6JIl/xB/3TFRVoTv5as0l11weORrTekA==",
             "resolved": "https://registry.npmjs.org/peek-stream/-/peek-stream-1.1.3.tgz",
             "version": "1.1.3"
         },
         "node_modules/picocolors": {
-            "dev": true,
             "integrity": "sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==",
             "resolved": "https://registry.npmjs.org/picocolors/-/picocolors-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/picomatch": {
             "dev": true,
             "engines": {
@@ -10096,14 +10464,24 @@
             "engines": {
                 "node": ">=10"
             },
             "integrity": "sha512-NPE8TDbzl/3YQYY7CSS228s3g2ollTFnc+Qi3tqmqJp9Vg2ovUpixcJEo2HJScN2Ez+kEaal6y70c0ehqJBJeA==",
             "resolved": "https://registry.npmjs.org/pkg-dir/-/pkg-dir-5.0.0.tgz",
             "version": "5.0.0"
         },
+        "node_modules/pkg-types": {
+            "dependencies": {
+                "confbox": "^0.1.7",
+                "mlly": "^1.7.0",
+                "pathe": "^1.1.2"
+            },
+            "integrity": "sha512-ko14TjmDuQJ14zsotODv7dBlwxKhUKQEhuhmbqo1uCi9BB0Z2alo/wAXg6q1dTR5TyuqYyWhjtfe/Tsh+X28jQ==",
+            "resolved": "https://registry.npmjs.org/pkg-types/-/pkg-types-1.1.1.tgz",
+            "version": "1.1.1"
+        },
         "node_modules/polished": {
             "dependencies": {
                 "@babel/runtime": "^7.17.8"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
@@ -10123,15 +10501,14 @@
         },
         "node_modules/postcss": {
             "dependencies": {
                 "nanoid": "^3.3.7",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.2.0"
             },
-            "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/postcss/"
@@ -10244,14 +10621,20 @@
             "engines": {
                 "node": ">= 0.10"
             },
             "integrity": "sha512-llQsMLSUDUPT44jdrU/O37qlnifitDP+ZwrmmZcoSKyLKvtZxpyV0n2/bD/N4tBAAZ/gJEdZU7KMraoK1+XYAg==",
             "resolved": "https://registry.npmjs.org/proxy-addr/-/proxy-addr-2.0.7.tgz",
             "version": "2.0.7"
         },
+        "node_modules/psl": {
+            "devOptional": true,
+            "integrity": "sha512-E/ZsdU4HLs/68gYzgGTkMicWTLPdAftJLfJFlLUAAKZGkStNU72sZjT66SnMDVOfOWY/YAoiD7Jxa9iHvngcag==",
+            "resolved": "https://registry.npmjs.org/psl/-/psl-1.9.0.tgz",
+            "version": "1.9.0"
+        },
         "node_modules/pump": {
             "dependencies": {
                 "end-of-stream": "^1.1.0",
                 "once": "^1.3.1"
             },
             "dev": true,
             "integrity": "sha512-LwZy+p3SFs1Pytd/jYct4wpv49HiYCqd9Rlc5ZVdk0V+8Yzv6jR5Blk3TRmPL1ft69TxP0IMZGJ+WPFU2BFhww==",
@@ -10275,14 +10658,23 @@
                 "once": "^1.3.1"
             },
             "dev": true,
             "integrity": "sha512-ruPMNRkN3MHP1cWJc9OWr+T/xDP0jhXYCLfJcBuX54hhfIBnaQmAUMfDcG4DM5UMWByBbJY69QSphm3jtDKIkA==",
             "resolved": "https://registry.npmjs.org/pump/-/pump-2.0.1.tgz",
             "version": "2.0.1"
         },
+        "node_modules/punycode": {
+            "devOptional": true,
+            "engines": {
+                "node": ">=6"
+            },
+            "integrity": "sha512-vYt7UD1U9Wg6138shLtLOvdAu+8DsC/ilFtEVHcH+wydcSpNE20AfSOduf6MkRFahL5FY7X1oU7nKVZFtfq8Fg==",
+            "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.3.1.tgz",
+            "version": "2.3.1"
+        },
         "node_modules/qs": {
             "dependencies": {
                 "side-channel": "^1.0.6"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.6"
@@ -10290,14 +10682,20 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-trVZiI6RMOkO476zLGaBIzszOdFPnCCXHPG9kn0yuS1uz6xdVxPfZdB3vUig9pxPFDM9BRAgz/YUIVQ1/vuiUg==",
             "resolved": "https://registry.npmjs.org/qs/-/qs-6.12.0.tgz",
             "version": "6.12.0"
         },
+        "node_modules/querystringify": {
+            "devOptional": true,
+            "integrity": "sha512-FIqgj2EUvTa7R50u0rGsyTftzjYmv/a3hO345bZNrqabNqjtgiDMgmo4mkUjd+nzU5oF3dClKqFIPUKybUyqoQ==",
+            "resolved": "https://registry.npmjs.org/querystringify/-/querystringify-2.2.0.tgz",
+            "version": "2.2.0"
+        },
         "node_modules/queue-microtask": {
             "dev": true,
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/feross"
                 },
@@ -10705,14 +11103,20 @@
                 "type": "opencollective",
                 "url": "https://opencollective.com/unified"
             },
             "integrity": "sha512-lWyvf/jwu+oS5+hL5eClVd3hNdmwM1kAC0BUvEGD19pajQMIzcNUd/k9GsfQ+FfECvX+JE+e9/btsKH0EjJT6A==",
             "resolved": "https://registry.npmjs.org/rehype-slug/-/rehype-slug-6.0.0.tgz",
             "version": "6.0.0"
         },
+        "node_modules/requires-port": {
+            "devOptional": true,
+            "integrity": "sha512-KigOCHcocU3XODJxsu8i/j8T9tzT4adHiecwORRQ0ZZFcp7ahwXuRU1m+yuO90C5ZUyGeGfocHDI14M3L3yDAQ==",
+            "resolved": "https://registry.npmjs.org/requires-port/-/requires-port-1.0.0.tgz",
+            "version": "1.0.0"
+        },
         "node_modules/resolve": {
             "bin": {
                 "resolve": "bin/resolve"
             },
             "dependencies": {
                 "is-core-module": "^2.13.0",
                 "path-parse": "^1.0.7",
@@ -10773,15 +11177,14 @@
         "node_modules/rollup": {
             "bin": {
                 "rollup": "dist/bin/rollup"
             },
             "dependencies": {
                 "@types/estree": "1.0.5"
             },
-            "dev": true,
             "engines": {
                 "node": ">=18.0.0",
                 "npm": ">=8.0.0"
             },
             "integrity": "sha512-3YegKemjoQnYKmsBlOHfMLVPPA5xLkQ8MHLLSw/fBrFaVkEayL51DilPpNNLq1exr98F2B1TzrV0FUlN3gWRPg==",
             "optionalDependencies": {
                 "@rollup/rollup-android-arm-eabi": "4.13.0",
@@ -10798,14 +11201,20 @@
                 "@rollup/rollup-win32-ia32-msvc": "4.13.0",
                 "@rollup/rollup-win32-x64-msvc": "4.13.0",
                 "fsevents": "~2.3.2"
             },
             "resolved": "https://registry.npmjs.org/rollup/-/rollup-4.13.0.tgz",
             "version": "4.13.0"
         },
+        "node_modules/rrweb-cssom": {
+            "devOptional": true,
+            "integrity": "sha512-APM0Gt1KoXBz0iIkkdB/kfvGOwC4UuJFeG/c+yV7wSc7q96cG/kJ0HiYCnzivD9SB53cLV1MlHFNfOuPaadYSw==",
+            "resolved": "https://registry.npmjs.org/rrweb-cssom/-/rrweb-cssom-0.6.0.tgz",
+            "version": "0.6.0"
+        },
         "node_modules/run-parallel": {
             "dependencies": {
                 "queue-microtask": "^1.2.2"
             },
             "dev": true,
             "funding": [
                 {
@@ -10828,25 +11237,37 @@
         "node_modules/safe-buffer": {
             "dev": true,
             "integrity": "sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==",
             "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.1.2.tgz",
             "version": "5.1.2"
         },
         "node_modules/safer-buffer": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
             "resolved": "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz",
             "version": "2.1.2"
         },
         "node_modules/sax": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-0s+oAmw9zLl1V1cS9BtZN7JAd0cW5e0QH4W3LWEK6a4LaLEA2OTpGYWDY+6XasBLtz6wkm3u1xRw95mRuJ59WA==",
             "resolved": "https://registry.npmjs.org/sax/-/sax-1.3.0.tgz",
             "version": "1.3.0"
         },
+        "node_modules/saxes": {
+            "dependencies": {
+                "xmlchars": "^2.2.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=v12.22.7"
+            },
+            "integrity": "sha512-xAg7SOnEhrm5zI3puOOKyy1OMcMlIJZYNJY7xLBwSze0UjhPLnWfj2GF2EpT0jmzaJKIWKHLsaSSajf35bcYnA==",
+            "resolved": "https://registry.npmjs.org/saxes/-/saxes-6.0.0.tgz",
+            "version": "6.0.0"
+        },
         "node_modules/scheduler": {
             "dependencies": {
                 "loose-envify": "^1.1.0"
             },
             "dev": true,
             "integrity": "sha512-CtuThmgHNg7zIZWAXi3AsyIzA3n4xx7aNyjwC2VJldO2LMVDhFK+63xGqq6CsJH4rTAt6/M+N4GhZiDYPx9eUw==",
             "resolved": "https://registry.npmjs.org/scheduler/-/scheduler-0.23.0.tgz",
@@ -10990,24 +11411,22 @@
             "resolved": "https://registry.npmjs.org/shallow-clone/-/shallow-clone-3.0.1.tgz",
             "version": "3.0.1"
         },
         "node_modules/shebang-command": {
             "dependencies": {
                 "shebang-regex": "^3.0.0"
             },
-            "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-kHxr2zZpYtdmrN1qDjrrX/Z1rR1kG8Dx+gkpK1G4eXmvXswmcE1hTWBWYUzlraYw1/yZp6YuDY77YtvbN0dmDA==",
             "resolved": "https://registry.npmjs.org/shebang-command/-/shebang-command-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/shebang-regex": {
-            "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==",
             "resolved": "https://registry.npmjs.org/shebang-regex/-/shebang-regex-3.0.0.tgz",
             "version": "3.0.0"
         },
@@ -11025,14 +11444,19 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-fDW/EZ6Q9RiO8eFG8Hj+7u/oW+XrPTIChwCOM2+th2A6OblDtYYIpve9m+KvI9Z4C9qSEXlaGR6bTEYHReuglA==",
             "resolved": "https://registry.npmjs.org/side-channel/-/side-channel-1.0.6.tgz",
             "version": "1.0.6"
         },
+        "node_modules/siginfo": {
+            "integrity": "sha512-ybx0WO1/8bSBLEWXZvEd7gMW3Sn3JFlW3TvX1nREbDLRNQNaeNN8WK0meBwPdAaOI7TtRRRJn/Es1zhrrCHu7g==",
+            "resolved": "https://registry.npmjs.org/siginfo/-/siginfo-2.0.0.tgz",
+            "version": "2.0.0"
+        },
         "node_modules/signal-exit": {
             "dev": true,
             "integrity": "sha512-wnD2ZE+l+SPC/uoS0vXeE9L1+0wuaMqKlfz9AMUo38JsyLSBWSFcHR1Rri62LZc12vLr1gb3jl7iwQhgwpAbGQ==",
             "resolved": "https://registry.npmjs.org/signal-exit/-/signal-exit-3.0.7.tgz",
             "version": "3.0.7"
         },
         "node_modules/sisteransi": {
@@ -11108,24 +11532,23 @@
             "peerDependencies": {
                 "solid-js": "^1.3"
             },
             "resolved": "https://registry.npmjs.org/solid-refresh/-/solid-refresh-0.6.3.tgz",
             "version": "0.6.3"
         },
         "node_modules/source-map": {
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-l3BikUxvPOcn5E74dZiq5BGsTb5yEwhaTSzccU6t4sDOH8NWJCstKO5QT2CvtFoK6F0saL7p9xHAqHOlCPJygA==",
             "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.7.4.tgz",
             "version": "0.7.4"
         },
         "node_modules/source-map-js": {
-            "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-itJW8lvSA0TXEphiRoawsCksnlf8SyvmFzIhltqAHluXd88pkCd+cXJVHTDwdCr0IzwptSm035IHQktUu1QUMg==",
             "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.2.0.tgz",
             "version": "1.2.0"
         },
@@ -11186,23 +11609,33 @@
         },
         "node_modules/spdx-license-ids": {
             "dev": true,
             "integrity": "sha512-sh8PWc/ftMqAAdFiBu6Fy6JUOYjqDJBJvIhpfDMyHrr0Rbp5liZqd4TjtQ/RgfLjKFZb+LMx5hpml5qOWy0qvg==",
             "resolved": "https://registry.npmjs.org/spdx-license-ids/-/spdx-license-ids-3.0.17.tgz",
             "version": "3.0.17"
         },
+        "node_modules/stackback": {
+            "integrity": "sha512-1XMJE5fQo1jGH6Y/7ebnwPOBEkIEnT4QF32d5R1+VXdXveM0IBMJt8zfaxX1P3QhVwrYe+576+jkANtSS2mBbw==",
+            "resolved": "https://registry.npmjs.org/stackback/-/stackback-0.0.2.tgz",
+            "version": "0.0.2"
+        },
         "node_modules/statuses": {
             "dev": true,
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-RwNA9Z/7PrK06rYLIzFMlaF+l73iwpzsqRIFgbMLbTcLD6cOao82TaWefPXQvB2fOC4AjuYSEndS7N/mTCbkdQ==",
             "resolved": "https://registry.npmjs.org/statuses/-/statuses-2.0.1.tgz",
             "version": "2.0.1"
         },
+        "node_modules/std-env": {
+            "integrity": "sha512-JPbdCEQLj1w5GilpiHAx3qJvFndqybBysA3qUOnznweH4QbNYUsW/ea8QzSrnh0vNsezMMw5bcVool8lM0gwzg==",
+            "resolved": "https://registry.npmjs.org/std-env/-/std-env-3.7.0.tgz",
+            "version": "3.7.0"
+        },
         "node_modules/stop-iteration-iterator": {
             "dependencies": {
                 "internal-slot": "^1.0.4"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
@@ -11424,26 +11857,42 @@
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "integrity": "sha512-6fPc+R4ihwqP6N/aIv2f1gMH8lOVtWQHoqC4yK6oSDVVocumAsfCqjkXnqiYMhmMwS/mEHLp7Vehlt3ql6lEig==",
             "resolved": "https://registry.npmjs.org/strip-json-comments/-/strip-json-comments-3.1.1.tgz",
             "version": "3.1.1"
         },
+        "node_modules/strip-literal": {
+            "dependencies": {
+                "js-tokens": "^9.0.0"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/antfu"
+            },
+            "integrity": "sha512-Op+UycaUt/8FbN/Z2TWPBLge3jWrP3xj10f3fnYxf052bKuS3EKs1ZQcVGjnEMdsNVAM+plXRdmjrZ/KgG3Skw==",
+            "resolved": "https://registry.npmjs.org/strip-literal/-/strip-literal-2.1.0.tgz",
+            "version": "2.1.0"
+        },
+        "node_modules/strip-literal/node_modules/js-tokens": {
+            "integrity": "sha512-WriZw1luRMlmV3LGJaR6QOJjWwgLUTf89OwT2lUOyjX2dJGBwgmIkbcz+7WFZjrZM635JOIR517++e/67CP9dQ==",
+            "resolved": "https://registry.npmjs.org/js-tokens/-/js-tokens-9.0.0.tgz",
+            "version": "9.0.0"
+        },
         "node_modules/stylus": {
             "bin": {
                 "stylus": "bin/stylus"
             },
             "dependencies": {
                 "@adobe/css-tools": "~4.3.3",
                 "debug": "^4.3.2",
                 "glob": "^7.1.6",
                 "sax": "~1.3.0",
                 "source-map": "^0.7.3"
             },
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": "*"
             },
             "funding": {
                 "url": "https://opencollective.com/stylus"
             },
             "integrity": "sha512-OMlgrTCPzE/ibtRMoeLVhOY0RcNuNWh0rhAVqeKnk/QwcuUKQbnqhZ1kg2vzD8VU/6h3FoPTq4RJPHgLBvX6Bw==",
@@ -11504,14 +11953,20 @@
             "engines": {
                 "node": ">= 10"
             },
             "integrity": "sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-7.2.0.tgz",
             "version": "7.2.0"
         },
+        "node_modules/symbol-tree": {
+            "devOptional": true,
+            "integrity": "sha512-9QNk5KwDF+Bvz+PyObkmSYjI5ksVUYtjW7AU22r2NKcfLJcXp96hkDWU3+XndOsUb+AQ9QhfzfCT2O+CNWT5Tw==",
+            "resolved": "https://registry.npmjs.org/symbol-tree/-/symbol-tree-3.2.4.tgz",
+            "version": "3.2.4"
+        },
         "node_modules/tar": {
             "dependencies": {
                 "chownr": "^2.0.0",
                 "fs-minipass": "^2.0.0",
                 "minipass": "^5.0.0",
                 "minizlib": "^2.1.1",
                 "mkdirp": "^1.0.3",
@@ -11668,16 +12123,42 @@
         },
         "node_modules/tiny-invariant": {
             "dev": true,
             "integrity": "sha512-+FbBPE1o9QAYvviau/qC5SE3caw21q3xkvWKBtja5vgqOWIHHJ3ioaq1VPfn/Szqctz2bU/oYeKd9/z5BL+PVg==",
             "resolved": "https://registry.npmjs.org/tiny-invariant/-/tiny-invariant-1.3.3.tgz",
             "version": "1.3.3"
         },
+        "node_modules/tinybench": {
+            "integrity": "sha512-1/eK7zUnIklz4JUUlL+658n58XO2hHLQfSk1Zf2LKieUjxidN16eKFEoDEfjHc3ohofSSqK3X5yO6VGb6iW8Lw==",
+            "resolved": "https://registry.npmjs.org/tinybench/-/tinybench-2.8.0.tgz",
+            "version": "2.8.0"
+        },
+        "node_modules/tinycolor2": {
+            "integrity": "sha512-XPaBkWQJdsf3pLKJV9p4qN/S+fm2Oj8AIPo1BTUhg5oxkvm9+SVEGFdhyOz7tTdUTfvxMiAs4sp6/eZO2Ew+pw==",
+            "resolved": "https://registry.npmjs.org/tinycolor2/-/tinycolor2-1.6.0.tgz",
+            "version": "1.6.0"
+        },
+        "node_modules/tinygradient": {
+            "dependencies": {
+                "@types/tinycolor2": "^1.4.0",
+                "tinycolor2": "^1.0.0"
+            },
+            "integrity": "sha512-8nIfc2vgQ4TeLnk2lFj4tRLvvJwEfQuabdsmvDdQPT0xlk9TaNtpGd6nNRxXoK6vQhN6RSzj+Cnp5tTQmpxmbw==",
+            "resolved": "https://registry.npmjs.org/tinygradient/-/tinygradient-1.1.5.tgz",
+            "version": "1.1.5"
+        },
+        "node_modules/tinypool": {
+            "engines": {
+                "node": ">=14.0.0"
+            },
+            "integrity": "sha512-i11VH5gS6IFeLY3gMBQ00/MmLncVP7JLXOw1vlgkytLmJK7QnEr7NXf0LBdxfmNPAeyetukOk0bOYrJrFGjYJQ==",
+            "resolved": "https://registry.npmjs.org/tinypool/-/tinypool-0.8.4.tgz",
+            "version": "0.8.4"
+        },
         "node_modules/tinyspy": {
-            "dev": true,
             "engines": {
                 "node": ">=14.0.0"
             },
             "integrity": "sha512-KYad6Vy5VDWV4GH3fjpseMQ/XU2BhIYP7Vzd0LG44qRWm/Yt2WCOTicFdvmgo6gWaqooMQCawTtILVQJupKu7A==",
             "resolved": "https://registry.npmjs.org/tinyspy/-/tinyspy-2.2.1.tgz",
             "version": "2.2.1"
         },
@@ -11713,14 +12194,38 @@
             "engines": {
                 "node": ">=0.6"
             },
             "integrity": "sha512-o5sSPKEkg/DIQNmH43V0/uerLrpzVedkUh8tGNvaeXpfpuwjKenlSox/2O/BTlZUtEe+JG7s5YhEz608PlAHRA==",
             "resolved": "https://registry.npmjs.org/toidentifier/-/toidentifier-1.0.1.tgz",
             "version": "1.0.1"
         },
+        "node_modules/tough-cookie": {
+            "dependencies": {
+                "psl": "^1.1.33",
+                "punycode": "^2.1.1",
+                "universalify": "^0.2.0",
+                "url-parse": "^1.5.3"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=6"
+            },
+            "integrity": "sha512-Loo5UUvLD9ScZ6jh8beX1T6sO1w2/MpCRpEP7V280GKMVUQ0Jzar2U3UJPsrdbziLEMMhu3Ujnq//rhiFuIeag==",
+            "resolved": "https://registry.npmjs.org/tough-cookie/-/tough-cookie-4.1.4.tgz",
+            "version": "4.1.4"
+        },
+        "node_modules/tough-cookie/node_modules/universalify": {
+            "devOptional": true,
+            "engines": {
+                "node": ">= 4.0.0"
+            },
+            "integrity": "sha512-CJ1QgKmNg3CwvAv/kOFmtnEN05f0D/cn9QntgNOQlQF9dgvVTHj3t+8JPdjqawCHk7V/KA+fbUqzZ9XWhcqPUg==",
+            "resolved": "https://registry.npmjs.org/universalify/-/universalify-0.2.0.tgz",
+            "version": "0.2.0"
+        },
         "node_modules/tr46": {
             "dev": true,
             "integrity": "sha512-N3WMsuqV66lT30CrXNbEjx4GEwlow3v6rr4mCcv6prnfwhS01rkgyFdjPNBYd9br7LpXV1+Emh01fHnq2Gdgrw==",
             "resolved": "https://registry.npmjs.org/tr46/-/tr46-0.0.3.tgz",
             "version": "0.0.3"
         },
         "node_modules/ts-dedent": {
@@ -11741,15 +12246,14 @@
         "node_modules/tween-functions": {
             "dev": true,
             "integrity": "sha512-PZBtLYcCLtEcjL14Fzb1gSxPBeL7nWvGhO5ZFPGqziCcr8uvHp0NDmdjBchp6KHL+tExcg0m3NISmKxhU394dA==",
             "resolved": "https://registry.npmjs.org/tween-functions/-/tween-functions-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/type-detect": {
-            "dev": true,
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-0fr/mIH1dlO+x7TlcMy+bIDqKPsw/70tVyeHW787goQjhmqaZe10uwLujubK9q9Lg6Fiho1KUKDYz0Z7k7g5/g==",
             "resolved": "https://registry.npmjs.org/type-detect/-/type-detect-4.0.8.tgz",
             "version": "4.0.8"
         },
@@ -11788,15 +12292,14 @@
                 "node": ">=14.17"
             },
             "integrity": "sha512-KrPd3PKaCLr78MalgiwJnA25Nm8HAmdwN3mYUYZgG/wizIo9EainNVQI9/yDavtVFRN2h3k8uf3GLHuhDMgEHg==",
             "resolved": "https://registry.npmjs.org/typescript/-/typescript-5.4.3.tgz",
             "version": "5.4.3"
         },
         "node_modules/ufo": {
-            "dev": true,
             "integrity": "sha512-Y7HYmWaFwPUmkoQCUIAYpKqkOf+SbVj/2fJJZ4RJMCfZp0rTGwRbzQD+HghfnhKOjL9E01okqz+ncJskGYfBNw==",
             "resolved": "https://registry.npmjs.org/ufo/-/ufo-1.5.3.tgz",
             "version": "1.5.3"
         },
         "node_modules/uglify-js": {
             "bin": {
                 "uglifyjs": "bin/uglifyjs"
@@ -11807,15 +12310,15 @@
             },
             "integrity": "sha512-T9q82TJI9e/C1TAxYvfb16xO120tMVFZrGA3f9/P4424DNu6ypK103y0GPFVa17yotwSyZW5iYXgjYHkGrJW/g==",
             "optional": true,
             "resolved": "https://registry.npmjs.org/uglify-js/-/uglify-js-3.17.4.tgz",
             "version": "3.17.4"
         },
         "node_modules/undici-types": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-JlCMO+ehdEIKqlFxk6IfVoAUVmgz7cU7zD/h9XZ0qzeosSHmUJVOzSQvvYSYWXkFXC+IfLKSIffhv0sVZup6pA==",
             "resolved": "https://registry.npmjs.org/undici-types/-/undici-types-5.26.5.tgz",
             "version": "5.26.5"
         },
         "node_modules/unicode-canonical-property-names-ecmascript": {
             "dev": true,
             "engines": {
@@ -11978,14 +12481,24 @@
             "integrity": "sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==",
             "peerDependencies": {
                 "browserslist": ">= 4.21.0"
             },
             "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.13.tgz",
             "version": "1.0.13"
         },
+        "node_modules/url-parse": {
+            "dependencies": {
+                "querystringify": "^2.1.1",
+                "requires-port": "^1.0.0"
+            },
+            "devOptional": true,
+            "integrity": "sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==",
+            "resolved": "https://registry.npmjs.org/url-parse/-/url-parse-1.5.10.tgz",
+            "version": "1.5.10"
+        },
         "node_modules/util": {
             "dependencies": {
                 "inherits": "^2.0.3",
                 "is-arguments": "^1.0.4",
                 "is-generator-function": "^1.0.7",
                 "is-typed-array": "^1.1.3",
                 "which-typed-array": "^1.1.2"
@@ -12053,15 +12566,14 @@
                 "vite": "bin/vite.js"
             },
             "dependencies": {
                 "esbuild": "^0.20.1",
                 "postcss": "^8.4.36",
                 "rollup": "^4.13.0"
             },
-            "dev": true,
             "engines": {
                 "node": "^18.0.0 || >=20.0.0"
             },
             "funding": {
                 "url": "https://github.com/vitejs/vite?sponsor=1"
             },
             "integrity": "sha512-FPtnxFlSIKYjZ2eosBQamz4CbyrTizbZ3hnGJlh/wMtCrlp1Hah6AzBLjGI5I2urTfNnpovpHdrL6YRuBOPnCA==",
@@ -12099,14 +12611,35 @@
                 "terser": {
                     "optional": true
                 }
             },
             "resolved": "https://registry.npmjs.org/vite/-/vite-5.2.6.tgz",
             "version": "5.2.6"
         },
+        "node_modules/vite-node": {
+            "bin": {
+                "vite-node": "vite-node.mjs"
+            },
+            "dependencies": {
+                "cac": "^6.7.14",
+                "debug": "^4.3.4",
+                "pathe": "^1.1.1",
+                "picocolors": "^1.0.0",
+                "vite": "^5.0.0"
+            },
+            "engines": {
+                "node": "^18.0.0 || >=20.0.0"
+            },
+            "funding": {
+                "url": "https://opencollective.com/vitest"
+            },
+            "integrity": "sha512-de6HJgzC+TFzOu0NTC4RAIsyf/DY/ibWDYQUcuEA84EMHhcefTUGkjFHKKEJhQN4A+6I0u++kr3l36ZF2d7XRw==",
+            "resolved": "https://registry.npmjs.org/vite-node/-/vite-node-1.6.0.tgz",
+            "version": "1.6.0"
+        },
         "node_modules/vite-plugin-prismjs": {
             "dependencies": {
                 "@babel/core": "^7.15.5",
                 "babel-plugin-prismjs": "^2.1.0"
             },
             "dev": true,
             "engines": {
@@ -12163,14 +12696,227 @@
                 "vite": {
                     "optional": true
                 }
             },
             "resolved": "https://registry.npmjs.org/vitefu/-/vitefu-0.2.5.tgz",
             "version": "0.2.5"
         },
+        "node_modules/vitest": {
+            "bin": {
+                "vitest": "vitest.mjs"
+            },
+            "dependencies": {
+                "@vitest/expect": "1.6.0",
+                "@vitest/runner": "1.6.0",
+                "@vitest/snapshot": "1.6.0",
+                "@vitest/spy": "1.6.0",
+                "@vitest/utils": "1.6.0",
+                "acorn-walk": "^8.3.2",
+                "chai": "^4.3.10",
+                "debug": "^4.3.4",
+                "execa": "^8.0.1",
+                "local-pkg": "^0.5.0",
+                "magic-string": "^0.30.5",
+                "pathe": "^1.1.1",
+                "picocolors": "^1.0.0",
+                "std-env": "^3.5.0",
+                "strip-literal": "^2.0.0",
+                "tinybench": "^2.5.1",
+                "tinypool": "^0.8.3",
+                "vite": "^5.0.0",
+                "vite-node": "1.6.0",
+                "why-is-node-running": "^2.2.2"
+            },
+            "engines": {
+                "node": "^18.0.0 || >=20.0.0"
+            },
+            "funding": {
+                "url": "https://opencollective.com/vitest"
+            },
+            "integrity": "sha512-H5r/dN06swuFnzNFhq/dnz37bPXnq8xB2xB5JOVk8K09rUtoeNN+LHWkoQ0A/i3hvbUKKcCei9KpbxqHMLhLLA==",
+            "peerDependencies": {
+                "@edge-runtime/vm": "*",
+                "@types/node": "^18.0.0 || >=20.0.0",
+                "@vitest/browser": "1.6.0",
+                "@vitest/ui": "1.6.0",
+                "happy-dom": "*",
+                "jsdom": "*"
+            },
+            "peerDependenciesMeta": {
+                "@edge-runtime/vm": {
+                    "optional": true
+                },
+                "@types/node": {
+                    "optional": true
+                },
+                "@vitest/browser": {
+                    "optional": true
+                },
+                "@vitest/ui": {
+                    "optional": true
+                },
+                "happy-dom": {
+                    "optional": true
+                },
+                "jsdom": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/vitest/-/vitest-1.6.0.tgz",
+            "version": "1.6.0"
+        },
+        "node_modules/vitest/node_modules/@vitest/expect": {
+            "dependencies": {
+                "@vitest/spy": "1.6.0",
+                "@vitest/utils": "1.6.0",
+                "chai": "^4.3.10"
+            },
+            "funding": {
+                "url": "https://opencollective.com/vitest"
+            },
+            "integrity": "sha512-ixEvFVQjycy/oNgHjqsL6AZCDduC+tflRluaHIzKIsdbzkLn2U/iBnVeJwB6HsIjQBdfMR8Z0tRxKUsvFJEeWQ==",
+            "resolved": "https://registry.npmjs.org/@vitest/expect/-/expect-1.6.0.tgz",
+            "version": "1.6.0"
+        },
+        "node_modules/vitest/node_modules/execa": {
+            "dependencies": {
+                "cross-spawn": "^7.0.3",
+                "get-stream": "^8.0.1",
+                "human-signals": "^5.0.0",
+                "is-stream": "^3.0.0",
+                "merge-stream": "^2.0.0",
+                "npm-run-path": "^5.1.0",
+                "onetime": "^6.0.0",
+                "signal-exit": "^4.1.0",
+                "strip-final-newline": "^3.0.0"
+            },
+            "engines": {
+                "node": ">=16.17"
+            },
+            "funding": {
+                "url": "https://github.com/sindresorhus/execa?sponsor=1"
+            },
+            "integrity": "sha512-VyhnebXciFV2DESc+p6B+y0LjSm0krU4OgJN44qFAhBY0TJ+1V61tYD2+wHusZ6F9n5K+vl8k0sTy7PEfV4qpg==",
+            "resolved": "https://registry.npmjs.org/execa/-/execa-8.0.1.tgz",
+            "version": "8.0.1"
+        },
+        "node_modules/vitest/node_modules/get-stream": {
+            "engines": {
+                "node": ">=16"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-VaUJspBffn/LMCJVoMvSAdmscJyS1auj5Zulnn5UoYcY531UWmdwhRWkcGKnGU93m5HSXP9LP2usOryrBtQowA==",
+            "resolved": "https://registry.npmjs.org/get-stream/-/get-stream-8.0.1.tgz",
+            "version": "8.0.1"
+        },
+        "node_modules/vitest/node_modules/human-signals": {
+            "engines": {
+                "node": ">=16.17.0"
+            },
+            "integrity": "sha512-AXcZb6vzzrFAUE61HnN4mpLqd/cSIwNQjtNWR0euPm6y0iqx3G4gOXaIDdtdDwZmhwe82LA6+zinmW4UBWVePQ==",
+            "resolved": "https://registry.npmjs.org/human-signals/-/human-signals-5.0.0.tgz",
+            "version": "5.0.0"
+        },
+        "node_modules/vitest/node_modules/is-stream": {
+            "engines": {
+                "node": "^12.20.0 || ^14.13.1 || >=16.0.0"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-LnQR4bZ9IADDRSkvpqMGvt/tEJWclzklNgSw48V5EAaAeDd6qGvN8ei6k5p0tvxSR171VmGyHuTiAOfxAbr8kA==",
+            "resolved": "https://registry.npmjs.org/is-stream/-/is-stream-3.0.0.tgz",
+            "version": "3.0.0"
+        },
+        "node_modules/vitest/node_modules/mimic-fn": {
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-vqiC06CuhBTUdZH+RYl8sFrL096vA45Ok5ISO6sE/Mr1jRbGH4Csnhi8f3wKVl7x8mO4Au7Ir9D3Oyv1VYMFJw==",
+            "resolved": "https://registry.npmjs.org/mimic-fn/-/mimic-fn-4.0.0.tgz",
+            "version": "4.0.0"
+        },
+        "node_modules/vitest/node_modules/npm-run-path": {
+            "dependencies": {
+                "path-key": "^4.0.0"
+            },
+            "engines": {
+                "node": "^12.20.0 || ^14.13.1 || >=16.0.0"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-ppwTtiJZq0O/ai0z7yfudtBpWIoxM8yE6nHi1X47eFR2EWORqfbu6CnPlNsjeN683eT0qG6H/Pyf9fCcvjnnnQ==",
+            "resolved": "https://registry.npmjs.org/npm-run-path/-/npm-run-path-5.3.0.tgz",
+            "version": "5.3.0"
+        },
+        "node_modules/vitest/node_modules/onetime": {
+            "dependencies": {
+                "mimic-fn": "^4.0.0"
+            },
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-1FlR+gjXK7X+AsAHso35MnyN5KqGwJRi/31ft6x0M194ht7S+rWAvd7PHss9xSKMzE0asv1pyIHaJYq+BbacAQ==",
+            "resolved": "https://registry.npmjs.org/onetime/-/onetime-6.0.0.tgz",
+            "version": "6.0.0"
+        },
+        "node_modules/vitest/node_modules/path-key": {
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-haREypq7xkM7ErfgIyA0z+Bj4AGKlMSdlQE2jvJo6huWD1EdkKYV+G/T4nq0YEF2vgTT8kqMFKo1uHn950r4SQ==",
+            "resolved": "https://registry.npmjs.org/path-key/-/path-key-4.0.0.tgz",
+            "version": "4.0.0"
+        },
+        "node_modules/vitest/node_modules/signal-exit": {
+            "engines": {
+                "node": ">=14"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/isaacs"
+            },
+            "integrity": "sha512-bzyZ1e88w9O1iNJbKnOlvYTrWPDl46O1bG0D3XInv+9tkPrxrN8jUUTiFlDkkmKWgn1M6CfIA13SuGqOa9Korw==",
+            "resolved": "https://registry.npmjs.org/signal-exit/-/signal-exit-4.1.0.tgz",
+            "version": "4.1.0"
+        },
+        "node_modules/vitest/node_modules/strip-final-newline": {
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-dOESqjYr96iWYylGObzd39EuNTa5VJxyvVAEm5Jnh7KGo75V43Hk1odPQkNDyXNmUR6k+gEiDVXnjB8HJ3crXw==",
+            "resolved": "https://registry.npmjs.org/strip-final-newline/-/strip-final-newline-3.0.0.tgz",
+            "version": "3.0.0"
+        },
+        "node_modules/w3c-xmlserializer": {
+            "dependencies": {
+                "xml-name-validator": "^5.0.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-o8qghlI8NZHU1lLPrpi2+Uq7abh4GGPpYANlalzWxyWteJOCsr/P+oPBA49TOLu5FTZO4d3F9MnWJfiMo4BkmA==",
+            "resolved": "https://registry.npmjs.org/w3c-xmlserializer/-/w3c-xmlserializer-5.0.0.tgz",
+            "version": "5.0.0"
+        },
         "node_modules/watchpack": {
             "dependencies": {
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.1.2"
             },
             "dev": true,
             "engines": {
@@ -12206,14 +12952,47 @@
         },
         "node_modules/webpack-virtual-modules": {
             "dev": true,
             "integrity": "sha512-poXpCylU7ExuvZK8z+On3kX+S8o/2dQ/SVYueKA0D4WEMXROXgY8Ez50/bQEUmvoSMMrWcrJqCHuhAbsiwg7Dg==",
             "resolved": "https://registry.npmjs.org/webpack-virtual-modules/-/webpack-virtual-modules-0.6.1.tgz",
             "version": "0.6.1"
         },
+        "node_modules/whatwg-encoding": {
+            "dependencies": {
+                "iconv-lite": "0.6.3"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-6qN4hJdMwfYBtE3YBTTHhoeuUrDBPZmbQaxWAqSALV/MeEnR5z1xd8UKud2RAkFoPkmB+hli1TZSnyi84xz1vQ==",
+            "resolved": "https://registry.npmjs.org/whatwg-encoding/-/whatwg-encoding-3.1.1.tgz",
+            "version": "3.1.1"
+        },
+        "node_modules/whatwg-encoding/node_modules/iconv-lite": {
+            "dependencies": {
+                "safer-buffer": ">= 2.1.2 < 3.0.0"
+            },
+            "devOptional": true,
+            "engines": {
+                "node": ">=0.10.0"
+            },
+            "integrity": "sha512-4fCk79wshMdzMp2rH06qWrJE4iolqLhCUH+OiuIgU++RB0+94NlDL81atO7GX55uUKueo0txHNtvEyI6D7WdMw==",
+            "resolved": "https://registry.npmjs.org/iconv-lite/-/iconv-lite-0.6.3.tgz",
+            "version": "0.6.3"
+        },
+        "node_modules/whatwg-mimetype": {
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-QaKxh0eNIi2mE9p2vEdzfagOKHCcj1pJ56EEHGQOVxp8r9/iszLUUV7v89x9O1p/T+NlTM5W7jW6+cz4Fq1YVg==",
+            "resolved": "https://registry.npmjs.org/whatwg-mimetype/-/whatwg-mimetype-4.0.0.tgz",
+            "version": "4.0.0"
+        },
         "node_modules/whatwg-url": {
             "dependencies": {
                 "tr46": "~0.0.3",
                 "webidl-conversions": "^3.0.0"
             },
             "dev": true,
             "integrity": "sha512-saE57nupxk6v3HY35+jzBwYa0rKSy0XR8JSxZPwgLr7ys0IBzhGviA1/TUGJLmSVqs8pb9AnvICXEuOHLprYTw==",
@@ -12223,15 +13002,14 @@
         "node_modules/which": {
             "bin": {
                 "node-which": "bin/node-which"
             },
             "dependencies": {
                 "isexe": "^2.0.0"
             },
-            "dev": true,
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==",
             "resolved": "https://registry.npmjs.org/which/-/which-2.0.2.tgz",
             "version": "2.0.2"
         },
@@ -12284,14 +13062,29 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-oV0jmFtUky6CXfkqehVvBP/LSWJ2sy4vWMioiENyJLePrBO/yKyV9OyJySfAKosh+RYkIl5zJCNZ8/4JncrpdA==",
             "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.15.tgz",
             "version": "1.1.15"
         },
+        "node_modules/why-is-node-running": {
+            "bin": {
+                "why-is-node-running": "cli.js"
+            },
+            "dependencies": {
+                "siginfo": "^2.0.0",
+                "stackback": "0.0.2"
+            },
+            "engines": {
+                "node": ">=8"
+            },
+            "integrity": "sha512-6tSwToZxTOcotxHeA+qGCq1mVzKR3CwcJGmVcY+QE8SHy6TnpFnh8PAvPNHYr7EcuVeG0QSMxtYCuO1ta/G/oA==",
+            "resolved": "https://registry.npmjs.org/why-is-node-running/-/why-is-node-running-2.2.2.tgz",
+            "version": "2.2.2"
+        },
         "node_modules/wordwrap": {
             "dev": true,
             "integrity": "sha512-gvVzJFlPycKc5dZN4yPkP8w7Dc37BtP1yczEneOb4uq34pXZcvrtRTmWV8W+Ume+XCxKgbjM+nevkyFPMybd4Q==",
             "resolved": "https://registry.npmjs.org/wordwrap/-/wordwrap-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/wrap-ansi": {
@@ -12406,15 +13199,15 @@
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "integrity": "sha512-HnLOCR3vjcY8beoNLtcjZ5/nxn2afmME6lhrDrebokqMap+XbeW8n9TXpPDOqdGK5qcI3oT0GKTW6wC7EMiVqA==",
             "resolved": "https://registry.npmjs.org/string-width/-/string-width-5.1.2.tgz",
             "version": "5.1.2"
         },
         "node_modules/wrappy": {
-            "dev": true,
+            "devOptional": true,
             "integrity": "sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==",
             "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/write-file-atomic": {
             "dependencies": {
                 "graceful-fs": "^4.1.11",
@@ -12423,15 +13216,15 @@
             },
             "dev": true,
             "integrity": "sha512-GaETH5wwsX+GcnzhPgKcKjJ6M2Cq3/iZp1WyY/X1CSqrW+jVNM9Y7D8EC2sM4ZG/V8wZlSniJnCKWPmBYAucRQ==",
             "resolved": "https://registry.npmjs.org/write-file-atomic/-/write-file-atomic-2.4.3.tgz",
             "version": "2.4.3"
         },
         "node_modules/ws": {
-            "dev": true,
+            "devOptional": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-HS0c//TP7Ina87TfiPUz1rQzMhHrl/SG2guqRcTOIUYD2q8uhUdNHZYJUaQ8aTGPzCh+c6oawMKW35nFl1dxyQ==",
             "peerDependencies": {
                 "bufferutil": "^4.0.1",
                 "utf-8-validate": ">=5.0.2"
@@ -12443,14 +13236,29 @@
                 "utf-8-validate": {
                     "optional": true
                 }
             },
             "resolved": "https://registry.npmjs.org/ws/-/ws-8.16.0.tgz",
             "version": "8.16.0"
         },
+        "node_modules/xml-name-validator": {
+            "devOptional": true,
+            "engines": {
+                "node": ">=18"
+            },
+            "integrity": "sha512-EvGK8EJ3DhaHfbRlETOWAS5pO9MZITeauHKJyb8wyajUfQUenkIg2MvLDTZ4T/TgIcm3HU0TFBgWWboAZ30UHg==",
+            "resolved": "https://registry.npmjs.org/xml-name-validator/-/xml-name-validator-5.0.0.tgz",
+            "version": "5.0.0"
+        },
+        "node_modules/xmlchars": {
+            "devOptional": true,
+            "integrity": "sha512-JZnDKK8B0RCDw84FNdDAIpZK+JuJw+s7Lz8nksI7SIuU3UXJJslUthsi+uWBUYOwPFwW7W7PRLRfUKpxjtjFCw==",
+            "resolved": "https://registry.npmjs.org/xmlchars/-/xmlchars-2.2.0.tgz",
+            "version": "2.2.0"
+        },
         "node_modules/xtend": {
             "dev": true,
             "engines": {
                 "node": ">=0.4"
             },
             "integrity": "sha512-LKYU1iAXJXUgAXn9URjiu+MWhyUXHsvfp7mcuYm9dSUKK0/CjtrUwFAxD82/mCWbtLsGjFIad0wIsod4zrTAEQ==",
             "resolved": "https://registry.npmjs.org/xtend/-/xtend-4.0.2.tgz",
```

### Comparing `relationalai-0.2.9/frontend/debugger/package.json` & `relationalai-0.3.0/frontend/debugger/package.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.850250626566416%*

 * *Differences: {"'dependencies'": "{'@solid-primitives/date': '^2.0.21', '@solid-primitives/timer': '^1.3.9', "*

 * *                   "'gradient-path': '^2.3.0', 'vitest': '^1.6.0'}",*

 * * "'devDependencies'": "{'jsdom': '^24.0.0'}",*

 * * "'engines'": "OrderedDict([('node', '22.1.0'), ('npm', '10.7.0')])",*

 * * "'scripts'": "{'test': 'vitest'}"}*

```diff
@@ -1,41 +1,51 @@
 {
     "dependencies": {
         "@kobalte/core": "^0.12.6",
+        "@solid-primitives/date": "^2.0.21",
+        "@solid-primitives/timer": "^1.3.9",
         "@tabler/icons": "^3.1.0",
+        "gradient-path": "^2.3.0",
         "prismjs": "^1.29.0",
-        "solid-js": "^1.8.11"
+        "solid-js": "^1.8.11",
+        "vitest": "^1.6.0"
     },
     "description": "",
     "devDependencies": {
         "@chromatic-com/storybook": "^1.2.25",
         "@storybook/addon-essentials": "^8.0.4",
         "@storybook/addon-interactions": "^8.0.4",
         "@storybook/addon-links": "^8.0.4",
         "@storybook/blocks": "^8.0.4",
         "@storybook/preview-api": "^8.0.4",
         "@storybook/testing-library": "^0.2.2",
         "@types/prismjs": "^1.26.3",
+        "jsdom": "^24.0.0",
         "solid-devtools": "^0.29.2",
         "storybook": "^8.0.4",
         "storybook-solidjs": "^1.0.0-beta.2",
         "storybook-solidjs-vite": "^1.0.0-beta.2",
         "stylus": "^0.63.0",
         "typescript": "^5.3.3",
         "vite": "^5.0.11",
         "vite-plugin-prismjs": "^0.0.11",
         "vite-plugin-solid": "^2.8.2",
         "vite-plugin-solid-svg": "^0.8.1"
     },
+    "engines": {
+        "node": "22.1.0",
+        "npm": "10.7.0"
+    },
     "license": "UNLICENSED",
     "name": "relationalai-debugger-ui",
     "scripts": {
         "build": "vite build",
         "build-storybook": "storybook build",
         "dev": "vite",
         "serve": "vite preview",
         "start": "vite",
-        "storybook": "storybook dev -p 6006"
+        "storybook": "storybook dev -p 6006",
+        "test": "vitest"
     },
     "type": "module",
     "version": "0.0.0"
 }
```

### Comparing `relationalai-0.2.9/frontend/debugger/tsconfig.json` & `relationalai-0.3.0/frontend/debugger/tsconfig.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980769230769231%*

 * *Differences: {"'compilerOptions'": "{'types': {insert: [(4, 'vitest/globals')]}}"}*

```diff
@@ -16,14 +16,15 @@
         },
         "strict": true,
         "target": "ESNext",
         "types": [
             "./src/types",
             "vite-plugin-solid-svg/types-component-solid",
             "vite/client",
-            "./node_modules/@types"
+            "./node_modules/@types",
+            "vitest/globals"
         ]
     },
     "include": [
         "src/**/*"
     ]
 }
```

### Comparing `relationalai-0.2.9/frontend/debugger/vite.config.ts` & `relationalai-0.3.0/frontend/debugger/vite.config.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import path from "path"
-import { defineConfig } from "vite";
+import { defineConfig } from 'vitest/config';
 import solid_plugin from "vite-plugin-solid";
 import solid_svg from "vite-plugin-solid-svg";
 import prism from "vite-plugin-prismjs";
 // import devtools from "solid-devtools/vite";
 
 export default defineConfig({
   plugins: [
@@ -17,14 +17,20 @@
     prism({
       languages: ["python", "json"],
       plugins: ["line-numbers", "line-highlight"], // "toolbar", "copy-to-clipboard"],
       theme: "okaidia", // "okaidia", // "default"
       css: true,
     })
   ],
+  test: { 
+    globals: true, 
+    testTransformMode: { 
+        web: ['tsx', 'ts'], 
+    }, 
+  },
   resolve: {
     alias: {
       "@src": path.resolve(__dirname, "./src"),
     }
   },
   css: {
     preprocessorOptions: {
```

### Comparing `relationalai-0.2.9/frontend/debugger/.storybook/main.ts` & `relationalai-0.3.0/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/App.tsx` & `relationalai-0.3.0/frontend/debugger/src/App.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,129 @@
-import { For, Match, Show, Switch, createEffect, createSignal } from "solid-js";
+import { Show, createEffect, createSignal, untrack } from "solid-js";
 import { EventListSelection, Selection } from "./Selection";
 import { EventList } from "./components/EventList";
-import { EventViewer } from "./components/EventViewer";
-import { Sidebar } from "./components/Sidebar";
 import { Button } from "./components/ui/Button";
 import { Field, Format } from "./components/ui/Field";
 import { Icon } from "./components/ui/Icon";
 import { Modal } from "./components/ui/Modal";
 import { Tooltip } from "./components/ui/Tooltip";
 import { FileDropZone } from "./components/FileDropZone";
-import { Message, Span, client, get_in, type Subject } from "./debugger_client";
+import { client, get_in, is_placeholder, type Subject } from "./debugger_client";
 import "./App.styl";
-import { Breadcrumbs } from "./components/ui/Breadcrumbs";
+import { SystemStatus } from "./components/SystemStatus";
+import Logo from "./logo.svg";
+import { begin_auto_scroll, set_auto_scroll_enabled, auto_scroll_enabled } from "./utils/solid";
 
 function App() {
     const event_list_selection = new Selection<Subject>("EventList");
 
     const clear = () => {
-        client.connection.disconnect();
         event_list_selection.clear()
         client.clear();
     };
 
     const exportData = () => {
         client.exportData();
 	};
 
     const handleFileDrop = (jsonObjects: any[]) => {
         clear();
         client.importData(jsonObjects[0]);
     }
 
+    const program_running = () => client.latest() && !client.latest()?.end_time;
+
     const [pinned, set_pinned] = createSignal<boolean>(true);
 
-    createEffect((prev_len: number|undefined) => {
-        const cur_len = client.spans().length;
-        const cur = event_list_selection.primary();
-        if (pinned() && cur_len !== prev_len && cur) {
-            event_list_selection.select({ event: "placeholder", selection_path: [cur_len - 1, ...cur.selection_path.slice(1)] })
+    // If we're pinned when a new program starts:
+    // replace the current selections with placeholders for their equivalents in the new program
+    createEffect((prev_run_count: number|undefined) => {
+        const cur_run_count = client.spans().length;
+        if (!pinned() || cur_run_count === prev_run_count) return cur_run_count;
+
+        for (let selected of untrack(() => event_list_selection.selected())) {
+            if (is_placeholder(selected)) continue;
+            event_list_selection.remove(selected);
+            event_list_selection.add({ event: "placeholder", selection_path: [cur_run_count - 1, ...selected.selection_path.slice(1)] })
         }
-        return cur_len;
+        return cur_run_count;
     });
 
-    createEffect(() => {
-        let selected = event_list_selection.primary();
-        if (selected?.event === "placeholder") {
+    // When a new message comes in:
+    // Replace any selected placeholders with the actual event if possible
+    createEffect((prev_message_count: number|undefined) => {
+        const cur_message_count = client.messages().length;
+        if(cur_message_count === prev_message_count) return cur_message_count;
+
+        for (let selected of untrack(() => event_list_selection.selected())) {
+            if (!is_placeholder(selected)) continue;
+
             let available = get_in(client.root, selected.selection_path);
             if(available) {
-                event_list_selection.select(available);
+                event_list_selection.remove(selected);
+                event_list_selection.add(available);
             }
         }
+
+        return cur_message_count
+    });
+
+    // If auto scroll is enabled when a new message comes in:
+    // Attempt to scroll to the bottom to keep it in view
+    createEffect((prev_message_count: number | undefined) => {
+        const cur_message_count = client.messages().length;
+        if (cur_message_count === prev_message_count) return cur_message_count;
+
+        if (auto_scroll_enabled()) {
+            begin_auto_scroll()
+        }
+        return cur_message_count
+    })
+
+    // If we open/close a group while auto scroll is enabled:
+    // disable auto scrolling until the user re-docks to bottom
+    createEffect(() => {
+        event_list_selection.selected();
+        set_auto_scroll_enabled(false);
     });
 
     return (
         <EventListSelection.Provider value={event_list_selection}>
-            <app-chrome>
-                <FileDropZone onFileDrop={handleFileDrop}>
-                    <Sidebar side="left" defaultOpen class="app-sidebar">
-                        <header>
-                            <Button class="icon" onclick={clear} tooltip="clear events">
+            <FileDropZone onFileDrop={handleFileDrop}>
+                <div class="app">
+                    <header>
+                        <Logo />
+                        <span style="flex: 1" />
+                        <div class="hidden-controls">
+                            <Button class="icon" onclick={clear} tooltip={program_running() ? "cannot clear events while program is running" : "clear events"} disabled={program_running()}>
                                 <Icon name="ban" />
                             </Button>
                             <Button class="icon" tooltip="Follow last run" onclick={() => set_pinned(v => !v)}>
                                 <Icon name="pin" type={pinned() ? "filled" : "outline"} />
                             </Button>
-                            <span style="flex: 1" />
+
 
                             <Button class="icon" tooltip="Export events" onclick={exportData}>
                                 <Icon name="download" />
                             </Button>
 
                             <Modal title="Settings" content={<Settings />}>
                                 <Modal.Trigger as={Button} class="icon" tooltip="settings">
                                     <Icon name="settings" />
                                 </Modal.Trigger>
                             </Modal>
-                        </header>
-                        <EventList events={client.spans()} />
-                    </Sidebar>
-                </FileDropZone >
-                <main>
-                    <Show when={event_list_selection.primary()}>
-                        <EventBreadcrumbs subject={event_list_selection.primary()!} select={event_list_selection.select} />
-                        <scroll-container>
-                            <scroll-inner>
-                                <EventViewer subject={event_list_selection.primary()!} />
-                            </scroll-inner>
-                        </scroll-container>
-                    </Show>
-                </main>
-                <Status />
-            </app-chrome>
+                        </div>
+
+                        <Status />
+                    </header>
+                    <SystemStatus />
+                    <EventList events={client.spans()} />
+
+                </div>
+            </FileDropZone>
         </EventListSelection.Provider>
     );
 };
 
 export default App;
 
 function Status() {
@@ -125,49 +154,7 @@
                     }} />
             </section>
 
         </>
     )
 }
 
-interface EventBreadcrumbsProps {
-    subject: Subject,
-    select?: (subject: Subject) => any,
-}
-function EventBreadcrumbs(props: EventBreadcrumbsProps) {
-    const crumbs = () => {
-        let cur: Subject|undefined = props.subject;
-        let crumbs = [];
-        while(cur) {
-            const item = cur;
-            if(Span.is_span(item) && item.span_type === "root") {
-                break;
-            }
-            crumbs.unshift(
-                <Breadcrumbs.Item onClick={() => props.select?.(item!)}>
-                    <Switch>
-                        <Match when={Span.is_span(item) && item.span_type === "program"}>
-                            run {(item as Span.Program).run}
-                        </Match>
-                        <Match when={Span.is_span(item)}>
-                            {(item as Span).span_type}
-                        </Match>
-                        <Match when={Message.is_time(item)}>
-                            {(item as Message.Time).type} result
-                        </Match>
-                        <Match when={true}>
-                            {(item as Message.Time).event}
-                        </Match>
-                    </Switch>
-                </Breadcrumbs.Item>
-            );
-            cur = cur.parent;
-        }
-        return crumbs;
-    }
-
-    return (
-        <Breadcrumbs>
-            {crumbs()}
-        </Breadcrumbs>
-    )
-}
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/Selection.tsx` & `relationalai-0.3.0/frontend/debugger/src/Selection.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,19 @@
             if(this.eq(cur[ix], v)) {
                 this.set_selected(cur.toSpliced(ix, 1));
                 break;
             }
         }
         return this;
     }
+
+    toggle = (v: T, on = !this.is_selected(v)) => {
+        if(on) return this.add(v)
+        return this.remove(v)
+    }
 }
 
 export function createSelectionContext<T>(name: string, eq?: (a: T, b: T) => boolean) {
     return createContext(new Selection<T>(name, eq));
 }
 
 //------------------------------------------------------------------------------
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/debugger_client.ts` & `relationalai-0.3.0/frontend/debugger/src/debugger_client.ts`

 * *Files 20% similar despite different names*

```diff
@@ -18,28 +18,34 @@
 export interface Placeholder {
     "event": "placeholder",
     selection_path: number[],
     span_type?: undefined,
     events?: undefined
     parent?: undefined
 }
+export function is_placeholder(msg: any): msg is Placeholder {
+    return typeof msg === "object" && msg.event === "placeholder";
+}
 
 export type Subject = Message.Event|Span|Placeholder;
 
 //------------------------------------------------------------------------------
 // Messages
 //------------------------------------------------------------------------------
 
 export namespace Message {
     export interface Base {
         event: string,
         selection_path: number[],
+        timestamp: string,
+        time: Date,
         span_type?: undefined,
         events?: undefined,
-        parent?: Span;
+        parent_id?: string,
+        parent?: Span
         [key: string]: unknown
     }
     
     export interface SpanStart extends Base {
         event: "span_start";
         span: {
             type: string;
@@ -59,40 +65,52 @@
     export interface Time extends Base {
         event: "time",
         type: string,
         elapsed: number,
         results?: ResultData
         code?: string
     }
-    export function is_time(span: any): span is Message.Time {
-        return span?.event === "time";
+    export function is_time(msg: any): msg is Message.Time {
+        return msg?.event === "time";
     }
 
     export interface Error extends Base {
         event: "error",
         err: any
     }
-    export function is_error(span: any): span is Message.Error {
-        return span?.event === "error";
+    export function is_error(msg: any): msg is Message.Error {
+        return msg?.event === "error";
     }
 
     export interface Compilation extends Base {
         event: "compilation",
         source: Source,
         passes: Pass[],
         emitted: string,
         emit_time: number,
         mech?: Mech.Machine,
         task?: string
     }
-    export function is_compilation(span: any): span is Message.Compilation {
-        return span?.event === "compilation";
+    export function is_compilation(msg: any): msg is Message.Compilation {
+        return msg?.event === "compilation";
+    }
+
+    export interface TransactionCreated extends Base {
+        event: "transaction_created",
+        txn_id: string
+    }
+    export function is_transaction_created(msg: any): msg is Message.TransactionCreated {
+        return msg?.event === "transaction_created";
     }
 
-    export type Event = Time | Error | Compilation;
+    export type Event = Time | Error | Compilation | TransactionCreated;
+
+    export function is_event(msg: any): msg is Message.Event {
+        return "event" in msg && !("span_type" in msg) && "time" in msg;
+    }
 
     export interface Pass {
         name: string,
         task: string,
         elapsed: number
     }
 
@@ -102,19 +120,45 @@
         block: string,
     }
 
     export interface ResultData {
         values: Record<string, any>[],
         count: number
     }
+
+    export interface RPCResponse {
+        event: "rpc_response"
+        rpc_id: number
+    }
+
+    export interface ListTransactions extends RPCResponse {
+        transactions: TransactionInfo[]
+    }
+
+    export interface TransactionInfo {
+        id: string,
+        state: string,
+        created_by: string,
+        created_on: number,
+        finished_at: number,
+
+        account?: string,
+        agent?: string,
+        database?: string,
+        engine?: string,
+        query?: string,
+        read_only?: boolean,
+        tags?: string[]
+    }
 }
 export type Message =
     | Message.SpanStart
     | Message.SpanEnd
     | Message.Event
+    | Message.RPCResponse
 
 //------------------------------------------------------------------------------
 // Spans
 //------------------------------------------------------------------------------
 
 export namespace Span {
     export interface Base {
@@ -135,21 +179,29 @@
     export function is_span(span: any): span is Span {
         return span?.event === "span" && Array.isArray(span.events);
     }
 
     export interface Program extends Base {
         span_type: "program",
         main: string,
-        run: number,
+        platform?: string,
     }
 
     export function is_program(span: any): span is Program {
         return is_span(span) && span.span_type === "program";
     }
 
+    export interface RuleBatch extends Base {
+        span_type: "rule_batch",
+    }
+
+    export function is_rule_batch(span: any): span is RuleBatch {
+        return is_span(span) && span.span_type === "rule_batch";
+    }
+
     export interface Block extends Base {
         span_type: "rule"|"query",
         task: string,
         mech: Mech.Machine
     }
 
     export function is_block(span: any): span is Block {
@@ -184,27 +236,26 @@
 //------------------------------------------------------------------------------
 
 export class DebuggerClient {
     connection: Connection;
     messages: Accessor<Message[]>;
     protected set_messages: Setter<Message[]>;
 
-
-    run_counter = 0;
     root: Span;
     protected set_root: SetStoreFunction<Span>;
 
     spans() {
         return this.root.events;
     }
 
     connected: Accessor<boolean>;
     protected set_connected: Setter<boolean>;
 
     protected path: number[] = [];
+    protected open_spans: Span[] = [];
 
     latest: Accessor<Span.Program|undefined>;
 
     constructor(ws_url: string) {
         this.connection = new Connection(ws_url);
         [this.messages, this.set_messages] = createSignal<Message[]>([], {equals: () => false});
         [this.root, this.set_root] = createStore<Span>({
@@ -221,18 +272,19 @@
 
         this.connection.onreceive = this.handle_message;
         this.connection.onconnect = this.set_connected;
     }
 
     clear() {
         batch(() => {
-            this.path = [];
+            this.open_spans = [];
             this.set_messages([]);
-            this.set_root({event: "span", span_type: "root", span: [], start_time: new Date(0), events: []});
+            this.set_root({event: "span", span_type: "root", span: [], start_time: new Date(0), events: [], selection_path: []});
         });
+        return this.send.clear();
     }
 
     exportData = () => {
         const data = JSON.stringify(unwrap(this.root));
         const blob = new Blob([data], {type: "application/json"});
 
 
@@ -247,75 +299,117 @@
     }
 
     importData = (data: Span) => {
         this.set_root(data);
     }
 
     send = {
-        ping: () => this._send({type: "ping"})
+        clear: () => this._send({type: "clear"}),
+        list_transactions: (limit = 20, only_active = false) => this._send<Message.ListTransactions>({type: "list_transactions", limit, only_active})
     }
+    rpc_callbacks = new Map<number, (v: any) => any>()
 
-    protected _send(msg: any) {
+    _next_rpc_id = 1;
+    protected _send<T = any>(msg: any): Promise<T> {
+        const rpc_id = msg.rpc_id = this._next_rpc_id++;
         this.connection.send(JSON.stringify(msg));
+
+        return new Promise<T>((resolve, reject) => {
+            this.rpc_callbacks.set(rpc_id, (response) => {
+                if(response.status === "error") reject(response);
+                else resolve(response);
+                this.rpc_callbacks.delete(rpc_id)
+            })
+        });
+    }
+
+    protected get_open_span(id: string|null|undefined, within: Span, pop = false) {
+        if(!id) return within;
+        for(let ix = this.open_spans.length - 1; ix >= 0; ix -= 1) {
+            let span = this.open_spans[ix];
+            if(span.id === id) {
+                if(pop) this.open_spans.splice(ix, 1);
+                return get_in(within, span.selection_path);
+            }
+        }
     }
 
     protected handle_span_start(msg: Message.SpanStart) {
         this.set_root(produce((root) => {
-            let parent = get_in(root, this.path);
-            if(!parent || !Span.is_span(parent)) throw new Error(`Parent not found at path ${this.path}`);
-            this.path.push(parent.events.length);
-            let span_type = msg.span.type;
+            const parent = this.get_open_span(msg.span.parent_id, root);
+            if(!parent || !Span.is_span(parent)) {
+                throw new Error(`Parent '${msg.span.parent_id}' not found for span '${msg.span.id}'`);
+            }
             let sub: Span = {
                 ...msg.span.attrs,
+                id: msg.span.id,
                 start_time: new Date(msg.span.start_timestamp),
                 end_time: undefined,
-                span_type,
+                span_type: msg.span.type,
                 event: "span",
-                selection_path: this.path.slice(),
-                run: span_type === "program" ? ++this.run_counter : undefined,
+                selection_path: [...parent.selection_path, parent.events.length],
                 events: []
             };
+            this.open_spans.push(sub);
             Object.defineProperty(sub, "parent", {value: unwrap(parent), enumerable: false, configurable: true, writable: true});
             parent.events.push(sub)
         }));
     }
 
     protected handle_span_end(msg: Message.SpanEnd) {
         this.set_root(produce((root) => {
-            let start = get_in(root, this.path);
-            if(!start || !Span.is_span(start)) throw new Error(`Start not found at path ${this.path}`);
+            let start = this.get_open_span(msg.id, root, true);
+            if(!start || !Span.is_span(start)) throw new Error(`Open span not found for close '${msg.id}'`);
             start.end_time = new Date(msg.end_timestamp);
-            start.elapsed = (start.end_time.getTime() - start.start_time.getTime()) / 1000;
+            start.elapsed = (start.end_time.getTime() - start.start_time.getTime());
             
             for (let key in msg.end_attrs) {
                 if (key === "span" || key === "event") continue;
                 start[key] = msg[key];
             }
-            this.path.pop();
         }));
     }
 
     protected handle_event(msg: Message.Event) {
         this.set_root(produce((root) => {
-            let span = get_in(root, this.path);
+            const span = this.get_open_span(msg.parent_id, root);
+            if(!span || !Span.is_span(span)) {
+                throw new Error(`Parent '${msg.parent_id}' not found for event '${msg.event}'`);
+            }
             if(!span || !Span.is_span(span)) throw new Error(`Span not found at path ${this.path}`);
-            msg.selection_path = [...this.path, span.events.length],
+            msg.time = new Date(msg.timestamp);
+            msg.selection_path = [...this.path, span.events.length];
             Object.defineProperty(msg, "parent", {value: unwrap(span), enumerable: false, configurable: true, writable: true});
             span.events.push(msg);
         }));
     }
 
-    protected handle_message = (msg: Message) => {
+    protected handle_rpc_response(msg: Message.RPCResponse) {
+        const callback = this.rpc_callbacks.get(msg.rpc_id);
+        if(!callback) throw new Error(`Got RPC response for unsent RPC: ${msg.rpc_id}`);
+        callback(msg);
+    }
+
+    protected handle_single_message = (msg: Message) => {
+        if(msg.event === "span_start") this.handle_span_start(msg)
+        else if(msg.event === "span_end") this.handle_span_end(msg)
+        else if(msg.event === "rpc_response") this.handle_rpc_response(msg)
+        else this.handle_event(msg);
+    }
+
+    protected handle_message = (msgs: Message[]) => {
         batch(() => {
-            if(msg.event === "span_start") this.handle_span_start(msg)
-            else if(msg.event === "span_end") this.handle_span_end(msg)
-            else this.handle_event(msg);
+            for(let msg of msgs) {
+                this.handle_single_message(msg)
+            }
 
             this.set_messages((prev) => {
-                prev.push(msg);
+                for(let msg of msgs) {
+                    prev.push(msg);
+                }
                 return prev;
             });
         });
     }
 }
 
 //------------------------------------------------------------------------------
@@ -327,28 +421,33 @@
     private shouldReconnect = true;
     private active = false;
 
     ws_url: string;
     reconnectInterval: number;
     onreceive?: (msg: any) => void;
     onconnect?: (is_connected: boolean) => void;
+    buffered_sends: any[] = [];
 
     constructor(ws_url: string, reconnectInterval: number = 1_000) {
         this.ws_url = ws_url;
         this.reconnectInterval = reconnectInterval;
         this.connect();
     }
 
     private connect(): void {
         // @NOTE: I wasted an hour trying to figure out how to suppress the default error message and then gave up.
         this.socket = create_ws(this.ws_url);
 
         this.socket.addEventListener("open", () => {
             this.active = true;
             this.onconnect?.(true);
+            for(let msg of this.buffered_sends) {
+                this.send(msg);
+            }
+            this.buffered_sends = [];
         });
 
         this.socket.addEventListener("message", (event) => {
             let msg;
             try {
                 msg = JSON.parse(event.data);
             } catch (err: any) {
@@ -378,14 +477,16 @@
             }
         });
     }
 
     public send(msg: string|ArrayBufferLike|Blob|ArrayBufferView) {
         if(this.active) {
             this.socket?.send(msg);
+        } else {
+            this.buffered_sends.push(msg);
         }
     }
 
     public disconnect() {
         if (this.socket) {
             this.socket.close();
         }
@@ -394,7 +495,9 @@
     public close(): void {
         this.shouldReconnect = false;
         this.disconnect();
     }
 }
 
 export const client = new DebuggerClient(`ws://${location.host}/ws/client`);
+
+(globalThis as any).client = client;
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/index.tsx` & `relationalai-0.3.0/frontend/debugger/src/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/util.styl` & `relationalai-0.3.0/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/util.ts` & `relationalai-0.3.0/frontend/debugger/src/util.ts`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import type { Component, JSX } from "solid-js";
+
 export function ends_in<T>(list: T[], one_of: T[]) {
     if(list.length === 0) return false;
 
     let last = list[list.length - 1];
     for(let v of one_of) {
         if(v === last) return true;
     }
@@ -54,20 +56,15 @@
         return;
     } catch {
         await fallback_copy_text_to_clipboard(text);
     }
 }
 
 
-const time_formatter_ms = new Intl.NumberFormat("en", {style: "unit", unit: "millisecond", unitDisplay: "short", maximumFractionDigits: 1});
-const time_formatter_s = new Intl.NumberFormat("en", {style: "unit", unit: "second", unitDisplay: "short", maximumFractionDigits: 2});
 
-export const fmt = {
-    time: {
-        ms(v: number) {
-            return time_formatter_ms.format(v);
-        },
-        s(v: number) {
-            return time_formatter_s.format(v);
-        }
-    }
-}
+export type PolymorphProps<T> =
+    T extends Component<infer U> ?
+        U : (T extends keyof JSX.HTMLElementTags ?
+             JSX.HTMLElementTags[T] :
+             JSX.HTMLAttributes<HTMLElement>);
+
+export type Polymorphic<T, P, P2 = {}> = PolymorphProps<T>&P&P2
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/assets/favicon.png` & `relationalai-0.3.0/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.styl` & `relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.styl`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 base-color = #121212;
 text-color = #f0f0f0;
 lighten-amount = 10%;
 
 .drop-zone {
   position: relative;
-  padding: 8px;
-  border: 2px dashed currentcolor;
   border-radius: 8px;
   transition: background-color 0.3s;
 
   &.dragging, &.draggingOver {
     background-color: lighten(base-color, lighten-amount);
+    outline: 2px dashed currentcolor;
   }
 }
 
 .overlay {
   position: absolute;
   top: 0;
   right: 0;
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/FileDropZone.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.3.0/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Breadcrumbs.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Button.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import {Button as KButton} from "@kobalte/core";
-import { JSXElement, Match, Switch, splitProps } from "solid-js";
+import { type JSXElement, Match, Switch, splitProps } from "solid-js";
 import {Tooltip} from "./Tooltip";
 import "./Button.styl";
+import { Polymorphic } from "@src/util";
 
-export interface ButtonProps extends KButton.ButtonRootProps {
+export type ButtonProps<T> = Polymorphic<T, KButton.ButtonRootProps, {
+    as?: T
+    class?: string
     tooltip?: JSXElement
-}
-export function Button(props: ButtonProps) {
+}>
+export function Button<const T = "button">(props: ButtonProps<T>) {
     const [local, remote] = splitProps(props, ["class", "tooltip"]);
     return (
         <Switch>
             <Match when={local.tooltip}>
                 <Tooltip content={local.tooltip}>
                     <Tooltip.Trigger as={KButton.Root} class={`ui-button ${local.class || ""}`} {...remote} />
                 </Tooltip>
             </Match>
             <Match when={true}>
-                <KButton.Root class={`ui-button ${local.class || ""}`} {...remote} />
+                <KButton.Root class={`ui-button ${local.class || ""}`} {...remote as KButton.ButtonRootProps} />
             </Match>
         </Switch>
     )
 }
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Code.styl`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 :root {
-  --code-block-bg: var(--section-bg);
-  --code-block-border: var(--section-border);
-  --code-block-shadow: var(--shadow);
+  --code-block-bg: var(--card-bg);
+  --code-block-border: var(--card-border);
+  --code-block-shadow: var(--card-shadow);
 }
 
 code.ui-code {
   box-sizing: border-box;
   font-family: "Fira Code", mono;
   border-radius: 4px;
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Code.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import { Collapsible as KCollapsible } from "@kobalte/core";
 import { JSXElement, splitProps } from "solid-js";
 import { Icon } from "./Icon";
 import "./Collapsible.styl";
 import { Button } from "./Button";
+import { Polymorphic } from "@src/util";
 
-export function CollapsibleTrigger(props: KCollapsible.CollapsibleTriggerProps) {
+export type CollapsibleTriggerProps<T> = Polymorphic<T, KCollapsible.CollapsibleTriggerProps, { as?: T }>
+export function CollapsibleTrigger<const T = typeof Button>(props: CollapsibleTriggerProps<T>) {
     let [local, remote] = splitProps(props, ["class", "children"]);
     return (
         <KCollapsible.Trigger as={Button} class={`ui-collapsible-trigger ${local.class ?? ""}`} {...remote}>
             {local.children}
         </KCollapsible.Trigger>
     )
 }
@@ -18,28 +20,29 @@
         <Icon name="chevron-down" class="ui-collapsible-trigger-icon" />
     )
 }
 
 export function CollapsibleContent(props: KCollapsible.CollapsibleContentProps) {
     let [local, remote] = splitProps(props, ["class", "children"]);
     return (
-        <KCollapsible.Content class={`ui-collapsible-content ${local.class ?? ""}`} {...remote}>
+        <div class={`ui-collapsible-content ${local.class ?? ""}`} {...remote}>
             <div class="ui-collapsible-inner">
                 {local.children}
             </div>
-        </KCollapsible.Content>
+        </div>
     )
 }
 
-export interface CollapsibleProps extends KCollapsible.CollapsibleRootProps {
+export type CollapsibleProps<T> = Polymorphic<T, KCollapsible.CollapsibleRootProps, {
+    as?: T
     class?: string,
     side: "right" | "left" | "bottom" | "top"
     children: JSXElement
-}
-export function Collapsible(props: CollapsibleProps) {
+}>
+export function Collapsible<const T = "div">(props: CollapsibleProps<T>) {
     let [local, remote] = splitProps(props, ["class", "side", "children"]);
     return (
         <KCollapsible.Root {...remote} class={`ui-collapsible ${local.side} ${local.class ?? ""}`}>
             {local.children}
         </KCollapsible.Root>
     )
 }
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Field.styl`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 @require "util.styl";
 
 :root {
   --field-border: var(--input-border);
   --field-bg: var(--input-bg, transparent);
-  --field-outline: var(--outline, #999);
+  --field-outline: var(--input-outline, #999);
   --field-control-bg: transparent;
 }
 
 .ui-field {
   .ui-field-input {
     position: relative;
     display: flex;
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.styl`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 :root {
-  --modal-bg: var(--section-bg);
-  --modal-border: var(--section-border);
-  --modal-shadow: var(--shadow);
-  --modal-overlay-bg: var(--shadow);
+  --modal-bg: var(--card-bg);
+  --modal-border: var(--card-border);
+  --modal-shadow: var(--card-shadow);
+  --modal-overlay-bg: var(--card-shadow);
 
   --modal-anim-open-duration: var(--anim-duration-normal);
   --modal-anim-close-duration: var(--anim-duration-slow);
 }
 
 .ui-modal {
   display: flex;
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import { Dialog as KDialog } from "@kobalte/core";
 import { JSXElement, splitProps } from "solid-js";
 import { Button } from "./Button";
 import "./Modal.styl";
 import { Icon } from "./Icon";
+import { Polymorphic } from "@src/util";
 
 export interface ModalProps extends KDialog.DialogRootProps {
     title?: string,
     class?: string,
     content?: JSXElement,
 }
 export function Modal(props: ModalProps) {
@@ -27,11 +28,13 @@
                         {local.content}
                     </KDialog.Content>
                 </div>
             </KDialog.Portal>
         </KDialog.Root>
     )
 }
-Modal.Trigger = KDialog.Trigger;
+
+export type ModalTriggerProps<T> = Polymorphic<T, KDialog.DialogTriggerProps, { as?: T }>
+Modal.Trigger = <const T = "button">(props: ModalTriggerProps<T>) => KDialog.Trigger(props);
 Modal.Title = KDialog.Title;
 Modal.CloseButton = KDialog.CloseButton;
 Modal.Description = KDialog.Description;
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 :root {
-  --tooltip-bg: var(--section-bg);
-  --tooltip-border: var(--section-border);
-  --tooltip-shadow: var(--shadow);
+  --tooltip-bg: var(--card-bg);
+  --tooltip-border: var(--card-border);
+  --tooltip-shadow: var(--card-shadow);
   --tooltip-anim-open-duration: var(--anim-duration-quick);
   --tooltip-anim-close-duration: var(--anim-duration-normal);
 }
 
 .ui-tooltip {
   z-index: 50;
```

### Comparing `relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.3.0/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.3.0/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.3.0/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.3.0/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.3.0/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.3.0/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/fixtures/union.json` & `relationalai-0.3.0/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.3.0/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/README.md` & `relationalai-0.3.0/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/emit.py` & `relationalai-0.3.0/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/fixtures.py` & `relationalai-0.3.0/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/patch.py` & `relationalai-0.3.0/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/util.py` & `relationalai-0.3.0/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/cli/__main__.py` & `relationalai-0.3.0/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/cli/collect_failures.py` & `relationalai-0.3.0/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/cli/collect_tests.py` & `relationalai-0.3.0/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/cli/repro.py` & `relationalai-0.3.0/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/cli/watch.py` & `relationalai-0.3.0/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/action.py` & `relationalai-0.3.0/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/context.py` & `relationalai-0.3.0/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/document.py` & `relationalai-0.3.0/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/group_limited.py` & `relationalai-0.3.0/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/ir.py` & `relationalai-0.3.0/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/scope.py` & `relationalai-0.3.0/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/task.py` & `relationalai-0.3.0/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/gen/test.py` & `relationalai-0.3.0/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/harness/database.py` & `relationalai-0.3.0/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/validate/diff.py` & `relationalai-0.3.0/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/validate/errors.py` & `relationalai-0.3.0/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/validate/mapping.py` & `relationalai-0.3.0/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/gentest/validate/roundtrip.py` & `relationalai-0.3.0/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/__init__.py` & `relationalai-0.3.0/src/relationalai/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,93 @@
-from typing import cast
 from .clients import config as cfg
 from . import clients
 from . import dsl
 from . import debugging
 from . import metamodel
 from . import rel
 from .loaders import csv
 from . import analysis
 from . import tools
+from . import dependencies
 import importlib.metadata
 from snowflake.connector import SnowflakeConnection
 
 # Set up global exception handler for debugging
 debugging.setup_exception_handler()
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 
 def Model(
     name: str,
     *,
     profile: str | None = None,
     config: cfg.Config | None = None,
     dry_run: bool = False,
-    debug=None,
+    debug: bool | None = None,
     connection: SnowflakeConnection | None = None,
+    keep_model: bool = None,
+    isolated: bool = None,
+    nowait_durable: bool = None,
+    format: str = "default",
 ):
     config = config or cfg.Config(profile=profile)
     if debug is None:
         debug = config.get("debug", False)
     if debug:
         from relationalai.tools.debugger_client import start_debugger_session
-        start_debugger_session() # @TODO: add config / env vars / kwargs for debug_host and debug_port
+        start_debugger_session(config) # @TODO: add config / env vars / kwargs for debug_host and debug_port
     if not config.file_path:
         if cfg.legacy_config_exists():
             message = (
                 "Use `rai init` to migrate your configuration file "
                 "to the new format (raiconfig.toml)"
             )
         else:
             message = "No configuration file found. Please run `rai init` to create one."
         raise Exception(message)
     if config.get("platform") is None:
         config.set("platform", "snowflake")
     platform = config.get("platform")
     if platform != "snowflake" and connection is not None:
         raise ValueError("The `connection` parameter is only supported with the Snowflake platform")
-    dry_run = cast(bool, dry_run or config.get("compiler.dry_run", False))
+    if dry_run is None:
+        dry_run = config.get("compiler.dry_run", False)
+    if keep_model is None:
+        keep_model = config.get("model.keep", False)
+    if isolated is None:
+        isolated = config.get("model.isolated", True)
+    if nowait_durable is None:
+        nowait_durable = config.get("model.nowait_durable", True)
+
     if platform == "azure":
-        return clients.azure.Graph(
-            name, profile=profile, config=config, dry_run=dry_run
+        model = clients.azure.Graph(
+            name,
+            profile=profile,
+            config=config,
+            dry_run=dry_run,
+            isolated=isolated,
+            keep_model=keep_model,
+            format=format,
         )
     elif platform == "snowflake":
-        return clients.snowflake.Graph(
-            name, profile=profile, config=config, dry_run=dry_run, connection=connection
+        model = clients.snowflake.Graph(
+            name,
+            profile=profile,
+            config=config,
+            dry_run=dry_run,
+            isolated=isolated,
+            connection=connection,
+            keep_model=keep_model,
+            nowait_durable=nowait_durable,
+            format=format,
         )
     else:
         raise Exception(f"Unknown platform: {platform}")
+    model._client.exec_control(dependencies.generate_query(), lambda res: dependencies.check_dependencies(res, platform))
+    return model
 
 def Resources(profile:str|None=None, config:cfg.Config|None=None):
     config = config or cfg.Config(profile)
     platform = config.get("platform", "snowflake")
     if platform == "azure":
         return clients.azure.Resources(config=config)
     elif platform == "snowflake":
```

### Comparing `relationalai-0.2.9/src/relationalai/compiler.py` & `relationalai-0.3.0/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/debugging.py` & `relationalai-0.3.0/src/relationalai/debugging.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,33 +34,35 @@
         original_excepthook(exc_type, exc_value, exc_traceback)
 
 original_excepthook = None
 
 def setup_exception_handler():
     global original_excepthook
     original_excepthook = sys.excepthook
-    sys.excepthook = global_exception_handler 
+    sys.excepthook = global_exception_handler
 
 #--------------------------------------------------
 # Log Formatters
 #--------------------------------------------------
 
-def my_encoder(obj):
+def encode_log_message(obj):
     if isinstance(obj, DataFrame):
         return obj.head(20).to_dict(orient="records")
+    if isinstance(obj, datetime.datetime):
+        return obj.isoformat() + "Z"
     if hasattr(obj, "to_dict"):
         return obj.to_dict()
     if hasattr(obj, "to_json"):
         return obj.to_json()
     else:
         return str(obj)
 
 class JsonFormatter(logging.Formatter):
     def format(self, record):
-        return json.dumps(record.msg, default=my_encoder)
+        return json.dumps(record.msg, default=encode_log_message)
 
 #--------------------------------------------------
 # Logging
 #--------------------------------------------------
 
 logger = logging.getLogger("pyrellogger")
 logger.setLevel(logging.DEBUG)
@@ -100,46 +102,45 @@
 #     logger.addHandler(TestHandler())
 
 #--------------------------------------------------
 # Debug Spans
 #--------------------------------------------------
 
 # The deepest span in the tree
-TIP_SPAN = None
-
-def span_start(type: str, **kwargs):
-    if not DEBUG:
-        return
+TIP_SPAN: 'Span | None' = None
 
+def span_start(type: str, **kwargs) -> 'Span':
     global TIP_SPAN
-
     span = Span(type, TIP_SPAN, kwargs)
     TIP_SPAN = span
 
-    logger.debug({
-        "event": "span_start",
-        "span": span,
-    })
+    if DEBUG:
+        logger.debug({"event": "span_start", "span": span})
+
     return span
 
 def span_end(span):
     if not DEBUG:
         return
 
     global TIP_SPAN
     TIP_SPAN = span.parent
     span.mark_finished()
 
     logger.debug({
         "event": "span_end",
         "id": str(span.id),
-        "end_timestamp": span.end_timestamp,
+        "end_timestamp": span.end_timestamp.isoformat() + "Z",
         "end_attrs": span.end_attrs,
     })
 
+def span_flush():
+    while TIP_SPAN:
+        span_end(TIP_SPAN)
+
 class Span:
     def __init__(self, type: str, parent, attrs: Dict):
         self.id = uuid.uuid4()
         self.parent = parent
         self.type = type
         self.attrs = attrs
         # additional attributes added during the lifetime of the span
@@ -155,21 +156,21 @@
         self.end_attrs[key] = value
 
     def to_json(self):
         return {
             "type": self.type,
             "id": str(self.id),
             "parent_id": str(self.parent.id) if self.parent else None,
-            "start_timestamp": self.start_timestamp.isoformat(),
-            "end_timestamp": None if self.end_timestamp is None else self.end_timestamp.isoformat(),
+            "start_timestamp": self.start_timestamp.isoformat() + "Z",
+            "end_timestamp": None if self.end_timestamp is None else (self.end_timestamp.isoformat() + "Z"),
             "attrs": self.attrs,
         }
 
 @contextlib.contextmanager
-def span(type: str, **kwargs):
+def span(type: str, **kwargs) -> Span:
     cur = span_start(type, **kwargs)
     try:
         yield cur
     except Exception as err:
         error(err)
         raise
     finally:
@@ -181,19 +182,27 @@
 
 #--------------------------------------------------
 # Debug Events
 #--------------------------------------------------
 
 EMPTY = {}
 
-def event(event:str, **kwargs):
+def event(event:str, parent:Span|None = None, **kwargs):
     if not DEBUG:
         return
 
-    d = {"event":event, **kwargs}
+    if not parent:
+        parent = TIP_SPAN
+
+    d = {
+        "event":event,
+        "timestamp": datetime.datetime.utcnow(),
+        "parent_id": parent.id if parent else None,
+        **kwargs
+    }
     logger.debug(d)
 
 def time(type:str, elapsed:float, results:DataFrame = DataFrame(), **kwargs):
     if DEBUG:
         event("time", type=type, elapsed=elapsed, results={
             "values": results,
             "count": len(results)
@@ -201,15 +210,15 @@
 
 def error(err, **kwargs):
     global handled_error
     if err is not handled_error:
         event("error", err=err, **kwargs)  # Emit the error event only if it's a new or different error
         for handler in logger.handlers:
             handler.flush()
-        handled_error = err 
+        handled_error = err
 
 def handle_compilation(compilation):
     if not DEBUG:
         return
 
     (file, line, block) = compilation.get_source()
     source = {"file": file, "line": line, "block": block}
```

### Comparing `relationalai-0.2.9/src/relationalai/dsl.py` & `relationalai-0.3.0/src/relationalai/dsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from enum import Enum
 import inspect
 from itertools import zip_longest
 import re
 import threading
 import typing
 from typing import Any, Dict, List, Optional, Set, Tuple, TypeGuard, Union, get_type_hints
@@ -11,14 +12,16 @@
 import datetime
 import hashlib
 import traceback
 import rich
 
 from pandas import DataFrame
 
+from .clients.client import Client
+
 from .metamodel import Behavior, Builtins, ActionType, Var, Task, Action, Builder, Type as mType, Property as mProperty
 from . import debugging
 from .errors import Errors, RAIException, RelQueryError
 
 from bytecode import Instr, Bytecode
 
 #--------------------------------------------------
@@ -82,14 +85,19 @@
     if isinstance(x, dict):
         return all(is_static(i) for i in x.values())
     return False
 
 def is_collection(x:Any) -> TypeGuard[Union[List, Tuple, Set]]:
     return isinstance(x, list) or isinstance(x, tuple) or isinstance(x, set)
 
+def rel_dict(**kwargs):
+    return InlineRelation(get_graph(), [
+        (Symbol(k), v) for k, v in kwargs.items()
+    ])
+
 #--------------------------------------------------
 # Base
 #--------------------------------------------------
 
 id = 0
 def next_id():
     global id
@@ -97,23 +105,22 @@
     return id
 
 #--------------------------------------------------
 # Producer
 #--------------------------------------------------
 
 class Producer():
-    def __init__(self, graph:'Graph', builtins:List[str]):
+    def __init__(self, graph:'Graph'):
         self._id = next_id()
         self._graph = graph
-        self._builtins = builtins
         self._subs = {}
 
-    def __getattribute__(self, name: str) -> Any:
-        if name.startswith("_") or name in self._builtins:
-            return object.__getattribute__(self, name)
+    def __getattr__(self, name: str) -> Any:
+        if name.startswith("_"):
+            return None
         if name == "getdoc":
             rich.print("[red bold]GETDOC CALLED")
             traceback.print_stack()
             return
         self._subs[name] = self._make_sub(name, self._subs.get(name))
         return self._subs[name]
 
@@ -211,18 +218,19 @@
 # Context
 #--------------------------------------------------
 
 class TaskExecType(Enum):
     Query = 1
     Rule = 2
     Procedure = 3
+    Export = 4
 
 class ContextSelect(Producer):
     def __init__(self, context:'Context'):
-        super().__init__(context.graph, ["add"])
+        super().__init__(context.graph)
         self._context = context
         self._select_len = None
         self._insts = []
         self._vars = []
         self._props = {}
 
     def _assign_vars(self):
@@ -236,27 +244,28 @@
     def __call__(self, *args: Any) -> Any:
         graph = self._context.graph
         task = self._context._task
         if task.behavior == Behavior.Query \
             and self._context._exec_type in [TaskExecType.Query, TaskExecType.Procedure]:
             if isinstance(args[0], tuple):
                 args = args[0]
-            graph._action(build.return_(list(args)))
+            export = self._context._format == "snowpark"
+            graph._action(build.return_(list(args), export=export))
         else:
             #TODO: good error message depending on the type of task we're dealing with
             raise Exception("Can't select in a non-query")
         return self._context
 
-    def __getattribute__(self, __name: str) -> Any:
-        if __name.startswith("_") or __name in ["add"]:
-            return object.__getattribute__(self, __name)
-        elif __name in self._props:
-            return Instance(self._context.graph, ActionType.Get, [], {}, var=to_var(self._props[__name]))
+    def __getattr__(self, name: str) -> Any:
+        if name.startswith("_"):
+            return None
+        if name in self._props:
+            return Instance(self._context.graph, ActionType.Get, [], {}, var=to_var(self._props[name]))
         else:
-            return getattr(Instance(self._context.graph, ActionType.Get, [], {}, var=to_var(self._vars[0])), __name)
+            return getattr(Instance(self._context.graph, ActionType.Get, [], {}, var=to_var(self._vars[0])), name)
 
     def add(self, item, **kwargs):
         arg_len = len(kwargs) + 1
         if self._select_len is not None and arg_len != self._select_len:
             raise Exception("Add must be provided the same arguments in each branch")
         self._select_len = arg_len
         self._assign_vars()
@@ -268,31 +277,39 @@
                 self._props[k] = v
 
         graph = self._context.graph
         graph._action(build.return_([item, *[kwargs[k] for k in self._props.keys()]]))
 
 class Context():
     def __init__(self, graph:'Graph', *args, behavior=Behavior.Query, op=None,
-                 exec_type=TaskExecType.Rule, dynamic=False, name="None",
-                 inputs=None, outputs=None, engine=None, tag=None):
+                 exec_type=TaskExecType.Rule, dynamic=False, format="default",
+                 props=None, engine=None, tag=None):
         self._id = next_id()
         self.results = DataFrame()
         self.graph = graph
         self._task = Task(behavior=behavior)
         self._op = op
         self._args = list(args)
         self._exec_type = exec_type
         self._select_len = None
-        self._rel = None
         self._dynamic = dynamic
-        self._name = name
-        self._inputs = inputs
-        self._outputs = outputs
+        self._props = props or {}
         self._engine= engine
         self._tag = tag # for benchmark reporting
+        self._format = self._resolve_format(format)
+
+    def _resolve_format(self, format):
+        if format == "default":
+            if self.graph._format != "default":
+                return self.graph._format
+            if self.graph._config.get("platform") == "snowflake":
+                # In the future we may want to default to snowpark
+                return "pandas"
+            return "pandas"
+        return format
 
     def __enter__(self):
         debugging.set_source(self._task, dynamic=self._dynamic)
         self.graph._push(self)
         return ContextSelect(self)
 
     def __exit__(self, *args):
@@ -310,19 +327,14 @@
                 raise RAIException(e.message) from None
             except RelQueryError as e:
                 raise RelQueryError(e.problems) from None
         else:
             self.graph._pop(self, exec=False)
         return False
 
-    def _ensure_rel(self, vs:List[Var]):
-        if self._rel is None:
-            self._rel = build.relation_action(ActionType.Get, self._task, vs)
-        self.graph._action(self._rel)
-
     def __iter__(self):
         if self._exec_type != TaskExecType.Query:
             raise Exception("Can't iterate over a non-query task")
         else:
             return self.results.itertuples(index=False)
 
     def _repr_html_(self):
@@ -344,15 +356,15 @@
     hasher = hashlib.sha256()
     hasher.update(combined_bytes)
     hash_128_bit = hasher.digest()[:16]
     return hash_128_bit
 
 class Type(Producer):
     def __init__(self, graph:'Graph', name:str, builtins:List[str] = [], scope:str=""):
-        super().__init__(graph, ["add", "persist", "extend", "known_properties"] + builtins)
+        super().__init__(graph)
         self._type = mType(scope+name)
         self._scope = scope
         if graph._config.get("compiler.use_value_types", False):
             self._type.parents.append(Builtins.ValueType)
             install = build.install(self._type)
             self._graph._action(install)
             debugging.set_source(install)
@@ -393,36 +405,51 @@
                 a = arg()
                 neue = self(a)
                 for k, v in kwargs.items():
                     if isinstance(v, Property):
                         v = getattr(a, v._prop.name)
                     neue.set(**{k:v})
 
+    def define(self, **kwargs):
+        for k, v in kwargs.items():
+            if isinstance(v, tuple):
+                (other_type, left, right) = v
+                with self._graph.rule():
+                    inst = other_type()
+                    me = self()
+                    getattr(inst, right) == getattr(me, left) # type: ignore
+                    if getattr(self, k).is_multi_valued:
+                        getattr(me, k).add(inst)
+                    else:
+                        me.set(**{k: inst})
+            else:
+                raise Exception("Define requires a tuple of (Type, left, right)")
+
     def __or__(self, __value: Any) -> 'TypeUnion':
         if isinstance(__value, Type):
             return TypeUnion(self._graph, [self, __value])
         if isinstance(__value, TypeUnion):
             return TypeUnion(self._graph, [self, *__value._types])
         raise Exception("Can't or a type with a non-type")
 
     def _make_sub(self, name: str, existing=None):
         if existing is not None:
             return existing
         return Property(self._graph, name, [self._type], self, scope=self._scope)
 
     def known_properties(self):
-        return [p.name for p in self._type.properties]
+        return [p.name.removeprefix(self._scope) for p in self._type.properties]
 
 #--------------------------------------------------
 # TypeUnion
 #--------------------------------------------------
 
 class TypeUnion(Producer):
     def __init__(self, graph:'Graph', types:List[Type]):
-        super().__init__(graph, [])
+        super().__init__(graph)
         self._types = types
 
     def __call__(self, *args, **kwargs) -> 'ContextSelect':
         if not len(self._graph._stack.stack):
             raise Exception("Can't create an instance outside of a context")
         graph = self._graph
         with graph.union(dynamic=True) as union:
@@ -445,15 +472,15 @@
 
 #--------------------------------------------------
 # Property
 #--------------------------------------------------
 
 class Property(Producer):
     def __init__(self, graph:'Graph', name:str, types:List[mType], provider:Type|TypeUnion, scope:str=""):
-        super().__init__(graph, ["to_property", "has_many", "is_multi_valued"])
+        super().__init__(graph)
         self._name = name
         self._type = types[0]
         self._scope = scope
         self._provider = provider
         self._prop = build.property_named(scope+name, types)
 
     def __call__(self, key:Any, value:Any):
@@ -478,15 +505,15 @@
 
 #--------------------------------------------------
 # Instance
 #--------------------------------------------------
 
 class Instance(Producer):
     def __init__(self, graph:'Graph', action_type:ActionType, positionals:List[Any], named:Dict[str,Any], var:Var|None=None, name=None, is_add=False, scope:str=""):
-        super().__init__(graph, RESERVED_PROPS)
+        super().__init__(graph)
         self._action = Action(action_type, to_var(var) if var else Var(name=name))
         self._actions = [self._action]
         self._sets = {}
         self._context = graph._stack.active()
         self._scope = scope
         available_types = []
         last_pos_var = None
@@ -543,15 +570,15 @@
 
         #--------------------------------------------------
         # Entities
         #--------------------------------------------------
         self._var = self._action.entity
         if self._var.type == Builtins.Unknown and len(self._action.types):
             self._var.type = self._action.types[0]
-        if not is_add:
+        if not is_add and (self._action.types or self._action.bindings):
             self._add_to_graph()
 
     def _to_var(self):
         if not self._graph._stack.contains(self._context):
             Errors.variable_out_of_context(Errors.call_source(), self._var.name)
         return self._var
 
@@ -593,15 +620,15 @@
 
 #--------------------------------------------------
 # InstanceProperty
 #--------------------------------------------------
 
 class InstanceProperty(Producer):
     def __init__(self, graph:'Graph', instance:Instance, name:str, var=None, scope:str=""):
-        super().__init__(graph, ["or_", "in_", "add", "extend", "choose"])
+        super().__init__(graph)
         self._instance = instance
         self._prop = build.property_named(scope+name, instance._action.types)
         self._var = var or Var(self._prop.type, name=name)
         self._check_context()
         self._scope = scope
         new = Instance(self._graph, ActionType.Get, [instance], {name: self._var}, scope=self._scope)
         self._action = new._action
@@ -611,15 +638,15 @@
             name = f"{self._instance._var.name}.{self._var.name}"
             Errors.variable_out_of_context(Errors.call_source(), name, is_property=True)
 
     def __call__(self, *args, **kwargs):
         raise Exception("Properties can't be called")
 
     def _make_sub(self, name: str, existing=None):
-        if existing is not None and existing._instance._context is self._graph._stack.active():
+        if existing is not None and self._graph._stack.is_active(existing._instance._context):
             return existing
         return getattr(Instance(self._graph, ActionType.Get, [self], {}), name)
 
     def _to_var(self):
         self._check_context()
         return self._var
 
@@ -628,14 +655,18 @@
         rel.pyrel_default(self._prop, other, self._instance, self)
         return self
 
     def in_(self, others):
         other_rel = InlineRelation(self._graph, [(x,) for x in others])
         return self == other_rel
 
+    def has_value(self):
+        self != rel.missing # type:ignore
+        return self
+
     def _remove_if_unused(self):
         # When calling append/extend we aren't necessarily doing a get on the property,
         # but we will already have added one. If we're the only thing using this get,
         # we remove it so that it doesn't unnecessarily constrain the query.
         remove = True
         for item in reversed(self._graph._stack.items):
             if item is self._action:
@@ -643,43 +674,48 @@
             elif isinstance(item, Action):
                 if self._var in item.vars():
                     remove = False
                     break
         if remove:
             self._graph._remove_action(self._action)
 
+    def set(self, *args, **kwargs):
+        return Instance(self._graph, ActionType.Get, [self], {}).set(*args, **kwargs)
+
     def add(self, other):
         self._remove_if_unused()
         self._graph._check_property(self._prop, multi_valued=True)
         rel = Action(ActionType.Bind, to_var(self._instance), [], {self._prop: to_var(other)})
         self._graph._action(rel)
 
     def extend(self, others):
         self._remove_if_unused()
         self._graph._check_property(self._prop, True)
         for other in others:
             rel = Action(ActionType.Bind, to_var(self._instance), [], {self._prop: to_var(other)})
             self._graph._action(rel)
 
     def choose(self, num, unique=True):
+        if num < 1:
+            raise ValueError("Must choose a positive number of items")
         self._remove_if_unused()
         items = [getattr(Instance(self._graph, ActionType.Get, [self._instance], {}), self._prop.name) for ix in range(num)]
         if unique:
             for ix in range(num-1):
                 items[ix] < items[ix+1]
         return items
 
 #--------------------------------------------------
 # Expression
 #--------------------------------------------------
 
 class Expression(Producer):
     def __init__(self, graph:'Graph', op:mType|Task, args:List[Any]):
 
-        super().__init__(graph, [])
+        super().__init__(graph)
         self._var = None
         self._context = graph._stack.active()
 
         # For calls to tasks with known signatures, normalize their arguments by
         # throwing on missing inputs or constructing vars for missing outputs
         if op.properties and not op.isa(Builtins.Anonymous):
             for prop, arg in zip_longest(op.properties, args):
@@ -734,19 +770,17 @@
         self._rel = self._build_rel()
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         op = self._rel
         self._ensure_args(len(args))
         return Expression(get_graph(), op, list(args))
 
-    def __getattribute__(self, __name: str) -> Any:
-        if __name.startswith("_") or __name in ["add"]:
-            return object.__getattribute__(self, __name)
-        self._subs[__name] = self._make_sub(__name, self._subs.get(__name))
-        return self._subs[__name]
+    def __getattr__(self, name: str) -> Any:
+        self._subs[name] = self._make_sub(name, self._subs.get(name))
+        return self._subs[name]
 
     def _make_sub(self, name: str, existing=None):
         if existing is not None:
             return existing
         ns = self._ns[:]
         if self._name:
             ns.append(self._name)
@@ -775,15 +809,15 @@
 
 #--------------------------------------------------
 # RawRelation
 #--------------------------------------------------
 
 class RawRelation(Producer):
     def __init__(self, graph:'Graph', name:str, arity:int):
-        super().__init__(graph, ["add"])
+        super().__init__(graph)
         self._name = name
         self._arity = arity
         self._type = build.relation(self._name, self._arity)
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         return Expression(self._graph, self._type, list(args))
 
@@ -798,15 +832,15 @@
 
 #--------------------------------------------------
 # InlineRelation
 #--------------------------------------------------
 
 class InlineRelation():
     def __init__(self, graph:'Graph', data:List[Tuple]):
-        self._var = Var()
+        self._var = Var(type=Builtins.InlineRawData)
         self._graph = graph
         cols = [[] for _ in range(len(data[0]))]
         for row in data:
             for i, val in enumerate(row):
                 cols[i].append(to_var(val))
 
         params = [Var(value=col) for col in cols]
@@ -830,15 +864,15 @@
 
 #--------------------------------------------------
 # RelationRef
 #--------------------------------------------------
 
 class RelationRef(Producer):
     def __init__(self, graph:'Graph', rel:Task|mType, args:List[Var]):
-        super().__init__(graph, [])
+        super().__init__(graph)
         self._rel = rel
         self._args = args
         self._var = args[-1]
         self._action = build.relation_action(ActionType.Get, self._rel, self._args)
 
     def _use_var(self):
         self._graph._action(self._action)
@@ -922,18 +956,19 @@
         new_code = new_bytecode.to_code()
 
         # Create a new function from the new code object with the correct globals
         new_func = type(func)(new_code, func.__globals__, func.__name__, func.__defaults__, func.__closure__)
 
         # Update the globals dictionary of the new function to include 'ret'
         name = f"{schema}.{func.__name__}" if schema else func.__name__
-        ctx = Context(model, exec_type=TaskExecType.Procedure, name=name, outputs=output_types, **kwargs)
+        props = {"outputs": output_types, "name": name}
+        ctx = Context(model, exec_type=TaskExecType.Procedure, props=props, format="snowpark", **kwargs)
         with ctx as ret:
             inputs = to_list(Vars(len(arg_names)))
-            ctx._inputs = list(zip(arg_names, [to_var(i) for i in inputs], input_types))
+            props["inputs"] = list(zip(arg_names, [to_var(i) for i in inputs], input_types))
             # Get the bytecode of the original function
             new_func.__globals__["ret"] = ret
             # Call the new function with the provided arguments
             new_func(*inputs)
 
         def wrapper():
             raise Exception("Exports can't be called directly. They are exported to the underlying platform")
@@ -965,14 +1000,24 @@
                 return compacted
 
     def contains(self, item):
         for i in self.stack:
             if i is item:
                 return True
 
+    def is_active(self, item):
+        if isinstance(item, Context) and item._task.behavior != Behavior.Query:
+            return False
+        return item == self.active()
+
+    def in_context(self, item):
+        if isinstance(item, Context) and item._task.behavior != Behavior.Query:
+            return False
+        return self.contains(item)
+
     def active(self):
         try:
             cur = self.stack[-1]
             if cur is self._graph._temp_rule:
                 Errors.out_of_context(Errors.call_source())
             return cur
         except IndexError:
@@ -1047,16 +1092,14 @@
                 stack.append(task)
 
             elif op == "pop":
                 cur = stack.pop()
                 cur.items.extend(buffer)
                 buffer.clear()
                 if not len(stack):
-                    if not self._graph._config.get("compiler.use_v2", False):
-                        cur.normalize()
                     return cur
                 if isinstance(value, Context) and value._op:
                     stack[-1].items.append(build.call(value._op, [Var(value=value._args), Var(Builtins.Task, value=cur)]))
                 else:
                     stack[-1].items.append(build.call(cur, list(cur.bindings.values())))
 
         raise Exception("No task found")
@@ -1089,23 +1132,24 @@
 
 def Vars(count) -> Any:
     if count == 1:
         return Instance(get_graph(), ActionType.Get, [], {}, Var(Builtins.Unknown))
     return [Instance(get_graph(), ActionType.Get, [], {}, Var(Builtins.Unknown)) for _ in range(count)]
 
 class Graph:
-    def __init__(self, client, name:str):
+    def __init__(self, client:Client, name:str, format:str="default"):
         self.name = name
-        self._stack = RuleStack(self)
-        self._temp_rule = Context(self)
         self._executed = []
         self._client = client
         self._config = client.resources.config
         self.resources = client.resources
         self._prop_is_multi:Dict[str, bool] = {}
+        self._format = format
+        self._stack = RuleStack(self)
+        self._temp_rule = Context(self)
 
         _ensure_stack().append(self)
         self._stack.push(self._temp_rule)
 
     #--------------------------------------------------
     # Rule stack
     #--------------------------------------------------
@@ -1147,60 +1191,74 @@
             return
         self._stack.items.append(action)
 
     def _remove_action(self, action):
         self._stack.items.remove(action)
 
     def _exec(self, context:Context, task):
+        props = context._props
         if context._exec_type == TaskExecType.Rule:
             self._client.install(f"rule{len(self._executed)}", context._task)
         elif context._exec_type == TaskExecType.Query:
-            context.results = self._client.query(context._task, tag=context._tag)
+            context.results = self._client.query(context._task, tag=context._tag, format=context._format)
         elif context._exec_type == TaskExecType.Procedure:
-            self._client.export_udf(context._name, context._inputs, context._outputs, context._task, context._engine)
+            self._client.export_udf(props["name"], props["inputs"], props["outputs"], context._task, props.get("engine"))
+        elif context._exec_type == TaskExecType.Export:
+            self._client.export_table(props["name"], props["rel"], props["columns"], context._task, engine=props.get("engine"), refresh=props.get("refresh"))
         self._executed.append(context)
 
     #--------------------------------------------------
     # Property handling
     #--------------------------------------------------
 
     def _check_property(self, prop:mProperty, multi_valued=False, unknown_cardinality=False):
         name = prop.name
         if name in RESERVED_PROPS:
             Errors.reserved_property(Errors.call_source(), name)
 
-        if not self._config.get("compiler.use_multi_valued", False):
-            if multi_valued:
-                raise Exception(f"Multi-valued properties aren't enabled. Trying to use a property `{name}` as a multi-valued property")
-            return
-        elif unknown_cardinality:
+        if unknown_cardinality:
             return
 
         if name in self._prop_is_multi:
             if self._prop_is_multi[name] != multi_valued:
                 raise Exception(f"Trying to use a property `{name}` as both singular and multi-valued")
+            elif self._prop_is_multi[name] and Builtins.MultiValued not in prop.parents:
+                prop.parents.append(Builtins.MultiValued)
         else:
             self._prop_is_multi[name] = multi_valued
+
         if not multi_valued and Builtins.FunctionAnnotation not in prop.parents:
             prop.parents.append(Builtins.FunctionAnnotation)
-
+        elif multi_valued and Builtins.MultiValued not in prop.parents:
+            prop.parents.append(Builtins.MultiValued)
 
     #--------------------------------------------------
     # Public API
     #--------------------------------------------------
 
-    def Type(self, name:str):
+    def Type(self, name:str, source=None):
+        if source:
+            return self.resources.to_model_type(self, name, source)
         return Type(self, name)
 
     def rule(self, **kwargs):
         return Context(self, **kwargs)
 
     def scope(self, **kwargs):
         return Context(self, **kwargs)
 
+    def case(self, **kwargs):
+        return Context(self, **kwargs)
+
+    def match(self, multiple=False, **kwargs):
+        if not multiple:
+            return Context(self, behavior=Behavior.OrderedChoice, **kwargs)
+        else:
+            return Context(self, behavior=Behavior.Union, **kwargs)
+
     def query(self, **kwargs):
         return Context(self, exec_type=TaskExecType.Query, **kwargs)
 
     def export(self, object:str = "", **kwargs):
         return export(self, object, kwargs)
 
     def found(self, **kwargs):
@@ -1226,13 +1284,12 @@
         elif os.path.isdir(path):
             for root, _, files in os.walk(path):
                 for file in files:
                     if file.endswith('.rel'):
                         file_path = os.path.join(root, file)
                         self._client.load_raw_file(file_path)
 
-    def exec_raw(self, code:str, readonly=True, raw_results=True, inputs:dict|None = None):
+    def exec_raw(self, code:str, readonly=True, raw_results=True, inputs={}):
         return self._client.exec_raw(code, readonly=readonly, raw_results=raw_results, inputs=inputs)
 
     def install_raw(self, code:str, name:str|None=None):
         self._client.install_raw(code, name)
-
```

### Comparing `relationalai-0.2.9/src/relationalai/errors.py` & `relationalai-0.3.0/src/relationalai/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import defaultdict
 import io
 import textwrap
 from typing import Any, List, Tuple
 from .metamodel import Action, Task
 from . import debugging
 from rich.console import Console
+from enum import Enum
 
 #--------------------------------------------------
 # Print helpers
 #--------------------------------------------------
 
 def rich_str(string:str, style:str|None = None) -> str:
     output = io.StringIO()
@@ -169,14 +170,42 @@
         self.problems = problems
 
     def pprint(self):
         body = "\n\n".join(f'{problem["error_code"]}\n{problem["report"]}\n{problem["message"]}'
                            for problem in self.problems)
         return f"Rel query error\n{body}"
 
+# whether the python library or the Rel schema is out of date (or both!)
+class InvalidVersionKind(Enum):
+    LibraryOutOfDate = 'LibraryOutOfDate'
+    SchemaOutOfDate = 'SchemaOutOfDate'
+    Incompatible = 'Incompatible'
+
+class RAIInvalidVersionError(RAIException):
+    def __init__(self, kind: InvalidVersionKind, expected, lock, platform, errors: list[tuple[InvalidVersionKind, str, str]] = []):
+        self.library_expected = expected
+        self.database_provided = lock
+        self.errors = errors
+
+        if kind == InvalidVersionKind.LibraryOutOfDate:
+            msg = "The RelationalAI python library is out of date with respect to the " \
+                "schema. Please, update the library before proceeding."
+        elif kind == InvalidVersionKind.SchemaOutOfDate:
+            schema_fix = "You can update the schema using the `API.update_libraries` stored procedure."
+            if platform == "azure":
+                schema_fix = "Unfortunately, the schema must be recreated in Azure."
+            msg = f"The schema is out of date with respect to the RelationalAI library. {schema_fix}"
+        else:
+            schema_fix = "executing the `API.update_libraries` stored procedure"
+            if platform == "azure":
+                schema_fix = "recreating the schema in Azure"
+            msg = "The RelationalAI python library is incompatible with the current schema. " \
+                f"Updating the python library and {schema_fix} may resolve the issue."
+        super().__init__(msg)
+
 #--------------------------------------------------
 # Errors
 #--------------------------------------------------
 
 class Errors:
     @staticmethod
     def call_source(steps=None):
@@ -343,17 +372,18 @@
         # group by source
         source_map = defaultdict(list)
         for (name, source) in undefineds:
             source_map[source.source].append((source, name))
 
         for names in source_map.values():
             source = names[0][0]
-            props = ", ".join([f"[yellow]{name}[/yellow]" for (_, name) in names])
-            prop_line = f"property {props} has" if len(names) == 1 else f"properties {props} have"
-            found = PropertyFinder(source.line, [name for (_, name) in names])
+            unique_names = list(set([name for (_, name) in names]))
+            props = ", ".join([f"[yellow]{name}[/yellow]" for name in unique_names])
+            prop_line = f"property {props} has" if len(unique_names) == 1 else f"properties {props} have"
+            found = PropertyFinder(source.line, unique_names)
             if source.block:
                 found.visit(source.block)
             found_lines = found.found_properties_lines or found.dynamic_properties
             marked = mark_source(source, -1, -1, indent=12, highlight_lines=found_lines)
             content = f"""
             The {prop_line} never been set or added to and so will always cause the rule or query to fail.
 
@@ -411,8 +441,8 @@
     def engine_not_found(name:str, message:str):
         content = f"""
         The engine [yellow]{name}[/yellow] isn't available. You can start the engine with the following command:
 
         [green]rai engines:create --name {name}[/green]
         """
         print_error("Engine unavailable", content)
-        raise RAIException(message) from None
+        raise RAIException(message) from None
```

### Comparing `relationalai-0.2.9/src/relationalai/metagen.py` & `relationalai-0.3.0/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/metamodel.py` & `relationalai-0.3.0/src/relationalai/metamodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         namer = Namer()
         for i in self.items:
             ent = i.entity.value
             if i.action == ActionType.Call and isinstance(ent, Task):
                 sub = ent.return_cols()
                 if len(sub):
                     return sub
-            if i.action == ActionType.Bind and i.entity.value == Builtins.Return:
+            if i.action == ActionType.Bind and i.entity.isa(Builtins.Return):
                 cols = []
                 for (prop, var) in i.bindings.items():
                     cols.append(namer.get(var) or namer.get(prop))
                 return cols
         return []
 
     def has_persist(self, seen=None) -> bool:
@@ -325,14 +325,17 @@
         if self is other:
             return True
         return self.action == other.action \
                 and self.entity == other.entity \
                 and self.types == other.types \
                 and self.bindings == other.bindings
 
+    def params_list(self) -> List[Var]:
+        return list(self.bindings.values())
+
     def __hash__(self) -> int:
         return self.id
 
 #--------------------------------------------------
 # All
 #--------------------------------------------------
 
@@ -352,20 +355,22 @@
         self.Number = Type("Number", parents=[self.Primitive])
         self.Int = Type("Int", parents=[self.Number])
         self.Decimal = Type("Decimal", parents=[self.Number])
         self.Bool = Type("Bool", parents=[self.Primitive])
         self.Type = Type("Type", parents=[self.Primitive])
         self.ValueType = Type("ValueType", parents=[self.Type])
         self.Symbol = Type("Type", parents=[self.Primitive])
+        self.Missing = Type("Missing", parents=[self.Primitive])
         self.Relation = Type("Relation", parents=[self.Primitive], properties=[Property(f"v{id}", self.Any) for i in range(1000)])
         self.Anonymous = Type("Anonymous") # A thing we assume to exist in the host DB for which we don't have information.
         self.Task = Type("Task", parents=[self.Type, self.Relation])
         Task._task_builtin = self.Task
         self.Install = Task("Install", parents=[self.Task], properties=[Property("item", self.Any)])
         self.Return = Type("Return", parents=[self.Relation], properties=[Property(f"v{id}", self.Any) for i in range(20)])
+        self.ExportReturn = Type("ExportReturn", parents=[self.Return], properties=[Property(f"v{id}", self.Any) for i in range(20)])
         self.RawCode = Type("RawCode", properties=[Property("code", self.String)])
         self.RawData = Type("RawData", parents=[self.Relation])
         self.Inline = Type("Inline", parents=[])
         self.Intermediate = Type("Intermediate", parents=[self.Relation])
         self.InlineRawData = Type("InlineRawData", parents=[self.RawData])
         self.InlineExpression = Type("InlineExpression", parents=[])
         self.Aggregate = Type("Aggregate", parents=[self.Task])
@@ -375,14 +380,16 @@
         self.Exists = Task("Exists", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
         self.Every = Task("Every", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
 
         self.Annotation = Type("Annotation")
         self.InlineAnnotation = Type("Inline", parents=[self.Annotation])
         self.FunctionAnnotation = Type("Function", parents=[self.Annotation])
 
+        self.MultiValued = Type("MultiValued")
+
         self.Identity = Type("Identity", parents=[self.String])
         self.make_identity = Task("make_identity", properties=[
             Property("params", self.Any, True),
             Property("identity", self.Any)
         ])
 
         self.Infix = Type("Infix")
@@ -442,15 +449,17 @@
 
     def call(self, op, params:List[Any]):
         a = Action(ActionType.Call, Var(Builtins.Task, value=op))
         for ix, p in enumerate(params):
             a.append(op.properties[ix], self.to_var(p))
         return a
 
-    def return_(self, params:List[Any]):
+    def return_(self, params:List[Any], export=False):
+        if export:
+            return self.relation_action(ActionType.Bind, Builtins.ExportReturn, params)
         return self.relation_action(ActionType.Bind, Builtins.Return, params)
 
     def relation(self, name:str, field_count:int):
         return Type(name,
                     parents=[Builtins.Relation, Builtins.Anonymous],
                     properties=[Builtins.Relation.properties[i] for i in range(field_count)])
 
@@ -511,34 +520,30 @@
 class Namer():
     def __init__(self, unnamed_vars=False):
         self.name_mapping = {}
         self.names = set()
         self.unnamed_vars = unnamed_vars
 
     def get_safe_name(self, name:str):
+        name = name.lower()
         if name in self.names:
             ix = 2
             while f"{name}{ix}" in self.names:
                 ix += 1
             name = f"{name}{ix}"
         self.names.add(name)
         return name
 
     def get(self, item:Var|Task|Type|Property):
         if item.id in self.name_mapping:
             return self.name_mapping[item.id]
 
         name = item.name if not self.unnamed_vars or not isinstance(item, Var) else None
         name = name or ("t" if isinstance(item, Task) else "v")
-        raw_name = name
-        ix = 2
-        while name in self.names:
-            name = f"{raw_name}{ix}"
-            ix += 1
-        self.names.add(name)
+        name = self.get_safe_name(name)
         self.name_mapping[item.id] = name
         return name
 
     def reset(self):
         self.name_mapping.clear()
         self.names.clear()
 
@@ -783,7 +788,27 @@
                     for var in v.value:
                         if isinstance(var, Var) and (with_values or var.value is None):
                             vars.add(var)
                 else:
                     if with_values or v.value is None:
                         vars.add(v)
         return vars
+
+    @staticmethod
+    def gather_task_vars(task:Task, with_values=False, only_direct_children=False, seen=None) -> Set[Var]:
+        if seen is None:
+            seen = set()
+        if task in seen:
+            return set()
+        seen.add(task)
+
+        refs = set()
+        for i in task.items:
+            vs = i.vars()
+            if only_direct_children and i.is_subtask_call():
+                refs.update(Utils.gather_task_vars(cast(Task, i.entity.value), with_values, only_direct_children, seen))
+            for v in vs:
+                if not only_direct_children and v.value and isinstance(v.value, Task):
+                    refs.update(Utils.gather_task_vars(v.value, with_values, seen))
+                elif with_values or (v.value is None and not v.isa(Builtins.InlineRawData)):
+                    refs.add(v)
+        return refs
```

### Comparing `relationalai-0.2.9/src/relationalai/rel_emitter.py` & `relationalai-0.3.0/src/relationalai/rel_emitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         code = ""
         try:
             if isinstance(task, Task):
                 code = getattr(self, task.behavior.value)(task)
             elif isinstance(task, Var):
                 code = self.emit_var(task)
         except Exception as e:
-            print("EMIT FAILED:", e)
-            # raise e
+            # print("EMIT FAILED:", e)
+            raise e
         return code
 
     #--------------------------------------------------
     # Helpers
     #--------------------------------------------------
 
     def sanitize(self, input_string, is_rel_name = False):
@@ -111,15 +111,15 @@
         if var.type.isa(Builtins.Symbol):
             return f":{self.sanitize(var.value)}"
         if var.value is not None:
             return self.emit_val(var.value, var)
         if var.name == "_":
             return "_"
         name = self.namer.get(var)
-        return f"_{self.sanitize(name).lower()}"
+        return f"_{self.sanitize(name)}"
 
     #--------------------------------------------------
     # Sequence
     #--------------------------------------------------
 
     def sequence_action(self, action: Action):
         if action.entity.value == Builtins.RawCode:
@@ -259,14 +259,15 @@
                 elif i.entity.value == Builtins.Install:
                     (item,) = i.bindings.values()
                     supporting_rules.append(f"declare {self.emit_var(item)}")
                     if isinstance(item.value, Type) and item.value.isa(Builtins.ValueType):
                         vtype = self.sanitize(item.value.name).capitalize() + "Type"
                         supporting_rules.append(f"value type {vtype} {{ UInt128 }}")
                         supporting_rules.append(f"@inline def pyrel_unwrap(y in {vtype}, x): ^{vtype}(x, y)")
+                        supporting_rules.append(f"def ::std::common::uuid_string(x in {vtype}, y): exists((z) | pyrel_unwrap(x, z) and uuid_string(z,y))")
                         for op in ["<", ">"]:
                             supporting_rules.append(f"def ::std::common::({op})[x in {vtype}, y in {vtype}]: exists((a, b) | ^{vtype}(a, x) and ^{vtype}(b, y) and a {op} b)")
                         for op in ["minimum", "maximum"]:
                             supporting_rules.append(f"def ::std::common::{op}(x in {vtype}, y in {vtype}, z in {vtype}): exists((a, b) | ^{vtype}(minimum[a, b], z) and ^{vtype}(a, x) and ^{vtype}(b, y))")
                 else:
                     body.append(self.to_relation(i, body_vars, body))
             elif i.action == ActionType.Bind and i.entity.value == Builtins.Return:
```

### Comparing `relationalai-0.2.9/src/relationalai/rel_utils.py` & `relationalai-0.3.0/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/analysis/mechanistic.py` & `relationalai-0.3.0/src/relationalai/analysis/mechanistic.py`

 * *Files 8% similar despite different names*

```diff
@@ -154,20 +154,23 @@
                 if item.is_subtask_call():
                     sub_task = func.value
                     if sub_task.behavior == Behavior.Query or sub_task.behavior == Behavior.Sequence:
                         self.sequence()
                         self.interpret(sub_task)
                         self.pop()
                     elif sub_task.behavior == Behavior.Union:
-                        self.union(next(iter(item.bindings.values())))
-                        self.interpret(sub_task)
-                        self.pop()
+                        params = list(item.bindings.values())
+                        if params:
+                            self.union(params[0])
+                            self.interpret(sub_task)
+                            self.pop()
 
                     elif sub_task.behavior == Behavior.OrderedChoice:
-                        print("CHOICE")
+                        # print("CHOICE")
+                        pass
                     else:
                         raise Exception(f"UNKNOWN SUB TASK {sub_task.behavior}")
                 elif func.isa(Builtins.Install):
                     self.install(params[0])
                 elif func.isa(Builtins.Quantifier):
                     self.sequence()
                     self.interpret(params[1].value)
@@ -179,20 +182,22 @@
                         quantifier = "every"
                     else:
                         raise Exception()
                     self.quantify(quantifier, params[0].value)
                     self.pop()
 
                 elif func.isa(Builtins.Aggregate):
-                    print("Aggregate")
+                    # print("Aggregate")
+                    pass
                 elif func.isa(Builtins.Infix) and len(params) == 2:
                     self.filter(func.value.name, params)
                 else:
                     self.compute(func.value.name, params[:-1], params[-1])
             elif item.action == ActionType.Bind and item.entity.isa(Builtins.Return):
                 self.return_(item.bindings.values())
             elif item.action.is_effect():
                 op = item.action.name
                 props = {key.name: value for key,value in item.bindings.items()}
                 self.effect(op, item.entity, [type.name for type in item.types], props)
             else:
-                print("hey!", item)
+                # print("hey!", item)
+                pass
```

### Comparing `relationalai-0.2.9/src/relationalai/analysis/whynot.py` & `relationalai-0.3.0/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/clients/azure.py` & `relationalai-0.3.0/src/relationalai/clients/azure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 from datetime import datetime, timedelta
 import json
 import textwrap
 import time
-from typing import Any, Tuple, List
-import base64
+from typing import Any, Dict, Tuple, List
 from urllib.error import HTTPError
 
 from pandas import DataFrame
-import pandas as pd
-import re
-import decimal
 
 from relationalai import debugging
 
 from ..errors import Errors, RAIException
 from ..rel_utils import assert_no_problems
 from ..loaders.loader import emit_delete_import, import_file, list_available_resources
 from .config import Config
 from .types import ImportSource, ImportSourceFile
-from .client import Client, ResourceProvider
+from .client import Client, ExportParams, ResourceProvider
 from .. import dsl, rel, metamodel as m
 from railib import api
+from . import result_helpers
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
-UNIXEPOCH = 62135683200000
-MILLISECONDS_PER_DAY = 24 * 60 * 60 * 1000
 TXN_FIELDS = ["id", "account_name", "state", "created_on", "finished_at", "duration", "database_name", "read_only", "engine_name", "query", "query_size", "tags", "user_agent", "response_format_version"]
 TXN_REPLACE_MAP = {"database_name": "database", "engine_name": "engine", "account_name": "account", "user_agent": "agent"}
 VALID_ENGINE_STATES = ["REQUESTED", "PROVISIONED", "PROVISIONING"]
 
 #--------------------------------------------------
 # Resources
 #--------------------------------------------------
@@ -53,14 +48,21 @@
     # Generic
     #--------------------------------------------------
 
     def get_version(self):
         raise Exception("Azure version not available")
 
     #--------------------------------------------------
+    # Databases
+    #--------------------------------------------------
+
+    def get_database(self, name:str):
+        return api.get_database(self._api_ctx(), name)
+
+    #--------------------------------------------------
     # Engines
     #--------------------------------------------------
 
     def list_engines(self, state:str|None = None):
         return api.list_engines(self._api_ctx(), state)
 
     def get_engine(self, name:str):
@@ -98,83 +100,108 @@
         with debugging.span("create_model", name=name):
             return api.create_database(self._api_ctx(), name)
 
     def delete_graph(self, name:str):
         with debugging.span("delete_model", name=name):
             return api.delete_database(self._api_ctx(), name)
 
+    def clone_graph(self, target_name:str, source_name:str, nowait_durable:bool=False):
+        # not a typo: the argument order is indeed target then source
+        return api.create_database(self._api_ctx(), target_name, source_name)
+
     #--------------------------------------------------
     # Models
     #--------------------------------------------------
 
     def list_models(self, database: str, engine: str):
         return api.list_databases(self._api_ctx())
 
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
+        rel_code = self.create_models_code(models)
+        results = self.exec_raw(database, engine, rel_code, readonly=False)
+        if results.problems:
+            return results.problems
+        return []
+
+    def delete_model(self, database:str, engine:str, name:str):
+        return api.delete_model(self._api_ctx(), database, engine, name)
+
+    def create_models_code(self, models:List[Tuple[str, str]]) -> str:
         lines = []
         for (name, code) in models:
             name = name.replace("\"", "\\\"")
             assert "\"\"\"\"\"\"\"" not in code, "Code literals must use fewer than 7 quotes."
 
             lines.append(textwrap.dedent(f"""
             def delete[:rel, :catalog, :model, "{name}"]: rel[:catalog, :model, "{name}"]
-            def insert[:rel, :catalog, :model, "{name}"]: raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
-            """))
+            def insert[:rel, :catalog, :model, "{name}"]: raw\"\"\"\"\"\"\"
+            """) + code + "\n\"\"\"\"\"\"\"")
         rel_code = "\n\n".join(lines)
-        results = self.exec_raw(database, engine, rel_code, readonly=False)
-        if results.problems:
-            return results.problems
-        return []
-
-    def delete_model(self, database:str, engine:str, name:str):
-        return api.delete_model(self._api_ctx(), database, engine, name)
+        return rel_code
 
     #--------------------------------------------------
     # Exports
     #--------------------------------------------------
 
     def list_exports(self, database: str, engine: str):
         raise Exception("Azure doesn't support exports")
 
-    def create_export(self, database: str, engine: str, name: str, inputs: List[str], out_fields: List[str], code: str):
+    def create_export(self, params: ExportParams):
+        if not params.dry_run:
+            raise Exception("Azure doesn't support exports")
+
+    def create_export_table(self, database: str, engine: str, table: str, relation: str, columns: Dict[str, str], code: str, refresh: str|None=None):
         raise Exception("Azure doesn't support exports")
 
     def delete_export(self, database: str, engine: str, name: str):
         raise Exception("Azure doesn't support exports")
 
     #--------------------------------------------------
     # Imports
     #--------------------------------------------------
 
-    def list_imports(self, model:str):
+    def list_imports(self, model:str|None, id:str|None, status:str|None = None, name:str|None = None, creator:str|None = None):
         return [*list_available_resources(self, model, self.get_default_engine_name()).values()]
 
     def create_import_stream(self, source:ImportSource, model:str, rate = 1, options: dict|None = None):
         raise Exception("Azure doesn't support import streams")
 
     def create_import_snapshot(self, source:ImportSource, model:str, options: dict|None = None):
         assert isinstance(source, ImportSourceFile), "Azure integration only supports loading from files and URLs right now."
         import_file(self, model, source, **(options or {}))
 
     def delete_import(self, import_name: str, model:str):
         res = self.exec_raw(model, self.get_default_engine_name(), emit_delete_import(import_name), False)
         assert_no_problems(res)
 
+    def set_imports_engine(self, engine:str):
+        raise Exception("Azure doesn't support setting imports engine")
+
+    def change_imports_status(self, status:str):
+        raise Exception("Azure doesn't support import status changes")
+
+    def change_stream_status(self, stream_id: str, model:str, suspend: bool):
+        raise Exception("Azure doesn't support stream status changes")
+
+    def get_import_stream(self, stream_id: str, model:str):
+        raise Exception("Azure doesn't support get import streams")
+
     #--------------------------------------------------
     # Exec
     #--------------------------------------------------
 
-    def exec_raw(self, database:str, engine:str, raw_code:str, readonly=True, raw_results=True, inputs: dict = {}):
+    def exec_raw(self, database:str, engine:str, raw_code:str, readonly=True, raw_results=True, inputs: dict = {}, nowait_durable=False, headers={}):
         try:
             with debugging.span("transaction") as txn_span:
                 ctx = self._api_ctx()
                 with debugging.span("create"):
                     txn = api.exec_async(ctx, database, engine, raw_code, readonly=readonly, inputs=inputs)
                 txn_id = txn.transaction["id"]
                 txn_span["txn_id"] = txn_id
+                debugging.event("transaction_created", txn_span, txn_id=txn_id)
 
                 # TODO: dedup with SDK
                 rsp = api.TransactionAsyncResponse()
                 txn = api.get_transaction(ctx, txn_id)
                 start_time = time.time()
 
                 def check_done():
@@ -203,51 +230,26 @@
             # RAI API uses a JSON payload in the body to explain why the request failed
             # This annotates the error with that to make the exception actually useful.
             if "engine not found" in res.get('message', ''):
                 print("") # the SDK appears to print some stuff before the error message
                 Errors.engine_not_found(self.config.get("engine", "Unknown"), res.get('message'))
             raise RAIException(f" {res.get('message', '')} {res.get('details', '')}")
 
-    def _has_errors(self, results):
-        if len(results.problems):
-            for problem in results.problems:
-                if problem.get('is_error') or problem.get('is_exception'):
-                    return True
-
-    def format_results(self, results, task:m.Task) -> Tuple[DataFrame, List[Any]]:
-        data_frame = DataFrame()
-        if len(results.results):
-            for result in results.results:
-                types = [t for t in result["relationId"].split("/") if t != "" and not t.startswith(":")]
-                result_frame:DataFrame = result["table"].to_pandas()
-                for i, col in enumerate(result_frame.columns):
-                    if "UInt128" in types[i]:
-                        result_frame[col] = result_frame[col].apply(lambda x: base64.b64encode(x.tobytes()).decode()[:-2])
-                    elif "FixedDecimal" in types[i]:
-                        decimal_info = re.search(r"FixedDecimal\{Int(\d+), (\d+)\}", types[i])
-                        if decimal_info:
-                            bits = int(decimal_info.group(1))
-                            scale = int(decimal_info.group(2))
-                            if bits == 128:
-                                result_frame[col] = result_frame[col].apply(lambda x: (decimal.Decimal(str((int(x[1]) << 64) + int(x[0]))) if x[1] > 0 else decimal.Decimal(str(x[0]))) / (10 ** scale))
-                            else:
-                                result_frame[col] = result_frame[col].apply(lambda x: decimal.Decimal(str(x)) / (10 ** scale))
-                    elif "Int128" in types[i]:
-                        result_frame[col] = result_frame[col].apply(lambda x: (int(x[1]) << 64) + int(x[0]) if x[1] > 0 else x[0])
-                    elif types[i] == "Dates.DateTime":
-                        result_frame[col] = pd.to_datetime(result_frame[col] - UNIXEPOCH, unit="ms")
-                    elif types[i] == "Dates.Date":
-                        result_frame[col] = pd.to_datetime(result_frame[col] * MILLISECONDS_PER_DAY - UNIXEPOCH, unit="ms")
-                ret_cols = task.return_cols()
-                if len(ret_cols) and len(result_frame.columns) == len(ret_cols):
-                    result_frame.columns = task.return_cols()[0:len(result_frame.columns)]
-                result["table"] = result_frame
-                if ":output" in result["relationId"]:
-                    data_frame = pd.concat([data_frame, result_frame], ignore_index=True)
-        return (data_frame, results.problems)
+    def format_results(self, results, task:m.Task|None=None) -> Tuple[DataFrame, List[Any]]:
+        return result_helpers.format_results(results, task)
+
+    #--------------------------------------------------
+    # Exec format
+    #--------------------------------------------------
+
+    def exec_format(self, database: str, engine: str, raw_code: str, task:m.Task, format:str, readonly: bool = True, inputs={}) -> Any: # @FIXME: Better type annotation
+        raise Exception("Azure doesn't support alternative formats yet")
+
+    def to_model_type(self, model:dsl.Graph, name: str, source:str):
+        raise Exception("Azure doesn't support import types yet")
 
     #--------------------------------------------------
     # Transactions
     #--------------------------------------------------
 
     def get_transaction(self, transaction_id):
         txn = api.get_transaction(self._api_ctx(), transaction_id)
@@ -314,16 +316,24 @@
         # all transactions are executed synchronously against azure
         pass
 
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
-def Graph(name, *, profile:str|None=None, config:Config, dry_run:bool=False):
-    client = Client(Resources(profile, config), rel.Compiler(config), name, dry_run=dry_run)
+def Graph(name, *, profile:str|None=None, config:Config, dry_run:bool=False, isolated=True, keep_model:bool=False, format="default"):
+    client = Client(
+        Resources(profile, config),
+        rel.Compiler(config),
+        name,
+        config,
+        dry_run=dry_run,
+        isolated=isolated,
+        keep_model=keep_model,
+    )
     client.install("pyrel_base", dsl.build.raw_task("""
         @inline
         def make_identity(x..., z):
             exists((u) | hash128({x...}, x..., u) and
             hash_value_uint128_convert(u, z))
 
         @inline
@@ -331,8 +341,8 @@
             F(k..., v) or (not F(k..., _) and v = c)
 
         @inline
         def pyrel_unwrap(x in UInt128, y): y = x
 
         declare __resource
     """))
-    return dsl.Graph(client, name)
+    return dsl.Graph(client, name, format=format)
```

### Comparing `relationalai-0.2.9/src/relationalai/clients/client.py` & `relationalai-0.3.0/src/relationalai/clients/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
 import atexit
 import re
 from collections import defaultdict
-from typing import Dict, List, Any, Tuple
+from typing import Dict, List, Any, Tuple, cast, Callable
 
 from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from pandas import DataFrame
 import time
 
 from .types import AvailableModel, Import, ImportSource
 from ..clients.config import Config
 from ..compiler import Compiler
 from .. import dsl, debugging, metamodel as m
@@ -16,14 +18,15 @@
 # InstallBatch
 #--------------------------------------------------
 
 class InstallBatch:
     def __init__(self):
         self.dirty = set()
         self.content:Dict[str, Dict[str, List[str]]] = defaultdict(lambda: defaultdict(list))
+        self.control_items:List[Tuple[str, Callable|None]] = []
         self.task_map = defaultdict(dict)
 
     def _cell(self):
         return debugging.jupyter.cell() or ""
 
     def _check_dirty_cells(self, name:str):
         for cell in debugging.jupyter.dirty_cells:
@@ -51,31 +54,61 @@
                     end = code.count("\n") + cur_line + 2
                     task_map[task] = (cur_line, end)
                     cur_line = end
             items.append((name, "\n\n".join(all_cells)))
         self.dirty.clear()
         return items
 
+    def get_all_models(self):
+        items = []
+        for name in self.content:
+            all_cells = []
+            for _, content in self.content[name].items():
+                for code, _ in content:
+                    all_cells.append(code)
+            items.append((name, "\n\n".join(all_cells)))
+        return items
+
+    def flush_control_items(self):
+        cur = self.control_items
+        self.control_items = []
+        return cur
+
     def is_dirty(self):
         return len(self.dirty) > 0
 
     def line_to_task(self, name:str, line:int):
         for task, (start, end) in self.task_map[name].items():
             if start <= line <= end:
                 return task
         return None
 
 #--------------------------------------------------
+# Helpers
+#--------------------------------------------------
+@dataclass
+class ExportParams:
+    source_database: str
+    database: str
+    engine: str
+    func_name: str
+    inputs: List[Tuple[str, str, Any]]
+    out_fields: List[Tuple[str, Any]]
+    code: str
+    dry_run: bool
+
+#--------------------------------------------------
 # Resources
 #--------------------------------------------------
 
 class ResourceProvider(ABC):
     def __init__(self, profile: str | None = None, config:Config|None=None):
         super().__init__()
         self.config = config or Config(profile)
+        self.delete_on_exit = True
         atexit.register(self.cancel_pending_transactions)
 
     @property
     def platform(self):
         return self.config.get("platform")
 
     @abstractmethod
@@ -119,18 +152,21 @@
         pass
 
     @abstractmethod
     def resume_engine(self, name: str):
         pass
 
     def get_default_engine_name(self) -> str:
-        return self.config.get("engine")
+        engine = self.config.get("engine")
+        if not engine:
+            raise Exception("No default engine in your configuration")
+        return engine
 
-    def get_app_name(self):
-        return self.config.get("rai_app_name", "relationalai")
+    def get_app_name(self) -> str:
+        return cast(str, self.config.get("rai_app_name", "relationalai"))
 
     #--------------------------------------------------
     # Transactions
     #--------------------------------------------------
     @abstractmethod
     def get_transaction(self, transaction_id):
         pass
@@ -163,14 +199,26 @@
     def create_graph(self, name: str):
         pass
 
     @abstractmethod
     def delete_graph(self, name: str):
         pass
 
+    @abstractmethod
+    def clone_graph(self, target_name: str, source_name: str, nowait_durable: bool = True):
+        pass
+
+    #--------------------------------------------------
+    # Databases
+    #--------------------------------------------------
+
+    @abstractmethod
+    def get_database(self, database: str):
+        pass
+
     #--------------------------------------------------
     # Models
     #--------------------------------------------------
 
     @abstractmethod
     def list_models(self, database: str, engine: str):
         pass
@@ -179,40 +227,64 @@
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
         pass
 
     @abstractmethod
     def delete_model(self, database: str, engine: str, name: str):
         pass
 
+    @abstractmethod
+    def create_models_code(self, models:List[Tuple[str, str]]) -> str:
+        pass
+
     #--------------------------------------------------
     # Exports
     #--------------------------------------------------
 
     @abstractmethod
     def list_exports(self, database: str, engine: str):
         pass
 
     @abstractmethod
-    def create_export(self, database: str, engine: str, name: str, inputs: List[Tuple[str, str, Any]], out_fields: List[Tuple[str, Any]], code: str):
+    def create_export(self, params: ExportParams):
+        pass
+
+    @abstractmethod
+    def create_export_table(self, database: str, engine: str, table: str, relation: str, columns: Dict[str, str], code: str, refresh: str|None=None):
         pass
 
     @abstractmethod
     def delete_export(self, database: str, engine: str, name: str):
         pass
 
     #--------------------------------------------------
     # Imports
     #--------------------------------------------------
 
     @abstractmethod
-    def list_imports(self, model: str) -> list[Import]:
+    def list_imports(self, id:str|None, name:str|None, model:str|None, status:str|None, creator:str|None) -> list[Import]:
+        pass
+
+    @abstractmethod
+    def get_import_stream(self, id:str|None, name:str|None):
+        pass
+
+    @abstractmethod
+    def create_import_stream(self, source: ImportSource, model: str, rate: int, resume: str|None, suspend: str|None, options: dict|None):
         pass
 
     @abstractmethod
-    def create_import_stream(self, source: ImportSource, model: str, rate: int, options: dict|None):
+    def change_stream_status(self, stream_id: str, model: str, suspend: bool):
+        pass
+
+    @abstractmethod
+    def set_imports_engine(self, engine: str):
+        pass
+
+    @abstractmethod
+    def change_imports_status(self, suspend: bool):
         pass
 
     @abstractmethod
     def create_import_snapshot(self, source: ImportSource, model: str, options: dict|None):
         pass
 
     @abstractmethod
@@ -220,40 +292,84 @@
         pass
 
     #--------------------------------------------------
     # Exec
     #--------------------------------------------------
 
     @abstractmethod
-    def exec_raw(self, database: str, engine: str, raw_code: str, readonly: bool = True, inputs={}) -> Any: # @FIXME: Better type annotation
+    def exec_raw(self, database: str, engine: str, raw_code: str, readonly: bool = True, inputs={}, nowait_durable=False, headers={}) -> Any: # @FIXME: Better type annotation
+        pass
+
+    def exec_format(self, database: str, engine: str, raw_code: str, task:m.Task, format:str, readonly: bool = True, inputs={}) -> Any: # @FIXME: Better type annotation
         pass
 
     @abstractmethod
     def format_results(self, results, task:m.Task|None=None) -> Tuple[DataFrame, List[Any]]:
         pass
 
+    #--------------------------------------------------
+    # Types
+    #--------------------------------------------------
+
+    @abstractmethod
+    def to_model_type(self, model:dsl.Graph, name:str, source:str) -> dsl.Type:
+        pass
+
 
 #--------------------------------------------------
 # Client
 #--------------------------------------------------
 
 class Client():
-    def __init__(self, resources:ResourceProvider, compiler:Compiler, database:str, dry_run=False):
+    def __init__(
+        self,
+        resources: ResourceProvider,
+        compiler: Compiler,
+        database: str,
+        config: Config,
+        dry_run=False,
+        isolated=True,
+        keep_model=False,
+        nowait_durable=True,
+    ):
         self.dry_run = dry_run
-        self._database = database
+        self._source_database = database
+        self._database = database[:30] + "_" + config.get_hash() if isolated else database
         self.compiler = compiler
         self._install_batch = InstallBatch()
         self.resources = resources
+        self.keep_model = keep_model
+        self.isolated = isolated
+        self.batch_span: debugging.Span|None = None
 
         if not self.dry_run:
-            start = time.perf_counter()
-            existing = self.resources.get_graph(self._database)
-            if not existing:
+            self.create_database(isolated=isolated, nowait_durable=nowait_durable)
+
+    def create_database(self, isolated=True, nowait_durable=True):
+        start = time.perf_counter()
+        with debugging.span("create_database", source=self._source_database, target=self._database):
+            database_exists = self.resources.get_graph(self._source_database)
+            if isolated:
+                if database_exists:
+                    temp = self._database
+                    self._database = self._source_database
+                    self.exec_raw("", readonly=False, internal=True, nowait_durable=True)
+                    self._database = temp
+                    self.resources.clone_graph(self._database, self._source_database, nowait_durable=nowait_durable)
+                else:
+                    self.resources.create_graph(self._database)
+            elif not database_exists:
                 self.resources.create_graph(self._database)
-                debugging.time("create_database", time.perf_counter() - start)
+            if isolated and not self.keep_model:
+                atexit.register(self.delete_database)
+            debugging.time("create_database", time.perf_counter() - start)
+
+    def delete_database(self):
+        if self.resources.delete_on_exit and not self.dry_run:
+            self.resources.delete_graph(self._database)
 
     def get_engine_name(self, name:str|None=None) -> str:
         return str(name or self.resources.config.get("engine"))
 
     def report_errors(self, errors:List[Any], abort_on_error=True, task=None):
         maybe_abort = False
         undefineds = []
@@ -286,64 +402,118 @@
             raise RelQueryError(errors)
 
     def load_raw_file(self, path:str):
         content = open(path).read()
         code = self.compiler.compile(dsl.build.raw_task(content))
         self._install_batch.set(path, code)
 
-    def exec_raw(self, code:str, readonly=True, raw_results=True, inputs={}):
-        return self.query(dsl.build.raw_task(code), readonly=readonly, raw_results=raw_results, inputs=inputs)
+    def exec_raw(self, code:str, readonly=True, raw_results=True, inputs={}, internal=False, nowait_durable=None, headers={}):
+        return self.query(dsl.build.raw_task(code), readonly=readonly, raw_results=raw_results, inputs=inputs, internal=internal, nowait_durable=nowait_durable, headers=headers)
+
+    def exec_control(self, code:str, cb:Callable|None=None):
+        self._install_batch.control_items.append((code, cb))
 
     def install_raw(self, code:str, name:str="pyrel_batch_0"):
         if not name:
             name = "pyrel_batch_0"
         self.compiler.compile(dsl.build.raw_task(code))
         self._install_batch.append(name, code)
 
-    def query(self, task:m.Task, rentrant=False, readonly=True, raw_results=False, inputs={}, tag=None) -> DataFrame|Any:
-        if self._install_batch.is_dirty():
-            self._install_batch_flush()
+    def _query(self, code:str, task:m.Task|None, end_span, readonly=True, raw_results=False, inputs={}, nowait_durable=None, headers={}):
+        if nowait_durable is None:
+            nowait_durable = self.isolated
+
+        results = self.resources.exec_raw(self._database, self.get_engine_name(), code, readonly=readonly, inputs=inputs, nowait_durable=nowait_durable, headers=headers)
+        dataframe, errors = self.resources.format_results(results, task)
+        end_span["results"] = dataframe
+        end_span["errors"] = errors
+        self.report_errors(errors, task=task, abort_on_error=not raw_results)
+        return results if raw_results else dataframe
+
+    def _query_format(self, code:str, task:m.Task, end_span, format, readonly=True, inputs={}):
+        results, errors = self.resources.exec_format(self._database, self.get_engine_name(), code, task, readonly=readonly, inputs=inputs, format=format)
+        # dataframe, errors = self.resources.format_results(results, task)
+        end_span["results"] = results
+        end_span["errors"] = errors
+        # self.report_errors(errors, task=task, abort_on_error=not raw_results)
+        # return results if raw_results else dataframe
+        return results
+
+    def query(self, task:m.Task, rentrant=False, readonly=True, raw_results=False, inputs={}, format="pandas", tag=None, nowait_durable=None, headers={}, internal=False) -> DataFrame|Any:
+        self._install_batch_flush()
 
-        with debugging.span("query", model=self._database, task=task, tag=tag) as end_span:
+        with debugging.span("query", model=self._database, task=task, tag=tag, internal=internal) as end_span:
             code = self.compiler.compile(task)
             if task.has_persist():
                 readonly = False
             if self.dry_run:
                 return DataFrame()
 
             start = time.perf_counter()
-            results = self.resources.exec_raw(self._database, self.get_engine_name(), code, readonly=readonly, inputs=inputs)
-            dataframe, errors = self.resources.format_results(results, task)
-            end_span["results"] = dataframe
-            end_span["errors"] = errors
-            if raw_results:
+            if format == "pandas":
+                results = self._query(code, task, end_span, readonly=readonly, raw_results=raw_results, inputs=inputs, nowait_durable=nowait_durable, headers=headers)
+                debugging.time("query", time.perf_counter() - start, DataFrame() if raw_results else results, internal=internal)
+            else:
+                results = self._query_format(code, task, end_span, readonly=readonly, inputs=inputs, format=format)
                 debugging.time("query", time.perf_counter() - start, DataFrame())
-                self.report_errors(errors, abort_on_error=False)
-                return results
-            self.report_errors(errors, task=task)
-            debugging.time("query", time.perf_counter() - start, dataframe)
-            return dataframe
+            return results
 
     def _install_batch_flush(self):
+        if not self._install_batch.is_dirty():
+            return
+
+        debugging.span_end(self.batch_span)
+        self.batch_span = None
+
         if not self.dry_run:
-            with debugging.span("install_batch", model=self._database):
+            with debugging.span("install_batch", model=self._database) as end_span:
                 start = time.perf_counter()
-                code = self._install_batch.flush()
-                errors = self.resources.create_models(self._database, self.get_engine_name(), code)
-                self.report_errors(errors)
-                debugging.time("install_batch", time.perf_counter() - start, code="\n".join([c[1] for c in code]))
+                rules = self._install_batch.flush()
+                control_items = self._install_batch.flush_control_items()
+                control_code = "\n\n".join([c[0] for c in control_items])
+                rule_code = self.resources.create_models_code(rules)
+                install_code = control_code + rule_code
+                dataframe = self._query(install_code, None, end_span, readonly=False, raw_results=True)
+                for (_, cb) in control_items:
+                    if cb:
+                        cb(dataframe)
+                debugging.time("install_batch", time.perf_counter() - start, code=install_code)
+
+    def get_install_models(self):
+        return self._install_batch.get_all_models()
 
     def install(self, name, task:m.Task):
+        if not self.batch_span:
+            self.batch_span = debugging.span_start("rule_batch")
         with debugging.span("rule", model=self._database, task=task, name=name):
             code = self.compiler.compile(task)
             self._install_batch.append("pyrel_batch_0", code, task=task)
 
     def export_udf(self, name, inputs:List[Tuple[str, m.Var, Any]], outputs, task:m.Task, engine=""):
+        self._install_batch_flush()
+
         cols = task.return_cols()
         if len(outputs) != len(cols):
             raise Exception(f"Expected {len(outputs)} outputs, got {len(cols)}")
+        rel_code = self.compiler.compile(task)
         emitted_inputs = [(name, self.compiler.emitter.emit(var), type) for (name, var, type) in inputs]
         outputs = list(zip(cols, outputs))
         if not engine:
             engine = self.get_engine_name()
+        params = ExportParams(
+            source_database=self._source_database,
+            database=self._database,
+            engine=engine,
+            func_name=name,
+            inputs=emitted_inputs,
+            out_fields=outputs,
+            code=rel_code,
+            dry_run=self.dry_run
+        )
+        self.resources.create_export(params)
+
+    def export_table(self, relation, name, cols, task:m.Task, engine="", refresh=""):
+        code = self.compiler.compile(task)
+        if not engine:
+            engine = self.get_engine_name()
         if not self.dry_run:
-            self.resources.create_export(self._database, engine, name, emitted_inputs, outputs, self.compiler.compile(task))
+            self.resources.create_export_table(self._database, engine, name, relation, cols, code, refresh=refresh)
```

### Comparing `relationalai-0.2.9/src/relationalai/clients/config.py` & `relationalai-0.3.0/src/relationalai/clients/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from copy import deepcopy
 import os
+import time
 from typing import Dict, Any
 from railib import config
 import configparser
 import toml
 import tomlkit
+import hashlib
 
 from relationalai.util.constants import DEFAULT_PROFILE_NAME, TOP_LEVEL_PROFILE_NAME
 
 #--------------------------------------------------
 # config defaults
 #--------------------------------------------------
 
@@ -475,14 +477,20 @@
     
     def items_with_dots(self):
         return items_with_dots(self.props)
     
     def __str__(self):
         return "\n".join(f"{k}: {map_toml_value(v)}" for k, v in self.items_with_dots())
 
+    def get_hash(self):
+        def hash_string(s: str):
+            return hashlib.md5(s.encode()).hexdigest()[:32]
+        user = self.get("user") if self.get("platform") == "snowflake" else self.get("client_id")
+        return hash_string((user or "") + str(time.time_ns()))
+
     def to_rai_config(self) -> Dict[str, Any]:
         return to_rai_config(self.props)
 
     def _fill_in_with_defaults(self, defaults: Dict[str, Any], **kwargs):
         props = {k: v for k, v in kwargs.items() if k in defaults}
         self.update({
             **defaults,
```

### Comparing `relationalai-0.2.9/src/relationalai/clients/test.py` & `relationalai-0.3.0/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/clients/types.py` & `relationalai-0.3.0/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/loaders/csv.py` & `relationalai-0.3.0/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/loaders/loader.py` & `relationalai-0.3.0/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/loaders/types.py` & `relationalai-0.3.0/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/std/aggregates.py` & `relationalai-0.3.0/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/std/graphs.py` & `relationalai-0.3.0/src/relationalai/std/graphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,35 +137,22 @@
         return (min, max)
 
     # --------------------------------------------------
     # Connectivity
     # --------------------------------------------------
 
     def is_connected(self):
-        model = self._graph.model
-        with model.ordered_choice() as v:
-            with model.scope():
-                self._lib.is_connected(self._graph)
-                v.add(True)
-            with model.scope():
-                v.add(False)
-        return v
+        return self._lib.is_connected(self._graph)
 
     def reachable_from(self, node: dsl.Producer) -> dsl.Expression:
-        return self._lib.transitive_closure(self._graph, unwrap(node))
+        reachable = self._lib.transitive_closure(self._graph, unwrap(node))
+        return self._lookup(reachable)
 
     def is_reachable(self, node1: dsl.Producer, node2: dsl.Producer) -> dsl.Expression:
-        model = self._graph.model
-        with model.ordered_choice() as v:
-            with model.scope():
-                self._lib.transitive_closure(self._graph, unwrap(node1), unwrap(node2))
-                v.add(True)
-            with model.scope():
-                v.add(False)
-        return v
+        return self._lib.transitive_closure(self._graph, unwrap(node1), unwrap(node2))
 
     # --------------------------------------------------
     # Triangles
     # --------------------------------------------------
 
     def num_triangles(self, node=None):
         if node is None:
@@ -228,28 +215,27 @@
     def adamic_adar(self, node1, node2):
         return self._lib.adamic_adar(self._graph, unwrap(node1), unwrap(node2))
 
     def preferential_attachment(self, node1, node2):
         return self._lib.preferential_attachment(self._graph, unwrap(node1), unwrap(node2))
 
     def common_neighbor(self, node1, node2):
-        return self._lib.common_neighbor(self._graph, unwrap(node1), unwrap(node2))
+        neighbor = self._lib.common_neighbor(self._graph, unwrap(node1), unwrap(node2))
+        return self._lookup(neighbor)
 
     # --------------------------------------------------
     # Similarity
     # --------------------------------------------------
 
     def cosine_similarity(self, node1, node2):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
         return self._lib.cosine_similarity(self._graph, unwrap(node1), unwrap(node2))
 
     def weighted_cosine_similarity(self, node1, node2):
-        if not self._graph.undirected:
-            invalid_param("graph", "must be undirected")
         return self._lib.weighted_cosine_similarity(self._graph, unwrap(node1), unwrap(node2))
 
     def jaccard_similarity(self, node1, node2):
         return self._lib.jaccard_similarity(self._graph, unwrap(node1), unwrap(node2))
 
     def weighted_jaccard_similarity(self, node1, node2):
         return self._lib.weighted_jaccard_similarity(self._graph, unwrap(node1), unwrap(node2))
@@ -304,15 +290,15 @@
             level_tolerance: float = 0.01,
             sweep_tolerance: float = 0.0001,
             teleportation_rate: float = 0.15,
             visit_rate_tolerance: float = 1e-15,
             randomization_seed: int | None = None,
     ):
         positive("max_levels", max_levels, type_=int)
-        positive("max_sweeps", max_sweeps, type_=int)
+        nonnegative("max_sweeps", max_sweeps, type_=int)
         nonnegative("level_tolerance", level_tolerance)
         nonnegative("sweep_tolerance", sweep_tolerance)
         positive("teleportation_rate", teleportation_rate)
         between("teleportation_rate", teleportation_rate, 0, 1)
         positive("visit_rate_tolerance", visit_rate_tolerance)
         _config_dict = {
             "graph": self._graph,
@@ -336,15 +322,15 @@
             max_levels: int = 4,
             max_sweeps: int = 8,
             level_tolerance: float = 0.01,
             sweep_tolerance: float = 0.0001,
             randomization_seed: int | None = None,
     ):
         positive("max_levels", max_levels, type_=int)
-        positive("max_sweeps", max_sweeps, type_=int)
+        nonnegative("max_sweeps", max_sweeps, type_=int)
         nonnegative("level_tolerance", level_tolerance)
         nonnegative("sweep_tolerance", sweep_tolerance)
         _config_dict = {
             "graph": self._graph,
             "max_levels": max_levels,
             "max_sweeps": max_sweeps,
             "level_tolerance": float(level_tolerance),
@@ -352,16 +338,16 @@
         }
         if randomization_seed is not None:
             positive("randomization_seed", randomization_seed, type_=int)
             _config_dict["randomization_seed"] = randomization_seed
         config = self._config(**_config_dict)
         return self._lib.louvain(config, unwrap(node))
 
-    def label_propagation(self, node, max_sweeps: int = 1000, randomization_seed: int | None = None):
-        positive("max_sweeps", max_sweeps, type_=int)
+    def label_propagation(self, node, max_sweeps: int = 20, randomization_seed: int | None = None):
+        nonnegative("max_sweeps", max_sweeps, type_=int)
         _config_dict = {
             "graph": self._graph,
             "max_sweeps": max_sweeps,
         }
         if randomization_seed is not None:
             positive("randomization_seed", randomization_seed, type_=int)
             _config_dict["randomization_seed"] = randomization_seed
@@ -434,22 +420,22 @@
         return self._props[__name]
 
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
 class Graph:
-    def __init__(self, model:dsl.Graph, undirected=False, weighted=False, default_weight=1.0, with_isolated_nodes=False):
+    def __init__(self, model:dsl.Graph, undirected=False, weighted=False, default_weight=1.0, with_isolated_nodes=True):
         self.model = model
         self.id = dsl.next_id()
         self.compute = Compute(self)
         self.Node = dsl.Type(model, "nodes", scope=f"graph{self.id}_")
         self.Edge = Edge(self)
-        self.undirected = undirected
-        self.weighted = weighted
+        self._undirected = undirected
+        self._weighted = weighted
         self.default_weight=default_weight
         self._last_fetch = None
 
         graph_type = "::graphlib::undirected_graph" if undirected else "::graphlib::directed_graph"
         if weighted:
             unwrapped = f"""
             def {self.Edge._prop("weight")._name}_unwrapped(au, bu, w): {{
@@ -502,14 +488,22 @@
 
     def _to_var(self):
         return getattr(rel, self._graph_ref())._to_var()
 
     def _is_weighted(self):
         return self.weighted
         # return self.edges._is_weighted()
+    
+    @property
+    def undirected(self):
+        return self._undirected
+
+    @property
+    def weighted(self):
+        return self._weighted
 
     #--------------------------------------------------
     # Fetch
     #--------------------------------------------------
 
     def fetch(self):
         code = []
@@ -587,14 +581,19 @@
         "arrow_color": "arrow_color",
     }
 
     def _visual_props(self, prop_def, metadata):
         for k, v in prop_def.items():
             if callable(v):
                 metadata[k] = v(metadata)
+        # For some reason, the existance of "id" in the metadata
+        # results in edges not getting displayed in the visualization,
+        # so we remove it.
+        if "id" in metadata:
+            del metadata["id"]
         return metadata
 
     def _visual_dict(self, style: dict, use_cache = False) -> dict:
         data = self._last_fetch if use_cache else None
         if not data:
             data = self.fetch()
         style = deepcopy(style)
@@ -635,14 +634,15 @@
         style = style if style is not None else {"node": {}, "edge": {}}
         vis = gv.vis if not three else gv.three
         graph_dict = self._visual_dict(style=style, use_cache=use_cache)
         # Use defaults for the following kwargs if not provided
         new_kwargs = {
             "node_label_data_source": "label",
             "edge_label_data_source": "label",
+            "show_edge_label": True,
             "edge_curvature": 0.4,
         } | kwargs
         fig = vis(graph_dict, **new_kwargs)
         return fig
 
 #--------------------------------------------------
 # Path
```

### Comparing `relationalai-0.2.9/src/relationalai/std/math.py` & `relationalai-0.3.0/src/relationalai/std/math.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/std/strings.py` & `relationalai-0.3.0/src/relationalai/std/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/tools/cli.py` & `relationalai-0.3.0/src/relationalai/tools/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,247 +1,68 @@
 #pyright: reportPrivateImportUsage=false
-from collections import defaultdict
-import functools
-import io
+import os
 import re
+import sys
+import rich
+import json
+import click
 import shlex
-from typing import Sequence, cast, Any, List
-from click.core import Context
-from click.formatting import HelpFormatter
 import requests
-
+from pathlib import Path
+from rich.table import Table
+from datetime import datetime
+from rich import box as rich_box
+from InquirerPy.base.control import Choice
+from .cli_controls import divider, Spinner
+from . import cli_controls as controls
 from relationalai.clients import azure
+from typing import Sequence, cast, Any, List
 from relationalai.errors import RelQueryError
 from relationalai.loaders.types import LoadType, UnsupportedTypeError
 from relationalai.loaders.csv import CSVLoader
 from relationalai.loaders.loader import Loader, rel_schema_to_type
-from relationalai.util.constants import (
-    DEFAULT_PROFILE_NAME,
-    PARTIAL_PROFILE_NAME,
-    TOP_LEVEL_PROFILE_NAME,
-)
-from relationalai.util.format import humanized_bytes, humanized_duration
 from ..clients.types import ImportSource, ImportSourceFile, ImportSourceTable
 from ..clients.client import ResourceProvider
-from .. import Resources
-import rich
-from rich.console import Console
-from rich import box as rich_box
-from rich.table import Table
 from ..tools import debugger as deb
 from ..clients import config, snowflake
+from relationalai.tools.cli_helpers import (
+    EMPTY_STRING_REGEX,
+    ENGINE_NAME_ERROR,
+    ENGINE_NAME_REGEX,
+    UUID,
+    RichGroup,
+    account_from_url,
+    coming_soon,
+    ensure_config,
+    exit_with_divider,
+    filter_profiles_by_platform,
+    format_row,
+    get_config, get_resource_provider,
+    issue_top_level_profile_warning,
+    show_dictionary_table,
+    show_engines,
+    show_imports,
+    show_transactions,
+    supports_platform,
+    unexpand_user_path,
+    validate_engine_name
+)
 from ..clients.config import (
     FIELD_PLACEHOLDER,
     CONFIG_FILE,
-    ConfigFile,
     ConfigStore,
     all_configs_including_legacy,
     get_from_snowflake_connections_toml,
     azure_default_props,
     map_toml_value,
     snowflake_default_props,
 )
-from InquirerPy.base.control import Choice
-from InquirerPy.validator import ValidationError
-
-import os
-import sys
-import click
-from pathlib import Path
-from .cli_controls import divider, Spinner
-from . import cli_controls as controls
-from datetime import datetime, timedelta
-
-#--------------------------------------------------
-# Constants
-#--------------------------------------------------
-
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
-ENGINE_SIZES = ["XS", "S", "M", "L", "XL"]
-PROFILE = None
-
-SNOWFLAKE = "Snowflake"
-AZURE = "Azure (Beta)"
-
-AZURE_ENVS = {
-    "Production": {
-        "host": "azure.relationalai.com",
-        "client_credentials_url": "https://login.relationalai.com/oauth/token"
-    },
-    "Early Access": {
-        "host": "azure-ea.relationalai.com",
-        "client_credentials_url": "https://login-ea.relationalai.com/oauth/token"
-    },
-    "Staging": {
-        "host": "azure-staging.relationalai.com",
-        "client_credentials_url": "https://login-staging.relationalai.com/oauth/token"
-    },
-    "Latest": {
-        "host": "azure-latest.relationalai.com",
-        "client_credentials_url": "https://login-latest.relationalai.com/oauth/token"
-    },
-}
-
-#--------------------------------------------------
-# Helpers
-#--------------------------------------------------
-
-@functools.cache
-def get_config(profile:str|None = None):
-    global PROFILE
-    return config.Config(profile or PROFILE)
-
-@functools.cache
-def get_resource_provider(platform:str|None=None, _cfg:config.Config|None = None) -> ResourceProvider:
-    cfg = _cfg or get_config()
-    provider = Resources(config=cfg)
-    return provider
-
-def supports_platform(*platform_names: str):
-    def decorator(cmd: click.Command):
-        setattr(cmd, "__available_platforms", platform_names)
-        cb = cmd.callback
-        assert cb
-        def checked(*args, **kwargs):
-            assert cmd.name
-            assert_command_available(cmd.name, command_available(cmd))
-            return cb(*args, **kwargs)
-
-        cmd.callback = checked
-        return cmd
-    return decorator
-
-def command_available(cmd: click.Command) -> bool:
-    available_platforms = getattr(cmd, "__available_platforms", ())
-    platform = get_config().get("platform", "")
-    return not available_platforms or not platform or platform in available_platforms
-
-def assert_command_available(name: str, available: bool, plural=False):
-    if not available:
-        platform = get_config().get("platform", "")
-        rich.print(f"[yellow]{name} {'are' if plural else 'is'} not available for {platform}")
-        divider()
-        sys.exit(1)
-
-def coming_soon():
-    rich.print("[yellow]This isn't quite ready yet, but it's coming soon!")
-    divider()
-    sys.exit(1)
-
-def issue_top_level_profile_warning():
-    rich.print("[yellow]Warning: Using a top-level profile is not recommended")
-    rich.print("[yellow]Consider naming the profile by adding \\[profile.<name>] to your raiconfig.toml file\n")
-    rich.print("[yellow]Example:")
-    rich.print("[yellow]\\[profile.default]")
-    rich.print("[yellow]platform = \"snowflake\"")
-    rich.print("[yellow]account = ...")
-    divider()
-
-def ensure_config(profile:str|None=None) -> config.Config:
-    cfg = get_config(profile)
-    if not cfg.file_path:
-        rich.print("[yellow bold]No configuration file found.")
-        rich.print("To create one, run: [green bold]rai init[/green bold]")
-        divider()
-        sys.exit(1)
-    return cfg
-
-#--------------------------------------------------
-# Validation
-#--------------------------------------------------
-
-EMPTY_STRING_REGEX = re.compile(r'^\S+$')
-ENGINE_NAME_REGEX = re.compile(r'^[a-zA-Z]\w{2,}$')
-ENGINE_NAME_ERROR = "Min 3 chars, start with letter, only letters, numbers, underscores allowed."
-
-def engine_name_validator(cfg:config.Config, name:str):
-    if not ENGINE_NAME_REGEX.match(name):
-        raise ValidationError(message=ENGINE_NAME_ERROR)
-
-    try:
-        provider = get_resource_provider(None, cfg)
-        engine = provider.get_engine(name)
-        if engine and provider.is_valid_engine_state(engine['state']):
-            raise ValidationError(message=f"Engine '{name}' already exists")
-        return True
-    except Exception as e:
-        raise ValidationError(message=f"{e}")
-
-def validate_engine_name(cfg:config.Config, name:str):
-    try:
-        return engine_name_validator(cfg, name)
-    except ValidationError as e:
-        return e.message
-
-#--------------------------------------------------
-# Custom help printer
-#--------------------------------------------------
-
-class RichGroup(click.Group):
-    def format_help(self, ctx: Context, formatter: HelpFormatter) -> None:
-        global PROFILE
-        # @NOTE: I couldn't find a sane way to access the --profile option from here, so insane it is.
-        if "--profile" in sys.argv:
-            ix = sys.argv.index("--profile") + 1
-            if ix < len(sys.argv):
-                PROFILE = sys.argv[ix]
-
-        profile = get_config().profile
-        if profile == TOP_LEVEL_PROFILE_NAME:
-            profile = "[yellow bold]None[/yellow bold]" if not get_config().get("platform", "") else "[ROOT]"
-
-        sio = io.StringIO()
-        console = Console(file=sio, force_terminal=True)
-        divider(console)
-        console.print("[bold]Welcome to [green]RelationalAI![/bold]")
-        console.print()
-        console.print("rai [magenta]\\[options][/magenta] [cyan]command[/cyan]")
-
-        console.print()
-        console.print(f"[magenta]--profile[/magenta][dim] - which config profile to use (current: [/dim][cyan]{profile}[/cyan][dim])")
-
-        unavailable_commands = []
-        groups = defaultdict(list)
-        for command in self.commands.keys():
-            if ":" in command:
-                group, _, _ = command.rpartition(":")
-                groups[group].append(command)
-            else:
-                groups[""].append(command)
-
-        console.print()
-        for command in groups[""]:
-            console.print(f"[cyan]{command}[/cyan][dim] - {self.commands[command].help}")
-
-        for group, commands in groups.items():
-            if not group:
-                continue
-
-            empty = True
-            for command in commands:
-                if command_available(self.commands[command]):
-                    if empty:
-                        empty = False
-                        console.print()
-
-                    console.print(f"[cyan]{command}[/cyan][dim] - {self.commands[command].help}")
-                else:
-                    unavailable_commands.append(command)
-
-        if unavailable_commands:
-            platform = get_config().get("platform", "")
-            console.print()
-            console.print(f"[yellow]Not available on {platform}[/yellow]")
-            console.print()
-            for command in unavailable_commands:
-                console.print(f"[dim yellow]{command} - {self.commands[command].help}")
-
-        divider(console)
-        formatter.write(sio.getvalue())
-        sio.close()
+from relationalai.tools.constants import AZURE, AZURE_ENVS, CONTEXT_SETTINGS, ENGINE_SIZES, SNOWFLAKE
+from relationalai.util.constants import DEFAULT_PROFILE_NAME, PARTIAL_PROFILE_NAME, TOP_LEVEL_PROFILE_NAME
+from packaging.version import Version
 
 #--------------------------------------------------
 # Custom Click Option and Argument Types
 #--------------------------------------------------
 
 ImportOption = tuple[list[str], str]
 
@@ -309,33 +130,14 @@
     cfg.fill_in_with_azure_defaults(
         client_id=client_id,
         client_secret=client_secret,
         host=host if host else None,
         client_credentials_url=client_credentials_url if client_credentials_url else None
     )
 
-def unexpand_user_path(path):
-    """Inverse of os.path.expanduser"""
-    home_dir = os.path.expanduser('~')
-    if path.startswith(home_dir):
-        return '~' + path[len(home_dir):]
-    return path
-
-def account_from_url(account_or_url:str):
-    regex = r"https://app.snowflake.com/([^/]+)/([^/]+)/?.*"
-    match = re.match(regex, account_or_url)
-    if match:
-        org = match.group(1)
-        account = match.group(2)
-        return f"{org}-{account}"
-    elif "app.snowflake.com" in account_or_url or "https://" in account_or_url:
-        raise ValueError("URL not of the form https://app.snowflake.com/[org]/[account]")
-    else:
-        return account_or_url
-
 def snowflake_flow(cfg:config.Config):
     pyrel_config = check_original_config_flow(cfg, "snowflake")
     if not pyrel_config:
         check_snowflake_connections_flow(cfg)
 
     # get account info
     user = controls.text(
@@ -377,26 +179,14 @@
     # setup the default config
     cfg.fill_in_with_snowflake_defaults(
         user=user,
         password=password,
         account=account,
     )
 
-def filter_profiles_by_platform(config:ConfigFile, platform:str):
-    filtered_config = {}
-    for profile, props in config.get_combined_profiles().items():
-        if profile == TOP_LEVEL_PROFILE_NAME:
-            continue
-        if props.get("platform") == platform or (
-            props.get("platform") is None
-            and platform == "azure"
-        ):
-            filtered_config[profile] = props
-    return filtered_config
-
 def check_original_config_flow(cfg:config.Config, platform:str):
     all_profiles = {}
     for config_file in all_configs_including_legacy():
         file_path = config_file.path
         plt_config = filter_profiles_by_platform(config_file, platform)
         for profile, props in plt_config.items():
             profile_id = (profile, file_path)
@@ -479,37 +269,44 @@
     provider.reset()
 
 def spcs_flow(provider: ResourceProvider, cfg: config.Config):
     role_flow(provider, cfg)
     warehouse_flow(provider, cfg)
     rai_app_flow(provider, cfg)
 
-def engine_flow(provider:ResourceProvider, cfg:config.Config):
-    if provider.config.get("platform") == "snowflake":
-        app_name = cfg.get("rai_app_name", None)
-        if not app_name:
-            rich.print("[yellow]App name is required for engine selection. Skipping step.\n")
-            raise Exception("App name is required for engine selection")
-        warehouse = cfg.get("warehouse", None)
-        if not warehouse:
-            rich.print("[yellow]Warehouse is required for engine selection. Skipping step.\n")
-            raise Exception("Warehouse is required for engine selection")
+def create_engine(cfg:config.Config, **kwargs):
+    provider = get_resource_provider(None, cfg)
+    prompt = kwargs.get("prompt", "Select an engine:")
     result = controls.fuzzy_with_refetch(
-        "Select an engine:",
+        prompt,
         "engines",
         lambda: ["[CREATE A NEW ENGINE]"] + [engine.get("name") for engine in provider.list_engines()],
         default=cfg.get("engine", None),
     )
     if not result or isinstance(result, Exception):
         raise Exception("Error fetching engines")
     else:
         engine = result
     if result == "[CREATE A NEW ENGINE]":
         engine = create_engine_flow(cfg)
         rich.print("")
+    return engine
+
+def engine_flow(provider:ResourceProvider, cfg:config.Config, **kwargs):
+    if provider.config.get("platform") == "snowflake":
+        app_name = cfg.get("rai_app_name", None)
+        if not app_name:
+            rich.print("[yellow]App name is required for engine selection. Skipping step.\n")
+            raise Exception("App name is required for engine selection")
+        warehouse = cfg.get("warehouse", None)
+        if not warehouse:
+            rich.print("[yellow]Warehouse is required for engine selection. Skipping step.\n")
+            raise Exception("Warehouse is required for engine selection")
+    prompt = kwargs.get("prompt", "Select an engine:")
+    engine = create_engine(cfg, prompt=prompt)
     cfg.set("engine", engine or FIELD_PLACEHOLDER)
 
 def gitignore_flow():
     current_dir = Path.cwd()
     prev_dir = None
     while current_dir != prev_dir:
         gitignore_path = current_dir / '.gitignore'
@@ -550,22 +347,24 @@
             return name_profile_flow(cfg)
     return profile
 
 def save_flow(cfg:config.Config):
     config_store = ConfigStore()
     if cfg.profile != PARTIAL_PROFILE_NAME and cfg.profile in config_store.get_profiles():
         if not controls.confirm(f"Overwrite existing {cfg.profile} profile"):
+            rich.print()
             profile_name = controls.text("Profile name:")
             if profile_name:
                 cfg.profile = profile_name
             else:
                 save_flow(cfg)
                 return
     config_store.add_profile(cfg)
     if cfg.profile != PARTIAL_PROFILE_NAME:
+        rich.print()
         if config_store.num_profiles() == 1 or controls.confirm("Activate this profile?"):
             config_store.change_active_profile(cfg.profile)
     config_store.save()
 
 def init_flow():
     cfg = config.Config(fetch=False)
     try:
@@ -636,23 +435,21 @@
 def profile_switch(profile:str|None=None):
     config_store = ConfigStore()
     profiles = list(config_store.get_profiles().keys())
     divider()
     if not profile:
         if len(profiles) == 0:
             rich.print("[yellow]No profiles found")
-            divider()
-            sys.exit(1)
+            exit_with_divider()
         profile = controls.fuzzy("Select a profile:", profiles)
         divider()
     else:
         if profile not in profiles:
             rich.print(f"[yellow]Profile '{profile}' not found")
-            divider()
-            sys.exit(1)
+            exit_with_divider()
     config_store.change_active_profile(profile)
     config_store.save()
     rich.print(f"[green]✓ Switched to profile '{profile}'")
     divider()
 
 #--------------------------------------------------
 # Explain config
@@ -725,17 +522,25 @@
     name="config:check",
     help="Check whether config is valid",
 )
 def config_check(all_profiles:bool=False):
     divider()
     if ConfigStore().get("platform"):
         issue_top_level_profile_warning()
-    ensure_config()
+    cfg = ensure_config()
     with Spinner("Connecting to platform...", "Connection successful!", "Error:"):
-        get_resource_provider().list_engines()
+        provider = get_resource_provider(None, cfg)
+        # Engine is required by both clients if it is not configured check would fail already
+        engine_name = cfg.get("engine")
+        # This essentially checks if the profile is valid since we are connecting to get the engine
+        engine = provider.get_engine(engine_name)
+        if not engine:
+            raise Exception(f"Configured engine '{engine_name}' not found")
+        if not provider.is_valid_engine_state(engine.get("state")):
+            raise Exception(f"Engine '{engine_name}' is in an invalid state: '{engine.get('state')}'")
     divider()
 
 #--------------------------------------------------
 # Version
 #--------------------------------------------------
 
 def latest_version(package_name):
@@ -752,15 +557,15 @@
 @cli.command(help="Print version info")
 def version():
     from .. import __version__
     from railib import __version__ as railib_version
 
     table = Table(show_header=False, border_style="dim", header_style="bold", box=rich_box.SIMPLE)
     def print_version(name, version, latest=None):
-        if latest is not None and version != latest:
+        if latest is not None and Version(version) < Version(latest):
             table.add_row(f"[bold]{name}[red]", f"[red bold]{version} → {latest}")
         else:
             table.add_row(f"[bold]{name}", f"[green]{version}")
 
     divider()
     print_version("RelationalAI", __version__, latest_version("relationalai"))
     print_version("Rai-sdk", railib_version, latest_version("rai-sdk"))
@@ -769,43 +574,43 @@
     try:
         cfg = get_config()
         if not cfg.file_path:
             table.add_row("[bold]App", "No configuration file found. To create one, run: [green]rai init")
         else:
             platform = cfg.get("platform", None)
             if platform == "snowflake":
-                # print()
                 with Spinner("Checking app version"):
                     try:
                         app_version = get_resource_provider().get_version()
                     except Exception as e:
                         rich.print(f"\n\n[yellow]Error fetching app version: {e}")
-                        exit(1)
+                        exit_with_divider(1)
                 print_version("App", app_version)
 
     except Exception as e:
         rich.print(f"[yellow]Error checking app version: {e}")
-        divider()
-        exit(1)
+        exit_with_divider(1)
 
     rich.print(table)
     divider()
 
 #--------------------------------------------------
 # Debugger
 #--------------------------------------------------
 
 @cli.command(help="Open the RAI debugger")
 @click.option("--host", help="Host to use", default="0.0.0.0")
 @click.option("--port", help="Port to use", default=8080)
 @click.option("--new", help="Use the new debugger", is_flag=True, default=False)
-def debugger(host, port, new):
+@click.option("--profile", help="Profile to use", default=None)
+
+def debugger(host, port, new, profile):
     if new:
         from relationalai.tools import debugger_server
-        debugger_server.start_server(host, port)
+        debugger_server.start_server(host, port, profile)
     else:
         deb.main(host, port)
 
 #--------------------------------------------------
 # Engine list
 #--------------------------------------------------
 
@@ -815,57 +620,48 @@
     divider(flush=True)
     ensure_config()
     with Spinner("Fetching engines"):
         try:
             engines = get_resource_provider().list_engines(state)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching engines: {e}")
-            exit(1)
+            exit_with_divider(1)
 
     if len(engines):
-        table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
-        table.add_column("Name")
-        table.add_column("Size")
-        table.add_column("State")
-        for engine in engines:
-            table.add_row(engine.get("name"), engine.get("size"), engine.get("state"))
-        rich.print(table)
+        show_engines(engines)
     else:
         rich.print("[yellow]No engines found")
-
     divider()
 
 @cli.command(name="engines:get", help="Get engine details")
 @click.option("--name", help="Name of the engine")
-def engines_get(name):
+def engines_get(name:str|None=None):
     divider(flush=True)
     ensure_config()
 
     if not name:
         name = controls.text("Engine name:", validator=ENGINE_NAME_REGEX.match, invalid_message=ENGINE_NAME_ERROR)
         rich.print("")
 
     with Spinner("Fetching engine"):
         try:
             engine = get_resource_provider().get_engine(name)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching engine: {e}")
-            divider(flush=True)
-            exit(1)
+            exit_with_divider(1)
 
     if engine:
         table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
         table.add_column("Name")
         table.add_column("Size")
         table.add_column("State")
         table.add_row(engine.get("name"), engine.get("size"), engine.get("state"))
         rich.print(table)
     else:
-        rich.print("[yellow]Engine not found")
-
+        rich.print(f'[yellow]Engine "{name}" not found')
     divider()
 
 #--------------------------------------------------
 # Engine create
 #--------------------------------------------------
 
 def create_engine_flow(cfg:config.Config, name=None, size=None, pool=None):
@@ -977,26 +773,26 @@
         if not name or isinstance(name, Exception):
             return
     else:
         try:
             engine = provider.get_engine(name)
             if not engine:
                 rich.print(f"[yellow]Engine '{name}' not found")
-                divider()
-                return
+                exit_with_divider(1)
         except Exception as e:
             rich.print(f"[yellow]Error fetching engine: {e}")
-            divider()
-            return
+            exit_with_divider(1)
 
-    with Spinner(f"Deleting '{name}' engine", f"Engine '{name}' deleted!"):
+    with Spinner(f"Deleting '{name}' engine", f"Engine '{name}' deleted!", "Error:"):
         try:
             provider.delete_engine(name)
         except Exception as e:
-            rich.print(f"\n\n[yellow]Error deleting engine: {e}")
+            if "SETUP_CDC" in f"{e}":
+                raise Exception("[yellow]Imports are setup to utilize this engine.\nUse '[cyan]rai imports:setup --engine[/cyan]' to set a different engine for imports.")
+            raise e
     divider()
 
 #--------------------------------------------------
 # Import Source flows
 #--------------------------------------------------
 
 def import_source_flow(provider: ResourceProvider) -> Sequence[ImportSource]:
@@ -1013,41 +809,41 @@
         try:
             dbs = provider.list_databases()
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching databases: {e}")
             dbs = []
     if len(dbs) == 0:
         rich.print("[yellow]No databases found")
-        exit(1)
+        exit_with_divider()
     rich.print()
     db = controls.fuzzy("Select a database:", [db["name"] for db in dbs])
     rich.print()
 
     with Spinner("Fetching schemas", "Schemas fetched"):
         try:
             schemas = provider.list_sf_schemas(db)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching schemas: {e}")
             schemas = []
     if len(schemas) == 0:
         rich.print("[yellow]No schemas found")
-        exit(1)
+        exit_with_divider()
     rich.print()
     schema = controls.fuzzy("Select a schema:", [s["name"] for s in schemas])
     rich.print()
 
     with Spinner("Fetching tables", "Tables fetched"):
         try:
             tables = provider.list_tables(db, schema)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching tables: {e}")
             tables = []
     if len(tables) == 0:
         rich.print("[yellow]No tables found")
-        exit(1)
+        exit_with_divider()
     rich.print()
     if tables:
         tables = controls.fuzzy("Select tables (tab for multiple):", [t["name"] for t in tables], multiselect=True)
     else:
         rich.print("[yellow]No tables found")
         tables = ""
     rich.print()
@@ -1141,122 +937,283 @@
 
     saved_args = " " + " ".join(saved_args) if saved_args else ""
     print()
     rich.print(message)
     print()
     rich.get_console().print(f"[dim]    rai {prev_cmd_args}{saved_args}[/dim] {solution_args}", highlight=False)
     divider()
-    sys.exit(0)
+    exit(0)
 
 
 def parse_source(provider: ResourceProvider, raw: str) -> Sequence[ImportSource]:
     if provider.platform == "azure":
         return [ImportSourceFile(raw)]
     elif provider.platform == "snowflake":
         parts = raw.split(".")
         assert len(parts) == 3, "Snowflake table imports must be in `database.schema.table` format"
         return [ImportSourceTable(*parts)]
     else:
         raise Exception(f"Unsupported platform: {provider.platform}")
 
 #--------------------------------------------------
-# Imports list
+# Imports
 #--------------------------------------------------
 
-@cli.command(name="imports:list", help="List objects imported into RAI")
-@click.option("--model", help="Model")
-def imports_list(model):
+@supports_platform("snowflake")
+@cli.command(name="imports:setup", help="Modify and view imports setup")
+@click.option("--engine", help="The engine name to set for imports")
+@click.option("--resume", help="Resume imports", is_flag=True)
+@click.option("--suspend", help="Suspend imports", is_flag=True)
+def imports_setup(engine:str|None=None, resume:bool=False, suspend:bool=False):
     divider(flush=True)
-    ensure_config()
+    cfg = ensure_config()
     provider = get_resource_provider()
+    data = None
+    is_engine_set = True
 
-    if not model:
-        with Spinner("Fetching models", "Models fetched"):
-            try:
-                models = [model["name"] for model in provider.list_graphs()]
-            except Exception as e:
-                rich.print(f"\n\n[yellow]Error fetching models: {e}")
-                exit(1)
-        if len(models) == 0:
-            rich.print("[yellow]No models found")
-            exit(1)
+    if resume or suspend:
+        if resume:
+            with Spinner("Resuming imports", "Imports resumed", "Error:"):
+                provider.change_imports_status(suspend=False)
+        if suspend:
+            with Spinner("Suspending imports", "Imports suspended", "Error:"):
+                provider.change_imports_status(suspend=True)
+        exit_with_divider()
+
+    # Passed in engine
+    if engine:
+        with Spinner("Validating engine", "Engine validated", "Error:"):
+                ve = provider.get_engine(engine)
         rich.print()
-        model = controls.fuzzy("Select a model:", models)
+        if not ve:
+            rich.print(f"[yellow]Engine[/yellow] '{engine}' [yellow]is invalid.[/yellow]\nPlease use '[cyan]rai engines:create[/cyan]' to create a valid engine.")
+            exit_with_divider()
+        else:
+            set_imports_engine(ve.get("name"))
+            exit_with_divider()
+
+    # Verify imports setup
+    with Spinner("Fetching imports setup", "Imports setup fetched", "Error:"):
+        try:
+            data = provider.get_imports_status()
+        except Exception as e:
+            if "SETUP_CDC" in f"{e}":
+                is_engine_set = False
+            else:
+                raise e
+    if not is_engine_set:
         rich.print()
+        engine = create_engine(cfg, prompt="Select an engine for imports:")
+        set_imports_engine(engine)
+        exit_with_divider()
 
-    with Spinner(f"Fetching imports for {model}", "Imports fetched"):
+    # Engine is already set for imports
+    if data:
+        rich.print()
+        if data["status"].lower() == "suspended":
+            rich.print("To resume imports, use '[cyan]rai imports:setup --resume[/cyan]'")
+        else:
+            rich.print("To suspend imports, use '[cyan]rai imports:setup --suspend[/cyan]'")
         try:
-            imports = provider.list_imports(model)
+            rich.print()
+            with Spinner("Validating imports engine", "Imports engine validated", "Error:"):
+                engine = provider.get_engine(data["engine"])
+            if not engine:
+                rich.print()
+                rich.print(f'[yellow]Previously set imports engine[/yellow] "{data["engine"]}" [yellow]is invalid.[/yellow]')
+                rich.print()
+                engine = create_engine(cfg, prompt="Select an engine for imports:")
+                set_imports_engine(engine)
+                exit_with_divider()
+            data = {**data, **json.loads(data["info"])}
+            del data["info"]
+            del data["state"]
+            data["status"] = data["status"].upper()
+            data["createdOn"] = datetime.strptime(data["createdOn"], '%Y-%m-%d %H:%M:%S.%f %z')
+            data["lastSuspendedOn"] = datetime.strptime(data["lastSuspendedOn"], '%Y-%m-%d %H:%M:%S.%f %z') if data["lastSuspendedOn"] else "N/A"
+            show_dictionary_table(
+                data,
+                lambda k, v: {k: v, "style": "red"} if k == "engine" and not engine else format_row(k, v)
+            )
         except Exception as e:
-            rich.print(f"\n\n[yellow]Error fetching imports: {e}")
-            imports = []
+            rich.print(f"\n\n[yellow]Error fetching imports setup: {e}")
+    divider()
 
-    rich.print()
-    if len(imports):
-        table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
-        cols = {"Import": "name"}
-        if len(imports) and "type" in imports[0]:
-            cols["Type"] = "type"
-        if len(imports) and "id" in imports[0]:
-            cols["ID"] = "id"
-        if len(imports) and "status" in imports[0]:
-            cols["Status"] = "status"
+def set_imports_engine(name:str|None=None):
+    cfg = ensure_config()
+    provider = get_resource_provider()
+    if not name:
+        name = controls.fuzzy_with_refetch(
+            "Select an engine for imports:",
+            "engines",
+            lambda: [engine["name"] for engine in provider.list_engines()],
+            not_found_message="No valid engines found."
+        )
+        if not name or isinstance(name, Exception):
+            if not name:
+                confirm = controls.confirm("Would you like to create a new engine for imports?", default=True)
+                if confirm:
+                    rich.print()
+                    name = create_engine_flow(cfg)
+                    rich.print()
+                else:
+                    return
+            else:
+                return
+    with Spinner("Setting imports engine", "Imports engine set to [cyan]'"+name+"'[/cyan]", "Error:"):
+        provider.set_imports_engine(name)
 
-        for label in cols.keys():
-            table.add_column(label)
+@supports_platform("snowflake")
+@cli.command(name="imports:get", help="Get specific import details")
+@click.option("--id", help="Filter by import id")
+def imports_get(id:str|None=None):
+    divider(flush=True)
+    ensure_config()
+    provider = get_resource_provider()
+    import_data = []
+    if id is None:
+        with Spinner("Fetching imports", "Imports fetched", "Error:"):
+            imports = provider.list_imports()
 
-        for imp in imports:
-            table.add_row(*[imp.get(attr, None) for attr in cols.values()])
-        rich.print(table)
-    else:
+    if not imports:
+        rich.print()
         rich.print("[yellow]No imports found")
+        exit_with_divider()
+
+    show_imports(imports, showId=True)
+    id = controls.fuzzy("Select an import id:", [i["id"] for i in imports], show_index=True)
+    obj = [{"name": item['name'], "model": item['model']} for item in imports if item['id'] == id][0]
+
+    rich.print()
+    with Spinner("Fetching import", "Import fetched", "Error:"):
+        import_data = provider.get_import_stream(obj.get("name"), obj.get("model"))
+    if len(import_data) > 0:
+        rich.print()
+        show_dictionary_table(import_data[0], format_row)
+    divider()
+
+#--------------------------------------------------
+# Imports list
+#--------------------------------------------------
+
+@cli.command(name="imports:list", help="List objects imported into RAI")
+@click.option("--id", help="Filter by import id")
+@click.option("--name", help="Filter by import name")
+@click.option("--model", help="Filter by model")
+@click.option("--status", help="Filter by import status")
+@click.option("--creator", help="Filter by import creator")
+def imports_list(id:str|None=None, name:str|None=None, model:str|None=None, status:str|None=None, creator:str|None=None):
+    divider(flush=True)
+    ensure_config()
+    provider = get_resource_provider()
+    data = None
+    with Spinner("Fetching imports config", "Imports config fetched", "Error:"):
+        try:
+            data = provider.get_imports_status()
+        except Exception as e:
+            if "SETUP_CDC" in f"{e}":
+                raise Exception("Imports are not configured.\n[yellow]To start use '[cyan]rai imports:setup[/cyan]' to set up an engine for imports.")
+            raise e
+    if data:
+        rich.print()
+        ds = f"[red]{data['status'].upper()}[/red]" if data["status"].lower() == "suspended" else data["status"].upper()
+        rich.print(f"Imports status: {ds}")
+
+    imports = None
+    rich.print()
+    with Spinner("Fetching imports", "Imports fetched", "Error:"):
+        imports = provider.list_imports(id, name, model, status, creator)
+
+    if imports is None:
+        exit_with_divider()
 
+    rich.print()
+    show_imports(imports)
     divider()
 
 #--------------------------------------------------
 # Imports stream
 #--------------------------------------------------
 
 @supports_platform("snowflake")
 @cli.command(name="imports:stream", help="Stream an object into RAI")
 @click.option("--source", help="Source")
 @click.option("--model", help="Model")
 @click.option("--rate", help="Rate")
+@click.option("--resume", help="Name of the import to resume")
+@click.option("--suspend", help="Name of the import to suspend")
 @click.argument('options', nargs=-1, type=ImportOptionsType())
-def imports_stream(source, model, rate, options):
+def imports_stream(source, model, rate, resume: None, suspend: None, options):
     divider(flush=True)
     ensure_config()
     provider = get_resource_provider()
     default_options = ImportOptionsType.reduce(options)
 
+    # Resume or suspend import stream
+    if resume or suspend:
+        import_name = resume if resume else suspend
+        is_suspend = True if suspend else False
+        with Spinner("Acquiring import", "Import stream fetched", "Error:"):
+            stream = provider.list_imports(name=import_name)
+        if not stream:
+            rich.print()
+            rich.print(f"[yellow]Import '{import_name}' not found")
+            exit_with_divider()
+        rich.print()
+        with Spinner(
+            f"{'Resume' if resume else 'Suspend'}ing import stream",
+            f"Import stream {'resumed' if resume else 'suspended'}",
+            "Error:"
+        ):
+            provider.change_stream_status(import_name, model=stream[0]["model"], suspend=is_suspend)
+        exit_with_divider()
+
+    # Model/database selection & validation
     if not model:
         with Spinner("Fetching models", "Models fetched"):
             try:
-                models = [model["name"] for model in provider.list_graphs()]
+                models = ["[CREATE MODEL]"] + [model["name"] for model in provider.list_graphs()]
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching models: {e}")
-                exit(1)
-        if len(models) == 0:
-            rich.print("[yellow]No models found")
-            exit(1)
+                exit_with_divider(1)
         rich.print()
         model = controls.fuzzy("Select a model:", models)
+        if model == "[CREATE MODEL]":
+            model = controls.text("Model name:")
+            rich.print()
+            with Spinner("Creating model", "Model created"):
+                provider.create_graph(model)
         rich.print()
+    else:
+        db = provider.get_database(model)
+        if not db:
+            with Spinner("Creating model", "Model created"):
+                provider.create_graph(model)
+
+    try:
+        sources = parse_source(provider, source) if source else import_source_flow(provider)
+    except Exception as e:
+        rich.print(f"[yellow]Error: {e}")
+        exit_with_divider(1)
 
-    sources = parse_source(provider, source) if source else import_source_flow(provider)
     for import_source in sources:
         try:
             options = import_source_options_flow(provider, import_source, default_options)
             with Spinner(f"Creating stream for {import_source.name}", f"Stream for {import_source.name} created"):
                 provider.create_import_stream(import_source, model, rate, options=options)
         except UnsupportedTypeError as err:
             rich.print(f"\n\n[yellow]The [bold]{provider.platform}[/bold] integration doesn't support streaming from [bold]'{err.type}'[/bold] sources.")
         except Exception as e:
-            rich.print(f"\n[yellow]Error creating stream: {e}")
-
+            if "use setup_cdc()" in f"{e}":
+                rich.print("\n\n[yellow]Imports are not configured.\n[yellow]To start use '[cyan]rai imports:setup[/cyan]' to set up an engine for imports.")
+            elif "stream already exists" in f"{e}":
+                rich.print(f"\n\n[yellow]Stream [cyan]'{import_source.name.upper()}'[/cyan] already exists.")
+            else:
+                rich.print()
+                rich.print(f"\n[yellow]Error creating stream: {e}")
     divider()
 
 #--------------------------------------------------
 # Imports snapshot
 #--------------------------------------------------
 
 @supports_platform("azure")
@@ -1275,18 +1232,18 @@
 
     if not model:
         with Spinner("Fetching models", "Models fetched"):
             try:
                 models = [model["name"] for model in provider.list_graphs()]
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching models: {e}")
-                exit(1)
+                exit_with_divider(1)
         if len(models) == 0:
             rich.print("[yellow]No models found")
-            exit(1)
+            exit_with_divider()
         rich.print()
         model = controls.fuzzy("Select a model:", models)
         rich.print()
 
     sources = parse_source(provider, source) if source else import_source_flow(provider)
     for import_source in sources:
         try:
@@ -1296,117 +1253,113 @@
                 provider.create_import_snapshot(import_source, model, options=options)
         except UnsupportedTypeError as err:
             rich.print(f"\n\n[yellow]The [bold]{provider.platform}[/bold] integration doesn't support loading [bold]'{err.type}'[/bold] files.")
         except RelQueryError as e:
             rich.print(f"\n\n[yellow]Error creating snapshot: {e.pprint()}")
         except Exception as e:
             rich.print(f"\n\n[yellow]Error creating snapshot: {e}")
-
-
     divider()
 
 #--------------------------------------------------
 # Imports delete
 #--------------------------------------------------
 
 @cli.command(name="imports:delete", help="Delete an import from RAI")
 @click.option("--object", help="Object")
 @click.option("--model", help="Model")
 def imports_delete(object, model):
     divider(flush=True)
     ensure_config()
     provider = cast(snowflake.Resources, get_resource_provider())
-
     if not model:
         with Spinner("Fetching models", "Models fetched"):
             try:
                 models = [model["name"] for model in provider.list_graphs()]
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching models: {e}")
-                exit(1)
+                exit_with_divider(1)
         if len(models) == 0:
+            rich.print()
             rich.print("[yellow]No models found")
-            exit(1)
+            exit_with_divider()
         rich.print()
         model = controls.fuzzy("Select a model:", models)
         rich.print()
 
     with Spinner(f"Fetching imports for {model}", "Imports fetched"):
         try:
             imports = provider.list_imports(model)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching imports: {e}")
-            exit(1)
+            exit_with_divider(1)
 
     if not imports:
         rich.print()
         rich.print("[yellow]No imports to delete")
+        rich.print()
     if object:
         objects = [object]
     else:
         if len(imports) == 0:
             rich.print("[yellow]No imports found")
-            exit(1)
+            exit_with_divider()
         rich.print()
         objects = controls.fuzzy("Select objects (tab for multiple):", [t["name"] for t in imports], multiselect=True)
         rich.print()
 
     for object in objects:
         with Spinner(f"Removing {object}", f"{object} removed"):
             try:
                 provider.delete_import(object, model)
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error deleting import: {e}")
-
     divider()
 
 #--------------------------------------------------
 # Exports list
 #--------------------------------------------------
 
 @supports_platform("snowflake")
 @cli.command(name="exports:list", help="List objects exported out of RAI")
 @click.option("--model", help="Model")
 def exports_list(model):
     divider(flush=True)
     ensure_config()
     provider = cast(snowflake.Resources, get_resource_provider())
     coming_soon()
-
     if not model:
         with Spinner("Fetching models", "Models fetched"):
             try:
                 models = [model["name"] for model in provider.list_graphs()]
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching models: {e}")
-                exit(1)
+                exit_with_divider(1)
         if len(models) == 0:
             rich.print("[yellow]No models found")
-            exit(1)
+            exit_with_divider()
         rich.print()
         model = controls.fuzzy("Select a model:", models)
         rich.print()
 
     with Spinner(f"Fetching exports for {model}", "Exports fetched"):
         try:
             exports = provider.list_exports(model, "")
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching exports: {e}")
-            exit(1)
+            exit_with_divider(1)
 
     rich.print()
     if len(exports):
         table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
         table.add_column("Object")
         for imp in exports:
             table.add_row(imp.get("name"))
         rich.print(table)
     else:
         rich.print("[yellow]No exports found")
-
     divider()
 
 #--------------------------------------------------
 # Exports delete
 #--------------------------------------------------
 
 @supports_platform("snowflake")
@@ -1414,162 +1367,68 @@
 @click.option("--export", help="export")
 @click.option("--model", help="Model")
 def exports_delete(export, model):
     divider(flush=True)
     ensure_config()
     provider = cast(snowflake.Resources, get_resource_provider())
     coming_soon()
-
     if not model:
         with Spinner("Fetching models", "Models fetched"):
             try:
                 models = [model["name"] for model in provider.list_graphs()]
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching models: {e}")
-                exit(1)
+                exit_with_divider(1)
         if len(models) == 0:
             rich.print("[yellow]No models found")
-            exit(1)
+            exit_with_divider()
         rich.print()
         model = controls.fuzzy("Select a model:", models)
         rich.print()
 
     # @FIXME It seems like we should just fuzzy list exports but this was the original behavior
     source_names = [export] if export else [source.name for source in import_source_flow(provider)]
     for source_name in source_names:
         with Spinner(f"Removing {source_name}", f"{source_name} removed"):
             try:
                 provider.delete_export(model, "", source_name)
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error deleting export: {e}")
-
     divider()
 
 #--------------------------------------------------
 # Transactions get
 #--------------------------------------------------
 
-def get_color_by_transaction_state(state:str) -> str:
-    match state.lower():
-        case "aborted":
-            return "red"
-        case "completed":
-            return "white"
-        case "created" | "running" | "cancelling":
-            return "bold yellow"
-        case _:
-            return ""
-
-def show_transaction_table(dict):
-    table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
-    table.add_column("Field")
-    table.add_column("Value")
-    for key, value in dict.items():
-        style = get_color_by_transaction_state(value) if key == "state" else ""
-
-        if key == "query_size" and isinstance(value, int):
-            value = humanized_bytes(value)
-
-        match value:
-            case None:
-                val = "N/A"
-            case int():
-                val = f"{value}"
-            case float():
-                val = f"{value}"
-            case list():
-                val = ", ".join(value)
-            case bool():
-                val = f"{value}"
-            case datetime():
-                val = value.strftime("%Y-%m-%d %H:%M:%S")
-            case timedelta():
-                val = humanized_duration(value.total_seconds() * 1000)
-            case _:
-                val = value
-        table.add_row(key, val, style=style)
-    rich.print(table)
-
 @cli.command(name="transactions:get", help="Get transaction details")
 @click.option("--id", help="Transaction id")
 def transactions_get(id):
     divider()
     ensure_config()
     provider = get_resource_provider()
     transaction = None
-
     if not id:
-        id = controls.text("Transaction id:")
+        id = controls.text("Transaction id:", mandatory=True, validator=UUID.match, invalid_message="Invalid transaction id")
         rich.print("")
 
     with Spinner("Fetching transaction", "Transaction fetched"):
         try:
             transaction = provider.get_transaction(id)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching transaction: {e}")
-            divider()
-            exit(1)
-
+            exit_with_divider(1)
     rich.print()
-
     if transaction:
-        show_transaction_table(transaction)
-
+        show_dictionary_table(transaction, format_row)
     divider()
 
 #--------------------------------------------------
 # Transactions list
 #--------------------------------------------------
 
-def show_transactions(transactions, limit, all_users):
-    config = ensure_config()
-    provider = get_resource_provider()
-    platform = provider.config.get("platform", "snowflake")
-    if len(transactions):
-        table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
-        table.add_column("ID")
-        table.add_column("Schema")
-        table.add_column("State")
-        table.add_column("Created")
-        table.add_column("Duration", justify="right")
-
-        added = 0
-        for txn in transactions:
-            if platform == "snowflake":
-                if (
-                    not all_users
-                    and txn.get("created_by", "").lower()
-                    != cast(str, config.get("user", "")).lower()
-                ):
-                    continue
-            if added >= limit:
-                break
-
-            state = txn.get("state", "")
-            duration = txn.get("duration")
-            created_on = txn.get("created_on")
-
-            if isinstance(created_on, int):
-                created_on = datetime.fromtimestamp(created_on / 1000)
-            if duration is None:
-                duration = (datetime.now(created_on.tzinfo) - created_on).total_seconds() * 1000
-
-            table.add_row(
-                txn.get("id"),
-                txn.get("database"),
-                state,
-                created_on.strftime("%Y-%m-%d %H:%M:%S"),
-                humanized_duration(duration),
-                style=get_color_by_transaction_state(state)
-            )
-            added += 1
-        rich.print(table)
-    else:
-        rich.print("[yellow]No transactions found")
-
 @cli.command(name="transactions:list", help="List transactions")
 @click.option("--id", help="Filter by transaction id", type=str)
 @click.option("--state", help="Filter by transaction state", type=str)
 @click.option("--limit", default=20, help="Limit")
 @click.option("--all-users", is_flag=True, default=False, help="Show transactions from all users")
 def transactions_list(id, state, limit, all_users):
     divider()
@@ -1580,19 +1439,17 @@
             transactions = provider.list_transactions(
                 id=id,
                 state=state,
                 limit=max(limit, 100)
             )
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching transactions: {e}\n")
-            exit(1)
-
+            exit_with_divider(1)
     rich.print()
     show_transactions(transactions, limit, all_users)
-
     divider()
 
 #--------------------------------------------------
 # Transaction cancel
 #--------------------------------------------------
 
 @cli.command(name="transactions:cancel", help="Cancel a transaction")
@@ -1604,29 +1461,27 @@
     provider = get_resource_provider()
     if id is None:
         with Spinner("Fetching transactions", "Transactions fetched"):
             try:
                 transactions = provider.list_transactions(limit=20, only_active=True)
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching transactions: {e}")
-                exit(0)
+                exit_with_divider(1)
 
         if not transactions:
             rich.print("\n[yellow]No active transactions found")
-            rich.print("")
-            exit(1)
+            exit_with_divider()
 
         show_transactions(transactions, 20, all_users)
 
         id = controls.fuzzy("Select a transaction to cancel:", [t["id"] for t in transactions])
         print()
 
     with Spinner("Cancelling transaction", "Transaction cancelled", "Error:"):
         provider.cancel_transaction(id)
-
     divider()
 
 #--------------------------------------------------
 # Main
 #--------------------------------------------------
 
 if __name__ == "__main__":
```

### Comparing `relationalai-0.2.9/src/relationalai/tools/cli_controls.py` & `relationalai-0.3.0/src/relationalai/tools/cli_controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,21 @@
     except KeyboardInterrupt:
         abort()
         raise Exception("Unreachable")
     if newline:
         rich.print("")
     return result
 
-def fuzzy(message:str, choices:List[str], default:str|None = None, multiselect=False, **kwargs) -> str:
+def fuzzy(message:str, choices:List[str], default:str|None = None, multiselect=False, show_index=False, **kwargs) -> str:
+    for i, choice in enumerate(choices):
+        if isinstance(choice, str):
+            choices[i] = {"name": f"{i+1} {choice}" if show_index else choice, "value": choice}
+
+    values = [choice["value"] for choice in choices]
+
     try:
         kwargs["keybindings"] = default_bindings
         if multiselect:
             kwargs["keybindings"] = {
                 "toggle": [
                     {"key": "tab"},   # toggle choices
                 ],
@@ -133,37 +139,41 @@
                     {"key": "tab", "filter":False},
                 ],
             }.update(default_bindings)
             kwargs["multiselect"] = True
 
         scroll_to_ix = None
         # @FIXME: Future improvement to make it optionally case insensitive
-        if default and default in choices:
-            scroll_to_ix = choices.index(default)
+        if default and default in values:
+            scroll_to_ix = values.index(default)
             default = None
 
         prompt = inquirer.fuzzy(message, choices=choices, default=default or "", max_height=8, border=True, style=STYLE, **kwargs)
         if scroll_to_ix is not None:
             prompt.content_control.selected_choice_index = scroll_to_ix
         return prompt.execute()
     except KeyboardInterrupt:
         return abort()
 
 def fuzzy_with_refetch(prompt: str, type: str, fn: callable = None, *args, **kwargs):
     exception = None
+    not_found_message = kwargs.get("not_found_message", None)
     with Spinner(f"Fetching {type}", f"Fetched {type}"):
         try:
             items = fn(*args)
         except Exception as e:
             exception = e
     if exception is not None:
         rich.print(f"\n[red]Error fetching {type}: {exception}\n")
         return exception
     if len(items) == 0:
-        rich.print(f"\n[yellow]No valid {type} found\n")
+        if not_found_message:
+            rich.print(f"\n[yellow]{not_found_message}\n")
+        else:
+            rich.print(f"\n[yellow]No valid {type} found\n")
         return None
 
     items.insert(0, REFETCH)
 
     passed_default = kwargs.get("default", None)
     passed_mandatory = kwargs.get("mandatory", False)
 
@@ -182,24 +192,25 @@
 
 def confirm(message:str, default:bool = False) -> bool:
     try:
         return inquirer.confirm(message, default=default, keybindings=default_bindings).execute()
     except KeyboardInterrupt:
         return abort()
 
-def text(message:str, default:str|None = None, validator:callable = None, invalid_message:str|None = None) -> str:
+def text(message:str, default:str|None = None, validator:callable = None, invalid_message:str|None = None, **kwargs) -> str:
     if validator and not invalid_message:
         invalid_message = "Invalid input"
     try:
         return inquirer.text(
             message,
             default=default or "",
             keybindings=default_bindings,
             validate=validator,
-            invalid_message=invalid_message
+            invalid_message=invalid_message,
+            **kwargs
         ).execute()
     except KeyboardInterrupt:
         return abort()
 
 def password(message:str, default:str|None = None, validator:callable = None, invalid_message:str|None = None) -> str:
     try:
         return inquirer.secret(
```

### Comparing `relationalai-0.2.9/src/relationalai/tools/debugger.py` & `relationalai-0.3.0/src/relationalai/tools/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,19 +100,19 @@
                 total_time += obj['elapsed']
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label(f"{obj['type']}")
                     ui.label(format_time(obj['elapsed']))
                     if obj.get('results'):
                         ui.label(f"{obj['results']['count']}")
-            elif obj['event'] == "span_start" and obj['span']['type'] == "wait":
+            elif obj['event'] == "transaction_created":
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label("transaction")
-                    ui.label(obj["span"]["attrs"]["txn_id"])
+                    ui.label(obj["txn_id"])
             elif obj.get('type'):
                 total_time += obj.get('elapsed', 0)
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label(f"{obj['type']}")
                     ui.label(format_time(obj.get('elapsed', 0)))
                     if obj.get('results'):
```

### Comparing `relationalai-0.2.9/src/relationalai/tools/debugger_client.py` & `relationalai-0.3.0/src/relationalai/tools/debugger_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,80 +2,108 @@
 import logging
 import os
 import threading
 import websockets
 import queue
 from relationalai import debugging
 import __main__ # to get the users root file path
+from relationalai.clients.config import Config
+
+class DummyRecord(logging.LogRecord):
+    def __init__(self, msg):
+        self.msg = msg
 
 #------------------------------------------------------------------------------
 # Logging Handler
 #------------------------------------------------------------------------------
 
 class WebSocketLoggingHandler(logging.Handler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         from relationalai.analysis.mechanistic import Mechanism
         self.Mechanism = Mechanism
         self.queue: queue.Queue[str] = queue.Queue()
 
-    def start(self, url: str):
+    def start(self, url: str, config: Config):
         main_path = getattr(__main__, "__file__", None)
-        program_span = debugging.span_start("program",  main=os.path.relpath(main_path) if main_path else "notebook")
+
+        # Catch any spans that are the programs parent that were added before the debug client was started.
+        open_spans = []
+        existing_parent = debugging.TIP_SPAN
+        while existing_parent:
+            open_spans.append(existing_parent)
+            existing_parent = existing_parent.parent
+        open_spans.reverse()
+
+        program_span = None
+
+        for span in open_spans:
+            if span.type == "program":
+                program_span = span
+            self.queue.put_nowait(self.format_raw({"event": "span_start", "span": span}))
+
+        if not program_span:
+            program_span = debugging.span_start("program",
+                                                main=os.path.relpath(main_path) if main_path else "notebook",
+                                                platform=config.get("platform", None))
+
         self.thread = threading.Thread(target=self.connect, args=(url, program_span))
         self.thread.start()
 
     def emit(self, record):
         d = record.msg
         if (isinstance(d, dict) and
             d["event"] == "span_start" and
             "task" in d["span"].attrs and
             "mech" not in d["span"].attrs):
             d["span"].attrs["mech"] = self.Mechanism(d["span"].attrs["task"])
         log_entry = self.format(record)
         self.queue.put_nowait(log_entry)
 
+    def format_raw(self, msg):
+        return self.format(DummyRecord(msg))
+
     def connect(self, url: str, span: debugging.Span):
         print(f"Connecting to {url}...")
         try:
             try:
                 loop = asyncio.get_running_loop()
                 loop.run_until_complete(self.connect_async(url, span))
             except RuntimeError:
                 asyncio.run(self.connect_async(url, span))
         except (ConnectionRefusedError, websockets.WebSocketException, OSError, asyncio.TimeoutError):
             print(f"Failed to connect to {url}. Running with debug sink disabled.")
 
     async def connect_async(self, url: str, span: debugging.Span):
         async with websockets.connect(url) as ws:
             print("Connected.")
+            alive = True
             while True:
                 if not threading.main_thread().is_alive():
-                    debugging.span_end(span)
-                    log_entry = self.queue.get(timeout=1)
-                    await ws.send(log_entry)
-                    break
+                    alive = False
+                    debugging.span_flush()
 
                 try:
                     log_entry = self.queue.get(timeout=1)
                     await ws.send(log_entry)
                 except queue.Empty:
-                    pass
+                    if not alive:
+                        break
                 except websockets.ConnectionClosedError:
                     break
 
 #------------------------------------------------------------------------------
 # Enable debugging
 #------------------------------------------------------------------------------
 
 already_debugging = False
-def start_debugger_session(host = "0.0.0.0", port = 8080):
+def start_debugger_session(config: Config, host = "0.0.0.0", port = 8080):
     global already_debugging
     if already_debugging:
         return
 
     ws_handler = WebSocketLoggingHandler()
     ws_handler.setFormatter(debugging.JsonFormatter())
     debugging.logger.addHandler(ws_handler)
-    ws_handler.start(f"ws://{host}:{port}/ws/program")
+    ws_handler.start(f"ws://{host}:{port}/ws/program", config)
 
     already_debugging = True
```

### Comparing `relationalai-0.2.9/src/relationalai/tools/debugger_server.py` & `relationalai-0.3.0/src/relationalai/tools/debugger_server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import asyncio
 import json
 from pathlib import Path
-from typing import Any, Callable, Coroutine, Protocol
+from typing import Any, Callable, Coroutine, Protocol, cast
 
 import aiohttp
-import websockets
+from websockets.exceptions import ConnectionClosed
 from aiohttp import web
 
 import relationalai
+from relationalai.clients.client import ResourceProvider
+from relationalai.debugging import encode_log_message
 
 PROJECT_ROOT = Path(relationalai.__file__).resolve().parent.parent.parent
 HTTP_DIST_DIR = PROJECT_ROOT / "frontend" / "debugger" / "dist"
 
+# The maximum number of messages to be sent at once when catching a new client up
+MAX_BATCH_SIZE = 500
+
+_resources: ResourceProvider|None = None
+
+def get_resources() -> ResourceProvider:
+    if not _resources:
+        raise Exception("Unable to acquire resources")
+
+    return _resources
+
 #------------------------------------------------------------------------------
 # Program Connections
 #------------------------------------------------------------------------------
 
 connected_program = None
 
 async def handle_program(req: web.Request):
@@ -24,15 +37,14 @@
 
     global connected_program
     if connected_program:
         print("Refusing to connect to new program until previous one finishes.")
         await ws.close()
 
     connected_program = ws
-    buffered_broadcasts.clear()
     print("Program connected")
     try:
         async for msg in ws:
             if msg.type == aiohttp.WSMsgType.TEXT:
                 await broadcast(msg.data)
             elif msg.type == aiohttp.WSMsgType.ERROR:
                 err = ws.exception()
@@ -48,59 +60,72 @@
 
 #------------------------------------------------------------------------------
 # Browser Client Connections
 #------------------------------------------------------------------------------
 
 connected_clients: set[web.WebSocketResponse] = set()
 
-async def handle_client_message(msg: Any, ws: web.WebSocketResponse):
-    try:
-        parsed = json.loads(msg)
-    except json.JSONDecodeError as e:
-        print("Got invalid json from client:", e)
-        return
-
-    action = client_actions.get(parsed["type"])
-    if not action:
-        print("Got action request from client for non-existent action of type", parsed["type"])
-        return
-
-    kwargs = {k: v for k, v in parsed.items() if k != 'type'}
-    res = action(ws, **kwargs)
-    if res:
-        if asyncio.iscoroutine(res):
-            res = await res
-
-        await ws.send_json(res)
-
 async def handle_client(req: web.Request):
     ws = web.WebSocketResponse()
     await ws.prepare(req)
     connected_clients.add(ws)
     try:
-        for msg in buffered_broadcasts:
-            await ws.send_str(msg)
+        for i in range(0, len(buffered_broadcasts), MAX_BATCH_SIZE):
+            chunk = ",".join(buffered_broadcasts[i:i + MAX_BATCH_SIZE])
+            await ws.send_str(f"[{chunk}]")
 
         async for msg in ws:
             if msg.type == aiohttp.WSMsgType.TEXT:
-                await handle_client_message(msg.data, ws)
+                await handle_client_action(msg.data, ws)
             elif msg.type == aiohttp.WSMsgType.ERROR:
                 err = ws.exception()
                 if err:
                     raise err
             else:
                 raise Exception("Unknown message type", msg.type)
 
-    except websockets.exceptions.ConnectionClosed as e:
+    except ConnectionClosed as e:
         print(f"Client disconnected with reason: {e}")
     finally:
         connected_clients.remove(ws)
 
     return ws
 
+class NoSuchActionError(KeyError):
+    def __init__(self, action: str|None):
+        super().__init__(f"Got action request from client for non-existent action of type '{action}'")
+
+async def handle_client_action(msg: Any, ws: web.WebSocketResponse):
+    parsed = None
+    try:
+        parsed = json.loads(msg)
+        action_type = parsed.get("type")
+        action = client_actions.get(action_type)
+        if not action:
+            raise NoSuchActionError(action_type)
+        kwargs = {k: v for k, v in parsed.items() if k != "type" and k != "rpc_id"}
+        res = action(ws, **kwargs) or {}
+
+    except Exception as e:
+        print("Error:", str(e))
+        res = {"error": str(e)}
+
+    if parsed:
+        if asyncio.iscoroutine(res):
+            res = await res
+
+        res = cast(dict, res)
+        res["event"] = "rpc_response"
+        res["rpc_id"] = parsed.get("rpc_id")
+
+        def dump_json(v):
+            return json.dumps(v, default=encode_log_message)
+
+        await ws.send_json([res], None, dumps=dump_json)
+
 #------------------------------------------------------------------------------
 # Browser Client Actions
 #------------------------------------------------------------------------------
 
 ClientActionReturn = Coroutine[Any, Any, dict|None]|dict|None
 
 class ClientAction(Protocol):
@@ -112,28 +137,31 @@
 def client_action(name: str|None = None):
     def decorator(fn: Callable[..., ClientActionReturn]):
         client_actions[name or fn.__name__] = fn
 
     return decorator
 
 @client_action()
-def ping(_):
-    print("Pinged!")
-    return {"type": "pong"}
+def clear(_):
+    buffered_broadcasts.clear()
+
+@client_action()
+def list_transactions(_, **kwargs):
+    return {"transactions": get_resources().list_transactions(**kwargs)}
 
 #------------------------------------------------------------------------------
 # Event Log
 #------------------------------------------------------------------------------
 
 buffered_broadcasts = []
 
 async def broadcast(message):
     buffered_broadcasts.append(message)
     if connected_clients:
-        tasks = [asyncio.create_task(client.send_str(message)) for client in connected_clients]
+        tasks = [asyncio.create_task(client.send_str(f"[{message}]" )) for client in connected_clients]
         await asyncio.wait(tasks)
 
 #------------------------------------------------------------------------------
 # Server
 #------------------------------------------------------------------------------
 
 async def serve_index(_):
@@ -155,15 +183,17 @@
     site = web.TCPSite(runner, host, port)
     await site.start()
 
     print(f"Server started at http://{host}:{port}")
 
     return runner
 
-def start_server(host: str, port: int):
+def start_server(host: str, port: int, profile:str|None = None):
+    global _resources
+    _resources = relationalai.Resources(profile)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(run_server(host, port))
     loop.run_forever()
 
 
 def stop_server():
     global runner
```

### Comparing `relationalai-0.2.9/src/relationalai/tools/dev.py` & `relationalai-0.3.0/src/relationalai/tools/dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,33 +127,31 @@
 @cli.command()
 def stats():
     dsl = cloc(["dsl.py"])
     compiler = cloc(["compiler.py"])
     metamodel = cloc(["metamodel.py"])
     emitter = cloc(["rel_emitter.py"])
     rel = cloc(["rel.py"])
-    rel2 = cloc(["rel2.py"])
     metagen = cloc(["metagen.py"])
     gentest = cloc(["../gentest", "metagen.py"])
     tools = cloc(["tools/"])
     clients = cloc(["clients/"])
     std = cloc(["std/"])
     non_test_total = cloc(["."]) - metagen
     total = non_test_total + gentest
-    core = dsl + compiler + metamodel + emitter + rel + rel2
+    core = dsl + compiler + metamodel + emitter + rel
 
     max_width = len(f"{total:,}")
 
     # Print statements with numbers right-aligned
     divider()
     rich.print(f"[yellow]RelationalAI  {non_test_total:>{max_width},} loc")
     rich.print(f"[yellow]  Core        {core:>{max_width},} loc")
     rich.print(f"[yellow]    dsl       {dsl:>{max_width},} loc")
     rich.print(f"[yellow]    rel       {rel:>{max_width},} loc")
-    rich.print(f"[yellow]    rel2      {rel2:>{max_width},} loc")
     rich.print(f"[yellow]    emitter   {emitter:>{max_width},} loc")
     rich.print(f"[yellow]    metamodel {metamodel:>{max_width},} loc")
     rich.print(f"[yellow]    compiler  {compiler:>{max_width},} loc")
     rich.print(f"[yellow]  Clients     {clients:>{max_width},} loc")
     rich.print(f"[yellow]  Std         {std:>{max_width},} loc")
     rich.print(f"[yellow]  Tools       {tools:>{max_width},} loc")
     rich.print("")
```

### Comparing `relationalai-0.2.9/src/relationalai/util/format.py` & `relationalai-0.3.0/src/relationalai/util/format.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/util/snowflake_logger.py` & `relationalai-0.3.0/src/relationalai/util/snowflake_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/src/relationalai/util/tracing_logger.py` & `relationalai-0.3.0/src/relationalai/util/tracing_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict, List
 
 from relationalai.debugging import Span
 from relationalai.util.keys import get_key
 
 ATTR_ALLOW_LIST = {
     'transaction': {'txn_id'},
+    'wait': {'txn_id'},
 }
 
 class TracingLogger(logging.Handler):
     """
     This logger prints spans to stdout as they start and finish.
     """
```

### Comparing `relationalai-0.2.9/tests/conftest.py` & `relationalai-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/util.py` & `relationalai-0.3.0/tests/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from pathlib import Path
 import random
 import os
 
+import pytest
 import snowflake.connector
 
 import relationalai as rai
 from relationalai import debugging
 from relationalai.debugging import logger
 from relationalai.clients import config as cfg
 from relationalai.util.snowflake_logger import SnowflakeLogger
+from relationalai.util.span_format_test import SpanCollectorHandler, assert_valid_span_structure
+from testutil.snapshot import path_to_slug, validate_block_snapshots
 
-def engine_config_fixture():
+def engine_config_fixture(size):
     # Check for an externally provided engine name
     # It is used in GitHub Actions to run tests against a specific engine
     engine_name = os.getenv("ENGINE_NAME")
     if engine_name:
         # If engine name was provided, just yield the config
         config = make_config(engine_name)
         yield config
@@ -25,28 +29,28 @@
     if config.file_path is not None:
         yield config
         return
 
     # Otherwise, create a new engine and delete it afterwards.
     random_number = random.randint(1000000000, 9999999999)
     engine_name = f"pyrel_test_{random_number}"
-    create_engine(engine_name)
+    create_engine(engine_name, size=size)
 
     yield make_config(engine_name)
 
     delete_engine(engine_name)
 
-def create_engine(engine_name: str):
+def create_engine(engine_name: str, size: str):
     config = make_config(engine_name)
 
     sf_compute_pool = os.getenv("SF_TEST_COMPUTE_POOL", config.get("compute_pool", ""))
 
     provider = rai.Resources(config=config)
     print(f"Creating engine {engine_name}")
-    provider.create_engine(name=engine_name, size="XS", pool=sf_compute_pool)
+    provider.create_engine(name=engine_name, size=size, pool=sf_compute_pool)
     print(f"Engine {engine_name} created")
 
 
 def delete_engine(engine_name: str):
     print(f"Deleting engine {engine_name}")
     config = make_config(engine_name)
     provider = rai.Resources(config=config)
@@ -83,14 +87,15 @@
         case "snowflake":
             sf_username = os.getenv("SF_TEST_ACCOUNT_USERNAME")
             sf_password = os.getenv("SF_TEST_ACCOUNT_PASSWORD")
             sf_account = os.getenv("SF_TEST_ACCOUNT_NAME")
             sf_warehouse = os.getenv("SF_TEST_WAREHOUSE_NAME")
             sf_app_name = os.getenv("SF_TEST_APP_NAME")
             sf_compute_pool = os.getenv("SF_TEST_COMPUTE_POOL")
+            sf_use_exec_async_v2 = os.getenv("SF_USE_EXEC_ASYNC_V2", False)
             if sf_username is None or sf_password is None:
                 raise ValueError(
                     "SF_TEST_ACCOUNT_USERNAME, SF_TEST_ACCOUNT_PASSWORD, SF_TEST_ACCOUNT_NAME must be set if RAI_CLOUD_PROVIDER is set to 'snowflake'"
                 )
             return cfg.Config(
                 {
                     "platform": "snowflake",
@@ -98,14 +103,15 @@
                     "password": sf_password,
                     "account": sf_account,
                     "role": "rai_integration_consumer",
                     "warehouse": sf_warehouse,
                     "rai_app_name": sf_app_name,
                     "engine": engine_name,
                     "compute_pool": sf_compute_pool,
+                    "sf_use_exec_async_v2": sf_use_exec_async_v2
                 }
             )
         case _:
             raise ValueError(f"Unsupported cloud provider: {cloud_provider}")
 
 def snowflake_logger_fixture():
     if not os.getenv("SF_REPORTING_PASSWORD"):
@@ -123,14 +129,21 @@
         schema=os.getenv("SF_REPORTING_SCHEMA"),
     )
     snowflake_logger = SnowflakeLogger(conn)
     logger.addHandler(snowflake_logger)
     yield
     snowflake_logger.shut_down()
 
+def span_structure_validator_fixture():
+    handler = SpanCollectorHandler()
+    logger.addHandler(handler)
+    yield handler
+    logger.removeHandler(handler)
+    assert_valid_span_structure(handler.nodes, handler.events)
+
 def root_span_fixture():
     git_info = get_git_info()
     attrs = {
         **git_info,
         "cloud_provider": os.getenv("RAI_CLOUD_PROVIDER"),
     }
     with debugging.span("test_session", **attrs):
@@ -144,7 +157,56 @@
         }
     else:
         # shell out to get the info
         return {
             'commit': 'local',
             'branch': 'local',
         }
+
+def randomize(name: str) -> str:
+    return f"{name}_{random.randint(1000000000, 9999999999)}"
+
+def do_snapshot_test(
+        config: cfg.Config,
+        engine_size: str,
+        snapshot,
+        file_path: Path,
+        runs: int = 1,
+        span_name: str = "test",
+        create_db: bool = True,
+    ):
+    """
+    Run the PyRel program in the given `file_path`, testing the results against a snapshot file,
+    using the given `config` and `engine_size`.
+    """
+
+    test_name = file_path.stem
+
+    provider = rai.Resources(config=config)
+
+    def get_results(event):
+        if "results" in event:
+            return str(event["results"]["values"])
+
+    with debugging.span(span_name, name=test_name, engine_size=engine_size):
+        for i in range(runs):
+            with debugging.span("run", idx=i):
+                with debugging.span("program", main=os.path.relpath(file_path), platform=config.get("platform", None)) as span:
+                    db_name = randomize(test_name)
+                    validate_block_snapshots(file_path, snapshot, get_results, "query", {
+                        "name": db_name,
+                        "config": config,
+                        "span": span,
+                    })
+                    # Some tests always use the same DB, never creating a DB named `db_name`,
+                    # so we don't need to delete it.
+                    if create_db:
+                        try:
+                            provider.delete_graph(db_name)
+                        except Exception as e:
+                            print(f"Failed to delete graph {db_name}: {e}")
+
+def all_files_in_dir(test_case_dir: Path):
+    test_case_files = [path for path in test_case_dir.rglob("*.py")]
+    return pytest.mark.parametrize(
+        "file_path", test_case_files, ids=lambda path: path_to_slug(path, test_case_dir)
+    )
```

### Comparing `relationalai-0.2.9/tests/benchmarks/conftest.py` & `relationalai-0.3.0/tests/end2end/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import os
 
 import pytest
 
-from relationalai import debugging
 from relationalai.debugging import logger
 from relationalai.util.tracing_logger import TracingLogger
-from tests.util import engine_config_fixture, root_span_fixture, snowflake_logger_fixture
+from tests.util import engine_config_fixture, root_span_fixture, snowflake_logger_fixture, span_structure_validator_fixture
 
-
-@pytest.fixture(scope="function")
-def engine_config():
-    yield from engine_config_fixture()
+# Engine is actually created in end-to-end/action.yml
+# keep this in sync with that
+@pytest.fixture(scope="session")
+def engine_size():
+    return "XS"
+
+@pytest.fixture(scope="session")
+def engine_config(engine_size):
+    yield from engine_config_fixture(engine_size)
 
 # Create a root span that all tests will be a part of
-# add `snowflake_logger` as a parameter, to make sure it is initialized before the root span
-# and finishes afterwards
+# - add `snowflake_logger` as a parameter, to make sure it is initialized before the root span
+#   and finishes afterwards
+# - add `span_structure_validator` as a parameter, to make sure it is initialized before the root span.
 @pytest.fixture(scope="session", autouse=True)
-def root_span(snowflake_logger):
+def root_span(snowflake_logger, span_structure_validator):
     yield from root_span_fixture()
 
+@pytest.fixture(scope="session", autouse=True)
+def span_structure_validator():
+    yield from span_structure_validator_fixture()
+
 # Attach Snowflake logger; shutting down that the end of the session
 @pytest.fixture(scope="session", autouse=True)
 def snowflake_logger():
     yield from snowflake_logger_fixture()
 
-# Wrap each test in a `benchmark` span
-@pytest.fixture(scope="function", autouse=True)
-def benchmark_span(request):
-    # trim 'test_' from the beginning of the test name
-    name = request.node.name[5:]
-    with debugging.span("benchmark", name=name):
-        yield
-
 if os.getenv('ENABLE_TRACING_LOGGER') is not None:
     logger.addHandler(TracingLogger())
```

### Comparing `relationalai-0.2.9/tests/benchmarks/test_tastybytes.py` & `relationalai-0.3.0/tests/benchmarks/benchmarks/tastybytes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,114 @@
 #pyright: reportUnusedExpression=false
 import relationalai as rai
 from relationalai.clients.snowflake import Snowflake
-from relationalai.clients import config as cfg
 from relationalai.std import aggregates, rel
 from relationalai.std.graphs import Graph
 
 from relationalai import debugging
 
-def test_tastybytes(engine_config: cfg.Config):
-    name = "LOYALTY_ORDERS_REGION_CALIFORNIA"
-    # provider = rai.Resources(config=engine_config)
-    # with debugging.span("clone"):
-    #     name = "LOYALTY_ORDERS_REGION_CALIFORNIA_" + str(random.randint(1000000000, 9999999999))
-    #     provider.clone_graph(name, "LOYALTY_ORDERS_REGION_CALIFORNIA")
-    #     atexit.register(lambda: provider.delete_graph(name))
-    
-    model = rai.Model(name, config=engine_config)
-    model._config.set("compiler.use_multi_valued", True)
-    sf = Snowflake(model)
-    Record = sf.TASTYBYTES.HARMONIZED.LOYALTY_ORDERS_REGION_CALIFORNIA
-
-    Customer = model.Type("Customer")
-    Truck = model.Type("Trucks")
-    Transaction = model.Type("Transaction")
-    RelevantConnection = model.Type("RelevantConnection")
-    
-    with model.query(tag="count_all") as select:
-        record = Record()
-        num_records = aggregates.count(record)
-        select(num_records)
-
-    # Define Customer Type
-    with model.rule(dynamic=True):
-        r = Record()
-        Customer.add(customer_id=r.customer_id)
-
-    # Check total number of customers
-    with model.query(tag="count_customers") as select:
-        record = Customer()
-        num_records = aggregates.count(record)
-        select(num_records)
-
-    # Define Truck Type
-    with model.rule():
-        r = Record()
-        Truck.add(truck_id=r.truck_id)
-
-    # Check total number of trucks
-    with model.query(tag="count_trucks") as select:
-        record = Truck()
-        num_records = aggregates.count(record)
-        select(num_records)
-
-    with model.rule():
-        r = Record()
-        Transaction.add(
-            customer_id=r.customer_id,
-            order_id=r.order_id,
-            truck_id=r.truck_id,
-            order_ts=r.order_ts,
-            order_ts_seconds=r.order_ts_seconds,
-            location_id=r.location_id,
-        )
-
-    with model.rule():
-        t1 = Transaction()
-        t2 = Transaction()
-
-        t1.truck_id == t2.truck_id
-        t1.customer_id != t2.customer_id
-        rel.abs(t1.order_ts_seconds - t2.order_ts_seconds) <= 1200
-
-        t1.connected.add(t2)
-
-    with model.query(tag="count_connected_customers") as select:
-        t = Transaction()
-        num_records = aggregates.count(t.customer_id, t.order_ts, t.connected, t.connected.customer_id)
-        select(num_records)
-
-    with model.rule():
-        t = Transaction()
-        total_connections = aggregates.count(
-            t, per=[t.customer_id, t.connected.customer_id]
-        )
-        total_connections > 4
-        RelevantConnection.add(
-            customer_1=Customer(customer_id=t.customer_id),
-            customer_2=Customer(customer_id=t.connected.customer_id),
-            total_connections=total_connections,
-        )        
-
-    # Get the total occurrences where pairs of customers coexisted together more than once
-    with model.query(tag="count_meaningful_connected_customers") as select:
-        record = RelevantConnection()
-        num_records = aggregates.count(record)
-        select(num_records)
-
-    community_graph = Graph(model, undirected=True)
-
-    # Add edges to the graph between customers / Nodes will be added automatically
-    with model.rule():
-        connection = RelevantConnection()
-        community_graph.Edge.add(
-            connection.customer_1,
-            connection.customer_2,
-            weight=connection.total_connections,
-        )
-
-    with model.rule():
-        customer = Customer()
-        community_id = community_graph.compute.louvain(customer)
-        customer.set(community_id=community_id)
-
-        community_graph.Node.add(
-            customer,
-            community_id=community_id,
-            customer_id=customer.customer_id
-        )
+# This benchmark expects the model to already be present, with the data loaded into it.
+model = rai.Model("PyRelTastyBytesBenchmark", config=globals().get("config"))
+model._config.set("compiler.use_multi_valued", True)
+sf = Snowflake(model)
+Record = sf.TASTYBYTES.HARMONIZED.LOYALTY_ORDERS_REGION_CALIFORNIA
+
+Customer = model.Type("Customer")
+Truck = model.Type("Trucks")
+Transaction = model.Type("Transaction")
+RelevantConnection = model.Type("RelevantConnection")
+
+with model.query(tag="count_all") as select:
+    record = Record()
+    num_records = aggregates.count(record)
+    select(num_records)
+
+# Define Customer Type
+with model.rule(dynamic=True):
+    r = Record()
+    Customer.add(customer_id=r.customer_id)
+
+# Check total number of customers
+with model.query(tag="count_customers") as select:
+    record = Customer()
+    num_records = aggregates.count(record)
+    select(num_records)
+
+# Define Truck Type
+with model.rule():
+    r = Record()
+    Truck.add(truck_id=r.truck_id)
+
+# Check total number of trucks
+with model.query(tag="count_trucks") as select:
+    record = Truck()
+    num_records = aggregates.count(record)
+    select(num_records)
+
+with model.rule():
+    r = Record()
+    Transaction.add(
+        customer_id=r.customer_id,
+        order_id=r.order_id,
+        truck_id=r.truck_id,
+        order_ts=r.order_ts,
+        order_ts_seconds=r.order_ts_seconds,
+        location_id=r.location_id,
+    )
+
+with model.rule():
+    t1 = Transaction()
+    t2 = Transaction()
+
+    t1.truck_id == t2.truck_id
+    t1.customer_id != t2.customer_id
+    rel.abs(t1.order_ts_seconds - t2.order_ts_seconds) <= 1200
+
+    t1.connected.add(t2)
+
+with model.query(tag="count_connected_customers") as select:
+    t = Transaction()
+    num_records = aggregates.count(t.customer_id, t.order_ts, t.connected, t.connected.customer_id)
+    select(num_records)
+
+with model.rule():
+    t = Transaction()
+    total_connections = aggregates.count(
+        t, per=[t.customer_id, t.connected.customer_id]
+    )
+    total_connections > 4
+    RelevantConnection.add(
+        customer_1=Customer(customer_id=t.customer_id),
+        customer_2=Customer(customer_id=t.connected.customer_id),
+        total_connections=total_connections,
+    )
+
+# Get the total occurrences where pairs of customers coexisted together more than once
+with model.query(tag="count_meaningful_connected_customers") as select:
+    record = RelevantConnection()
+    num_records = aggregates.count(record)
+    select(num_records)
+
+community_graph = Graph(model, undirected=True)
+
+# Add edges to the graph between customers / Nodes will be added automatically
+with model.rule():
+    connection = RelevantConnection()
+    community_graph.Edge.add(
+        connection.customer_1,
+        connection.customer_2,
+        weight=connection.total_connections,
+    )
+
+with model.rule():
+    customer = Customer()
+    community_id = community_graph.compute.louvain(customer)
+    customer.set(community_id=community_id)
+
+    community_graph.Node.add(
+        customer,
+        community_id=community_id,
+        customer_id=customer.customer_id
+    )
 
-    with debugging.span("fetch", graph="louvain"):
-        community_graph.fetch()
+with debugging.span("fetch", graph="louvain"):
+    community_graph.fetch()
```

### Comparing `relationalai-0.2.9/tests/end2end/README.md` & `relationalai-0.3.0/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/conftest.py` & `relationalai-0.3.0/tests/benchmarks/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 import pytest
 
 from relationalai.debugging import logger
 from relationalai.util.tracing_logger import TracingLogger
 from tests.util import engine_config_fixture, root_span_fixture, snowflake_logger_fixture
 
+@pytest.fixture(scope="function")
+def engine_size():
+    return "M"
 
-@pytest.fixture(scope="session")
-def engine_config():
-    yield from engine_config_fixture()
+@pytest.fixture(scope="function")
+def engine_config(engine_size):
+    yield from engine_config_fixture(engine_size)
 
 # Create a root span that all tests will be a part of
 # add `snowflake_logger` as a parameter, to make sure it is initialized before the root span
 # and finishes afterwards
 @pytest.fixture(scope="session", autouse=True)
 def root_span(snowflake_logger):
     yield from root_span_fixture()
```

### Comparing `relationalai-0.2.9/tests/end2end/test_graph_visualize.py` & `relationalai-0.3.0/tests/end2end/test_graph_visualize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import random
 import pytest
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 DEFAULT_METADATA = {
     'arrow_color': '#999',
     'arrow_size': 4,
@@ -49,20 +48,14 @@
     with model.rule(dynamic=True):
         for ((id1, id2), props) in test_input["edge_props"].items():
             node1, node2 = Node(id=id1), Node(id=id2)
             graph.Edge.add(node1, node2, **props)
 
     return graph
 
-# @NOTE: This should replaced with the globals lookup from
-# https://github.com/RelationalAI/relationalai-python/pull/117 once that drops.
-def unique_model_name(name: str):
-    random_number = random.randint(1000000000, 9999999999)
-    return f"{name}_{random_number}"
-
 # Test that graph._visual_dict() returns a dictionary with the correct keys and values
 @pytest.mark.parametrize(
     ["test_input", "expected_dict"],
     [
         # Undirected graph with one data edge, no props, default style
         pytest.param(
             {
@@ -165,15 +158,15 @@
                 'metadata': DEFAULT_METADATA,
             },
             id="directed_with_props_custom_style",
         ),
     ],
 )
 def test_visual_dict(engine_config, test_input, expected_dict):
-    model_name = unique_model_name("testGraphVisualDict")
+    model_name = "testGraphVisualDict"
     model = rai.Model(model_name, config=engine_config)
     graph = make_graph(model, test_input)
     visual_dict = graph._visual_dict(style=test_input["style"])
     assert visual_dict == {'graph': expected_dict}
 
 # Test that graph.visualize() returns a value and does not raise an exception.
 @pytest.mark.parametrize(
@@ -204,14 +197,11 @@
                     },
                 },
                 id="no_style_override_kwargs",
             ),
         ]
 )
 def test_visualize(engine_config, test_input):
-    model_name = unique_model_name("testGraphVisualize")
+    model_name = "testGraphVisualize"
     model = rai.Model(model_name, config=engine_config)
     graph = make_graph(model, test_input)
     assert graph.visualize(style=test_input["style"], **test_input["kwargs"]) is not None
-    # delete the DB
-    provider = rai.Resources(config=engine_config)
-    provider.delete_graph(model_name)
```

### Comparing `relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.3.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/after_errors.py` & `relationalai-0.3.0/tests/end2end/test_cases/after_errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     p.age >= 18
     p.set(Adult)
 
 
 try:
     with model.query() as select:
         a = Adult()
-        a.foo # this will cause the rel to fail, since foo doesn't exist
+        a.foo > 0 # this will cause the rel to fail, since foo doesn't exist
         z = select(a, a.name, a.age)
 except Exception:
     pass
 
 # adding a type when value types are on causes initialization code to be added
 # to the model's temporary rule
 woop = model.Type("Woop")
```

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/bool.py` & `relationalai-0.3.0/tests/end2end/test_cases/bool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #pyright: reportUnusedExpression=false
 import relationalai as rai
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_bool"), config=globals().get("config"))
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
 with model.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
     Person.add(name="Jane", age=10)
```

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/bottom.py` & `relationalai-0.3.0/tests/end2end/test_cases/bottom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #pyright: reportUnusedExpression=false
 import relationalai as rai
 from relationalai.std import aggregates
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_bottom"), config=globals().get("config"))
 Person = model.Type("Person")
 
 with model.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
     Person.add(name="Jane", age=15)
     Person.add(name="Alex", age=33)
```

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/export.py` & `relationalai-0.3.0/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.3.0/tests/end2end/test_cases/multi_valued.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,10 +60,8 @@
 
 print(z.results)
 
 with model.query() as select:
     a = Adult()
     z = select(a, a.name, a.age)
 
-print(z.results)
-
-model._config.set("compiler.use_multi_valued", False)
+print(z.results)
```

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/numeric_outputs.py` & `relationalai-0.3.0/tests/end2end/test_cases/numeric_outputs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/out_of_context.py` & `relationalai-0.3.0/tests/end2end/test_cases/out_of_context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/smoke.py` & `relationalai-0.3.0/tests/end2end/test_cases/smoke.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,12 +19,17 @@
     p = Person()
     with p.age == 10:
         p.set(coolness=100)
 
 with model.query() as select:
     a = Adult()
     10 <= a.age <= 80
-    select(a, a.name, a.age)
+    z = select(a, a.name, a.age)
+print(z.results.dtypes)
 
 with model.query() as select:
     p = Person()
-    select(p, p.coolness)
+    with model.found():
+        p.coolness
+    z = select(p, p.coolness)
+
+print(z.results.dtypes)
```

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/std_math.py` & `relationalai-0.3.0/tests/end2end/test_cases/std_math.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/strings.py` & `relationalai-0.3.0/tests/end2end/test_cases/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/top.py` & `relationalai-0.3.0/tests/end2end/test_cases/top.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #pyright: reportUnusedExpression=false
 import relationalai as rai
 from relationalai.std import aggregates
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_top"), config=globals().get("config"))
 Person = model.Type("Person")
 
 with model.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
     Person.add(name="Jane", age=15)
     Person.add(name="Alex", age=33)
```

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.3.0/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/centrality.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/clustering.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/clustering.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/community.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/community.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,28 +35,28 @@
         select(o, algo)
 
 
 # Check that exceptions are raised when invalid parameters are passed.
 PARAMETERS = {
     "infomap": {
         "max_levels": [-1, 0, -1.23, 0.0, 1.23, "a", []],
-        "max_sweeps": [-1, 0, -1.23, 0.0, 1.23, "a", []],
+        "max_sweeps": [-1, -1.23, 0.0, 1.23, "a", []],
         "level_tolerance": [-1.0, -1, "a", []],
         "sweep_tolerance": [-1.0, -1, "a", []],
         "teleportation_rate": [-1.0, -1, 0.0, 0, 1.0001, 2, "a", []],
         "visit_rate_tolerance": [-1.0, -1, 0.0, 0, "a", []],
         "randomization_seed": [-1, 1.23, "a", []],
     },
     "label_propagation": {
-        "max_sweeps": [-1, 0, -1.23, 0.0, 1.23, "a", []],
+        "max_sweeps": [-1, -1.23, 0.0, 1.23, "a", []],
         "randomization_seed": [-1, 1.23, "a", []],
     },
     "louvain": {
         "max_levels": [-1, 0, -1.23, 0.0, 1.23, "a", []],
-        "max_sweeps": [-1, 0, -1.23, 0.0, 1.23, "a", []],
+        "max_sweeps": [-1, -1.23, 0.0, 1.23, "a", []],
         "level_tolerance": [-1.0, -1, "a", []],
         "sweep_tolerance": [-1.0, -1, "a", []],
         "randomization_seed": [-1, 1.23, "a", []],
     },
 }
 with model.query(dynamic=True):
     o = Object()
```

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/degree.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/distance.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/distance.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/link_prediction.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/link_prediction.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/mixed_value_types.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/mixed_value_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/similarity.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/similarity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/end2end/test_cases/graphs/triangles.py` & `relationalai-0.3.0/tests/end2end/test_cases/graphs/triangles.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "triangles", # included here because of optional 'node' parameter
 ]
 
 THREE_ARGS = [
     "is_triangle",
 ]
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_triangles"), config=globals().get("config"))
 Object = model.Type("Object")
 Relationship = model.Type("Relationship")
 
 # Create a graph with 4 nodes and 4 edges, forming a triangle with a dangling node.
 with model.rule(dynamic=True):
     object = [Object.add(id=i) for i in range(4)]
     for i in range(3):
@@ -38,24 +38,24 @@
         algo = getattr(graph.compute, algo_name)()
         if isinstance(algo, tuple):
             select(*algo)
         else:
             select(algo)
 
 for algo_name in ONE_ARG:
-    with model.query() as select:
+    with model.query(dynamic=True) as select:
         o = Object()
         algo = getattr(graph.compute, algo_name)(o)
         if isinstance(algo, tuple):
             select(o.id, *algo)
         else:
             select(o.id, algo)
 
 for algo_name in THREE_ARGS:
-    with model.query() as select:
+    with model.query(dynamic=True) as select:
         o1, o2, o3 = Object(), Object(), Object()
         o1.id < o2.id < o3.id
         algo = getattr(graph.compute, algo_name)(o1, o2, o3)
         if isinstance(algo, tuple):
             select(o1.id, o2.id, o3.id, *algo)
         else:
             select(o1.id, o2.id, o3.id, algo)
```

### Comparing `relationalai-0.2.9/tests/init-cli/README.md` & `relationalai-0.3.0/tests/init-cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/init-cli/azure_basic.py` & `relationalai-0.3.0/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/init-cli/common.py` & `relationalai-0.3.0/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/roundtrip/test_document.py` & `relationalai-0.3.0/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/roundtrip/test_task.py` & `relationalai-0.3.0/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/unit/test_config_store.py` & `relationalai-0.3.0/tests/unit/test_config_store.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/unit/test_configs/config_with_new_profile.toml` & `relationalai-0.3.0/tests/unit/test_configs/config_with_new_profile.toml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/tests/unit/test_configs/raiconfig_example.toml` & `relationalai-0.3.0/tests/unit/test_configs/raiconfig_example.toml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.9/pyproject.toml` & `relationalai-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = 'relationalai'
-version = '0.2.9'
+version = '0.3.0'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
     "snowflake-connector-python[secure-local-storage]",
-    "rai-sdk>=0.7.4",
+    "snowflake-snowpark-python",
+    "rai-sdk>=0.7.5",
     "rich",
     "nicegui",
     "numpy",
     "pandas",
     "colorama",
     "inquirerpy",
     "click",
@@ -21,31 +22,33 @@
     "bytecode",
     "toml",
     "tomlkit",
     "requests",
     "pyarrow",
     "websockets",
     "aiohttp",
+    "packaging"
 ]
 [project.optional-dependencies]
 dev = [
     "pytest",
+    "pytest-cov",
+    "pytest-mock",
+    "pytest-snapshot",
     "hypothesis",
     "faker",
     "argcomplete",
     "watchdog",
     "hupper",
     "prompt_toolkit",
     "build",
-    "pytest-snapshot",
     "ruff",
     "pexpect",
     "ddtrace",
     "coverage",
-    "pytest-cov",
 ]
 
 [project.scripts]
 rai = "relationalai.tools.cli:cli"
 rai-dev = "relationalai.tools.dev:cli"
 gentest = "gentest.cli.__main__:main"
 
@@ -53,8 +56,8 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/relationalai", "src/gentest"]
+packages = ["src/relationalai", "src/gentest", "src/testutil"]
```

### Comparing `relationalai-0.2.9/PKG-INFO` & `relationalai-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.9
+Version: 0.3.0
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: aiohttp
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
 Requires-Dist: inquirerpy
 Requires-Dist: nicegui
 Requires-Dist: numpy
+Requires-Dist: packaging
 Requires-Dist: pandas
 Requires-Dist: pyarrow
-Requires-Dist: rai-sdk>=0.7.4
+Requires-Dist: rai-sdk>=0.7.5
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: snowflake-connector-python[secure-local-storage]
+Requires-Dist: snowflake-snowpark-python
 Requires-Dist: toml
 Requires-Dist: tomlkit
 Requires-Dist: websockets
 Provides-Extra: dev
 Requires-Dist: argcomplete; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
@@ -29,14 +31,15 @@
 Requires-Dist: faker; extra == 'dev'
 Requires-Dist: hupper; extra == 'dev'
 Requires-Dist: hypothesis; extra == 'dev'
 Requires-Dist: pexpect; extra == 'dev'
 Requires-Dist: prompt-toolkit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest-snapshot; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: watchdog; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # The RelationalAI Python Library
```

