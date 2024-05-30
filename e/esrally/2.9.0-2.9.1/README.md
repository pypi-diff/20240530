# Comparing `tmp/esrally-2.9.0.tar.gz` & `tmp/esrally-2.9.1.tar.gz`

## Comparing `esrally-2.9.0.tar` & `esrally-2.9.1.tar`

### file list

```diff
@@ -1,263 +1,268 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esrally-2.9.0/.coveragerc
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 esrally-2.9.0/.fossa.yml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 esrally-2.9.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 esrally-2.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 esrally-2.9.0/.pylintrc
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 esrally-2.9.0/.readthedocs.yaml
--rw-r--r--   0        0        0    85355 2020-02-02 00:00:00.000000 esrally-2.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 esrally-2.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 esrally-2.9.0/Makefile
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 esrally-2.9.0/catalog-info.yaml
--rwxr-xr-x   0        0        0     3902 2020-02-02 00:00:00.000000 esrally-2.9.0/changelog.py
--rwxr-xr-x   0        0        0     4579 2020-02-02 00:00:00.000000 esrally-2.9.0/create-notice.sh
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 esrally-2.9.0/noxfile.py
--rwxr-xr-x   0        0        0     2169 2020-02-02 00:00:00.000000 esrally-2.9.0/prepare-release.sh
--rwxr-xr-x   0        0        0     1739 2020-02-02 00:00:00.000000 esrally-2.9.0/rally
--rwxr-xr-x   0        0        0     1926 2020-02-02 00:00:00.000000 esrally-2.9.0/rallyd
--rwxr-xr-x   0        0        0     2392 2020-02-02 00:00:00.000000 esrally-2.9.0/release-checks.sh
--rwxr-xr-x   0        0        0     5573 2020-02-02 00:00:00.000000 esrally-2.9.0/release-docker-test.sh
--rwxr-xr-x   0        0        0     2409 2020-02-02 00:00:00.000000 esrally-2.9.0/release-docker.sh
--rwxr-xr-x   0        0        0     4983 2020-02-02 00:00:00.000000 esrally-2.9.0/run.sh
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 esrally-2.9.0/.buildkite/pull-requests.json
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 esrally-2.9.0/.buildkite/it/pipeline.yml
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 esrally-2.9.0/.buildkite/it/run.sh
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 esrally-2.9.0/.buildkite/release-docker/pipeline.yml
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 esrally-2.9.0/.buildkite/release-docker/run.sh
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esrally-2.9.0/.ci/variables.json
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 esrally-2.9.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 esrally-2.9.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 esrally-2.9.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 esrally-2.9.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/benchmarks/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/benchmarks/driver/__init__.py
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 esrally-2.9.0/benchmarks/driver/parsing_test.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 esrally-2.9.0/benchmarks/driver/runner_test.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/benchmarks/track/__init__.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 esrally-2.9.0/benchmarks/track/bulk_params_test.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 esrally-2.9.0/docker/docker-compose-tests.yml
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 esrally-2.9.0/docker/Dockerfiles/Dockerfile-dev
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 esrally-2.9.0/docker/Dockerfiles/Dockerfile-release
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 esrally-2.9.0/docker/bin/entrypoint.sh
--rw-r--r--   0        0        0     8234 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/Makefile
--rw-r--r--   0        0        0    23958 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/adding_tracks.rst
--rw-r--r--   0        0        0    26756 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/advanced.rst
--rw-r--r--   0        0        0    18401 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/benchmark_distributed_load.gliffy
--rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/benchmark_distributed_load.png
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/benchmark_existing.gliffy
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/benchmark_existing.png
--rw-r--r--   0        0        0    18424 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/benchmark_remote.gliffy
--rw-r--r--   0        0        0    30736 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/benchmark_remote.png
--rw-r--r--   0        0        0     9697 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/car.rst
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/cluster_management.rst
--rw-r--r--   0        0        0    54105 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/command_line_reference.rst
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/community.rst
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/conf.py
--rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/configuration.rst
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/create_scheduler_plot.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/developing.rst
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/docker.rst
--rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/elasticsearch_plugins.rst
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/faq.rst
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/glossary.rst
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/index.rst
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/install.rst
--rw-r--r--   0        0        0   322917 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/jfr-es.png
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/make.bat
--rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/metrics.rst
--rw-r--r--   0        0        0    45223 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/migrate.rst
--rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/nested-streams.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/nested-streams.puml
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/offline.rst
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/pipelines.rst
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/quickstart.rst
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/race.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/rally-logo.svg
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/rally_daemon.rst
--rw-r--r--   0        0        0    81206 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/recency.png
--rw-r--r--   0        0        0    22262 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/recipes.rst
--rw-r--r--   0        0        0    23079 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/schedulers_10s.png
--rw-r--r--   0        0        0    14727 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/summary_report.rst
--rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/telemetry.rst
--rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/tournament.rst
--rw-r--r--   0        0        0    24101 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/track-ramp-up.png
--rw-r--r--   0        0        0   159265 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/track.rst
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/versions.rst
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/_templates/breadcrumbs.html
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 esrally-2.9.0/docs/architecture/actor_system.md
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/_version.py
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/actor.py
--rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/config.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/exceptions.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/log.py
--rw-r--r--   0        0        0    99683 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/metrics.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/min-es-version.txt
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/paths.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/racecontrol.py
--rw-r--r--   0        0        0    57243 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/rally.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/rallyd.py
--rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/reporter.py
--rw-r--r--   0        0        0   109610 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/telemetry.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/time.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/version.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/client/__init__.py
--rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/client/asynchronous.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/client/common.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/client/context.py
--rw-r--r--   0        0        0    21809 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/client/factory.py
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/client/synchronous.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/driver/__init__.py
--rw-r--r--   0        0        0   110525 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/driver/driver.py
--rw-r--r--   0        0        0   121685 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/driver/runner.py
--rw-r--r--   0        0        0    11927 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/driver/scheduler.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/__init__.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/cluster.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/java_resolver.py
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/launcher.py
--rw-r--r--   0        0        0    28952 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/mechanic.py
--rw-r--r--   0        0        0    22380 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/provisioner.py
--rw-r--r--   0        0        0    45447 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/supplier.py
--rw-r--r--   0        0        0    22353 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/mechanic/team.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/annotation-template.json
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/docker-compose.yml.j2
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/logging.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/metrics-template.json
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/races-template.json
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/rally.ini
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/results-template.json
--rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/track-schema.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/resources/track.json.j2
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/track/__init__.py
--rw-r--r--   0        0        0    84711 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/track/loader.py
--rw-r--r--   0        0        0    58246 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/track/params.py
--rw-r--r--   0        0        0    42605 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/track/track.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/tracker/__init__.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/tracker/corpus.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/tracker/index.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/tracker/tracker.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/__init__.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/collections.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/console.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/convert.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/git.py
--rw-r--r--   0        0        0    19710 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/io.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/jvm.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/modules.py
--rw-r--r--   0        0        0    12648 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/net.py
--rw-r--r--   0        0        0     9245 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/opts.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/process.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/repo.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/sysstats.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 esrally-2.9.0/esrally/utils/versions.py
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 esrally-2.9.0/it/__init__.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 esrally-2.9.0/it/basic_test.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 esrally-2.9.0/it/dependencies_test.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 esrally-2.9.0/it/distribution_test.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 esrally-2.9.0/it/docker_dev_image_test.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 esrally-2.9.0/it/download_test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 esrally-2.9.0/it/error_test.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 esrally-2.9.0/it/esrallyd_test.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 esrally-2.9.0/it/info_test.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 esrally-2.9.0/it/installation_test.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esrally-2.9.0/it/list_test.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 esrally-2.9.0/it/proxy_test.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 esrally-2.9.0/it/sources_test.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 esrally-2.9.0/it/static_responses_test.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 esrally-2.9.0/it/tracker_test.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 esrally-2.9.0/it/resources/rally-es-it.ini
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 esrally-2.9.0/it/resources/rally-in-memory-it.ini
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 esrally-2.9.0/it/resources/static-responses.json
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 esrally-2.9.0/it/resources/squid/squid.conf
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 esrally-2.9.0/it/resources/squid/squidpasswords
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 esrally-2.9.0/it/resources/track_with_dependency/track.json
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 esrally-2.9.0/it/resources/track_with_dependency/track.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 esrally-2.9.0/it/track_repo_compatibility/conftest.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 esrally-2.9.0/recipes/ccr/.elastic-version
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 esrally-2.9.0/recipes/ccr/docker-compose.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esrally-2.9.0/recipes/ccr/metricstore-docker-compose.yml
--rwxr-xr-x   0        0        0     2761 2020-02-02 00:00:00.000000 esrally-2.9.0/recipes/ccr/start.sh
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 esrally-2.9.0/recipes/ccr/stop.sh
--rwxr-xr-x   0        0        0     4406 2020-02-02 00:00:00.000000 esrally-2.9.0/scripts/offline-install.sh
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/__init__.py
--rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/config_test.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/log_test.py
--rw-r--r--   0        0        0   104079 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/metrics_test.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/racecontrol_test.py
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/reporter_test.py
--rw-r--r--   0        0        0   229690 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/telemetry_test.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/time_test.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/client/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/client/asynchronous_test.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/client/common_test.py
--rw-r--r--   0        0        0    28124 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/client/factory_test.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/driver/__init__.py
--rw-r--r--   0        0        0    82934 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/driver/driver_test.py
--rw-r--r--   0        0        0   255790 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/driver/runner_test.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/driver/scheduler_test.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/__init__.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/java_resolver_test.py
--rw-r--r--   0        0        0    16280 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/launcher_test.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/mechanic_test.py
--rw-r--r--   0        0        0    30143 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/provisioner_test.py
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/supplier_test.py
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/team_test.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/32gheap.ini
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/another_with_hook.ini
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/default.ini
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/ea.ini
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/empty_cfg_base.ini
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/missing_cfg_base.ini
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/multi_hook.ini
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/verbose.ini
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/with_hook.ini
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/hook2/config.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/vanilla/config.ini
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/verbose_logging/config.ini
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/cars/v1/with_hook/config.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/plugins/v1/core-plugins.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/plugins/v1/complex_plugin/config-a.ini
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/plugins/v1/complex_plugin/config-b.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/mechanic/data/plugins/v1/my_core_plugin_with_config/.gitkeep
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/track/__init__.py
--rw-r--r--   0        0        0   169325 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/track/loader_test.py
--rw-r--r--   0        0        0   107401 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/track/params_test.py
--rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/track/track_test.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/track/resources/track_fragment_1.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/track/resources/track_fragment_2.json
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/tracker/__init__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/tracker/corpus_test.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/tracker/index_test.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/collections_test.py
--rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/console_test.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/convert_test.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/git_test.py
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/io_test.py
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/jvm_test.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/net_test.py
--rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/opts_test.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/process_test.py
--rw-r--r--   0        0        0    14182 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/repo_test.py
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/versions_test.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/client_options_1.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/client_options_2.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/target_hosts_1.json
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/target_hosts_2.json
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt.bz2
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt.gz
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt.tar
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt.tar.bz2
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt.tar.gz
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt.tgz
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/test.txt.zip
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/certs/ca.crt
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/certs/client.crt
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 esrally-2.9.0/tests/utils/resources/certs/client.key
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 esrally-2.9.0/.gitignore
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esrally-2.9.0/AUTHORS
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 esrally-2.9.0/LICENSE
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 esrally-2.9.0/NOTICE
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 esrally-2.9.0/README.md
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 esrally-2.9.0/pyproject.toml
--rw-r--r--   0        0        0    10271 2020-02-02 00:00:00.000000 esrally-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esrally-2.9.1/.coveragerc
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 esrally-2.9.1/.fossa.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 esrally-2.9.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 esrally-2.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 esrally-2.9.1/.pylintrc
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 esrally-2.9.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    85820 2020-02-02 00:00:00.000000 esrally-2.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 esrally-2.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 esrally-2.9.1/Makefile
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 esrally-2.9.1/catalog-info.yaml
+-rwxr-xr-x   0        0        0     3902 2020-02-02 00:00:00.000000 esrally-2.9.1/changelog.py
+-rwxr-xr-x   0        0        0     4579 2020-02-02 00:00:00.000000 esrally-2.9.1/create-notice.sh
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 esrally-2.9.1/noxfile.py
+-rwxr-xr-x   0        0        0     2169 2020-02-02 00:00:00.000000 esrally-2.9.1/prepare-release.sh
+-rwxr-xr-x   0        0        0     1739 2020-02-02 00:00:00.000000 esrally-2.9.1/rally
+-rwxr-xr-x   0        0        0     1926 2020-02-02 00:00:00.000000 esrally-2.9.1/rallyd
+-rwxr-xr-x   0        0        0     2392 2020-02-02 00:00:00.000000 esrally-2.9.1/release-checks.sh
+-rwxr-xr-x   0        0        0     5573 2020-02-02 00:00:00.000000 esrally-2.9.1/release-docker-test.sh
+-rwxr-xr-x   0        0        0     2409 2020-02-02 00:00:00.000000 esrally-2.9.1/release-docker.sh
+-rwxr-xr-x   0        0        0     4983 2020-02-02 00:00:00.000000 esrally-2.9.1/run.sh
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/pull-requests.json
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/retry.sh
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/it/pipeline.yml
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/it/run.sh
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/it/run_serverless.sh
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/it/serverless-pipeline.yml
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/release-docker/pipeline.yml
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 esrally-2.9.1/.buildkite/release-docker/run.sh
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esrally-2.9.1/.ci/variables.json
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 esrally-2.9.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 esrally-2.9.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 esrally-2.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 esrally-2.9.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/benchmarks/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/benchmarks/driver/__init__.py
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 esrally-2.9.1/benchmarks/driver/parsing_test.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 esrally-2.9.1/benchmarks/driver/runner_test.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/benchmarks/track/__init__.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 esrally-2.9.1/benchmarks/track/bulk_params_test.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 esrally-2.9.1/docker/docker-compose-tests.yml
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 esrally-2.9.1/docker/Dockerfiles/Dockerfile-dev
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 esrally-2.9.1/docker/Dockerfiles/Dockerfile-release
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 esrally-2.9.1/docker/bin/entrypoint.sh
+-rw-r--r--   0        0        0     8234 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/Makefile
+-rw-r--r--   0        0        0    23958 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/adding_tracks.rst
+-rw-r--r--   0        0        0    26756 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/advanced.rst
+-rw-r--r--   0        0        0    18401 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/benchmark_distributed_load.gliffy
+-rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/benchmark_distributed_load.png
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/benchmark_existing.gliffy
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/benchmark_existing.png
+-rw-r--r--   0        0        0    18424 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/benchmark_remote.gliffy
+-rw-r--r--   0        0        0    30736 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/benchmark_remote.png
+-rw-r--r--   0        0        0     9697 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/car.rst
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/cluster_management.rst
+-rw-r--r--   0        0        0    54231 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/command_line_reference.rst
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/community.rst
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/conf.py
+-rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/configuration.rst
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/create_scheduler_plot.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/developing.rst
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/docker.rst
+-rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/elasticsearch_plugins.rst
+-rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/faq.rst
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/glossary.rst
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/index.rst
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/install.rst
+-rw-r--r--   0        0        0   322917 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/jfr-es.png
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/make.bat
+-rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/metrics.rst
+-rw-r--r--   0        0        0    45223 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/migrate.rst
+-rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/nested-streams.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/nested-streams.puml
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/offline.rst
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/pipelines.rst
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/quickstart.rst
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/race.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/rally-logo.svg
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/rally_daemon.rst
+-rw-r--r--   0        0        0    81206 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/recency.png
+-rw-r--r--   0        0        0    22262 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/recipes.rst
+-rw-r--r--   0        0        0    23079 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/schedulers_10s.png
+-rw-r--r--   0        0        0    14727 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/summary_report.rst
+-rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/telemetry.rst
+-rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/tournament.rst
+-rw-r--r--   0        0        0    24101 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/track-ramp-up.png
+-rw-r--r--   0        0        0   159265 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/track.rst
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/versions.rst
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 esrally-2.9.1/docs/architecture/actor_system.md
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/_version.py
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/actor.py
+-rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/config.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/exceptions.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/log.py
+-rw-r--r--   0        0        0    99716 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/metrics.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/min-es-version.txt
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/paths.py
+-rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/racecontrol.py
+-rw-r--r--   0        0        0    57482 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/rally.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/rallyd.py
+-rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/reporter.py
+-rw-r--r--   0        0        0   111298 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/telemetry.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/time.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/version.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/client/__init__.py
+-rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/client/asynchronous.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/client/common.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/client/context.py
+-rw-r--r--   0        0        0    22768 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/client/factory.py
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/client/synchronous.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/driver/__init__.py
+-rw-r--r--   0        0        0   110862 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/driver/driver.py
+-rw-r--r--   0        0        0   121686 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/driver/runner.py
+-rw-r--r--   0        0        0    11927 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/driver/scheduler.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/__init__.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/cluster.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/java_resolver.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/launcher.py
+-rw-r--r--   0        0        0    28952 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/mechanic.py
+-rw-r--r--   0        0        0    22380 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/provisioner.py
+-rw-r--r--   0        0        0    45447 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/supplier.py
+-rw-r--r--   0        0        0    22353 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/mechanic/team.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/annotation-template.json
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/docker-compose.yml.j2
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/logging.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/metrics-template.json
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/races-template.json
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/rally.ini
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/results-template.json
+-rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/track-schema.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/resources/track.json.j2
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/track/__init__.py
+-rw-r--r--   0        0        0    84739 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/track/loader.py
+-rw-r--r--   0        0        0    58246 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/track/params.py
+-rw-r--r--   0        0        0    42584 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/track/track.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/tracker/__init__.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/tracker/corpus.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/tracker/index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/tracker/tracker.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/__init__.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/collections.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/console.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/convert.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/git.py
+-rw-r--r--   0        0        0    19710 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/io.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/jvm.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/modules.py
+-rw-r--r--   0        0        0    12648 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/net.py
+-rw-r--r--   0        0        0     9245 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/opts.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/process.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/repo.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/serverless.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/sysstats.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 esrally-2.9.1/esrally/utils/versions.py
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 esrally-2.9.1/it/__init__.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 esrally-2.9.1/it/basic_test.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 esrally-2.9.1/it/dependencies_test.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 esrally-2.9.1/it/distribution_test.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 esrally-2.9.1/it/docker_dev_image_test.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 esrally-2.9.1/it/download_test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 esrally-2.9.1/it/error_test.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 esrally-2.9.1/it/esrallyd_test.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 esrally-2.9.1/it/info_test.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 esrally-2.9.1/it/installation_test.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esrally-2.9.1/it/list_test.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 esrally-2.9.1/it/proxy_test.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 esrally-2.9.1/it/sources_test.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 esrally-2.9.1/it/static_responses_test.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 esrally-2.9.1/it/tracker_test.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 esrally-2.9.1/it/resources/rally-es-it.ini
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 esrally-2.9.1/it/resources/rally-in-memory-it.ini
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 esrally-2.9.1/it/resources/static-responses.json
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 esrally-2.9.1/it/resources/squid/squid.conf
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 esrally-2.9.1/it/resources/squid/squidpasswords
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 esrally-2.9.1/it/resources/track_with_dependency/track.json
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 esrally-2.9.1/it/resources/track_with_dependency/track.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 esrally-2.9.1/it/track_repo_compatibility/conftest.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 esrally-2.9.1/it_serverless/serverless_test.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 esrally-2.9.1/recipes/ccr/.elastic-version
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 esrally-2.9.1/recipes/ccr/docker-compose.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esrally-2.9.1/recipes/ccr/metricstore-docker-compose.yml
+-rwxr-xr-x   0        0        0     2761 2020-02-02 00:00:00.000000 esrally-2.9.1/recipes/ccr/start.sh
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 esrally-2.9.1/recipes/ccr/stop.sh
+-rwxr-xr-x   0        0        0     4406 2020-02-02 00:00:00.000000 esrally-2.9.1/scripts/offline-install.sh
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/__init__.py
+-rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/config_test.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/log_test.py
+-rw-r--r--   0        0        0   104079 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/metrics_test.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/racecontrol_test.py
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/reporter_test.py
+-rw-r--r--   0        0        0   232297 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/telemetry_test.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/time_test.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/client/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/client/asynchronous_test.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/client/common_test.py
+-rw-r--r--   0        0        0    28124 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/client/factory_test.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/driver/__init__.py
+-rw-r--r--   0        0        0    82934 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/driver/driver_test.py
+-rw-r--r--   0        0        0   255790 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/driver/runner_test.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/driver/scheduler_test.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/__init__.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/java_resolver_test.py
+-rw-r--r--   0        0        0    16280 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/launcher_test.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/mechanic_test.py
+-rw-r--r--   0        0        0    30143 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/provisioner_test.py
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/supplier_test.py
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/team_test.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/32gheap.ini
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/another_with_hook.ini
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/default.ini
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/ea.ini
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/empty_cfg_base.ini
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/missing_cfg_base.ini
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/multi_hook.ini
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/verbose.ini
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/with_hook.ini
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/hook2/config.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/vanilla/config.ini
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/verbose_logging/config.ini
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/cars/v1/with_hook/config.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/plugins/v1/core-plugins.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/plugins/v1/complex_plugin/config-a.ini
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/plugins/v1/complex_plugin/config-b.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/mechanic/data/plugins/v1/my_core_plugin_with_config/.gitkeep
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/track/__init__.py
+-rw-r--r--   0        0        0   169325 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/track/loader_test.py
+-rw-r--r--   0        0        0   107401 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/track/params_test.py
+-rw-r--r--   0        0        0    17569 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/track/track_test.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/track/resources/track_fragment_1.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/track/resources/track_fragment_2.json
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/tracker/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/tracker/corpus_test.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/tracker/index_test.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/collections_test.py
+-rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/console_test.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/convert_test.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/git_test.py
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/io_test.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/jvm_test.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/net_test.py
+-rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/opts_test.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/process_test.py
+-rw-r--r--   0        0        0    14182 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/repo_test.py
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/versions_test.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/client_options_1.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/client_options_2.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/target_hosts_1.json
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/target_hosts_2.json
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt.bz2
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt.gz
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt.tar
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt.tar.bz2
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt.tar.gz
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt.tgz
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/test.txt.zip
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/certs/ca.crt
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/certs/client.crt
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 esrally-2.9.1/tests/utils/resources/certs/client.key
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 esrally-2.9.1/.gitignore
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esrally-2.9.1/AUTHORS
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 esrally-2.9.1/LICENSE
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 esrally-2.9.1/NOTICE
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 esrally-2.9.1/README.md
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 esrally-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0    10271 2020-02-02 00:00:00.000000 esrally-2.9.1/PKG-INFO
```

### Comparing `esrally-2.9.0/.pre-commit-config.yaml` & `esrally-2.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/.pylintrc` & `esrally-2.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/CHANGELOG.md` & `esrally-2.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+### 2.9.1
+
+#### Enhancements
+
+* [#1778](https://github.com/elastic/rally/pull/1778): Support API key authentication
+* [#1770](https://github.com/elastic/rally/pull/1770): Exclude telemetry devices based on serverless status
+* [#1768](https://github.com/elastic/rally/pull/1768): Detect serverless operator status automatically
+
+#### Bug Fixes
+
+* [#1772](https://github.com/elastic/rally/pull/1772): Fix "Could not checkout. Do you have uncommitted changes?" error
+
 ### 2.9.0
 
 #### Highlights
 
 * [#1760](https://github.com/elastic/rally/pull/1760): Exclude tasks based on serverless status
 * [#1750](https://github.com/elastic/rally/pull/1750) (Breaking): Inject build_flavor in track templates
```

### Comparing `esrally-2.9.0/CONTRIBUTING.md` & `esrally-2.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/Makefile` & `esrally-2.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/catalog-info.yaml` & `esrally-2.9.1/catalog-info.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
       url: https://esrally.readthedocs.io/en/stable/
 spec:
   type: application
   owner: group:es-perf
   lifecycle: production
   dependsOn:
     - resource:rally-it-pipeline
+    - resource:rally-it-serverless-pipeline
     - resource:rally-releaser-docker-pipeline
 
 
 # Declare Rally's Buildkite IT pipeline.
 # yaml-language-server: $schema=https://gist.githubusercontent.com/elasticmachine/988b80dae436cafea07d9a4a460a011d/raw/e57ee3bed7a6f73077a3f55a38e76e40ec87a7cf/rre.schema.json
 ---
 apiVersion: backstage.io/v1alpha1
@@ -60,14 +61,50 @@
           cronline: "0 14 * * *"
           message: periodic it
       teams:
         es-perf: {}
         everyone:
           access_level: READ_ONLY
 
+# Declare Rally's Buildkite IT pipeline.
+# yaml-language-server: $schema=https://gist.githubusercontent.com/elasticmachine/988b80dae436cafea07d9a4a460a011d/raw/e57ee3bed7a6f73077a3f55a38e76e40ec87a7cf/rre.schema.json
+---
+apiVersion: backstage.io/v1alpha1
+kind: Resource
+metadata:
+  name: rally-it-serverless-pipeline
+  description: Run Rally Serverless integration tests
+  links:
+    - title: Pipeline
+      url: https://buildkite.com/elastic/rally-it-serverless
+
+spec:
+  type: buildkite-pipeline
+  owner: group:es-perf
+  system: buildkite
+
+  implementation:
+    apiVersion: buildkite.elastic.dev/v1
+    kind: Pipeline
+    metadata:
+      name: Rally - IT Serverless
+      description:  Macrobenchmarking framework for Elasticsearch
+    spec:
+      pipeline_file: .buildkite/it/serverless-pipeline.yml
+      repository: elastic/rally
+      schedules:
+        Daily:
+          branch: master
+          cronline: "0 14 * * *"
+          message: periodic it serverless
+      teams:
+        es-perf: {}
+        everyone:
+          access_level: READ_ONLY
+
 # Declare Rally Release Docker pipeline.
 # yaml-language-server: $schema=https://gist.githubusercontent.com/elasticmachine/988b80dae436cafea07d9a4a460a011d/raw/e57ee3bed7a6f73077a3f55a38e76e40ec87a7cf/rre.schema.json
 ---
 apiVersion: backstage.io/v1alpha1
 kind: Resource
 metadata:
   name: rally-release-docker-pipeline
```

### Comparing `esrally-2.9.0/changelog.py` & `esrally-2.9.1/changelog.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/create-notice.sh` & `esrally-2.9.1/create-notice.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/noxfile.py` & `esrally-2.9.1/noxfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,11 +10,17 @@
 @nox.session(python=["3.8", "3.9", "3.10", "3.11"])
 def it(session: nox.Session) -> None:
     session.install(".[develop]")
     session.run("pytest", "-s", "it")
 
 
 @nox.session(python="3")
+def it_serverless(session: nox.Session) -> None:
+    session.install(".[develop]")
+    session.run("pytest", "-s", "it_serverless", *session.posargs)
+
+
+@nox.session(python="3")
 def rally_tracks_compat(session: nox.Session) -> None:
     session.install(".[develop]")
     session.install("pytest-rally @ git+https://github.com/elastic/pytest-rally.git")
     session.run("pytest", "it/track_repo_compatibility", "--log-cli-level=INFO")
```

### Comparing `esrally-2.9.0/prepare-release.sh` & `esrally-2.9.1/prepare-release.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/rally` & `esrally-2.9.1/rally`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/rallyd` & `esrally-2.9.1/rallyd`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/release-checks.sh` & `esrally-2.9.1/release-checks.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/release-docker-test.sh` & `esrally-2.9.1/release-docker-test.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/release-docker.sh` & `esrally-2.9.1/release-docker.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/run.sh` & `esrally-2.9.1/run.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/.buildkite/release-docker/run.sh` & `esrally-2.9.1/.buildkite/retry.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-#!/usr/bin/env bash
-
-set -eo pipefail
-
 # based on https://gist.github.com/sj26/88e1c6584397bb7c13bd11108a579746?permalink_comment_id=4155247#gistcomment-4155247
 function retry {
   local retries=$1
   shift
   local cmd=($@)
   local cmd_string="${@}"
   local count=0
@@ -28,20 +24,8 @@
       return $retcode
     fi
   done
   # restore settings to fail immediately on error
   set -o errexit
   set -o pipefail
   return 0
-}
-
-set +x
-RELEASE_VERSION=$(buildkite-agent meta-data get RELEASE_VERSION)
-# login to docker registry
-DOCKER_PASSWORD=$(vault read -field token /secret/ci/elastic-rally/release/docker-hub-rally)
-retry 5 docker login -u elasticmachine -p $DOCKER_PASSWORD
-unset DOCKER_PASSWORD
-
-set -x
-export TERM=dumb
-export LC_ALL=en_US.UTF-8
-./release-docker.sh "$RELEASE_VERSION"
+}
```

### Comparing `esrally-2.9.0/.github/ISSUE_TEMPLATE.md` & `esrally-2.9.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/.github/PULL_REQUEST_TEMPLATE.md` & `esrally-2.9.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/.github/workflows/ci.yml` & `esrally-2.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/.github/workflows/release.yml` & `esrally-2.9.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/benchmarks/__init__.py` & `esrally-2.9.1/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/benchmarks/driver/__init__.py` & `esrally-2.9.1/benchmarks/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/benchmarks/driver/parsing_test.py` & `esrally-2.9.1/benchmarks/driver/parsing_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/benchmarks/driver/runner_test.py` & `esrally-2.9.1/benchmarks/driver/runner_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/benchmarks/track/__init__.py` & `esrally-2.9.1/benchmarks/track/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/benchmarks/track/bulk_params_test.py` & `esrally-2.9.1/benchmarks/track/bulk_params_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docker/docker-compose-tests.yml` & `esrally-2.9.1/docker/docker-compose-tests.yml`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docker/Dockerfiles/Dockerfile-dev` & `esrally-2.9.1/docker/Dockerfiles/Dockerfile-dev`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docker/Dockerfiles/Dockerfile-release` & `esrally-2.9.1/docker/Dockerfiles/Dockerfile-release`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/Makefile` & `esrally-2.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/adding_tracks.rst` & `esrally-2.9.1/docs/adding_tracks.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/advanced.rst` & `esrally-2.9.1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/benchmark_distributed_load.gliffy` & `esrally-2.9.1/docs/benchmark_distributed_load.gliffy`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/benchmark_distributed_load.png` & `esrally-2.9.1/docs/benchmark_distributed_load.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/benchmark_existing.gliffy` & `esrally-2.9.1/docs/benchmark_existing.gliffy`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/benchmark_existing.png` & `esrally-2.9.1/docs/benchmark_existing.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/benchmark_remote.gliffy` & `esrally-2.9.1/docs/benchmark_remote.gliffy`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/benchmark_remote.png` & `esrally-2.9.1/docs/benchmark_remote.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/car.rst` & `esrally-2.9.1/docs/car.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/cluster_management.rst` & `esrally-2.9.1/docs/cluster_management.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/command_line_reference.rst` & `esrally-2.9.1/docs/command_line_reference.rst`

 * *Files 1% similar despite different names*

```diff
@@ -707,20 +707,24 @@
 Rally recognizes the following client options in addition:
 
 * ``max_connections``: By default, Rally will choose the maximum allowed number of connections automatically (equal to the number of simulated clients but at least 256 connections). With this property it is possible to override that logic but a minimum of 256 is enforced internally.
 * ``enable_cleanup_closed`` (default: ``true``): In some cases, `Elasticsearch does not properly close SSL connections <https://github.com/elastic/elasticsearch/issues/76642>`_ and the number of open connections increases as a result. When this client option is set to ``true``, the Elasticsearch client will check and forcefully close these connections.
 * ``static_responses``: The path to a JSON file containing path patterns and the corresponding responses. When this value is set to ``true``, Rally will not send requests to Elasticsearch but return static responses as specified by the file. This is useful to diagnose performance issues in Rally itself. See below for a specific example.
 * ``create_api_key_per_client`` (default: ``false``): If set to ``true``, Rally will create a unique `Elasticsearch API key <https://www.elastic.co/guide/en/elasticsearch/reference/current/security-api-create-api-key.html>`_ for each simulated client that issues requests against Elasticsearch during the benchmark. This is useful for simulating workloads where data is indexed by many distinct agents, each configured with its own API key, as is typical with Elastic Agent. Note that ``basic_auth_user`` and ``basic_auth_password`` must also be provided, and the ``basic_auth_user`` must have `sufficient privileges <https://www.elastic.co/guide/en/elasticsearch/reference/current/security-api-create-api-key.html#security-api-create-api-key-prereqs>`_ to create API keys. These basic auth credentials are used to create the API keys at the start of the benchmark and delete them at the end, but only the generated API keys will be used during benchmark execution.
 
-**Examples**
+**Authentication**
 
-Here are a few common examples:
+You can choose between two authentication modes:
 
-* Enable HTTP compression: ``--client-options="http_compress:true"``
-* Enable basic authentication: ``--client-options="basic_auth_user:'user',basic_auth_password:'password'"``. Avoid the characters ``'``, ``,`` and ``:`` in user name and password as Rally's parsing of these options is currently really simple and there is no possibility to escape characters.
+* API key authentication (preferred): ``--client-options="api_key:'a0V...2dw=='"``
+* Basic authentication: ``--client-options="basic_auth_user:'user',basic_auth_password:'password'"``. Avoid the characters ``'``, ``,`` and ``:`` in user name and password as Rally's parsing of these options is currently really simple and there is no possibility to escape characters.
+
+**HTTP compression**
+
+Enable HTTP compression using ``--client-options="http_compress:true"``.
 
 **TLS/SSL**
 
 This is applicable e.g. if you have X-Pack Security installed.
 Enable it with ``use_ssl:true``.
 
 **TLS/SSL Certificate Verification**
```

### Comparing `esrally-2.9.0/docs/community.rst` & `esrally-2.9.1/docs/community.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/conf.py` & `esrally-2.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/configuration.rst` & `esrally-2.9.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/create_scheduler_plot.py` & `esrally-2.9.1/docs/create_scheduler_plot.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/developing.rst` & `esrally-2.9.1/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/docker.rst` & `esrally-2.9.1/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/elasticsearch_plugins.rst` & `esrally-2.9.1/docs/elasticsearch_plugins.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/faq.rst` & `esrally-2.9.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/glossary.rst` & `esrally-2.9.1/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/index.rst` & `esrally-2.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/install.rst` & `esrally-2.9.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/jfr-es.png` & `esrally-2.9.1/docs/jfr-es.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/make.bat` & `esrally-2.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/metrics.rst` & `esrally-2.9.1/docs/metrics.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/migrate.rst` & `esrally-2.9.1/docs/migrate.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/nested-streams.png` & `esrally-2.9.1/docs/nested-streams.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/offline.rst` & `esrally-2.9.1/docs/offline.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/pipelines.rst` & `esrally-2.9.1/docs/pipelines.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/quickstart.rst` & `esrally-2.9.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/race.rst` & `esrally-2.9.1/docs/race.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/rally-logo.svg` & `esrally-2.9.1/docs/rally-logo.svg`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/rally_daemon.rst` & `esrally-2.9.1/docs/rally_daemon.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/recency.png` & `esrally-2.9.1/docs/recency.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/recipes.rst` & `esrally-2.9.1/docs/recipes.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/schedulers_10s.png` & `esrally-2.9.1/docs/schedulers_10s.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/summary_report.rst` & `esrally-2.9.1/docs/summary_report.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/telemetry.rst` & `esrally-2.9.1/docs/telemetry.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/tournament.rst` & `esrally-2.9.1/docs/tournament.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/track-ramp-up.png` & `esrally-2.9.1/docs/track-ramp-up.png`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/track.rst` & `esrally-2.9.1/docs/track.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/versions.rst` & `esrally-2.9.1/docs/versions.rst`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/_templates/breadcrumbs.html` & `esrally-2.9.1/docs/_templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/docs/architecture/actor_system.md` & `esrally-2.9.1/docs/architecture/actor_system.md`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/__init__.py` & `esrally-2.9.1/esrally/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/actor.py` & `esrally-2.9.1/esrally/actor.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/config.py` & `esrally-2.9.1/esrally/config.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/exceptions.py` & `esrally-2.9.1/esrally/exceptions.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/log.py` & `esrally-2.9.1/esrally/log.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/metrics.py` & `esrally-2.9.1/esrally/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,17 @@
             client_options["ca_certs"] = ca_path
         if user and password:
             client_options["basic_auth_user"] = user
             client_options["basic_auth_password"] = password
 
         # TODO #1335: Use version-specific support for metrics stores after 7.8.0.
         if self.probe_version:
-            distribution_flavor, distribution_version, _ = client.cluster_distribution_version(hosts=hosts, client_options=client_options)
+            distribution_flavor, distribution_version, _, _ = client.cluster_distribution_version(
+                hosts=hosts, client_options=client_options
+            )
             self._cluster_version = distribution_version
 
         factory = client.EsClientFactory(
             hosts=hosts,
             client_options=client_options,
             distribution_version=distribution_version,
             distribution_flavor=distribution_flavor,
```

### Comparing `esrally-2.9.0/esrally/paths.py` & `esrally-2.9.1/esrally/paths.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/racecontrol.py` & `esrally-2.9.1/esrally/racecontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,33 +182,36 @@
     def setup(self, sources=False):
         # to load the track we need to know the correct cluster distribution version. Usually, this value should be set
         # but there are rare cases (external pipeline and user did not specify the distribution version) where we need
         # to derive it ourselves. For source builds we always assume "main"
         if not sources and not self.cfg.exists("mechanic", "distribution.version"):
             hosts = self.cfg.opts("client", "hosts").default
             client_options = self.cfg.opts("client", "options").default
-            distribution_flavor, distribution_version, distribution_build_hash = client.factory.cluster_distribution_version(
-                hosts, client_options
-            )
+            (
+                distribution_flavor,
+                distribution_version,
+                distribution_build_hash,
+                serverless_operator,
+            ) = client.factory.cluster_distribution_version(hosts, client_options)
 
             self.logger.info(
                 "Automatically derived distribution flavor [%s], version [%s], and build hash [%s]",
                 distribution_flavor,
                 distribution_version,
                 distribution_build_hash,
             )
             self.cfg.add(config.Scope.benchmark, "mechanic", "distribution.version", distribution_version)
             self.cfg.add(config.Scope.benchmark, "mechanic", "distribution.flavor", distribution_flavor)
             if versions.is_serverless(distribution_flavor):
                 if not self.cfg.exists("driver", "serverless.mode"):
                     self.cfg.add(config.Scope.benchmark, "driver", "serverless.mode", True)
 
                 if not self.cfg.exists("driver", "serverless.operator"):
-                    # operator privileges assumed for now
-                    self.cfg.add(config.Scope.benchmark, "driver", "serverless.operator", True)
+                    self.cfg.add(config.Scope.benchmark, "driver", "serverless.operator", serverless_operator)
+                console.info(f"Detected Elasticsearch Serverless mode with operator=[{serverless_operator}].")
             else:
                 min_es_version = versions.Version.from_string(version.minimum_es_version())
                 specified_version = versions.Version.from_string(distribution_version)
                 if specified_version < min_es_version:
                     raise exceptions.SystemSetupError(
                         f"Cluster version must be at least [{min_es_version}] but was [{distribution_version}]"
                     )
```

### Comparing `esrally-2.9.0/esrally/rally.py` & `esrally-2.9.1/esrally/rally.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,17 @@
         if v:
             min_es_version = versions.Version.from_string(version.minimum_es_version())
             specified_version = versions.Version.from_string(v)
             if specified_version < min_es_version:
                 raise argparse.ArgumentTypeError(f"must be at least {min_es_version} but was {v}")
         return v
 
+    def revision(v):
+        return v.strip()
+
     def add_track_source(subparser):
         track_source_group = subparser.add_mutually_exclusive_group()
         track_source_group.add_argument(
             "--track-repository",
             help="Define the repository from where Rally will load tracks (default: default).",
             # argparse is smart enough to use this default only if the user did not use --track-path and also did not specify anything
             default="default",
@@ -110,14 +113,15 @@
             "--track-path",
             help="Define the path to a track.",
         )
         subparser.add_argument(
             "--track-revision",
             help="Define a specific revision in the track repository that Rally should use.",
             default=None,
+            type=revision,
         )
 
     # try to preload configurable defaults, but this does not work together with `--configuration-name` (which is undocumented anyway)
     cfg = config.Config()
     if cfg.config_present():
         cfg.load_config()
         preserve_install = cfg.opts("defaults", "preserve_benchmark_candidate", default_value=False, mandatory=False)
@@ -291,14 +295,15 @@
         "--revision",
         help="Define the source code revision for building the benchmark candidate. 'current' uses the source tree as is,"
         " 'latest' fetches the latest version on the main branch. It is also possible to specify a commit id or a timestamp."
         ' The timestamp must be specified as: "@ts" where "ts" must be a valid ISO 8601 timestamp, '
         'e.g. "@2013-07-27T10:37:00Z" (default: current). A combination of branch and timestamp is also possible,'
         'e.g. "@feature-branch@2023-04-06T14:52:31Z".',
         default="current",
+        type=revision,
     )  # optimized for local usage, don't fetch sources
     build_parser.add_argument(
         "--target-os",
         help="The name of the target operating system for which an artifact should be downloaded (default: current OS)",
     )
     build_parser.add_argument(
         "--target-arch",
@@ -309,14 +314,15 @@
         help="Define the repository from where Rally will load teams and cars (default: default).",
         default="default",
     )
     build_parser.add_argument(
         "--team-revision",
         help="Define a specific revision in the team repository that Rally should use.",
         default=None,
+        type=revision,
     )
     build_parser.add_argument(
         "--team-path",
         help="Define the path to the car and plugin configurations to use.",
     )
     build_parser.add_argument(
         "--car",
@@ -351,14 +357,15 @@
         help="Define the repository from where Rally will load teams and cars (default: default).",
         default="default",
     )
     download_parser.add_argument(
         "--team-revision",
         help="Define a specific revision in the team repository that Rally should use.",
         default=None,
+        type=revision,
     )
     download_parser.add_argument(
         "--team-path",
         help="Define the path to the car and plugin configurations to use.",
     )
     download_parser.add_argument(
         "--distribution-version",
@@ -395,14 +402,15 @@
     install_parser.add_argument(
         "--revision",
         help="Define the source code revision for building the benchmark candidate. 'current' uses the source tree as is,"
         " 'latest' fetches the latest version on the main branch. It is also possible to specify a commit id or a timestamp."
         ' The timestamp must be specified as: "@ts" where "ts" must be a valid ISO 8601 timestamp, '
         'e.g. "@2013-07-27T10:37:00Z" (default: current).',
         default="current",
+        type=revision,
     )  # optimized for local usage, don't fetch sources
     # Intentionally undocumented as we do not consider Docker a fully supported option.
     install_parser.add_argument(
         "--build-type",
         help=argparse.SUPPRESS,
         choices=["tar", "docker"],
         default="tar",
@@ -412,14 +420,15 @@
         help="Define the repository from where Rally will load teams and cars (default: default).",
         default="default",
     )
     install_parser.add_argument(
         "--team-revision",
         help="Define a specific revision in the team repository that Rally should use.",
         default=None,
+        type=revision,
     )
     install_parser.add_argument(
         "--team-path",
         help="Define the path to the car and plugin configurations to use.",
     )
     install_parser.add_argument(
         "--runtime-jdk",
@@ -567,14 +576,15 @@
             help="Define the repository from where Rally will load teams and cars (default: default).",
             default="default",
         )
         p.add_argument(
             "--team-revision",
             help="Define a specific revision in the team repository that Rally should use.",
             default=None,
+            type=revision,
         )
 
     race_parser.add_argument(
         "--race-id",
         help="Define a unique id for this race.",
         default=str(uuid.uuid4()),
     )
@@ -587,14 +597,15 @@
     race_parser.add_argument(
         "--revision",
         help="Define the source code revision for building the benchmark candidate. 'current' uses the source tree as is,"
         " 'latest' fetches the latest version on master. It is also possible to specify a commit id or a timestamp."
         ' The timestamp must be specified as: "@ts" where "ts" must be a valid ISO 8601 timestamp, '
         'e.g. "@2013-07-27T10:37:00Z" (default: current).',
         default="current",
+        type=revision,
     )  # optimized for local usage, don't fetch sources
     add_track_source(race_parser)
     race_parser.add_argument(
         "--track",
         help=f"Define the track to use. List possible tracks with `{PROGRAM_NAME} list tracks`.",
     )
     race_parser.add_argument(
```

### Comparing `esrally-2.9.0/esrally/rallyd.py` & `esrally-2.9.1/esrally/rallyd.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/reporter.py` & `esrally-2.9.1/esrally/reporter.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/telemetry.py` & `esrally-2.9.1/esrally/telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import threading
 
 import tabulate
 
 from esrally import exceptions, metrics, time
 from esrally.metrics import MetaInfoScope
-from esrally.utils import console, io, opts, process, sysstats
+from esrally.utils import console, io, opts, process, serverless, sysstats
 from esrally.utils.versions import Version
 
 
 def list_telemetry():
     console.println("Available telemetry devices:\n")
     devices = [
         [device.command, device.human_name, device.help]
@@ -51,21 +51,23 @@
         ]
     ]
     console.println(tabulate.tabulate(devices, ["Command", "Name", "Description"]))
     console.println("\nKeep in mind that each telemetry device may incur a runtime overhead which can skew results.")
 
 
 class Telemetry:
-    def __init__(self, enabled_devices=None, devices=None):
+    def __init__(self, enabled_devices=None, devices=None, serverless_mode=False, serverless_operator=False):
         if devices is None:
             devices = []
         if enabled_devices is None:
             enabled_devices = []
         self.enabled_devices = enabled_devices
         self.devices = devices
+        self.serverless_mode = serverless_mode
+        self.serverless_operator = serverless_operator
 
     def instrument_candidate_java_opts(self):
         opts = []
         for device in self.devices:
             if self._enabled(device):
                 additional_opts = device.instrument_java_opts()
                 # properly merge values with the same key
@@ -86,14 +88,20 @@
         for device in self.devices:
             if self._enabled(device):
                 device.detach_from_node(node, running)
 
     def on_benchmark_start(self):
         for device in self.devices:
             if self._enabled(device):
+                if self.serverless_mode and not self._available_on_serverless(device):
+                    # Only inform about exclusion if the user explicitly asked for this device
+                    if getattr(device, "command", None) in self.enabled_devices:
+                        console.info(f"Excluding telemetry device [{device.command}] as it is unavailable on serverless.")
+                    continue
+
                 device.on_benchmark_start()
 
     def on_benchmark_stop(self):
         for device in self.devices:
             if self._enabled(device):
                 device.on_benchmark_stop()
 
@@ -101,14 +109,20 @@
         for device in self.devices:
             if self._enabled(device):
                 device.store_system_metrics(node, metrics_store)
 
     def _enabled(self, device):
         return device.internal or device.command in self.enabled_devices
 
+    def _available_on_serverless(self, device):
+        if self.serverless_operator:
+            return device.serverless_status >= serverless.Status.Internal
+        else:
+            return device.serverless_status == serverless.Status.Public
+
 
 ########################################################################################
 #
 # Telemetry devices
 #
 ########################################################################################
 
@@ -336,14 +350,15 @@
             cmd = f"jmap -dump:format=b,file={heap_dump_file} {node.pid}"
             if process.run_subprocess_with_logging(cmd):
                 self.logger.warning("Could not write heap dump to [%s]", heap_dump_file)
 
 
 class SegmentStats(TelemetryDevice):
     internal = False
+    serverless_status = serverless.Status.Internal
     command = "segment-stats"
     human_name = "Segment Stats"
     help = "Determines segment stats at the end of the benchmark."
 
     def __init__(self, log_root, client):
         super().__init__()
         self.log_root = log_root
@@ -359,14 +374,15 @@
                 f.write(segment_stats)
         except BaseException:
             self.logger.exception("Could not retrieve segment stats.")
 
 
 class CcrStats(TelemetryDevice):
     internal = False
+    serverless_status = serverless.Status.Blocked
     command = "ccr-stats"
     human_name = "CCR Stats"
     help = "Regularly samples Cross Cluster Replication (CCR) related stats"
 
     """
     Gathers CCR stats on a cluster level
     """
@@ -503,14 +519,15 @@
                 shard_metadata = {"cluster": self.cluster_name, "index": name}
 
                 self.metrics_store.put_doc(doc, level=MetaInfoScope.cluster, meta_data=shard_metadata)
 
 
 class RecoveryStats(TelemetryDevice):
     internal = False
+    serverless_status = serverless.Status.Internal
     command = "recovery-stats"
     human_name = "Recovery Stats"
     help = "Regularly samples shard recovery stats"
 
     """
     Gathers recovery stats on a cluster level
     """
@@ -629,14 +646,15 @@
 
 class ShardStats(TelemetryDevice):
     """
     Collects and pushes shard stats for the specified cluster to the metric store.
     """
 
     internal = False
+    serverless_status = serverless.Status.Internal
     command = "shard-stats"
     human_name = "Shard Stats"
     help = "Regularly samples nodes stats at shard level"
 
     def __init__(self, telemetry_params, clients, metrics_store):
         """
         :param telemetry_params: The configuration object for telemetry_params.
@@ -736,14 +754,15 @@
 
 class NodeStats(TelemetryDevice):
     """
     Gathers different node stats.
     """
 
     internal = False
+    serverless_status = serverless.Status.Internal
     command = "node-stats"
     human_name = "Node Stats"
     help = "Regularly samples node stats"
     warning = """You have enabled the node-stats telemetry device with Elasticsearch < 7.2.0. Requests to the
           _nodes/stats Elasticsearch endpoint trigger additional refreshes and WILL SKEW results.
     """
 
@@ -920,14 +939,15 @@
             logging.getLogger(__name__).exception("Could not retrieve node stats.")
             return {}
         return stats["nodes"].values()
 
 
 class TransformStats(TelemetryDevice):
     internal = False
+    serverless_status = serverless.Status.Public
     command = "transform-stats"
     human_name = "Transform Stats"
     help = "Regularly samples transform stats"
 
     """
     Gathers Transform stats
     """
@@ -1098,14 +1118,15 @@
         if processing_time > 0:
             throughput = documents_processed / processing_time * 1000
             self.metrics_store.put_value_cluster_level(prefix + "transform_throughput", throughput, "docs/s", meta_data=meta_data)
 
 
 class SearchableSnapshotsStats(TelemetryDevice):
     internal = False
+    serverless_status = serverless.Status.Blocked
     command = "searchable-snapshots-stats"
     human_name = "Searchable Snapshots Stats"
     help = "Regularly samples searchable snapshots stats"
 
     """
     Gathers searchable snapshots stats on a cluster level
     """
@@ -1293,14 +1314,15 @@
 
 class DataStreamStats(TelemetryDevice):
     """
     Collects and pushes data stream stats for the specified cluster to the metric store.
     """
 
     internal = False
+    serverless_status = serverless.Status.Public
     command = "data-stream-stats"
     human_name = "Data Stream Stats"
     help = "Regularly samples data stream stats"
 
     def __init__(self, telemetry_params, clients, metrics_store):
         """
         :param telemetry_params: The configuration object for telemetry_params.
@@ -1411,14 +1433,15 @@
                 "maximum_timestamp": ds["maximum_timestamp"],
             }
             self.metrics_store.put_doc(doc, level=MetaInfoScope.cluster, meta_data=data_stream_metadata)
 
 
 class IngestPipelineStats(InternalTelemetryDevice):
     command = "ingest-pipeline-stats"
+    serverless_status = serverless.Status.Internal
     human_name = "Ingest Pipeline Stats"
     help = "Reports Ingest Pipeline stats at the end of the benchmark."
 
     def __init__(self, clients, metrics_store):
         super().__init__()
         self.logger = logging.getLogger(__name__)
         self.clients = clients
@@ -1758,14 +1781,16 @@
 
 
 class ClusterEnvironmentInfo(InternalTelemetryDevice):
     """
     Gathers static environment information on a cluster level (e.g. version numbers).
     """
 
+    serverless_status = serverless.Status.Public
+
     def __init__(self, client, metrics_store, revision_override):
         super().__init__()
         self.metrics_store = metrics_store
         self.client = client
         self.revision_override = revision_override
 
     def on_benchmark_start(self):
@@ -1814,14 +1839,16 @@
 
 
 class ExternalEnvironmentInfo(InternalTelemetryDevice):
     """
     Gathers static environment information for externally provisioned clusters.
     """
 
+    serverless_status = serverless.Status.Internal
+
     def __init__(self, client, metrics_store):
         super().__init__()
         self.metrics_store = metrics_store
         self.client = client
 
     # noinspection PyBroadException
     def on_benchmark_start(self):
@@ -1858,14 +1885,16 @@
 
 
 class JvmStatsSummary(InternalTelemetryDevice):
     """
     Gathers a summary of various JVM statistics during the whole race.
     """
 
+    serverless_status = serverless.Status.Internal
+
     def __init__(self, client, metrics_store):
         super().__init__()
         self.metrics_store = metrics_store
         self.client = client
         self.jvm_stats_per_node = {}
 
     def on_benchmark_start(self):
@@ -1946,14 +1975,16 @@
 
 
 class IndexStats(InternalTelemetryDevice):
     """
     Gathers statistics via the Elasticsearch index stats API
     """
 
+    serverless_status = serverless.Status.Internal
+
     def __init__(self, client, metrics_store):
         super().__init__()
         self.client = client
         self.metrics_store = metrics_store
         self.first_time = True
 
     def on_benchmark_start(self):
@@ -2074,14 +2105,16 @@
             return value
         except KeyError:
             self.logger.warning("Could not determine value at path [%s]. Returning default value [%s]", ",".join(path), str(default_value))
             return default_value
 
 
 class MlBucketProcessingTime(InternalTelemetryDevice):
+    serverless_status = serverless.Status.Public
+
     def __init__(self, client, metrics_store):
         super().__init__()
         self.client = client
         self.metrics_store = metrics_store
 
     def on_benchmark_stop(self):
         # pylint: disable=import-outside-toplevel
@@ -2172,14 +2205,15 @@
 
 
 class MasterNodeStats(InternalTelemetryDevice):
     """
     Collects and pushes the current master node name to the metric store.
     """
 
+    serverless_status = serverless.Status.Internal
     command = "master-node-stats"
     human_name = "Master Node Stats"
     help = "Regularly samples master node name"
 
     def __init__(self, telemetry_params, client, metrics_store):
         """
         :param telemetry_params: The configuration object for telemetry_params.
@@ -2262,14 +2296,15 @@
 
 class DiskUsageStats(TelemetryDevice):
     """
     Measures the space taken by each field
     """
 
     internal = False
+    serverless_status = serverless.Status.Internal
     command = "disk-usage-stats"
     human_name = "Disk usage of each field"
     help = "Runs the indices disk usage API after benchmarking"
 
     def __init__(self, telemetry_params, client, metrics_store, index_names, data_stream_names):
         """
         :param telemetry_params: The configuration object for telemetry_params.
@@ -2364,14 +2399,15 @@
                 knn_vectors = field_info.get("knn_vectors_in_bytes", 0)
                 if knn_vectors > 0:
                     self.metrics_store.put_value_cluster_level("disk_usage_knn_vectors", knn_vectors, meta_data=meta, unit="byte")
 
 
 class BlobStoreStats(TelemetryDevice):
     internal = False
+    serverless_status = serverless.Status.Internal
     command = "blob-store-stats"
     human_name = "Blob Store Stats"
     help = "Regularly samples blob store stats, only applicable to serverless Elasticsearch"
 
     """
     Gathers blob snapshots stats on both a cluster and node level
     """
```

### Comparing `esrally-2.9.0/esrally/time.py` & `esrally-2.9.1/esrally/time.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/version.py` & `esrally-2.9.1/esrally/version.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/client/__init__.py` & `esrally-2.9.1/esrally/client/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/client/asynchronous.py` & `esrally-2.9.1/esrally/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/client/common.py` & `esrally-2.9.1/esrally/client/common.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/client/context.py` & `esrally-2.9.1/esrally/client/context.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/client/factory.py` & `esrally-2.9.1/esrally/client/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         self.logger = logging.getLogger(__name__)
 
         masked_client_options = dict(client_options)
         if "basic_auth_password" in masked_client_options:
             masked_client_options["basic_auth_password"] = "*****"
         if "http_auth" in masked_client_options:
             masked_client_options["http_auth"] = (masked_client_options["http_auth"][0], "*****")
+        if "api_key" in masked_client_options:
+            masked_client_options["api_key"] = "*****"
         self.logger.info("Creating ES client connected to %s with options [%s]", hosts, masked_client_options)
 
         # we're using an SSL context now and it is not allowed to have use_ssl present in client options anymore
         if self.client_options.pop("use_ssl", False):
             # pylint: disable=import-outside-toplevel
             import ssl
 
@@ -136,14 +138,19 @@
 
         if self._is_set(self.client_options, "basic_auth_user") and self._is_set(self.client_options, "basic_auth_password"):
             self.client_options["basic_auth"] = (self.client_options.pop("basic_auth_user"), self.client_options.pop("basic_auth_password"))
             self.logger.debug("HTTP basic authentication: on")
         else:
             self.logger.debug("HTTP basic authentication: off")
 
+        if self._is_set(self.client_options, "api_key"):
+            self.logger.debug("API key authentication: on")
+        else:
+            self.logger.debug("API key authentication: off")
+
         if self._is_set(self.client_options, "compressed"):
             console.warn("You set the deprecated client option 'compressed‘. Please use 'http_compress' instead.", logger=self.logger)
             self.client_options["http_compress"] = self.client_options.pop("compressed")
 
         if self._is_set(self.client_options, "http_compress"):
             self.logger.debug("HTTP compression: on")
         else:
@@ -328,29 +335,39 @@
     Attempt to get the target cluster's distribution version, build flavor, and build hash by creating and using
     a 'sync' Elasticsearch client.
 
     :param hosts: The host(s) to connect to.
     :param client_options: The client options to customize the Elasticsearch client.
     :param client_factory: Factory class that creates the Elasticsearch client.
     :return: The cluster's build flavor, version number, and build hash. For Serverless Elasticsearch these may all be
-      the build flavor value.
+      the build flavor value. Also returns the operator status (always False for stateful).
     """
     # no way for us to know whether we're talking to a serverless elasticsearch or not, so we default to the sync client
     es = client_factory(hosts, client_options).create()
-    # unconditionally wait for the REST layer - if it's not up by then, we'll intentionally raise the original error
-    wait_for_rest_layer(es)
+
+    # wait_for_rest_layer  calls the Cluster Health API, which is not available for unprivileged users on Serverless
+    # As a result, we need to call the info API first to know if we can call wait_for_rest_layer().
     version = es.info()["version"]
 
     version_build_flavor = version.get("build_flavor", "oss")
     # build hash will only be available for serverless if the client has operator privs
     version_build_hash = version.get("build_hash", version_build_flavor)
     # version number does not exist for serverless
     version_number = version.get("number", version_build_flavor)
 
-    return version_build_flavor, version_number, version_build_hash
+    serverless_operator = False
+    if versions.is_serverless(version_build_flavor):
+        authentication_info = es.perform_request(method="GET", path="/_security/_authenticate")
+        serverless_operator = authentication_info.body.get("operator", False)
+
+    if not versions.is_serverless(version_build_flavor) or serverless_operator is True:
+        # if available, unconditionally wait for the REST layer - if it's not up, we'll intentionally raise the original error
+        wait_for_rest_layer(es)
+
+    return version_build_flavor, version_number, version_build_hash, serverless_operator
 
 
 def create_api_key(es, client_id, max_attempts=5):
     """
     Creates an API key for the provided ``client_id``.
 
     :param es: Elasticsearch client to use for connecting.
```

### Comparing `esrally-2.9.0/esrally/client/synchronous.py` & `esrally-2.9.1/esrally/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/driver/__init__.py` & `esrally-2.9.1/esrally/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/driver/driver.py` & `esrally-2.9.1/esrally/driver/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -616,15 +616,15 @@
             # Use retries to avoid aborts on long living connections for telemetry devices
             cluster_client_options["retry_on_timeout"] = True
             es[cluster_name] = self.es_client_factory(
                 cluster_hosts, cluster_client_options, distribution_version=distribution_version, distribution_flavor=distribution_flavor
             ).create()
         return es
 
-    def prepare_telemetry(self, es, enable, index_names, data_stream_names, build_hash):
+    def prepare_telemetry(self, es, enable, index_names, data_stream_names, build_hash, serverless_mode, serverless_operator):
         enabled_devices = self.config.opts("telemetry", "devices")
         telemetry_params = self.config.opts("telemetry", "params")
         log_root = paths.race_root(self.config)
 
         es_default = es["default"]
 
         if enable:
@@ -645,15 +645,20 @@
                 telemetry.DataStreamStats(telemetry_params, es, self.metrics_store),
                 telemetry.IngestPipelineStats(es, self.metrics_store),
                 telemetry.DiskUsageStats(telemetry_params, es_default, self.metrics_store, index_names, data_stream_names),
                 telemetry.BlobStoreStats(telemetry_params, es, self.metrics_store),
             ]
         else:
             devices = []
-        self.telemetry = telemetry.Telemetry(enabled_devices, devices=devices)
+        self.telemetry = telemetry.Telemetry(
+            enabled_devices,
+            devices=devices,
+            serverless_mode=serverless_mode,
+            serverless_operator=serverless_operator,
+        )
 
     def wait_for_rest_api(self, es):
         es_default = es["default"]
         self.logger.info("Checking if REST API is available.")
         if client.wait_for_rest_layer(es_default, max_attempts=40):
             self.logger.info("REST API is available.")
         else:
@@ -702,14 +707,16 @@
         )
 
         es_clients = self.create_es_clients()
         self.default_sync_es_client = es_clients["default"]
 
         skip_rest_api_check = self.config.opts("mechanic", "skip.rest.api.check")
         uses_static_responses = self.config.opts("client", "options").uses_static_responses
+        serverless_mode = False
+        serverless_operator = False
         build_hash = None
         if skip_rest_api_check:
             self.logger.info("Skipping REST API check as requested explicitly.")
         elif uses_static_responses:
             self.logger.info("Skipping REST API check as static responses are used.")
         else:
             self.wait_for_rest_api(es_clients)
@@ -725,14 +732,16 @@
         # are not useful and attempts to connect to a non-existing cluster just lead to exception traces in logs.
         self.prepare_telemetry(
             es_clients,
             enable=not uses_static_responses,
             index_names=self.track.index_names(),
             data_stream_names=self.track.data_stream_names(),
             build_hash=build_hash,
+            serverless_mode=serverless_mode,
+            serverless_operator=serverless_operator,
         )
 
         for host in self.config.opts("driver", "load_driver_hosts"):
             host_config = {
                 # for simplicity we assume that all benchmark machines have the same specs
                 "cores": num_cores(self.config)
             }
```

### Comparing `esrally-2.9.0/esrally/driver/runner.py` & `esrally-2.9.1/esrally/driver/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2571,15 +2571,15 @@
 class Composite(Runner):
     """
     Executes a complex request structure which is measured by Rally as one composite operation.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        # Since Composite is marked as ServerlessStatus.Public, only add public
+        # Since Composite is marked as serverless.Status.Public, only add public
         # operation types here.
         self.supported_op_types = [
             "open-point-in-time",
             "close-point-in-time",
             "search",
             "paginated-search",
             "composite-agg",
```

### Comparing `esrally-2.9.0/esrally/driver/scheduler.py` & `esrally-2.9.1/esrally/driver/scheduler.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/__init__.py` & `esrally-2.9.1/esrally/mechanic/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/cluster.py` & `esrally-2.9.1/esrally/mechanic/cluster.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/java_resolver.py` & `esrally-2.9.1/esrally/mechanic/java_resolver.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/launcher.py` & `esrally-2.9.1/esrally/mechanic/launcher.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/mechanic.py` & `esrally-2.9.1/esrally/mechanic/mechanic.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/provisioner.py` & `esrally-2.9.1/esrally/mechanic/provisioner.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/supplier.py` & `esrally-2.9.1/esrally/mechanic/supplier.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/mechanic/team.py` & `esrally-2.9.1/esrally/mechanic/team.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/annotation-template.json` & `esrally-2.9.1/esrally/resources/annotation-template.json`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/docker-compose.yml.j2` & `esrally-2.9.1/esrally/resources/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/logging.json` & `esrally-2.9.1/esrally/resources/logging.json`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/metrics-template.json` & `esrally-2.9.1/esrally/resources/metrics-template.json`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/races-template.json` & `esrally-2.9.1/esrally/resources/races-template.json`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/rally.ini` & `esrally-2.9.1/esrally/resources/rally.ini`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/results-template.json` & `esrally-2.9.1/esrally/resources/results-template.json`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/track-schema.json` & `esrally-2.9.1/esrally/resources/track-schema.json`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/resources/track.json.j2` & `esrally-2.9.1/esrally/resources/track.json.j2`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/track/__init__.py` & `esrally-2.9.1/esrally/track/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/track/loader.py` & `esrally-2.9.1/esrally/track/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,25 @@
 import jsonschema
 import tabulate
 from jinja2 import meta
 
 from esrally import PROGRAM_NAME, config, exceptions, paths, time, version
 from esrally.track import params, track
 from esrally.track.track import Parallel
-from esrally.utils import collections, console, convert, io, modules, net, opts, repo
+from esrally.utils import (
+    collections,
+    console,
+    convert,
+    io,
+    modules,
+    net,
+    opts,
+    repo,
+    serverless,
+)
 
 
 class TrackSyntaxError(exceptions.InvalidSyntax):
     """
     Raised whenever a syntax problem is encountered when loading the track specification.
     """
 
@@ -904,19 +914,19 @@
             return not operation.run_on_serverless
 
         if operation.type == "raw-request":
             self.logger.info("Treating raw-request operation for operation [%s] as public.", operation.name)
 
         try:
             op = track.OperationType.from_hyphenated_string(operation.type)
-            # Comparisons rely on the ordering of auto() in track.ServerlessStatus which is an IntEnum
+            # Comparisons rely on the ordering in serverless.Status which is an IntEnum
             if self.serverless_operator:
-                return op.serverless_status < track.ServerlessStatus.Internal
+                return op.serverless_status < serverless.Status.Internal
             else:
-                return op.serverless_status < track.ServerlessStatus.Public
+                return op.serverless_status < serverless.Status.Public
         except KeyError:
             self.logger.info("Treating user-provided operation type [%s] for operation [%s] as public.", operation.type, operation.name)
             return False
 
     def on_after_load_track(self, track):
         if not self.serverless_mode:
             return track
```

### Comparing `esrally-2.9.0/esrally/track/params.py` & `esrally-2.9.1/esrally/track/params.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/track/track.py` & `esrally-2.9.1/esrally/track/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import collections
 import numbers
 import re
-from enum import Enum, IntEnum, auto, unique
+from enum import Enum, auto, unique
 
 from esrally import exceptions
+from esrally.utils import serverless
 
 
 class Index:
     """
     Defines an index in Elasticsearch.
     """
 
@@ -670,87 +671,80 @@
 class AdminStatus(Enum):
     # We can't use True/False as they are keywords
     Yes = auto()
     No = auto()
 
 
 @unique
-class ServerlessStatus(IntEnum):
-    Blocked = auto()
-    Internal = auto()
-    Public = auto()
-
-
-@unique
 class OperationType(Enum):
     # TODO replace manual counts with auto() when we drop support for Python 3.10
     # https://docs.python.org/3/library/enum.html#enum.auto
-    IndexStats = (1, AdminStatus.No, ServerlessStatus.Internal)
-    NodeStats = (2, AdminStatus.No, ServerlessStatus.Internal)
-    Search = (3, AdminStatus.No, ServerlessStatus.Public)
-    Bulk = (4, AdminStatus.No, ServerlessStatus.Public)
+    IndexStats = (1, AdminStatus.No, serverless.Status.Internal)
+    NodeStats = (2, AdminStatus.No, serverless.Status.Internal)
+    Search = (3, AdminStatus.No, serverless.Status.Public)
+    Bulk = (4, AdminStatus.No, serverless.Status.Public)
     # Public as we can't verify the actual status
-    RawRequest = (5, AdminStatus.No, ServerlessStatus.Public)
-    WaitForRecovery = (6, AdminStatus.No, ServerlessStatus.Internal)
-    WaitForSnapshotCreate = (7, AdminStatus.No, ServerlessStatus.Internal)
+    RawRequest = (5, AdminStatus.No, serverless.Status.Public)
+    WaitForRecovery = (6, AdminStatus.No, serverless.Status.Internal)
+    WaitForSnapshotCreate = (7, AdminStatus.No, serverless.Status.Internal)
     # Public as all supported operation types are Public too (including RawRequest as
     # mentioned above)
-    Composite = (8, AdminStatus.No, ServerlessStatus.Public)
-    SubmitAsyncSearch = (9, AdminStatus.No, ServerlessStatus.Public)
-    GetAsyncSearch = (10, AdminStatus.No, ServerlessStatus.Public)
-    DeleteAsyncSearch = (11, AdminStatus.No, ServerlessStatus.Public)
-    PaginatedSearch = (12, AdminStatus.No, ServerlessStatus.Public)
-    ScrollSearch = (13, AdminStatus.No, ServerlessStatus.Public)
-    OpenPointInTime = (14, AdminStatus.No, ServerlessStatus.Public)
-    ClosePointInTime = (15, AdminStatus.No, ServerlessStatus.Public)
-    Sql = (16, AdminStatus.No, ServerlessStatus.Public)
-    FieldCaps = (17, AdminStatus.No, ServerlessStatus.Public)
-    CompositeAgg = (18, AdminStatus.No, ServerlessStatus.Public)
-    WaitForCurrentSnapshotsCreate = (19, AdminStatus.No, ServerlessStatus.Internal)
-    Downsample = (20, AdminStatus.No, ServerlessStatus.Internal)
+    Composite = (8, AdminStatus.No, serverless.Status.Public)
+    SubmitAsyncSearch = (9, AdminStatus.No, serverless.Status.Public)
+    GetAsyncSearch = (10, AdminStatus.No, serverless.Status.Public)
+    DeleteAsyncSearch = (11, AdminStatus.No, serverless.Status.Public)
+    PaginatedSearch = (12, AdminStatus.No, serverless.Status.Public)
+    ScrollSearch = (13, AdminStatus.No, serverless.Status.Public)
+    OpenPointInTime = (14, AdminStatus.No, serverless.Status.Public)
+    ClosePointInTime = (15, AdminStatus.No, serverless.Status.Public)
+    Sql = (16, AdminStatus.No, serverless.Status.Public)
+    FieldCaps = (17, AdminStatus.No, serverless.Status.Public)
+    CompositeAgg = (18, AdminStatus.No, serverless.Status.Public)
+    WaitForCurrentSnapshotsCreate = (19, AdminStatus.No, serverless.Status.Internal)
+    Downsample = (20, AdminStatus.No, serverless.Status.Internal)
 
     # administrative actions
-    ForceMerge = (21, AdminStatus.Yes, ServerlessStatus.Internal)
-    ClusterHealth = (22, AdminStatus.Yes, ServerlessStatus.Internal)
-    PutPipeline = (23, AdminStatus.Yes, ServerlessStatus.Public)
-    Refresh = (24, AdminStatus.Yes, ServerlessStatus.Public)
-    CreateIndex = (25, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteIndex = (26, AdminStatus.Yes, ServerlessStatus.Public)
-    CreateIndexTemplate = (27, AdminStatus.Yes, ServerlessStatus.Blocked)
-    DeleteIndexTemplate = (28, AdminStatus.Yes, ServerlessStatus.Blocked)
-    ShrinkIndex = (29, AdminStatus.Yes, ServerlessStatus.Blocked)
-    CreateMlDatafeed = (30, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteMlDatafeed = (31, AdminStatus.Yes, ServerlessStatus.Public)
-    StartMlDatafeed = (32, AdminStatus.Yes, ServerlessStatus.Public)
-    StopMlDatafeed = (33, AdminStatus.Yes, ServerlessStatus.Public)
-    CreateMlJob = (34, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteMlJob = (35, AdminStatus.Yes, ServerlessStatus.Public)
-    OpenMlJob = (36, AdminStatus.Yes, ServerlessStatus.Public)
-    CloseMlJob = (37, AdminStatus.Yes, ServerlessStatus.Public)
-    Sleep = (38, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteSnapshotRepository = (39, AdminStatus.Yes, ServerlessStatus.Internal)
-    CreateSnapshotRepository = (40, AdminStatus.Yes, ServerlessStatus.Internal)
-    CreateSnapshot = (41, AdminStatus.Yes, ServerlessStatus.Internal)
-    RestoreSnapshot = (42, AdminStatus.Yes, ServerlessStatus.Internal)
-    PutSettings = (43, AdminStatus.Yes, ServerlessStatus.Internal)
-    CreateTransform = (44, AdminStatus.Yes, ServerlessStatus.Public)
-    StartTransform = (45, AdminStatus.Yes, ServerlessStatus.Public)
-    WaitForTransform = (46, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteTransform = (47, AdminStatus.Yes, ServerlessStatus.Public)
-    CreateDataStream = (48, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteDataStream = (49, AdminStatus.Yes, ServerlessStatus.Public)
-    CreateComposableTemplate = (50, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteComposableTemplate = (51, AdminStatus.Yes, ServerlessStatus.Public)
-    CreateComponentTemplate = (52, AdminStatus.Yes, ServerlessStatus.Public)
-    DeleteComponentTemplate = (53, AdminStatus.Yes, ServerlessStatus.Public)
-    TransformStats = (54, AdminStatus.Yes, ServerlessStatus.Public)
-    CreateIlmPolicy = (55, AdminStatus.Yes, ServerlessStatus.Blocked)
-    DeleteIlmPolicy = (56, AdminStatus.Yes, ServerlessStatus.Blocked)
+    ForceMerge = (21, AdminStatus.Yes, serverless.Status.Internal)
+    ClusterHealth = (22, AdminStatus.Yes, serverless.Status.Internal)
+    PutPipeline = (23, AdminStatus.Yes, serverless.Status.Public)
+    Refresh = (24, AdminStatus.Yes, serverless.Status.Public)
+    CreateIndex = (25, AdminStatus.Yes, serverless.Status.Public)
+    DeleteIndex = (26, AdminStatus.Yes, serverless.Status.Public)
+    CreateIndexTemplate = (27, AdminStatus.Yes, serverless.Status.Blocked)
+    DeleteIndexTemplate = (28, AdminStatus.Yes, serverless.Status.Blocked)
+    ShrinkIndex = (29, AdminStatus.Yes, serverless.Status.Blocked)
+    CreateMlDatafeed = (30, AdminStatus.Yes, serverless.Status.Public)
+    DeleteMlDatafeed = (31, AdminStatus.Yes, serverless.Status.Public)
+    StartMlDatafeed = (32, AdminStatus.Yes, serverless.Status.Public)
+    StopMlDatafeed = (33, AdminStatus.Yes, serverless.Status.Public)
+    CreateMlJob = (34, AdminStatus.Yes, serverless.Status.Public)
+    DeleteMlJob = (35, AdminStatus.Yes, serverless.Status.Public)
+    OpenMlJob = (36, AdminStatus.Yes, serverless.Status.Public)
+    CloseMlJob = (37, AdminStatus.Yes, serverless.Status.Public)
+    Sleep = (38, AdminStatus.Yes, serverless.Status.Public)
+    DeleteSnapshotRepository = (39, AdminStatus.Yes, serverless.Status.Internal)
+    CreateSnapshotRepository = (40, AdminStatus.Yes, serverless.Status.Internal)
+    CreateSnapshot = (41, AdminStatus.Yes, serverless.Status.Internal)
+    RestoreSnapshot = (42, AdminStatus.Yes, serverless.Status.Internal)
+    PutSettings = (43, AdminStatus.Yes, serverless.Status.Internal)
+    CreateTransform = (44, AdminStatus.Yes, serverless.Status.Public)
+    StartTransform = (45, AdminStatus.Yes, serverless.Status.Public)
+    WaitForTransform = (46, AdminStatus.Yes, serverless.Status.Public)
+    DeleteTransform = (47, AdminStatus.Yes, serverless.Status.Public)
+    CreateDataStream = (48, AdminStatus.Yes, serverless.Status.Public)
+    DeleteDataStream = (49, AdminStatus.Yes, serverless.Status.Public)
+    CreateComposableTemplate = (50, AdminStatus.Yes, serverless.Status.Public)
+    DeleteComposableTemplate = (51, AdminStatus.Yes, serverless.Status.Public)
+    CreateComponentTemplate = (52, AdminStatus.Yes, serverless.Status.Public)
+    DeleteComponentTemplate = (53, AdminStatus.Yes, serverless.Status.Public)
+    TransformStats = (54, AdminStatus.Yes, serverless.Status.Public)
+    CreateIlmPolicy = (55, AdminStatus.Yes, serverless.Status.Blocked)
+    DeleteIlmPolicy = (56, AdminStatus.Yes, serverless.Status.Blocked)
 
-    def __init__(self, id: int, admin_status: AdminStatus, serverless_status: ServerlessStatus):
+    def __init__(self, id: int, admin_status: AdminStatus, serverless_status: serverless.Status):
         self.id = id
         self.admin_status = admin_status
         self.serverless_status = serverless_status
 
     @property
     def admin_op(self):
         return self.admin_status == AdminStatus.Yes
```

### Comparing `esrally-2.9.0/esrally/tracker/__init__.py` & `esrally-2.9.1/esrally/tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/tracker/corpus.py` & `esrally-2.9.1/esrally/tracker/corpus.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/tracker/index.py` & `esrally-2.9.1/esrally/tracker/index.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/tracker/tracker.py` & `esrally-2.9.1/esrally/tracker/tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     track_name = cfg.opts("track", "track.name")
     indices = cfg.opts("generator", "indices")
     root_path = cfg.opts("generator", "output.path")
     target_hosts = cfg.opts("client", "hosts").default
     client_options = cfg.opts("client", "options").default
     data_streams = cfg.opts("generator", "data_streams")
 
-    distribution_flavor, distribution_version, _ = factory.cluster_distribution_version(target_hosts, client_options)
+    distribution_flavor, distribution_version, _, _ = factory.cluster_distribution_version(target_hosts, client_options)
     client = factory.EsClientFactory(
         hosts=target_hosts,
         client_options=client_options,
         distribution_version=distribution_version,
         distribution_flavor=distribution_flavor,
     ).create()
```

### Comparing `esrally-2.9.0/esrally/utils/__init__.py` & `esrally-2.9.1/esrally/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/collections.py` & `esrally-2.9.1/esrally/utils/collections.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/console.py` & `esrally-2.9.1/esrally/utils/console.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/convert.py` & `esrally-2.9.1/esrally/utils/convert.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/git.py` & `esrally-2.9.1/esrally/utils/git.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/io.py` & `esrally-2.9.1/esrally/utils/io.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/jvm.py` & `esrally-2.9.1/esrally/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/modules.py` & `esrally-2.9.1/esrally/utils/modules.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/net.py` & `esrally-2.9.1/esrally/utils/net.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/opts.py` & `esrally-2.9.1/esrally/utils/opts.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/process.py` & `esrally-2.9.1/esrally/utils/process.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/repo.py` & `esrally-2.9.1/esrally/utils/repo.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/sysstats.py` & `esrally-2.9.1/esrally/utils/sysstats.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/esrally/utils/versions.py` & `esrally-2.9.1/esrally/utils/versions.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/__init__.py` & `esrally-2.9.1/it/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/basic_test.py` & `esrally-2.9.1/it/basic_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/dependencies_test.py` & `esrally-2.9.1/it/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/distribution_test.py` & `esrally-2.9.1/it/distribution_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/docker_dev_image_test.py` & `esrally-2.9.1/it/docker_dev_image_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/download_test.py` & `esrally-2.9.1/it/download_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/error_test.py` & `esrally-2.9.1/it/error_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/esrallyd_test.py` & `esrally-2.9.1/it/esrallyd_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/info_test.py` & `esrally-2.9.1/it/info_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/installation_test.py` & `esrally-2.9.1/it/installation_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/list_test.py` & `esrally-2.9.1/it/list_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/proxy_test.py` & `esrally-2.9.1/it/proxy_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/sources_test.py` & `esrally-2.9.1/it/sources_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/static_responses_test.py` & `esrally-2.9.1/it/static_responses_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/tracker_test.py` & `esrally-2.9.1/it/tracker_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/resources/rally-es-it.ini` & `esrally-2.9.1/it/resources/rally-es-it.ini`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/resources/rally-in-memory-it.ini` & `esrally-2.9.1/it/resources/rally-in-memory-it.ini`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/resources/static-responses.json` & `esrally-2.9.1/it/resources/static-responses.json`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/resources/track_with_dependency/track.py` & `esrally-2.9.1/it/resources/track_with_dependency/track.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/it/track_repo_compatibility/conftest.py` & `esrally-2.9.1/it/track_repo_compatibility/conftest.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/recipes/ccr/docker-compose.yml` & `esrally-2.9.1/recipes/ccr/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/recipes/ccr/metricstore-docker-compose.yml` & `esrally-2.9.1/recipes/ccr/metricstore-docker-compose.yml`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/recipes/ccr/start.sh` & `esrally-2.9.1/recipes/ccr/start.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/scripts/offline-install.sh` & `esrally-2.9.1/scripts/offline-install.sh`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/__init__.py` & `esrally-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/config_test.py` & `esrally-2.9.1/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/log_test.py` & `esrally-2.9.1/tests/log_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/metrics_test.py` & `esrally-2.9.1/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/racecontrol_test.py` & `esrally-2.9.1/tests/racecontrol_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/reporter_test.py` & `esrally-2.9.1/tests/reporter_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/telemetry_test.py` & `esrally-2.9.1/tests/telemetry_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import elasticsearch
 import pytest
 
 from esrally import config, exceptions, metrics, telemetry
 from esrally.mechanic import cluster
 from esrally.metrics import MetaInfoScope
-from esrally.utils import console
+from esrally.utils import console, serverless
 
 
 class TestSamplerThread:
     def test_sampler_thread_start_join(self):
         sampler = telemetry.SamplerThread(recorder=mock.Mock())
         sampler.stop = True
         sampler.start()
@@ -98,43 +98,103 @@
     # disable version probing to avoid any network calls in tests
     cfg.add(config.Scope.application, "reporting", "datastore.probe.cluster_version", False)
     # only internal devices are active
     cfg.add(config.Scope.application, "telemetry", "devices", [])
     return cfg
 
 
-class MockTelemetryDevice(telemetry.InternalTelemetryDevice):
+class MockJavaOptsTelemetryDevice(telemetry.InternalTelemetryDevice):
     def __init__(self, mock_java_opts):
         super().__init__()
         self.mock_java_opts = mock_java_opts
 
     def instrument_java_opts(self):
         return self.mock_java_opts
 
 
+class MockTelemetryDevice(telemetry.TelemetryDevice):
+    def __init__(self, *, internal: bool, serverless_status: serverless.Status):
+        super().__init__()
+        self.internal = internal
+        self.serverless_status = serverless_status
+        self.command = f"{'default' if internal else 'optional'}-{serverless_status.name.lower()}"
+        self.on_benchmark_start_called = False
+
+    def on_benchmark_start(self):
+        self.on_benchmark_start_called = True
+
+
 class TestTelemetry:
     def test_merges_options_set_by_different_devices(self):
         cfg = config.Config()
         cfg.add(config.Scope.application, "telemetry", "devices", "jfr")
         cfg.add(config.Scope.application, "system", "challenge.root.dir", "challenge-root")
         cfg.add(config.Scope.application, "benchmarks", "metrics.log.dir", "telemetry")
 
         devices = [
-            MockTelemetryDevice(["-Xms256M"]),
-            MockTelemetryDevice(["-Xmx512M"]),
-            MockTelemetryDevice(["-Des.network.host=127.0.0.1"]),
+            MockJavaOptsTelemetryDevice(["-Xms256M"]),
+            MockJavaOptsTelemetryDevice(["-Xmx512M"]),
+            MockJavaOptsTelemetryDevice(["-Des.network.host=127.0.0.1"]),
         ]
 
         t = telemetry.Telemetry(enabled_devices=None, devices=devices)
 
         opts = t.instrument_candidate_java_opts()
 
         assert opts == ["-Xms256M", "-Xmx512M", "-Des.network.host=127.0.0.1"]
 
 
+@pytest.mark.parametrize(
+    ["enabled_devices", "serverless_mode", "serverless_operator", "started", "expected_msgs"],
+    [
+        (["optional-blocked"], False, False, {"default-public", "default-internal", "default-blocked", "optional-blocked"}, []),
+        ([], True, False, {"default-public"}, []),
+        ([], True, True, {"default-public", "default-internal"}, []),
+        (
+            ["optional-public", "optional-internal"],
+            True,
+            False,
+            {"default-public", "optional-public"},
+            ["Excluding telemetry device [optional-internal] as it is unavailable on serverless."],
+        ),
+    ],
+)
+def test_serverless_exclusion(enabled_devices, serverless_mode, serverless_operator, started, expected_msgs, monkeypatch):
+    info_msg = []
+
+    def console_info(msg):
+        nonlocal info_msg
+        info_msg.append(msg)
+
+    monkeypatch.setattr(telemetry.console, "info", console_info)
+    devices = {
+        "default-public": MockTelemetryDevice(internal=True, serverless_status=serverless.Status.Public),
+        "default-internal": MockTelemetryDevice(internal=True, serverless_status=serverless.Status.Internal),
+        "default-blocked": MockTelemetryDevice(internal=True, serverless_status=serverless.Status.Blocked),
+        "optional-public": MockTelemetryDevice(internal=False, serverless_status=serverless.Status.Public),
+        "optional-internal": MockTelemetryDevice(internal=False, serverless_status=serverless.Status.Internal),
+        "optional-blocked": MockTelemetryDevice(internal=False, serverless_status=serverless.Status.Blocked),
+    }
+
+    t = telemetry.Telemetry(
+        enabled_devices=enabled_devices,
+        devices=devices.values(),
+        serverless_mode=serverless_mode,
+        serverless_operator=serverless_operator,
+    )
+    t.on_benchmark_start()
+    actually_started = set()
+    for device_key, device in devices.items():
+        if device.on_benchmark_start_called:
+            actually_started.add(device_key)
+
+    assert actually_started == started
+    assert info_msg == expected_msgs
+
+
 class TestStartupTime:
     @mock.patch("esrally.time.StopWatch")
     @mock.patch("esrally.metrics.EsMetricsStore.put_value_node_level")
     def test_store_calculated_metrics(self, metrics_store_put_value, stop_watch):
         stop_watch.total_time.return_value = 2
         metrics_store = metrics.EsMetricsStore(create_config())
         node = cluster.Node(None, "/bin", "io", "rally0", None)
```

### Comparing `esrally-2.9.0/tests/time_test.py` & `esrally-2.9.1/tests/time_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/client/__init__.py` & `esrally-2.9.1/tests/client/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/client/asynchronous_test.py` & `esrally-2.9.1/tests/client/asynchronous_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/client/common_test.py` & `esrally-2.9.1/tests/client/common_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/client/factory_test.py` & `esrally-2.9.1/tests/client/factory_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/driver/__init__.py` & `esrally-2.9.1/tests/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/driver/driver_test.py` & `esrally-2.9.1/tests/driver/driver_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/driver/runner_test.py` & `esrally-2.9.1/tests/driver/runner_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/driver/scheduler_test.py` & `esrally-2.9.1/tests/driver/scheduler_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/__init__.py` & `esrally-2.9.1/tests/mechanic/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/java_resolver_test.py` & `esrally-2.9.1/tests/mechanic/java_resolver_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/launcher_test.py` & `esrally-2.9.1/tests/mechanic/launcher_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/mechanic_test.py` & `esrally-2.9.1/tests/mechanic/mechanic_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/provisioner_test.py` & `esrally-2.9.1/tests/mechanic/provisioner_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/supplier_test.py` & `esrally-2.9.1/tests/mechanic/supplier_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/team_test.py` & `esrally-2.9.1/tests/mechanic/team_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/data/cars/v1/hook2/config.py` & `esrally-2.9.1/tests/mechanic/data/cars/v1/hook2/config.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/mechanic/data/cars/v1/with_hook/config.py` & `esrally-2.9.1/tests/mechanic/data/cars/v1/with_hook/config.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/track/__init__.py` & `esrally-2.9.1/tests/track/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/track/loader_test.py` & `esrally-2.9.1/tests/track/loader_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/track/params_test.py` & `esrally-2.9.1/tests/track/params_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/track/track_test.py` & `esrally-2.9.1/tests/track/track_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 import pytest
 
 from esrally import exceptions
 from esrally.track import track
+from esrally.utils import serverless
 
 
 class TestTrack:
     def test_finds_default_challenge(self):
         default_challenge = track.Challenge("default", description="default challenge", default=True)
         another_challenge = track.Challenge("other", description="non-default challenge", default=False)
 
@@ -270,23 +271,23 @@
     def test_string_hyphenation_is_symmetric(self):
         for op_type in track.OperationType:
             assert track.OperationType.from_hyphenated_string(op_type.to_hyphenated_string()) == op_type
 
     def test_attributes(self):
         create_ilm_policy = track.OperationType.CreateIlmPolicy
         assert create_ilm_policy.admin_op is True
-        assert create_ilm_policy.serverless_status == track.ServerlessStatus.Blocked
+        assert create_ilm_policy.serverless_status == serverless.Status.Blocked
 
         node_stats = track.OperationType.NodeStats
         assert node_stats.admin_op is False
-        assert node_stats.serverless_status == track.ServerlessStatus.Internal
+        assert node_stats.serverless_status == serverless.Status.Internal
 
         bulk = track.OperationType.Bulk
         assert bulk.admin_op is False
-        assert bulk.serverless_status == track.ServerlessStatus.Public
+        assert bulk.serverless_status == serverless.Status.Public
 
 
 class TestTaskFilter:
     def create_index_task(self):
         return track.Task(
             "create-index-task",
             track.Operation("create-index-op", operation_type=track.OperationType.CreateIndex.to_hyphenated_string()),
```

### Comparing `esrally-2.9.0/tests/tracker/__init__.py` & `esrally-2.9.1/tests/tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/tracker/corpus_test.py` & `esrally-2.9.1/tests/tracker/corpus_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/tracker/index_test.py` & `esrally-2.9.1/tests/tracker/index_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/__init__.py` & `esrally-2.9.1/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/collections_test.py` & `esrally-2.9.1/tests/utils/collections_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/console_test.py` & `esrally-2.9.1/tests/utils/console_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/convert_test.py` & `esrally-2.9.1/tests/utils/convert_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/git_test.py` & `esrally-2.9.1/tests/utils/git_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/io_test.py` & `esrally-2.9.1/tests/utils/io_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/jvm_test.py` & `esrally-2.9.1/tests/utils/jvm_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/net_test.py` & `esrally-2.9.1/tests/utils/net_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/opts_test.py` & `esrally-2.9.1/tests/utils/opts_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/process_test.py` & `esrally-2.9.1/tests/utils/process_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/repo_test.py` & `esrally-2.9.1/tests/utils/repo_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/versions_test.py` & `esrally-2.9.1/tests/utils/versions_test.py`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/resources/test.txt.tar` & `esrally-2.9.1/tests/utils/resources/test.txt.tar`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/resources/certs/ca.crt` & `esrally-2.9.1/tests/utils/resources/certs/ca.crt`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/resources/certs/client.crt` & `esrally-2.9.1/tests/utils/resources/certs/client.crt`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/tests/utils/resources/certs/client.key` & `esrally-2.9.1/tests/utils/resources/certs/client.key`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/.gitignore` & `esrally-2.9.1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 .rally_it/
 # Virtualenv for development
 .venv*/
 # Autogenerated files
 NOTICE.txt
 recipes/ccr/ccr-target-hosts.json
 
-# Emacs backup files
+# Editors
 *~
 /.project
 /.pydevproject
+/.vscode
 
 # Tracker tracks
 tracks/
```

### Comparing `esrally-2.9.0/AUTHORS` & `esrally-2.9.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/LICENSE` & `esrally-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/README.md` & `esrally-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/pyproject.toml` & `esrally-2.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esrally-2.9.0/PKG-INFO` & `esrally-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrally
-Version: 2.9.0
+Version: 2.9.1
 Summary: Macrobenchmarking framework for Elasticsearch
 Project-URL: Changelog, https://github.com/elastic/rally/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://esrally.readthedocs.io/
 Project-URL: Code, https://github.com/elastic/rally
 Project-URL: Issue tracker, https://github.com/elastic/rally/issues
 Author-email: Daniel Mitterdorfer <daniel.mitterdorfer@gmail.com>
 License: Apache License 2.0
```

