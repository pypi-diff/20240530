# Comparing `tmp/scrapegraphai-1.5.2.tar.gz` & `tmp/scrapegraphai-1.5.3b1.tar.gz`

## Comparing `scrapegraphai-1.5.2.tar` & `scrapegraphai-1.5.3b1.tar`

### file list

```diff
@@ -1,294 +1,364 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.gitattributes
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.releaserc.yml
--rw-r--r--   0        0        0    55282 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/Dockerfile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/SECURITY.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/citation.cff
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docker-compose.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/readthedocs.yml
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/requirements-dev.lock
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/requirements-dev.txt
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/requirements.lock
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/Makefile
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/make.bat
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/apikey_1.png
--rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/apikey_2.png
--rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/apikey_3.png
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/apikey_4.png
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/codespaces-badge.png
--rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/logo_authors.png
--rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/omniscrapergraph.png
--rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/omnisearchgraph.png
--rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/project_overview_diagram.fig
--rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/project_overview_diagram.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/scrapegraphai_logo.png
--rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/searchgraph.png
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/serp_api_logo.png
--rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/smartscrapergraph.png
--rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/speechgraph.png
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/assets/transparent_stat.png
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/conf.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/index.rst
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/getting_started/examples.rst
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/introduction/contributing.rst
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/introduction/overview.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/modules.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.builders.rst
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.docloaders.rst
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.graphs.rst
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.helpers.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.integrations.rst
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.models.rst
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.nodes.rst
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.rst
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.utils.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/scrapers/benchmarks.rst
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/scrapers/graph_config.rst
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/scrapers/graphs.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/docs/source/scrapers/llm.rst
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/readme.md
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/anthropic/smart_scraper_haiku.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/anthropic/smart_scraper_schema_haiku.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/azure/json_scraper_azure.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/azure/search_graph_azure.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/azure/smart_scraper_azure_openai.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/azure/xml_scraper_azure.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/azure/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/azure/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/azure/inputs/username.csv
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/.env.example
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/README.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/csv_scraper_bedrock.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/custom_graph_bedrock.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/json_scraper_bedrock.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/scrape_plain_text_bedrock.py
--rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/scrapegraphai_bedrock.png
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/script_generator_bedrock.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/search_graph_bedrock.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/smart_scraper_bedrock.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/smart_scraper_schema_bedrock.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/xml_scraper_bedrock.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/inputs/books.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/bedrock/inputs/username.csv
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/readme.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/.env.example
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/.env.example
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/Readme.md
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/.env.example
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/csv_scraper_deepseek.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/json_scraper_deepseek.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/script_generator_deepseek.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/search_graph_deepseek.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/smart_scarper_deepseek.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/smart_scraper_schema_deepseek.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/xml_scraper_deepseek.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/deepseek/inputs/username.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/.env.example
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/csv_scraper_gemini.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/custom_graph_gemini.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/json_scraper_gemini.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/readme.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/scrape_plain_text_gemini.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/scrape_xml_gemini.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/script_generator_gemini.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/search_graph_gemini.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/smart_scraper_gemini.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/smart_scraper_schema_gemini.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/gemini/inputs/username.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/groq/.env.example
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/groq/search_graph_groq_openai.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/groq/smart_scraper_groq_ollama.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/groq/smart_scraper_groq_openai.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/groq/smart_scraper_schema_groq_openai.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/huggingfacehub/smart_scraper_huggingfacehub.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/csv_scraper_ollama.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/json_scraper_ollama.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/pdf_scraper_ollama.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/scrape_plain_text_ollama.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/scrape_xml_ollama.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/script_generator_ollama.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/search_graph_ollama.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/smart_scraper_ollama.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/smart_scraper_schema_ollama.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/xml_scraper_ollama.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/local_models/inputs/username.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/mixed_models/.env.example
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/mixed_models/readme.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/mixed_models/search_graph_groq_ollama.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/mixed_models/smart_scraper_mixed.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/mixed_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/mixed_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/mixed_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/oneapi/smart_scraper_schema_oneapi.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/oneapi/smartscraper_oneapi.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/.env.example
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/csv_scraper_openai.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/custom_graph_openai.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/deep_scraper_openai.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/json_scraper_openai.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/omni_scraper_openai.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/omni_search_graph_openai.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/pdf_scraper_graph_openai.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/readme.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/scrape_plain_text_openai.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/script_generator_openai.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/search_graph_openai.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/smart_scraper_multi_openai.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/smart_scraper_openai.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/smart_scraper_schema_openai.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/speech_graph_openai.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/openai/inputs/username.csv
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/single_node/fetch_node.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/single_node/image2text_node.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/single_node/kg_node.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/examples/single_node/robot_node.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/manual deployment/commit_and_push.sh
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/manual deployment/commit_and_push_with_tests.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/manual deployment/deploy_on_pip.sh
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/manual deployment/installation.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/docloaders/__init__.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/docloaders/chromium.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    15828 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/deep_scraper_graph.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/omni_scraper_graph.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/omni_search_graph.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/smart_scraper_multi_graph.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_prompts.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/integrations/__init__.py
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/integrations/burr_bridge.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/anthropic.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/deepseek.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/oneapi.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_omni_node.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/search_node_with_context.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/cleanup_html.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/logging.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/sys_dynamic_import.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/Readme.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/scrape_json_ollama.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/scrape_plain_text_llama3_test.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/scrape_plain_text_mistral_test.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/scrape_xml_ollama_test.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/script_generator_test.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/smart_scraper_ollama_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/graphs/inputs/username.csv
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/nodes/fetch_node_test.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/nodes/robot_node_test.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/nodes/search_link_node_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/nodes/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/nodes/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/nodes/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/nodes/inputs/username.csv
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/utils/test_proxy_rotation.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/tests/utils/test_sys_dynamic_import.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/LICENSE
--rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/README.md
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/pyproject.toml
--rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 scrapegraphai-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.gitattributes
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.releaserc.yml
+-rw-r--r--   0        0        0    55529 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/CHANGELOG.md
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/Dockerfile
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/SECURITY.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/citation.cff
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docker-compose.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/readthedocs.yml
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/requirements-dev.lock
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/requirements-dev.txt
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/requirements.lock
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/Makefile
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/make.bat
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/apikey_1.png
+-rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/apikey_2.png
+-rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/apikey_3.png
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/apikey_4.png
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/codespaces-badge.png
+-rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/logo_authors.png
+-rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/omniscrapergraph.png
+-rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/omnisearchgraph.png
+-rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/project_overview_diagram.fig
+-rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/project_overview_diagram.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/scrapegraphai_logo.png
+-rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/searchgraph.png
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/serp_api_logo.png
+-rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/smartscrapergraph.png
+-rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/speechgraph.png
+-rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/assets/transparent_stat.png
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/conf.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/index.rst
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/getting_started/examples.rst
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/introduction/contributing.rst
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/introduction/overview.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/modules.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.builders.rst
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.docloaders.rst
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.graphs.rst
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.helpers.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.integrations.rst
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.models.rst
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.nodes.rst
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.rst
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.utils.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/scrapers/benchmarks.rst
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/scrapers/graph_config.rst
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/scrapers/graphs.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/docs/source/scrapers/llm.rst
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/readme.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/.env.example
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/csv_scraper_haiku.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/custom_graph_haiku.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/json_scraper_haiku.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/pdf_scraper_graph_haiku.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/scrape_plain_text_haiku.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/script_generator_haiku.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/search_graph_haiku.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/smart_scraper_haiku.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/smart_scraper_multi_haiku.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/smart_scraper_schema_haiku.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/xml_scraper_haiku.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/anthropic/inputs/username.csv
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/csv_scraper_azure.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/custom_graph_azure.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/json_scraper_azure.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/pdf_scraper_azure.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/scrape_plain_text_azure.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/script_generator_azure.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/search_graph_azure.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/smart_scraper_azure.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/smart_scraper_schema_azure.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/xml_scraper_azure.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/azure/inputs/username.csv
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/.env.example
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/README.md
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/csv_scraper_bedrock.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/custom_graph_bedrock.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/json_scraper_bedrock.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/pdf_scraper_graph_bedrock.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/scrape_plain_text_bedrock.py
+-rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/scrapegraphai_bedrock.png
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/script_generator_bedrock.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/search_graph_bedrock.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/smart_scraper_bedrock.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/smart_scraper_multi_bedrock.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/smart_scraper_schema_bedrock.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/xml_scraper_bedrock.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/inputs/books.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/bedrock/inputs/username.csv
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/readme.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/.env.example
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/.env.example
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/Readme.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/.env.example
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/csv_scraper_deepseek.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/custom_graph_deepseek.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/json_scraper_deepseek.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/pdf_scraper_graph_deepseek.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/scrape_plain_text_deepseek.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/script_generator_deepseek.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/search_graph_deepseek.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/smart_scraper_deepseek.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/smart_scraper_schema_deepseek.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/xml_scraper_deepseek.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/deepseek/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/.env.example
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/csv_scraper_gemini.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/custom_graph_gemini.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/json_scraper_gemini.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/pdf_scraper_graph_gemini.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/readme.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/scrape_plain_text_gemini.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/scrape_xml_gemini.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/script_generator_gemini.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/search_graph_gemini.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/smart_scraper_gemini.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/smart_scraper_multi_gemini.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/smart_scraper_schema_gemini.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/gemini/inputs/username.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/.env.example
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/csv_scraper_groq.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/custom_graph_groq.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/json_scraper_groq.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/pdf_scraper_graph_groq.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/scrape_plain_text_groq.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/script_generator_groq.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/search_graph_groq.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/smart_scraper_groq.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/smart_scraper_multi_groq.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/smart_scraper_schema_groq.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/xml_scraper_groq.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/groq/inputs/username.csv
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/csv_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/custom_graph_huggingfacehub.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/json_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/pdf_scraper_graph_huggingfacehub.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/scrape_plain_text_huggingfacehub.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/script_generator_huggingfacehub.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/search_graph_huggingfacehub.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/smart_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/smart_scraper_multi_huggingfacehub.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/smart_scraper_schema_huggingfacehub.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/xml_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/huggingfacehub/inputs/username.csv
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/csv_scraper_ollama.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/custom_graph_ollama.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/json_scraper_ollama.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/pdf_scraper_ollama.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/scrape_plain_text_ollama.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/scrape_xml_ollama.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/script_generator_ollama.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/search_graph_ollama.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/smart_scraper_ollama.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/smart_scraper_schema_ollama.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/xml_scraper_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/local_models/inputs/username.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/.env.example
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/custom_graph_groq_openai.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/readme.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/search_graph_groq_ollama.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/search_graph_groq_openai.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/smart_scraper_groq_ollama.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/smart_scraper_schema_groq_openai.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/smartscraper_oneapi_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/mixed_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/csv_scraper_oneapi.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/custom_graph_oneapi.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/json_scraper_oneapi.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/pdf_scraper_graph_oneapi.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/scrape_plain_text_oneapi.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/script_generator_oneapi.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/search_graph_oneapi.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/smart_scraper_multi_oneapi.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/smart_scraper_schema_oneapi.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/smartscraper_oneapi.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/xml_scraper_oneapi.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/inputs/plain_html_example copy.txt
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/oneapi/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/.env.example
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/csv_scraper_openai.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/custom_graph_openai.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/deep_scraper_openai.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/json_scraper_openai.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/omni_scraper_openai.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/omni_search_graph_openai.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/pdf_scraper_graph_openai.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/readme.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/scrape_plain_text_openai.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/script_generator_openai.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/search_graph_openai.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/smart_scraper_multi_openai.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/smart_scraper_openai.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/smart_scraper_schema_openai.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/speech_graph_openai.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/openai/inputs/username.csv
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/single_node/fetch_node.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/single_node/image2text_node.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/single_node/kg_node.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/examples/single_node/robot_node.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/manual deployment/commit_and_push.sh
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/manual deployment/commit_and_push_with_tests.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/manual deployment/deploy_on_pip.sh
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/manual deployment/installation.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/docloaders/__init__.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/docloaders/chromium.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    15828 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/deep_scraper_graph.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/omni_scraper_graph.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/omni_search_graph.py
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/smart_scraper_multi_graph.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_prompts.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/integrations/__init__.py
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/integrations/burr_bridge.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/anthropic.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/deepseek.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/oneapi.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_omni_node.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/search_node_with_context.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/cleanup_html.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/logging.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/sys_dynamic_import.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/Readme.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/scrape_json_ollama.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/scrape_plain_text_llama3_test.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/scrape_plain_text_mistral_test.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/scrape_xml_ollama_test.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/script_generator_test.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/smart_scraper_ollama_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/graphs/inputs/username.csv
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/nodes/fetch_node_test.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/nodes/robot_node_test.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/nodes/search_link_node_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/nodes/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/nodes/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/nodes/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/nodes/inputs/username.csv
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/utils/test_proxy_rotation.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/tests/utils/test_sys_dynamic_import.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/LICENSE
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/README.md
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/pyproject.toml
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 scrapegraphai-1.5.3b1/PKG-INFO
```

### Comparing `scrapegraphai-1.5.2/.releaserc.yml` & `scrapegraphai-1.5.3b1/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/CHANGELOG.md` & `scrapegraphai-1.5.3b1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [1.5.3-beta.1](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.2...v1.5.3-beta.1) (2024-05-29)
+
+
+### Bug Fixes
+
+* oneapi model ([4fcb990](https://github.com/VinciGit00/Scrapegraph-ai/commit/4fcb9902fe4c147c61a1622a919ade338c03b8d8))
+
 ## [1.5.2](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.1...v1.5.2) (2024-05-26)
 
 
 ### Bug Fixes
 
 * fixed typo ([54e8216](https://github.com/VinciGit00/Scrapegraph-ai/commit/54e82163f077b90422eb0ba1202167d0ed0e7814))
 * Update __init__.py ([8f2c8d5](https://github.com/VinciGit00/Scrapegraph-ai/commit/8f2c8d5d1289b0dd2417df955310b4323f2df2d2))
```

### Comparing `scrapegraphai-1.5.2/CODE_OF_CONDUCT.md` & `scrapegraphai-1.5.3b1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/CONTRIBUTING.md` & `scrapegraphai-1.5.3b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/readthedocs.yml` & `scrapegraphai-1.5.3b1/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/requirements-dev.lock` & `scrapegraphai-1.5.3b1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/requirements.lock` & `scrapegraphai-1.5.3b1/requirements.lock`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `scrapegraphai-1.5.3b1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `scrapegraphai-1.5.3b1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/.github/workflows/codeql.yml` & `scrapegraphai-1.5.3b1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/.github/workflows/dependency-review.yml` & `scrapegraphai-1.5.3b1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/.github/workflows/pylint.yml` & `scrapegraphai-1.5.3b1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/.github/workflows/python-publish.yml` & `scrapegraphai-1.5.3b1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/.github/workflows/release.yml` & `scrapegraphai-1.5.3b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/Makefile` & `scrapegraphai-1.5.3b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/README.md` & `scrapegraphai-1.5.3b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/make.bat` & `scrapegraphai-1.5.3b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/apikey_1.png` & `scrapegraphai-1.5.3b1/docs/assets/apikey_1.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/apikey_2.png` & `scrapegraphai-1.5.3b1/docs/assets/apikey_2.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/apikey_3.png` & `scrapegraphai-1.5.3b1/docs/assets/apikey_3.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/apikey_4.png` & `scrapegraphai-1.5.3b1/docs/assets/apikey_4.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/codespaces-badge.png` & `scrapegraphai-1.5.3b1/docs/assets/codespaces-badge.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/logo_authors.png` & `scrapegraphai-1.5.3b1/docs/assets/logo_authors.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/omniscrapergraph.png` & `scrapegraphai-1.5.3b1/docs/assets/omniscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/omnisearchgraph.png` & `scrapegraphai-1.5.3b1/docs/assets/omnisearchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/project_overview_diagram.fig` & `scrapegraphai-1.5.3b1/docs/assets/project_overview_diagram.fig`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/project_overview_diagram.png` & `scrapegraphai-1.5.3b1/docs/assets/project_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/scrapegraphai_logo.png` & `scrapegraphai-1.5.3b1/docs/assets/scrapegraphai_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/searchgraph.png` & `scrapegraphai-1.5.3b1/docs/assets/searchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/serp_api_logo.png` & `scrapegraphai-1.5.3b1/docs/assets/serp_api_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/smartscrapergraph.png` & `scrapegraphai-1.5.3b1/docs/assets/smartscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/speechgraph.png` & `scrapegraphai-1.5.3b1/docs/assets/speechgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/assets/transparent_stat.png` & `scrapegraphai-1.5.3b1/docs/assets/transparent_stat.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/conf.py` & `scrapegraphai-1.5.3b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/index.rst` & `scrapegraphai-1.5.3b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/getting_started/examples.rst` & `scrapegraphai-1.5.3b1/docs/source/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/getting_started/installation.rst` & `scrapegraphai-1.5.3b1/docs/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/introduction/contributing.rst` & `scrapegraphai-1.5.3b1/docs/source/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/introduction/overview.rst` & `scrapegraphai-1.5.3b1/docs/source/introduction/overview.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.graphs.rst` & `scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.helpers.rst` & `scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.helpers.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.models.rst` & `scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.models.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.nodes.rst` & `scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.nodes.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/modules/scrapegraphai.utils.rst` & `scrapegraphai-1.5.3b1/docs/source/modules/scrapegraphai.utils.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/scrapers/benchmarks.rst` & `scrapegraphai-1.5.3b1/docs/source/scrapers/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/scrapers/graph_config.rst` & `scrapegraphai-1.5.3b1/docs/source/scrapers/graph_config.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/scrapers/graphs.rst` & `scrapegraphai-1.5.3b1/docs/source/scrapers/graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/docs/source/scrapers/llm.rst` & `scrapegraphai-1.5.3b1/docs/source/scrapers/llm.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/readme.md` & `scrapegraphai-1.5.3b1/examples/readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/anthropic/smart_scraper_haiku.py` & `scrapegraphai-1.5.3b1/examples/huggingfacehub/smart_scraper_schema_huggingfacehub.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,53 +5,69 @@
 import os
 from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
 from langchain_community.llms import HuggingFaceEndpoint
 from langchain_community.embeddings import HuggingFaceInferenceAPIEmbeddings
 
+# ************************************************
+# Define the output schema for the graph
+# ************************************************
+
+schema= """
+    { 
+    "Projects": [
+        "Project #": 
+            { 
+                "title": "...", 
+                "description": "...", 
+            }, 
+        "Project #": 
+            { 
+                "title": "...", 
+                "description": "...", 
+            } 
+        ] 
+    } 
+"""
 
-# required environment variables in .env
-# HUGGINGFACEHUB_API_TOKEN
-# ANTHROPIC_API_KEY
+## required environment variable in .env
+#HUGGINGFACEHUB_API_TOKEN
 load_dotenv()
 
 HUGGINGFACEHUB_API_TOKEN = os.getenv('HUGGINGFACEHUB_API_TOKEN')
 # ************************************************
 # Initialize the model instances
 # ************************************************
 
+repo_id = "mistralai/Mistral-7B-Instruct-v0.2"
+
+llm_model_instance = HuggingFaceEndpoint(
+    repo_id=repo_id, max_length=128, temperature=0.5, token=HUGGINGFACEHUB_API_TOKEN
+)
 
 embedder_model_instance = HuggingFaceInferenceAPIEmbeddings(
     api_key=HUGGINGFACEHUB_API_TOKEN, model_name="sentence-transformers/all-MiniLM-l6-v2"
 )
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 graph_config = {
-    "llm": {
-        "api_key": os.getenv("ANTHROPIC_API_KEY"),
-        "model": "claude-3-haiku-20240307",
-        "max_tokens": 4000},
+    "llm": {"model_instance": llm_model_instance},
     "embeddings": {"model_instance": embedder_model_instance}
 }
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="""Don't say anything else. Output JSON only. List me all the events, with the following fields: company_name, event_name, event_start_date, event_start_time, 
-    event_end_date, event_end_time, location, event_mode, event_category, 
-    third_party_redirect, no_of_days, 
-    time_in_hours, hosted_or_attending, refreshments_type, 
-    registration_available, registration_link""",
-    # also accepts a string with the already downloaded HTML code
-    source="https://www.hmhco.com/event",
+    prompt="List me all the projects with their description",
+    source="https://perinim.github.io/projects/",
+    schema=schema,
     config=graph_config
 )
-
 result = smart_scraper_graph.run()
 print(result)
 
 # ************************************************
 # Get graph execution info
 # ************************************************
```

### Comparing `scrapegraphai-1.5.2/examples/anthropic/smart_scraper_schema_haiku.py` & `scrapegraphai-1.5.3b1/examples/deepseek/smart_scraper_schema_deepseek.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 """ 
-Basic example of scraping pipeline using SmartScraper using Azure OpenAI Key
+Basic example of scraping pipeline using SmartScraper
 """
 
 import os
 from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
-from langchain_community.llms import HuggingFaceEndpoint
-from langchain_community.embeddings import HuggingFaceInferenceAPIEmbeddings
 
-
-# required environment variables in .env
-# HUGGINGFACEHUB_API_TOKEN
-# ANTHROPIC_API_KEY
 load_dotenv()
 
-HUGGINGFACEHUB_API_TOKEN = os.getenv('HUGGINGFACEHUB_API_TOKEN')
-# ************************************************
-# Initialize the model instances
-# ************************************************
-
-
-embedder_model_instance = HuggingFaceInferenceAPIEmbeddings(
-    api_key=HUGGINGFACEHUB_API_TOKEN, model_name="sentence-transformers/all-MiniLM-l6-v2"
-)
-
 # ************************************************
 # Define the output schema for the graph
 # ************************************************
 
 schema= """
     { 
     "Projects": [
@@ -43,30 +27,37 @@
                 "description": "...", 
             } 
         ] 
     } 
 """
 
 # ************************************************
-# Create the SmartScraperGraph instance and run it
+# Define the configuration for the graph
 # ************************************************
 
+deepseek_key = os.getenv("DEEPSEEK_APIKEY")
+
 graph_config = {
     "llm": {
-        "api_key": os.getenv("ANTHROPIC_API_KEY"),
-        "model": "claude-3-haiku-20240307",
-        "max_tokens": 4000},
-    "embeddings": {"model_instance": embedder_model_instance}
+        "model": "deepseek-chat",
+        "openai_api_key": deepseek_key,
+        "openai_api_base": 'https://api.deepseek.com/v1',
+    },
+    "verbose": True,
 }
 
+# ************************************************
+# Create the SmartScraperGraph instance and run it
+# ************************************************
+
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description",
+    prompt="List me all the projects with their description.",
     # also accepts a string with the already downloaded HTML code
-    schema=schema,
     source="https://perinim.github.io/projects/",
+    schema=schema,
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 
 # ************************************************
```

### Comparing `scrapegraphai-1.5.2/examples/azure/json_scraper_azure.py` & `scrapegraphai-1.5.3b1/examples/azure/json_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/azure/search_graph_azure.py` & `scrapegraphai-1.5.3b1/examples/azure/search_graph_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/azure/smart_scraper_azure_openai.py` & `scrapegraphai-1.5.3b1/examples/azure/smart_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/azure/xml_scraper_azure.py` & `scrapegraphai-1.5.3b1/examples/azure/xml_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/azure/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/anthropic/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/azure/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/anthropic/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/bedrock/csv_scraper_bedrock.py` & `scrapegraphai-1.5.3b1/examples/bedrock/csv_scraper_bedrock.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
 graph_config = {
     "llm": {
+        "client": "client_name",
         "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
         "temperature": 0.0
     },
     "embeddings": {
         "model": "bedrock/cohere.embed-multilingual-v3"
     }
 }
-
 # ************************************************
 # Create the CSVScraperGraph instance and run it
 # ************************************************
 
 csv_scraper_graph = CSVScraperGraph(
     prompt="List me all the last names",
     source=str(text),  # Pass the content of the file, not the file object
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/custom_graph_bedrock.py` & `scrapegraphai-1.5.3b1/examples/bedrock/custom_graph_bedrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
 graph_config = {
     "llm": {
+        "client": "client_name",
         "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
         "temperature": 0.0
     },
     "embeddings": {
         "model": "bedrock/cohere.embed-multilingual-v3"
     }
 }
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/json_scraper_bedrock.py` & `scrapegraphai-1.5.3b1/examples/bedrock/scrape_plain_text_bedrock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,60 @@
-"""
-Basic example of scraping pipeline using JSONScraperGraph from JSON documents
+""" 
+Basic example of scraping pipeline using SmartScraper from text
 """
 
 import os
 import json
 
 from dotenv import load_dotenv
 
-from scrapegraphai.graphs import JSONScraperGraph
-from scrapegraphai.utils import convert_to_csv, convert_to_json, prettify_exec_info
+from scrapegraphai.graphs import SmartScraperGraph
+from scrapegraphai.utils import prettify_exec_info
 
 load_dotenv()
 
 # ************************************************
-# Read the JSON file
+# Read the text file
 # ************************************************
 
-FILE_NAME = "inputs/example.json"
+FILE_NAME = "inputs/plain_html_example.txt"
 curr_dir = os.path.dirname(os.path.realpath(__file__))
 file_path = os.path.join(curr_dir, FILE_NAME)
 
+# It could be also a http request using the request model
 with open(file_path, 'r', encoding="utf-8") as file:
     text = file.read()
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
 graph_config = {
     "llm": {
+        "client": "client_name",
         "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
         "temperature": 0.0
     },
     "embeddings": {
         "model": "bedrock/cohere.embed-multilingual-v3"
     }
 }
 
 # ************************************************
-# Create the JSONScraperGraph instance and run it
+# Create the SmartScraperGraph instance and run it
 # ************************************************
 
-json_scraper_graph = JSONScraperGraph(
-    prompt="List me all questions and options in the math section, no answers.",
-    source=text,  # Pass the content of the file, not the file object
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the projects with their description.",
+    source=text,
     config=graph_config
 )
 
-result = json_scraper_graph.run()
+result = smart_scraper_graph.run()
 print(json.dumps(result, indent=4))
 
 # ************************************************
 # Get graph execution info
 # ************************************************
 
-graph_exec_info = json_scraper_graph.get_execution_info()
+graph_exec_info = smart_scraper_graph.get_execution_info()
 print(prettify_exec_info(graph_exec_info))
-
-# Save to json or csv
-convert_to_csv(result, "result")
-convert_to_json(result, "result")
-
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/scrape_plain_text_bedrock.py` & `scrapegraphai-1.5.3b1/examples/anthropic/scrape_plain_text_haiku.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """ 
 Basic example of scraping pipeline using SmartScraper from text
 """
 
 import os
-import json
-
 from dotenv import load_dotenv
-
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
 
 load_dotenv()
 
 # ************************************************
 # Read the text file
@@ -26,34 +23,32 @@
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
 graph_config = {
     "llm": {
-        "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
-        "temperature": 0.0
-    },
-    "embeddings": {
-        "model": "bedrock/cohere.embed-multilingual-v3"
-    }
+        "api_key": os.getenv("ANTHROPIC_API_KEY"),
+        "model": "claude-3-haiku-20240307",
+        "max_tokens": 4000
+        },
 }
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
     prompt="List me all the projects with their description.",
     source=text,
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
-print(json.dumps(result, indent=4))
+print(result)
 
 # ************************************************
 # Get graph execution info
 # ************************************************
 
 graph_exec_info = smart_scraper_graph.get_execution_info()
 print(prettify_exec_info(graph_exec_info))
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/scrapegraphai_bedrock.png` & `scrapegraphai-1.5.3b1/examples/bedrock/scrapegraphai_bedrock.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/bedrock/script_generator_bedrock.py` & `scrapegraphai-1.5.3b1/examples/bedrock/script_generator_bedrock.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
 graph_config = {
     "llm": {
+        "client": "client_name",
         "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
         "temperature": 0.0
     },
     "embeddings": {
         "model": "bedrock/cohere.embed-multilingual-v3"
     },
-    "library": "beautifulsoup"
+        "library": "beautifulsoup"
 }
 
 # ************************************************
 # Create the ScriptCreatorGraph instance and run it
 # ************************************************
 
 script_creator_graph = ScriptCreatorGraph(
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/search_graph_bedrock.py` & `scrapegraphai-1.5.3b1/examples/mixed_models/search_graph_groq_ollama.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """
 Example of Search Graph
 """
 
+import os
 from dotenv import load_dotenv
 from scrapegraphai.graphs import SearchGraph
 from scrapegraphai.utils import convert_to_csv, convert_to_json, prettify_exec_info
-
 load_dotenv()
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
+groq_key = os.getenv("GROQ_APIKEY")
+
 graph_config = {
     "llm": {
-        "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
-        "temperature": 0.0
+        "model": "groq/gemma-7b-it",
+        "api_key": groq_key,
+        "temperature": 0
     },
     "embeddings": {
-        "model": "bedrock/amazon.titan-embed-text-v2:0"
-    }
+        "model": "ollama/nomic-embed-text",
+        "temperature": 0,
+        "base_url": "http://localhost:11434",  # set ollama URL arbitrarily
+    },
+    "max_results": 2,
+    "verbose": True, 
 }
 
 # ************************************************
 # Create the SearchGraph instance and run it
 # ************************************************
 
 search_graph = SearchGraph(
-    prompt="List me Chioggia's famous dishes",
+    prompt="List me all the regions of Italy.",
     config=graph_config
 )
 
 result = search_graph.run()
 print(result)
 
 # ************************************************
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/smart_scraper_bedrock.py` & `scrapegraphai-1.5.3b1/examples/groq/smart_scraper_groq.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 load_dotenv()
 
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-openai_key = os.getenv("OPENAI_APIKEY")
+groq_key = os.getenv("GROQ_APIKEY")
 
 graph_config = {
     "llm": {
-        "api_key": openai_key,
-        "model": "gpt-4o",
+        "model": "groq/gemma-7b-it",
+        "api_key": groq_key,
+        "temperature": 0
     },
-    "verbose": True,
-    "headless": False,
+    "headless": False
 }
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description",
+    prompt="List me all the projects with their description.",
     # also accepts a string with the already downloaded HTML code
     source="https://perinim.github.io/projects/",
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/smart_scraper_schema_bedrock.py` & `scrapegraphai-1.5.3b1/examples/gemini/smart_scraper_schema_gemini.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """ 
-Basic example of scraping pipeline using SmartScraper
+Basic example of scraping pipeline using SmartScraper with schema
 """
 
 import os
 from dotenv import load_dotenv
-from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
-
+from scrapegraphai.graphs import SmartScraperGraph
 load_dotenv()
+
 # ************************************************
 # Define the output schema for the graph
 # ************************************************
-
 schema= """
     { 
     "Projects": [
         "Project #": 
             { 
                 "title": "...", 
                 "description": "...", 
@@ -29,33 +28,31 @@
     } 
 """
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-openai_key = os.getenv("OPENAI_APIKEY")
+gemini_key = os.getenv("GOOGLE_APIKEY")
 
 graph_config = {
     "llm": {
-        "api_key": openai_key,
-        "model": "gpt-4o",
+        "api_key": gemini_key,
+        "model": "gemini-pro",
     },
-    "verbose": True,
-    "headless": False,
 }
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description",
+    prompt="List me all the news with their description.",
     # also accepts a string with the already downloaded HTML code
-    source="https://perinim.github.io/projects/",
+    source="https://www.wired.com",
     schema=schema,
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/xml_scraper_bedrock.py` & `scrapegraphai-1.5.3b1/examples/bedrock/xml_scraper_bedrock.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
 graph_config = {
     "llm": {
+        "client": "client_name",
         "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
         "temperature": 0.0
     },
     "embeddings": {
         "model": "bedrock/cohere.embed-multilingual-v3"
     }
 }
@@ -55,8 +56,7 @@
 
 graph_exec_info = xml_scraper_graph.get_execution_info()
 print(prettify_exec_info(graph_exec_info))
 
 # Save to json or csv
 convert_to_csv(result, "result")
 convert_to_json(result, "result")
-
```

### Comparing `scrapegraphai-1.5.2/examples/bedrock/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/azure/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/bedrock/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/bedrock/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/bedrock/inputs/plain_html_example.txt` & `scrapegraphai-1.5.3b1/examples/anthropic/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/Readme.md` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_groq.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_llama3.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_mistral.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/inputs/example_1.txt` & `scrapegraphai-1.5.3b1/examples/bedrock/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/GenerateScraper/inputs/example_2.txt` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/Readme.md` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_docker.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_docker.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_groq.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_llama3.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_mistral.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/inputs/example_1.txt` & `scrapegraphai-1.5.3b1/examples/benchmarks/GenerateScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/benchmarks/SmartScraper/inputs/example_2.txt` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/csv_scraper_deepseek.py` & `scrapegraphai-1.5.3b1/examples/deepseek/csv_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/json_scraper_deepseek.py` & `scrapegraphai-1.5.3b1/examples/deepseek/json_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/script_generator_deepseek.py` & `scrapegraphai-1.5.3b1/examples/deepseek/script_generator_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/search_graph_deepseek.py` & `scrapegraphai-1.5.3b1/examples/deepseek/search_graph_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/smart_scarper_deepseek.py` & `scrapegraphai-1.5.3b1/examples/deepseek/smart_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/smart_scraper_schema_deepseek.py` & `scrapegraphai-1.5.3b1/examples/mixed_models/smart_scraper_schema_groq_openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ 
-Basic example of scraping pipeline using SmartScraper
+Basic example of scraping pipeline using SmartScraper with schema
 """
 
-import os
+import os, json
 from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
 
 load_dotenv()
 
 # ************************************************
@@ -30,25 +30,32 @@
     } 
 """
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-deepseek_key = os.getenv("DEEPSEEK_APIKEY")
+groq_key = os.getenv("GROQ_APIKEY")
+openai_key = os.getenv("OPENAI_APIKEY")
 
 graph_config = {
     "llm": {
-        "model": "deepseek-chat",
-        "openai_api_key": deepseek_key,
-        "openai_api_base": 'https://api.deepseek.com/v1',
+        "model": "groq/gemma-7b-it",
+        "api_key": groq_key,
+        "temperature": 0
     },
-    "verbose": True,
+    "embeddings": {
+        "api_key": openai_key,
+        "model": "openai",
+    },
+    "headless": False
 }
 
+
+
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
     prompt="List me all the projects with their description.",
     # also accepts a string with the already downloaded HTML code
```

### Comparing `scrapegraphai-1.5.2/examples/deepseek/xml_scraper_deepseek.py` & `scrapegraphai-1.5.3b1/examples/deepseek/xml_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/bedrock/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/deepseek/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/azure/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/csv_scraper_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/csv_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/custom_graph_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/custom_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/json_scraper_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/json_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/scrape_plain_text_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/scrape_plain_text_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/scrape_xml_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/scrape_xml_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/script_generator_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/script_generator_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/search_graph_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/search_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/smart_scraper_gemini.py` & `scrapegraphai-1.5.3b1/examples/gemini/smart_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/smart_scraper_schema_gemini.py` & `scrapegraphai-1.5.3b1/examples/bedrock/smart_scraper_schema_bedrock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """ 
-Basic example of scraping pipeline using SmartScraper with schema
+Basic example of scraping pipeline using SmartScraper
 """
 
 import os
 from dotenv import load_dotenv
-from scrapegraphai.utils import prettify_exec_info
 from scrapegraphai.graphs import SmartScraperGraph
-load_dotenv()
+from scrapegraphai.utils import prettify_exec_info
 
+load_dotenv()
 # ************************************************
 # Define the output schema for the graph
 # ************************************************
+
 schema= """
     { 
     "Projects": [
         "Project #": 
             { 
                 "title": "...", 
                 "description": "...", 
@@ -28,31 +29,33 @@
     } 
 """
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-gemini_key = os.getenv("GOOGLE_APIKEY")
-
 graph_config = {
     "llm": {
-        "api_key": gemini_key,
-        "model": "gemini-pro",
+        "client": "client_name",
+        "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
+        "temperature": 0.0
     },
+    "embeddings": {
+        "model": "bedrock/cohere.embed-multilingual-v3"
+    }
 }
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the news with their description.",
+    prompt="List me all the projects with their description",
     # also accepts a string with the already downloaded HTML code
-    source="https://www.wired.com",
+    source="https://perinim.github.io/projects/",
     schema=schema,
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
```

### Comparing `scrapegraphai-1.5.2/examples/gemini/xml_scraper_openai.py` & `scrapegraphai-1.5.3b1/examples/anthropic/json_scraper_haiku.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 """
-Basic example of scraping pipeline using XMLScraperGraph from XML documents
+Basic example of scraping pipeline using JSONScraperGraph from JSON documents
 """
 
 import os
 from dotenv import load_dotenv
-from scrapegraphai.graphs import XMLScraperGraph
+from scrapegraphai.graphs import JSONScraperGraph
 from scrapegraphai.utils import convert_to_csv, convert_to_json, prettify_exec_info
 load_dotenv()
 
 # ************************************************
-# Read the XML file
+# Read the JSON file
 # ************************************************
 
-FILE_NAME = "inputs/books.xml"
+FILE_NAME = "inputs/example.json"
 curr_dir = os.path.dirname(os.path.realpath(__file__))
 file_path = os.path.join(curr_dir, FILE_NAME)
 
 with open(file_path, 'r', encoding="utf-8") as file:
     text = file.read()
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-openai_key = os.getenv("OPENAI_APIKEY")
-
 graph_config = {
     "llm": {
-        "api_key": openai_key,
-        "model": "gemini-pro",
-    },
+        "api_key": os.getenv("ANTHROPIC_API_KEY"),
+        "model": "claude-3-haiku-20240307",
+        "max_tokens": 4000
+        },
 }
 
 # ************************************************
-# Create the XMLScraperGraph instance and run it
+# Create the JSONScraperGraph instance and run it
 # ************************************************
 
-xml_scraper_graph = XMLScraperGraph(
+json_scraper_graph = JSONScraperGraph(
     prompt="List me all the authors, title and genres of the books",
     source=text,  # Pass the content of the file, not the file object
     config=graph_config
 )
 
-result = xml_scraper_graph.run()
+result = json_scraper_graph.run()
 print(result)
 
 # ************************************************
 # Get graph execution info
 # ************************************************
 
-graph_exec_info = xml_scraper_graph.get_execution_info()
+graph_exec_info = json_scraper_graph.get_execution_info()
 print(prettify_exec_info(graph_exec_info))
 
 # Save to json or csv
 convert_to_csv(result, "result")
 convert_to_json(result, "result")
+
```

### Comparing `scrapegraphai-1.5.2/examples/gemini/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/deepseek/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/deepseek/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/gemini/inputs/plain_html_example.txt` & `scrapegraphai-1.5.3b1/examples/benchmarks/SmartScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/groq/search_graph_groq_openai.py` & `scrapegraphai-1.5.3b1/examples/mixed_models/search_graph_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/groq/smart_scraper_groq_ollama.py` & `scrapegraphai-1.5.3b1/examples/mixed_models/smart_scraper_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/groq/smart_scraper_groq_openai.py` & `scrapegraphai-1.5.3b1/examples/oneapi/smart_scraper_schema_oneapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 """ 
-Basic example of scraping pipeline using SmartScraper
+Basic example of scraping pipeline using SmartScraper and OneAPI
 """
 
-import os
-from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
 
-load_dotenv()
-
-
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
+schema= """
+    { 
+    "Projects": [
+        "Project #": 
+            { 
+                "title": "...", 
+                "description": "...", 
+            }, 
+        "Project #": 
+            { 
+                "title": "...", 
+                "description": "...", 
+            } 
+        ] 
+    } 
+"""
 
-groq_key = os.getenv("GROQ_APIKEY")
-openai_key = os.getenv("OPENAI_APIKEY")
+# ************************************************
+# Define the configuration for the graph
+# *********************************************
 
 graph_config = {
     "llm": {
-        "model": "groq/gemma-7b-it",
-        "api_key": groq_key,
-        "temperature": 0
-    },
-    "embeddings": {
-        "api_key": openai_key,
-        "model": "openai",
-    },
-    "headless": False
+        "api_key": "***************************",
+        "model": "oneapi/qwen-turbo",
+        "base_url": "http://127.0.0.1:3000/v1",  # 设置 OneAPI URL
+    }
 }
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description.",
+     prompt="List me all the projects with their description",
     # also accepts a string with the already downloaded HTML code
     source="https://perinim.github.io/projects/",
-    config=graph_config
+    config=graph_config,
 )
 
-result = smart_scraper_graph.run()
-print(result)
-
 # ************************************************
 # Get graph execution info
 # ************************************************
-
-graph_exec_info = smart_scraper_graph.get_execution_info()
-print(prettify_exec_info(graph_exec_info))
+result = smart_scraper_graph.run()
+print(result)
+print(prettify_exec_info(result))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scrapegraphai-1.5.2/examples/groq/smart_scraper_schema_groq_openai.py` & `scrapegraphai-1.5.3b1/examples/bedrock/smart_scraper_bedrock.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,42 @@
 """ 
-Basic example of scraping pipeline using SmartScraper with schema
+Basic example of scraping pipeline using SmartScraper
 """
 
-import os, json
+import os
 from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
 
 load_dotenv()
 
-# ************************************************
-# Define the output schema for the graph
-# ************************************************
-
-schema= """
-    { 
-    "Projects": [
-        "Project #": 
-            { 
-                "title": "...", 
-                "description": "...", 
-            }, 
-        "Project #": 
-            { 
-                "title": "...", 
-                "description": "...", 
-            } 
-        ] 
-    } 
-"""
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-groq_key = os.getenv("GROQ_APIKEY")
-openai_key = os.getenv("OPENAI_APIKEY")
-
 graph_config = {
     "llm": {
-        "model": "groq/gemma-7b-it",
-        "api_key": groq_key,
-        "temperature": 0
+        "client": "client_name",
+        "model": "bedrock/anthropic.claude-3-sonnet-20240229-v1:0",
+        "temperature": 0.0
     },
     "embeddings": {
-        "api_key": openai_key,
-        "model": "openai",
-    },
-    "headless": False
+        "model": "bedrock/cohere.embed-multilingual-v3"
+    }
 }
 
-
-
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description.",
+    prompt="List me all the projects with their description",
     # also accepts a string with the already downloaded HTML code
     source="https://perinim.github.io/projects/",
-    schema=schema,
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 
 # ************************************************
```

### Comparing `scrapegraphai-1.5.2/examples/huggingfacehub/smart_scraper_huggingfacehub.py` & `scrapegraphai-1.5.3b1/examples/huggingfacehub/smart_scraper_huggingfacehub.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 repo_id = "mistralai/Mistral-7B-Instruct-v0.2"
 
 llm_model_instance = HuggingFaceEndpoint(
     repo_id=repo_id, max_length=128, temperature=0.5, token=HUGGINGFACEHUB_API_TOKEN
 )
 
 
-
-
 embedder_model_instance = HuggingFaceInferenceAPIEmbeddings(
     api_key=HUGGINGFACEHUB_API_TOKEN, model_name="sentence-transformers/all-MiniLM-l6-v2"
 )
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
```

### Comparing `scrapegraphai-1.5.2/examples/local_models/csv_scraper_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/csv_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/json_scraper_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/json_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/pdf_scraper_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/pdf_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/scrape_plain_text_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/scrape_plain_text_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/scrape_xml_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/scrape_xml_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/script_generator_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/script_generator_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/search_graph_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/search_graph_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/smart_scraper_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/smart_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/smart_scraper_schema_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/smart_scraper_schema_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/xml_scraper_ollama.py` & `scrapegraphai-1.5.3b1/examples/local_models/xml_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/gemini/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/gemini/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/local_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.3b1/examples/gemini/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/mixed_models/search_graph_groq_ollama.py` & `scrapegraphai-1.5.3b1/examples/anthropic/search_graph_haiku.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,37 +8,28 @@
 from scrapegraphai.utils import convert_to_csv, convert_to_json, prettify_exec_info
 load_dotenv()
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-groq_key = os.getenv("GROQ_APIKEY")
-
 graph_config = {
     "llm": {
-        "model": "groq/gemma-7b-it",
-        "api_key": groq_key,
-        "temperature": 0
-    },
-    "embeddings": {
-        "model": "ollama/nomic-embed-text",
-        "temperature": 0,
-        "base_url": "http://localhost:11434",  # set ollama URL arbitrarily
-    },
-    "max_results": 2,
-    "verbose": True, 
+        "api_key": os.getenv("ANTHROPIC_API_KEY"),
+        "model": "claude-3-haiku-20240307",
+        "max_tokens": 4000
+        },
 }
 
 # ************************************************
 # Create the SearchGraph instance and run it
 # ************************************************
 
 search_graph = SearchGraph(
-    prompt="List me all the regions of Italy.",
+    prompt="List me Chioggia's famous dishes",
     config=graph_config
 )
 
 result = search_graph.run()
 print(result)
 
 # ************************************************
```

### Comparing `scrapegraphai-1.5.2/examples/mixed_models/smart_scraper_mixed.py` & `scrapegraphai-1.5.3b1/examples/openai/smart_scraper_openai.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,46 +2,42 @@
 Basic example of scraping pipeline using SmartScraper
 """
 
 import os
 from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
+
 load_dotenv()
 
+
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-groq_key = os.getenv("GROQ_APIKEY")
+openai_key = os.getenv("OPENAI_APIKEY")
 
 graph_config = {
     "llm": {
-        "model": "groq/gemma-7b-it",
-        "api_key": groq_key,
-        "temperature": 0
-    },
-    "embeddings": {
-        "model": "ollama/nomic-embed-text",
-        "temperature": 0,
-        "base_url": "http://localhost:11434",  # set ollama URL arbitrarily
+        "api_key": openai_key,
+        "model": "gpt-3.5-turbo",
     },
+    "verbose": False,
     "headless": False,
-    "verbose": True,
 }
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description and the author.",
+    prompt="List me all the projects with their description",
     # also accepts a string with the already downloaded HTML code
-    source="https://perinim.github.io/projects",
-    config=graph_config
+    source="https://perinim.github.io/projects/",
+    config=graph_config,
 )
 
 result = smart_scraper_graph.run()
 print(result)
 
 # ************************************************
 # Get graph execution info
```

### Comparing `scrapegraphai-1.5.2/examples/mixed_models/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/groq/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/mixed_models/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/groq/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/mixed_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.3b1/examples/groq/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/oneapi/smart_scraper_schema_oneapi.py` & `scrapegraphai-1.5.3b1/examples/openai/smart_scraper_schema_openai.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """ 
-Basic example of scraping pipeline using SmartScraper and OneAPI
+Basic example of scraping pipeline using SmartScraper with schema
 """
 
+import os, json
+from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
-from scrapegraphai.utils import prettify_exec_info
+
+load_dotenv()
 
 # ************************************************
-# Define the configuration for the graph
+# Define the output schema for the graph
 # ************************************************
+
 schema= """
     { 
     "Projects": [
         "Project #": 
             { 
                 "title": "...", 
                 "description": "...", 
@@ -23,39 +27,33 @@
             } 
         ] 
     } 
 """
 
 # ************************************************
 # Define the configuration for the graph
-# *********************************************
+# ************************************************
+
+openai_key = os.getenv("OPENAI_APIKEY")
 
 graph_config = {
     "llm": {
-        "api_key": "***************************",
-        "model": "oneapi/qwen-turbo",
-        "base_url": "http://127.0.0.1:3000/v1",  # 设置 OneAPI URL
+        "api_key":openai_key,
+        "model": "gpt-3.5-turbo",
     },
-    "embeddings": {
-        "model": "ollama/nomic-embed-text",
-        "base_url": "http://127.0.0.1:11434",  # 设置 Ollama URL
-    }
+    "verbose": True,
+    "headless": False,
 }
 
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="该网站为XXXXX,请提取出标题、发布时间、发布来源以及内容摘要,并以中文回答",
-    # 也可以使用已下载的 HTML 代码的字符串
-    source="http://XXXX",
+    prompt="List me all the projects with their description",
+    source="https://perinim.github.io/projects/",
     schema=schema,
     config=graph_config
 )
 
-# ************************************************
-# Get graph execution info
-# ************************************************
 result = smart_scraper_graph.run()
-print(result)
-print(prettify_exec_info(result))
+print(json.dumps(result, indent=4))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scrapegraphai-1.5.2/examples/oneapi/smartscraper_oneapi.py` & `scrapegraphai-1.5.3b1/examples/mixed_models/smartscraper_oneapi_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/csv_scraper_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/csv_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/custom_graph_openai.py` & `scrapegraphai-1.5.3b1/examples/anthropic/custom_graph_haiku.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 from scrapegraphai.nodes import FetchNode, ParseNode, RAGNode, GenerateAnswerNode, RobotsNode
 load_dotenv()
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-openai_key = os.getenv("OPENAI_APIKEY")
-
 graph_config = {
     "llm": {
-        "api_key": openai_key,
-        "model": "gpt-3.5-turbo",
-        "temperature": 0,
-        "streaming": False
-    },
+        "api_key": os.getenv("ANTHROPIC_API_KEY"),
+        "model": "claude-3-haiku-20240307",
+        "max_tokens": 4000
+        },
 }
 
 # ************************************************
 # Define the graph nodes
 # ************************************************
 
 llm_model = OpenAI(graph_config["llm"])
```

### Comparing `scrapegraphai-1.5.2/examples/openai/deep_scraper_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/deep_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/json_scraper_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/json_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/omni_scraper_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/omni_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/omni_search_graph_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/omni_search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/pdf_scraper_graph_openai.py` & `scrapegraphai-1.5.3b1/examples/oneapi/pdf_scraper_graph_oneapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import os, json
-from dotenv import load_dotenv
 from scrapegraphai.graphs import PDFScraperGraph
 
-load_dotenv()
-
-
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-openai_key = os.getenv("OPENAI_APIKEY")
-
 graph_config = {
     "llm": {
-        "api_key": openai_key,
-        "model": "gpt-3.5-turbo",
-    },
-    "verbose": True,
-    "headless": False,
+        "api_key": "***************************",
+        "model": "oneapi/qwen-turbo",
+        "base_url": "http://127.0.0.1:3000/v1",  # 设置 OneAPI URL
+    }
 }
 
 source = """
     The Divine Comedy, Italian La Divina Commedia, original name La commedia, long narrative poem written in Italian 
     circa 1308/21 by Dante. It is usually held to be one of the world s great works of literature. 
     Divided into three major sections—Inferno, Purgatorio, and Paradiso—the narrative traces the journey of Dante 
     from darkness and error to the revelation of the divine light, culminating in the Beatific Vision of God.
```

### Comparing `scrapegraphai-1.5.2/examples/openai/scrape_plain_text_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/scrape_plain_text_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/script_generator_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/script_generator_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/search_graph_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/smart_scraper_multi_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/smart_scraper_multi_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/smart_scraper_openai.py` & `scrapegraphai-1.5.3b1/examples/deepseek/scrape_plain_text_deepseek.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 """ 
-Basic example of scraping pipeline using SmartScraper
+Basic example of scraping pipeline using SmartScraper from text
 """
 
 import os
 from dotenv import load_dotenv
 from scrapegraphai.graphs import SmartScraperGraph
 from scrapegraphai.utils import prettify_exec_info
-
 load_dotenv()
 
+# ************************************************
+# Read the text file
+# ************************************************
+
+FILE_NAME = "inputs/plain_html_example.txt"
+curr_dir = os.path.dirname(os.path.realpath(__file__))
+file_path = os.path.join(curr_dir, FILE_NAME)
+
+# It could be also a http request using the request model
+with open(file_path, 'r', encoding="utf-8") as file:
+    text = file.read()
 
 # ************************************************
 # Define the configuration for the graph
 # ************************************************
 
-openai_key = os.getenv("OPENAI_APIKEY")
+deepseek_key = os.getenv("DEEPSEEK_APIKEY")
 
 graph_config = {
     "llm": {
-        "api_key": openai_key,
-        "model": "gpt-3.5-turbo",
+        "model": "deepseek-chat",
+        "openai_api_key": deepseek_key,
+        "openai_api_base": 'https://api.deepseek.com/v1',
     },
-    "verbose": False,
-    "headless": False,
+    "verbose": True,
 }
-
 # ************************************************
 # Create the SmartScraperGraph instance and run it
 # ************************************************
 
 smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description",
-    # also accepts a string with the already downloaded HTML code
-    source="https://perinim.github.io/projects/",
-    config=graph_config,
+    prompt="List me all the news with their description.",
+    source=text,
+    config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 
 # ************************************************
 # Get graph execution info
```

### Comparing `scrapegraphai-1.5.2/examples/openai/smart_scraper_schema_openai.py` & `scrapegraphai-1.5.3b1/tests/graphs/smart_scraper_ollama_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 """ 
-Basic example of scraping pipeline using SmartScraper with schema
+Module for testing th smart scraper class
 """
-
-import os, json
-from dotenv import load_dotenv
+import pytest
 from scrapegraphai.graphs import SmartScraperGraph
 
-load_dotenv()
 
-# ************************************************
-# Define the output schema for the graph
-# ************************************************
-
-schema= """
-    { 
-    "Projects": [
-        "Project #": 
-            { 
-                "title": "...", 
-                "description": "...", 
-            }, 
-        "Project #": 
-            { 
-                "title": "...", 
-                "description": "...", 
-            } 
-        ] 
-    } 
-"""
+@pytest.fixture
+def graph_config():
+    """
+    Configuration of the graph
+    """
+    return {
+        "llm": {
+            "model": "ollama/mistral",
+            "temperature": 0,
+            "format": "json",
+            "base_url": "http://localhost:11434",
+        },
+        "embeddings": {
+            "model": "ollama/nomic-embed-text",
+            "temperature": 0,
+            "base_url": "http://localhost:11434",
+        }
+    }
+
+
+def test_scraping_pipeline(graph_config: dict):
+    """
+    Start of the scraping pipeline
+    """
+    smart_scraper_graph = SmartScraperGraph(
+        prompt="List me all the news with their description.",
+        source="https://perinim.github.io/projects",
+        config=graph_config
+    )
+
+    result = smart_scraper_graph.run()
+
+    assert result is not None
+
+
+def test_get_execution_info(graph_config: dict):
+    """
+    Get the execution info
+    """
+    smart_scraper_graph = SmartScraperGraph(
+        prompt="List me all the news with their description.",
+        source="https://perinim.github.io/projects",
+        config=graph_config
+    )
+
+    smart_scraper_graph.run()
 
-# ************************************************
-# Define the configuration for the graph
-# ************************************************
-
-openai_key = os.getenv("OPENAI_APIKEY")
-
-graph_config = {
-    "llm": {
-        "api_key":openai_key,
-        "model": "gpt-3.5-turbo",
-    },
-    "verbose": True,
-    "headless": False,
-}
-
-# ************************************************
-# Create the SmartScraperGraph instance and run it
-# ************************************************
-
-smart_scraper_graph = SmartScraperGraph(
-    prompt="List me all the projects with their description",
-    source="https://perinim.github.io/projects/",
-    schema=schema,
-    config=graph_config
-)
+    graph_exec_info = smart_scraper_graph.get_execution_info()
 
-result = smart_scraper_graph.run()
-print(json.dumps(result, indent=4))
+    assert graph_exec_info is not None
```

### Comparing `scrapegraphai-1.5.2/examples/openai/speech_graph_openai.py` & `scrapegraphai-1.5.3b1/examples/openai/speech_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/xml_scraper_openai.py` & `scrapegraphai-1.5.3b1/examples/oneapi/xml_scraper_oneapi.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/huggingfacehub/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/huggingfacehub/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/openai/inputs/plain_html_example.txt` & `scrapegraphai-1.5.3b1/examples/huggingfacehub/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/single_node/fetch_node.py` & `scrapegraphai-1.5.3b1/examples/single_node/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/single_node/image2text_node.py` & `scrapegraphai-1.5.3b1/examples/single_node/image2text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/single_node/kg_node.py` & `scrapegraphai-1.5.3b1/examples/single_node/kg_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/examples/single_node/robot_node.py` & `scrapegraphai-1.5.3b1/examples/single_node/robot_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/manual deployment/commit_and_push.sh` & `scrapegraphai-1.5.3b1/manual deployment/commit_and_push.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/manual deployment/commit_and_push_with_tests.sh` & `scrapegraphai-1.5.3b1/manual deployment/commit_and_push_with_tests.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-1.5.3b1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/docloaders/chromium.py` & `scrapegraphai-1.5.3b1/scrapegraphai/docloaders/chromium.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/__init__.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/deep_scraper_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/deep_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/omni_scraper_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/omni_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/omni_search_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/omni_search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/smart_scraper_multi_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/smart_scraper_multi_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-1.5.3b1/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/__init__.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_csv_prompts.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_csv_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_omni_prompts.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_omni_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/generate_answer_node_prompts.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/generate_answer_node_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/models_tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         # embedding models
         "nomic-embed-text": 8192,
         "snowflake-arctic-embed:335m": 8192,
         "snowflake-arctic-embed:l": 8192,
         "mxbai-embed-large": 512,
     },
     "oneapi": {
-        "qwen-turbo": 16380
+        "qwen-turbo": 6000 
     },
     "groq": {
         "llama3-8b-8192": 8192,
         "llama3-70b-8192": 8192,
         "mixtral-8x7b-32768": 32768,
         "gemma-7b-it": 8192,
     },
```

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/helpers/schemas.py` & `scrapegraphai-1.5.3b1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/integrations/burr_bridge.py` & `scrapegraphai-1.5.3b1/scrapegraphai/integrations/burr_bridge.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/models/bedrock.py` & `scrapegraphai-1.5.3b1/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/models/gemini.py` & `scrapegraphai-1.5.3b1/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/models/openai_itt.py` & `scrapegraphai-1.5.3b1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/models/openai_tts.py` & `scrapegraphai-1.5.3b1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/__init__.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/base_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_omni_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_omni_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/search_node_with_context.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/search_node_with_context.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-1.5.3b1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/cleanup_html.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/cleanup_html.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/logging.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/research_web.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/sys_dynamic_import.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-1.5.3b1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/scrape_json_ollama.py` & `scrapegraphai-1.5.3b1/tests/graphs/scrape_json_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/scrape_plain_text_llama3_test.py` & `scrapegraphai-1.5.3b1/tests/graphs/scrape_plain_text_llama3_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/scrape_plain_text_mistral_test.py` & `scrapegraphai-1.5.3b1/tests/graphs/scrape_plain_text_mistral_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/scrape_xml_ollama_test.py` & `scrapegraphai-1.5.3b1/tests/graphs/scrape_xml_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/script_generator_test.py` & `scrapegraphai-1.5.3b1/tests/graphs/script_generator_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/local_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/local_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/graphs/inputs/plain_html_example.txt` & `scrapegraphai-1.5.3b1/examples/local_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/nodes/fetch_node_test.py` & `scrapegraphai-1.5.3b1/tests/nodes/fetch_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/nodes/robot_node_test.py` & `scrapegraphai-1.5.3b1/tests/nodes/robot_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/nodes/search_link_node_test.py` & `scrapegraphai-1.5.3b1/tests/nodes/search_link_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/nodes/inputs/books.xml` & `scrapegraphai-1.5.3b1/examples/mixed_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/nodes/inputs/example.json` & `scrapegraphai-1.5.3b1/examples/mixed_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/nodes/inputs/plain_html_example.txt` & `scrapegraphai-1.5.3b1/examples/mixed_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/utils/test_proxy_rotation.py` & `scrapegraphai-1.5.3b1/tests/utils/test_proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/tests/utils/test_sys_dynamic_import.py` & `scrapegraphai-1.5.3b1/tests/utils/test_sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/LICENSE` & `scrapegraphai-1.5.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.2/README.md` & `scrapegraphai-1.5.3b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/scrapegraphai_logo.png" alt="Scrapegraph-ai Logo" style="width: 50%;">
 </p>
 
 ## 🚀 Quick install
 
-The reference page for Scrapegraph-ai is available on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
+The reference page for Scrapegraph-ai is available on the official page of PyPI: [pypi](https://pypi.org/project/scrapegraphai/).
 
 ```bash
 pip install scrapegraphai
 ```
 
 **Note**: it is recommended to install the library in a virtual environment to avoid conflicts with other libraries 🐱
 
 ## 🔍 Demo
 Official streamlit demo:
 
-[![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-demo.streamlit.app/)
+[![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-web-dashboard.streamlit.app)
 
 Try it directly on the web using Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1sEZBonBMGP44CtO6GQTwAlL0BGJXjtfd?usp=sharing)
 
 ## 📖 Documentation
```

### Comparing `scrapegraphai-1.5.2/pyproject.toml` & `scrapegraphai-1.5.3b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "scrapegraphai"
 
 
-version = "1.5.2"
+version = "1.5.3b1"
 
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     { name = "Marco Vinciguerra", email = "mvincig11@gmail.com" },
     { name = "Marco Perini", email = "perinim.98@gmail.com" },
     { name = "Lorenzo Padoan", email = "lorenzo.padoan977@gmail.com" }
```

### Comparing `scrapegraphai-1.5.2/PKG-INFO` & `scrapegraphai-1.5.3b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scrapegraphai
-Version: 1.5.2
+Version: 1.5.3b1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Author-email: Marco Vinciguerra <mvincig11@gmail.com>, Marco Perini <perinim.98@gmail.com>, Lorenzo Padoan <lorenzo.padoan977@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ai,artificial intelligence,gpt,graph,langchain,machine learning,natural language processing,nlp,openai,rag,scrapegraph,scrapegraphai,scraping,web scraping,web scraping library,web scraping tool,webscraping
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -52,26 +52,26 @@
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/scrapegraphai_logo.png" alt="Scrapegraph-ai Logo" style="width: 50%;">
 </p>
 
 ## 🚀 Quick install
 
-The reference page for Scrapegraph-ai is available on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
+The reference page for Scrapegraph-ai is available on the official page of PyPI: [pypi](https://pypi.org/project/scrapegraphai/).
 
 ```bash
 pip install scrapegraphai
 ```
 
 **Note**: it is recommended to install the library in a virtual environment to avoid conflicts with other libraries 🐱
 
 ## 🔍 Demo
 Official streamlit demo:
 
-[![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-demo.streamlit.app/)
+[![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-web-dashboard.streamlit.app)
 
 Try it directly on the web using Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1sEZBonBMGP44CtO6GQTwAlL0BGJXjtfd?usp=sharing)
 
 ## 📖 Documentation
```

