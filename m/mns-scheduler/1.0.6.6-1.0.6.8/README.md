# Comparing `tmp/mns-scheduler-1.0.6.6.tar.gz` & `tmp/mns-scheduler-1.0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.6.6.tar", last modified: Wed May 29 13:08:04 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.6.8.tar", last modified: Wed May 29 15:17:35 2024, max compression
```

## Comparing `mns-scheduler-1.0.6.6.tar` & `mns-scheduler-1.0.6.8.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.817261 mns-scheduler-1.0.6.6/
--rw-rw-rw-   0        0        0       62 2024-05-29 13:08:04.817261 mns-scheduler-1.0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.775372 mns-scheduler-1.0.6.6/mns_scheduler/
--rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.6.6/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.778365 mns-scheduler-1.0.6.6/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.778365 mns-scheduler-1.0.6.6/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.780360 mns-scheduler-1.0.6.6/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.781357 mns-scheduler-1.0.6.6/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.782354 mns-scheduler-1.0.6.6/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.784348 mns-scheduler-1.0.6.6/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.6.6/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    22727 2024-05-24 07:13:02.000000 mns-scheduler-1.0.6.6/mns_scheduler/company_info/company_info_sync_api.py
--rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.6.6/mns_scheduler/company_info/de_list_stock_service.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.784348 mns-scheduler-1.0.6.6/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.785346 mns-scheduler-1.0.6.6/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.786344 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.787342 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.789336 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5315 2024-05-29 04:39:42.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3990 2024-05-29 13:06:57.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.790332 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.791330 mns-scheduler-1.0.6.6/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-29 07:44:21.000000 mns-scheduler-1.0.6.6/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.792327 mns-scheduler-1.0.6.6/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.795319 mns-scheduler-1.0.6.6/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/__init__.py
--rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
--rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/em_financial_profit_sync_service_api.py
--rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/finance_common_api.py
--rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
--rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/sync_financial_report_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.796317 mns-scheduler-1.0.6.6/mns_scheduler/finance/test/
--rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/test/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.6.6/mns_scheduler/finance/test/fix_blask_list.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.796317 mns-scheduler-1.0.6.6/mns_scheduler/hk/
--rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.6.6/mns_scheduler/hk/__init__.py
--rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.6.6/mns_scheduler/hk/hk_company_info_sync_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.797314 mns-scheduler-1.0.6.6/mns_scheduler/irm/
--rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.6.6/mns_scheduler/irm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.799308 mns-scheduler-1.0.6.6/mns_scheduler/irm/api/
--rw-rw-rw-   0        0        0      163 2024-05-24 14:59:41.000000 mns-scheduler-1.0.6.6/mns_scheduler/irm/api/__init__.py
--rw-rw-rw-   0        0        0     4931 2024-05-24 22:45:39.000000 mns-scheduler-1.0.6.6/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
--rw-rw-rw-   0        0        0     6199 2024-05-25 08:40:25.000000 mns-scheduler-1.0.6.6/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
--rw-rw-rw-   0        0        0     8923 2024-05-29 13:05:22.000000 mns-scheduler-1.0.6.6/mns_scheduler/irm/stock_irm_cninfo_service.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.799308 mns-scheduler-1.0.6.6/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.801303 mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    22262 2024-05-23 09:26:20.000000 mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     8118 2024-05-23 15:00:37.000000 mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py
--rw-rw-rw-   0        0        0     2628 2024-05-23 15:06:42.000000 mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.802300 mns-scheduler-1.0.6.6/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.6.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.802300 mns-scheduler-1.0.6.6/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.802300 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.804296 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.805292 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.806290 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.806290 mns-scheduler-1.0.6.6/mns_scheduler/lhb/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.6.6/mns_scheduler/lhb/__init__.py
--rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.6.6/mns_scheduler/lhb/stock_lhb_sync_service.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.808285 mns-scheduler-1.0.6.6/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-28 09:19:49.000000 mns-scheduler-1.0.6.6/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.809282 mns-scheduler-1.0.6.6/mns_scheduler/risk/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.6.6/mns_scheduler/risk/__init__.py
--rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.6.6/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
--rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.6.6/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.811277 mns-scheduler-1.0.6.6/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.6.6/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.6.6/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.6.6/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.812274 mns-scheduler-1.0.6.6/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.815266 mns-scheduler-1.0.6.6/mns_scheduler/zt/
--rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.6.6/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17525 2024-05-29 09:53:47.000000 mns-scheduler-1.0.6.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-05-29 09:53:47.000000 mns-scheduler-1.0.6.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.6.6/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.816263 mns-scheduler-1.0.6.6/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    16847 2024-05-25 09:07:13.000000 mns-scheduler-1.0.6.6/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:08:04.816263 mns-scheduler-1.0.6.6/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-29 13:08:04.000000 mns-scheduler-1.0.6.6/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4351 2024-05-29 13:08:04.000000 mns-scheduler-1.0.6.6/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 13:08:04.000000 mns-scheduler-1.0.6.6/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 13:08:04.000000 mns-scheduler-1.0.6.6/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 13:08:04.817261 mns-scheduler-1.0.6.6/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-29 13:07:23.000000 mns-scheduler-1.0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.521816 mns-scheduler-1.0.6.8/
+-rw-rw-rw-   0        0        0       62 2024-05-29 15:17:35.520818 mns-scheduler-1.0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.6.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.480954 mns-scheduler-1.0.6.8/mns_scheduler/
+-rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.6.8/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.482920 mns-scheduler-1.0.6.8/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.483947 mns-scheduler-1.0.6.8/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.485940 mns-scheduler-1.0.6.8/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.486938 mns-scheduler-1.0.6.8/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.487935 mns-scheduler-1.0.6.8/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.488932 mns-scheduler-1.0.6.8/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.6.8/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    22727 2024-05-24 07:13:02.000000 mns-scheduler-1.0.6.8/mns_scheduler/company_info/company_info_sync_api.py
+-rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.6.8/mns_scheduler/company_info/de_list_stock_service.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.489935 mns-scheduler-1.0.6.8/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.490930 mns-scheduler-1.0.6.8/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.490930 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.492895 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.493918 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5315 2024-05-29 04:39:42.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3990 2024-05-29 13:06:57.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.495886 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.496910 mns-scheduler-1.0.6.8/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-29 07:44:21.000000 mns-scheduler-1.0.6.8/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.497908 mns-scheduler-1.0.6.8/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.499902 mns-scheduler-1.0.6.8/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+-rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/em_financial_profit_sync_service_api.py
+-rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/finance_common_api.py
+-rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+-rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/sync_financial_report_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.500900 mns-scheduler-1.0.6.8/mns_scheduler/finance/test/
+-rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/test/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.6.8/mns_scheduler/finance/test/fix_blask_list.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.501898 mns-scheduler-1.0.6.8/mns_scheduler/hk/
+-rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.6.8/mns_scheduler/hk/__init__.py
+-rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.6.8/mns_scheduler/hk/hk_company_info_sync_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.502896 mns-scheduler-1.0.6.8/mns_scheduler/irm/
+-rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.6.8/mns_scheduler/irm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.503892 mns-scheduler-1.0.6.8/mns_scheduler/irm/api/
+-rw-rw-rw-   0        0        0      163 2024-05-24 14:59:41.000000 mns-scheduler-1.0.6.8/mns_scheduler/irm/api/__init__.py
+-rw-rw-rw-   0        0        0     4931 2024-05-24 22:45:39.000000 mns-scheduler-1.0.6.8/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     6199 2024-05-25 08:40:25.000000 mns-scheduler-1.0.6.8/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     8923 2024-05-29 13:05:22.000000 mns-scheduler-1.0.6.8/mns_scheduler/irm/stock_irm_cninfo_service.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.503892 mns-scheduler-1.0.6.8/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.505887 mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    22262 2024-05-23 09:26:20.000000 mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     8118 2024-05-23 15:00:37.000000 mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+-rw-rw-rw-   0        0        0     2628 2024-05-23 15:06:42.000000 mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.506884 mns-scheduler-1.0.6.8/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.6.8/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.506884 mns-scheduler-1.0.6.8/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.507882 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.508879 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.509848 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.510846 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.510846 mns-scheduler-1.0.6.8/mns_scheduler/lhb/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.6.8/mns_scheduler/lhb/__init__.py
+-rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.6.8/mns_scheduler/lhb/stock_lhb_sync_service.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.512840 mns-scheduler-1.0.6.8/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9491 2024-05-29 15:14:09.000000 mns-scheduler-1.0.6.8/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.513837 mns-scheduler-1.0.6.8/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.6.8/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.6.8/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+-rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.6.8/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.515832 mns-scheduler-1.0.6.8/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.6.8/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.6.8/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.6.8/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.515832 mns-scheduler-1.0.6.8/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.518824 mns-scheduler-1.0.6.8/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.6.8/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17525 2024-05-29 09:53:47.000000 mns-scheduler-1.0.6.8/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-05-29 09:53:47.000000 mns-scheduler-1.0.6.8/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.6.8/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.519821 mns-scheduler-1.0.6.8/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16850 2024-05-29 13:46:49.000000 mns-scheduler-1.0.6.8/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.8/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:17:35.520818 mns-scheduler-1.0.6.8/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-29 15:17:35.000000 mns-scheduler-1.0.6.8/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4351 2024-05-29 15:17:35.000000 mns-scheduler-1.0.6.8/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 15:17:35.000000 mns-scheduler-1.0.6.8/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 15:17:35.000000 mns-scheduler-1.0.6.8/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 15:17:35.521816 mns-scheduler-1.0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-29 15:17:09.000000 mns-scheduler-1.0.6.8/setup.py
```

### Comparing `mns-scheduler-1.0.6.6/README.md` & `mns-scheduler-1.0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.6.8/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.6.8/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.6.8/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/company_info/de_list_stock_service.py` & `mns-scheduler-1.0.6.8/mns_scheduler/company_info/de_list_stock_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.6.8/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.6.8/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/finance/em_financial_profit_sync_service_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/finance/em_financial_profit_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/finance/finance_common_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/finance/finance_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/finance/sync_financial_report_service_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/finance/sync_financial_report_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/finance/test/fix_blask_list.py` & `mns-scheduler-1.0.6.8/mns_scheduler/finance/test/fix_blask_list.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/hk/hk_company_info_sync_service_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/hk/hk_company_info_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/irm/stock_irm_cninfo_service.py` & `mns-scheduler-1.0.6.8/mns_scheduler/irm/stock_irm_cninfo_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py` & `mns-scheduler-1.0.6.8/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/lhb/stock_lhb_sync_service.py` & `mns-scheduler-1.0.6.8/mns_scheduler/lhb/stock_lhb_sync_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.6.8/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,28 +182,33 @@
                                                                          str_now_date, number)
                 save_real_time_quotes(real_time_quotes_now.copy(), now_date, db_name_constant.REAL_TIME_QUOTES_NOW,
                                       number)
                 try:
                     auto_sell_service_api.auto_sell_stock(real_time_quotes_now.copy())
                 except Exception as e:
                     logger.error("自动卖出执行异常:{}", e)
+                if date_util.is_call_auction(str_now_date):
+                    if number % 4 == 0:
+                        save_real_time_quotes_his(real_time_quotes_now.copy(), now_date, realtime_quotes_db_name,
+                                                  number_his)
+                        number_his = number_his + 1
 
-                if date_util.is_call_auction(str_now_date) or date_util.is_afternoon_time(now_date):
+                if date_util.is_afternoon_time(now_date):
                     if number % 3 == 0:
                         save_real_time_quotes_his(real_time_quotes_now.copy(), now_date, realtime_quotes_db_name,
                                                   number_his)
                         number_his = number_his + 1
 
                 elif date_util.is_begin_one_hour(now_date):
                     save_real_time_quotes_his(real_time_quotes_now.copy(), now_date, realtime_quotes_db_name,
                                               number_his)
                     number_his = number_his + 1
 
                 else:
-
+                    # 10:30 到11:30
                     if number % 2 == 0:
                         save_real_time_quotes_his(real_time_quotes_now.copy(), now_date, realtime_quotes_db_name,
                                                   number_his)
                         number_his = number_his + 1
 
                 logger.info("同步实时行情信息:{}", number)
                 number = number + 1
```

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/risk/register_and_investigate_stock_sync_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/risk/register_and_investigate_stock_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/risk/stock_equity_mortgage_sync_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/risk/stock_equity_mortgage_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zt/__init__.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zt/__init__.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 # 更新概念指数下所有股票组成 by 概念代码
 blockingScheduler.add_job(update_one_concept_all_symbol_detail, 'cron', hour='08,18,12', minute='30')
 
 # 同步单只股票下所有概念 by 股票代码
 blockingScheduler.add_job(update_one_symbol_all_concepts, 'cron', hour='09,18,12', minute='15')
 
 # 开盘前同步同花顺新概念指数
-blockingScheduler.add_job(sync_new_concept_data_web, 'cron', hour='09', minute='05,10,15,20,25')
+blockingScheduler.add_job(sync_new_concept_data_web, 'cron', hour='09', minute='05,10,15,20,25,29')
 
 # 同步同花顺新增概念指数(定时轮训,暂时10分钟)
 blockingScheduler.add_job(sync_new_concept_data_web, 'interval', minutes=10, max_instances=4)
 
 # 同步开盘啦新增精选概念(定时轮训,暂时五分钟)
 blockingScheduler.add_job(sync_all_kpl_plate_info, 'interval', minutes=5, max_instances=4)
```

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.6.8/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.6/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.6.8/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

