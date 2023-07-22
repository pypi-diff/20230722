# Comparing `tmp/ultibi-0.3.4.tar.gz` & `tmp/ultibi-0.4.0.tar.gz`

## Comparing `ultibi-0.3.4.tar` & `ultibi-0.4.0.tar`

### file list

```diff
@@ -1,153 +1,163 @@
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/frtb_engine/Cargo.toml
--rw-r--r--   0     1001      123      481 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/README.md
--rw-r--r--   0     1001      123    14931 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/Delta.csv
--rw-r--r--   0     1001      123      541 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
--rw-r--r--   0     1001      123     2160 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
--rw-r--r--   0     1001      123      159 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/hms.csv
--rw-r--r--   0     1001      123      177 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
--rw-r--r--   0     1001      123    20066 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/calc_params.rs
--rw-r--r--   0     1001      123       25 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/docs/mod.rs
--rw-r--r--   0     1001      123     1226 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/docs/optional_params.rs
--rw-r--r--   0     1001      123     1424 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/common.rs
--rw-r--r--   0     1001      123    11840 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
--rw-r--r--   0     1001      123     9483 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
--rw-r--r--   0     1001      123     7606 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_weights.rs
--rw-r--r--   0     1001      123       96 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/mod.rs
--rw-r--r--   0     1001      123      787 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/totals.rs
--rw-r--r--   0     1001      123     4811 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/helpers.rs
--rw-r--r--   0     1001      123     8968 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/lib.rs
--rw-r--r--   0     1001      123     3780 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/measures.rs
--rw-r--r--   0     1001      123      188 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/prelude.rs
--rw-r--r--   0     1001      123    26516 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights.rs
--rw-r--r--   0     1001      123     5408 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
--rw-r--r--   0     1001      123     5268 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/rrao/mod.rs
--rw-r--r--   0     1001      123     1374 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/buckets.rs
--rw-r--r--   0     1001      123    14177 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
--rw-r--r--   0     1001      123    13866 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
--rw-r--r--   0     1001      123     3699 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
--rw-r--r--   0     1001      123     7432 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
--rw-r--r--   0     1001      123    29827 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common.rs
--rw-r--r--   0     1001      123     9793 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common_curv.rs
--rw-r--r--   0     1001      123    19318 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
--rw-r--r--   0     1001      123    17703 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
--rw-r--r--   0     1001      123     3841 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
--rw-r--r--   0     1001      123    11803 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
--rw-r--r--   0     1001      123    15617 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
--rw-r--r--   0     1001      123    12459 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
--rw-r--r--   0     1001      123     2904 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
--rw-r--r--   0     1001      123     8782 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
--rw-r--r--   0     1001      123    15261 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
--rw-r--r--   0     1001      123    13479 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
--rw-r--r--   0     1001      123     2988 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
--rw-r--r--   0     1001      123     8063 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
--rw-r--r--   0     1001      123    17052 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
--rw-r--r--   0     1001      123    10900 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
--rw-r--r--   0     1001      123     2162 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
--rw-r--r--   0     1001      123    10428 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
--rw-r--r--   0     1001      123    14289 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
--rw-r--r--   0     1001      123    11992 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
--rw-r--r--   0     1001      123     2162 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
--rw-r--r--   0     1001      123    10166 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
--rw-r--r--   0     1001      123    14030 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
--rw-r--r--   0     1001      123    21887 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
--rw-r--r--   0     1001      123     2295 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
--rw-r--r--   0     1001      123    15657 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
--rw-r--r--   0     1001      123      221 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/mod.rs
--rw-r--r--   0     1001      123     5170 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/totals.rs
--rw-r--r--   0     1001      123    28643 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/statics.rs
--rw-r--r--   0     1001      123      753 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/totals.rs
--rw-r--r--   0     1001      123     1881 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/validate.rs
--rw-r--r--   0     1001      123     1756 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/common/mod.rs
--rw-r--r--   0     1001      123     1486 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/dependant.rs
--rw-r--r--   0     1001      123     4487 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/drc.rs
--rw-r--r--   0     1001      123      420 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/rrao.rs
--rw-r--r--   0     1001      123    18903 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm.rs
--rw-r--r--   0     1001      123      744 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm_totals.rs
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/ultibi_server/Cargo.toml
--rw-r--r--   0     1001      123      219 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/build.rs
--rw-r--r--   0     1001      123       35 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/api/mod.rs
--rw-r--r--   0     1001      123      754 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/api/open_api.rs
--rw-r--r--   0     1001      123     6651 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/api/routers.rs
--rw-r--r--   0     1001      123     1264 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/app.rs
--rw-r--r--   0     1001      123     2593 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/helpers.rs
--rw-r--r--   0     1001      123     1432 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/lib.rs
--rw-r--r--   0     1001      123      433 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/visual.rs
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/ultibi/Cargo.toml
--rw-r--r--   0     1001      123        0 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi/README.md
--rw-r--r--   0     1001      123       73 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi/src/lib.rs
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/ultibi_core/Cargo.toml
--rw-r--r--   0     1001      123     2031 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/add_row.rs
--rw-r--r--   0     1001      123     3486 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/aggregations.rs
--rw-r--r--   0     1001      123      654 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/cache.rs
--rw-r--r--   0     1001      123     4244 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datarequest.rs
--rw-r--r--   0     1001      123     9751 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/dataset.rs
--rw-r--r--   0     1001      123     1782 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/acquire.rs
--rw-r--r--   0     1001      123     2059 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/awss3.rs
--rw-r--r--   0     1001      123     5329 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/helpers.rs
--rw-r--r--   0     1001      123     7509 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/mod.rs
--rw-r--r--   0     1001      123      700 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/errors.rs
--rw-r--r--   0     1001      123    10956 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg.rs
--rw-r--r--   0     1001      123     4594 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
--rw-r--r--   0     1001      123      464 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/mod.rs
--rw-r--r--   0     1001      123     2663 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/filters.rs
--rw-r--r--   0     1001      123       18 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/helpers/mod.rs
--rw-r--r--   0     1001      123      545 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/helpers/searches.rs
--rw-r--r--   0     1001      123      375 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/lib.rs
--rw-r--r--   0     1001      123    11996 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/measure.rs
--rw-r--r--   0     1001      123     5459 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/overrides.rs
--rw-r--r--   0     1001      123      230 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/prelude.rs
--rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/reports/mod.rs
--rw-r--r--   0     1001      123     1178 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/reports/report.rs
--rw-r--r--   0     1001      123     1884 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/add_row.rs
--rw-r--r--   0     1001      123      741 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/agg_request.rs
--rw-r--r--   0     1001      123     1543 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/aggregations.rs
--rw-r--r--   0     1001      123        1 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/cache.rs
--rw-r--r--   0     1001      123     2067 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/common/mod.rs
--rw-r--r--   0     1001      123       95 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/bad_config.toml
--rw-r--r--   0     1001      123      553 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/bad_config2.toml
--rw-r--r--   0     1001      123      116 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/test_config.toml
--rw-r--r--   0     1001      123      354 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/testset.csv
--rw-r--r--   0     1001      123     1250 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/datasource.rs
--rw-r--r--   0     1001      123     3115 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/dependants.rs
--rw-r--r--   0     1001      123     1485 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/filters.rs
--rw-r--r--   0     1001      123        1 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/overrides.rs
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 ultibi-0.3.4/Cargo.toml
--rw-r--r--   0     1001      123      728 2023-06-20 17:50:17.000000 ultibi-0.3.4/.gitignore
--rw-r--r--   0     1001      123     5183 2023-06-20 17:50:17.000000 ultibi-0.3.4/LICENSE
--rw-r--r--   0     1001      123     2403 2023-06-20 17:50:17.000000 ultibi-0.3.4/Makefile
--rw-r--r--   0     1001      123     5565 2023-06-20 17:50:17.000000 ultibi-0.3.4/README.md
--rw-r--r--   0     1001      123     1559 2023-06-20 17:50:17.000000 ultibi-0.3.4/example.py
--rw-r--r--   0     1001      123     2104 2023-06-20 17:50:17.000000 ultibi-0.3.4/pyproject.toml
--rw-r--r--   0     1001      123       36 2023-06-20 17:50:17.000000 ultibi-0.3.4/requirements-lint.txt
--rw-r--r--   0     1001      123      307 2023-06-20 17:50:17.000000 ultibi-0.3.4/requirements.txt
--rw-r--r--   0     1001      123     3842 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/calculator.rs
--rw-r--r--   0     1001      123       48 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/conversions/mod.rs
--rw-r--r--   0     1001      123     3542 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/conversions/series.rs
--rw-r--r--   0     1001      123     3049 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/conversions/wrappers.rs
--rw-r--r--   0     1001      123     7737 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/dataset.rs
--rw-r--r--   0     1001      123     3303 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/errors.rs
--rw-r--r--   0     1001      123      693 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/filter.rs
--rw-r--r--   0     1001      123     2021 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/lib.rs
--rw-r--r--   0     1001      123     2521 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/measure.rs
--rw-r--r--   0     1001      123     1353 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/requests.rs
--rw-r--r--   0     1001      123     1762 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/data/datasource_config.toml
--rw-r--r--   0     1001      123     4042 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/docs/run_doc_examples.py
--rw-r--r--   0     1001      123      591 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/unit/test_compute.py
--rw-r--r--   0     1001      123     1507 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/unit/test_ds.py
--rw-r--r--   0     1001      123     2658 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/unit/test_measure.py
--rw-r--r--   0     1001      123      848 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/__init__.py
--rw-r--r--   0     1001      123     1060 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/__init__.py
--rw-r--r--   0     1001      123     6733 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/dataset.py
--rw-r--r--   0     1001      123     3131 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/filters.py
--rw-r--r--   0     1001      123     5200 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/measure.py
--rw-r--r--   0     1001      123     2950 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/requests.py
--rw-r--r--   0     1001      123        0 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/rust_module/__init__.py
--rw-r--r--   0        0        0   100635 2023-06-20 17:54:29.000000 ultibi-0.3.4/Cargo.lock
--rw-r--r--   0        0        0     6488 1970-01-01 00:00:00.000000 ultibi-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/ultibi/Cargo.toml
+-rw-r--r--   0     1001      123        0 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi/README.md
+-rw-r--r--   0     1001      123       98 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi/src/lib.rs
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/frtb_engine/Cargo.toml
+-rw-r--r--   0     1001      123      481 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/README.md
+-rw-r--r--   0     1001      123    14931 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/Delta.csv
+-rw-r--r--   0     1001      123      541 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
+-rw-r--r--   0     1001      123     2160 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
+-rw-r--r--   0     1001      123      159 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/hms.csv
+-rw-r--r--   0     1001      123      177 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
+-rw-r--r--   0     1001      123    20066 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/calc_params.rs
+-rw-r--r--   0     1001      123       25 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/docs/mod.rs
+-rw-r--r--   0     1001      123     1226 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/docs/optional_params.rs
+-rw-r--r--   0     1001      123     1424 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/common.rs
+-rw-r--r--   0     1001      123    11847 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
+-rw-r--r--   0     1001      123     9484 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
+-rw-r--r--   0     1001      123     7614 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs
+-rw-r--r--   0     1001      123       96 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/mod.rs
+-rw-r--r--   0     1001      123      787 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/totals.rs
+-rw-r--r--   0     1001      123     4811 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/helpers.rs
+-rw-r--r--   0     1001      123    10170 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/lib.rs
+-rw-r--r--   0     1001      123     4151 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/measures.rs
+-rw-r--r--   0     1001      123      188 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/prelude.rs
+-rw-r--r--   0     1001      123       40 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/reports/mod.rs
+-rw-r--r--   0     1001      123      349 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/reports/sbm/equity.rs
+-rw-r--r--   0     1001      123       12 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/reports/sbm/mod.rs
+-rw-r--r--   0     1001      123    26569 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights.rs
+-rw-r--r--   0     1001      123     5421 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
+-rw-r--r--   0     1001      123     5268 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/rrao/mod.rs
+-rw-r--r--   0     1001      123     1374 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/buckets.rs
+-rw-r--r--   0     1001      123    14537 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
+-rw-r--r--   0     1001      123    13888 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
+-rw-r--r--   0     1001      123     3704 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
+-rw-r--r--   0     1001      123     7443 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
+-rw-r--r--   0     1001      123    30238 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common.rs
+-rw-r--r--   0     1001      123     9869 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs
+-rw-r--r--   0     1001      123    19328 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
+-rw-r--r--   0     1001      123    17723 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
+-rw-r--r--   0     1001      123     3846 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
+-rw-r--r--   0     1001      123    11817 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
+-rw-r--r--   0     1001      123    15622 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
+-rw-r--r--   0     1001      123    12479 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
+-rw-r--r--   0     1001      123     2904 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
+-rw-r--r--   0     1001      123     8796 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
+-rw-r--r--   0     1001      123    15266 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
+-rw-r--r--   0     1001      123    13490 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
+-rw-r--r--   0     1001      123     2988 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
+-rw-r--r--   0     1001      123     8074 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
+-rw-r--r--   0     1001      123    17062 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
+-rw-r--r--   0     1001      123    10966 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
+-rw-r--r--   0     1001      123    10440 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
+-rw-r--r--   0     1001      123    14299 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
+-rw-r--r--   0     1001      123    12036 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
+-rw-r--r--   0     1001      123    10230 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
+-rw-r--r--   0     1001      123    14040 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
+-rw-r--r--   0     1001      123    21914 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
+-rw-r--r--   0     1001      123     2295 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
+-rw-r--r--   0     1001      123    15734 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
+-rw-r--r--   0     1001      123      221 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/mod.rs
+-rw-r--r--   0     1001      123     5180 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/totals.rs
+-rw-r--r--   0     1001      123    28643 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/statics.rs
+-rw-r--r--   0     1001      123      753 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/totals.rs
+-rw-r--r--   0     1001      123     1846 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/src/validate.rs
+-rw-r--r--   0     1001      123     1832 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/common/mod.rs
+-rw-r--r--   0     1001      123     1520 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/dependant.rs
+-rw-r--r--   0     1001      123     4453 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/drc.rs
+-rw-r--r--   0     1001      123      420 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/rrao.rs
+-rw-r--r--   0     1001      123    18951 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm.rs
+-rw-r--r--   0     1001      123      710 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm_totals.rs
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/ultibi_server/Cargo.toml
+-rw-r--r--   0     1001      123      219 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/build.rs
+-rw-r--r--   0     1001      123       35 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/api/mod.rs
+-rw-r--r--   0     1001      123      754 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/api/open_api.rs
+-rw-r--r--   0     1001      123     6456 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/api/routers.rs
+-rw-r--r--   0     1001      123     1243 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/app.rs
+-rw-r--r--   0     1001      123     2593 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/helpers.rs
+-rw-r--r--   0     1001      123     1418 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/lib.rs
+-rw-r--r--   0     1001      123      358 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_server/src/visual.rs
+-rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 ultibi-0.4.0/local_dependencies/ultibi_core/Cargo.toml
+-rw-r--r--   0     1001      123     2031 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/add_row.rs
+-rw-r--r--   0     1001      123     3486 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/aggregations.rs
+-rw-r--r--   0     1001      123      654 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/cache.rs
+-rw-r--r--   0     1001      123     4782 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/datarequest.rs
+-rw-r--r--   0     1001      123     2903 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/datasource.rs
+-rw-r--r--   0     1001      123    10820 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/mod.rs
+-rw-r--r--   0     1001      123     2156 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/new.rs
+-rw-r--r--   0     1001      123      700 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/errors.rs
+-rw-r--r--   0     1001      123    10937 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs
+-rw-r--r--   0     1001      123     4628 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
+-rw-r--r--   0     1001      123      478 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/mod.rs
+-rw-r--r--   0     1001      123     2663 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/filters.rs
+-rw-r--r--   0     1001      123       18 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/helpers/mod.rs
+-rw-r--r--   0     1001      123      588 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/helpers/searches.rs
+-rw-r--r--   0     1001      123     1413 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/acquire.rs
+-rw-r--r--   0     1001      123     2059 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/awss3.rs
+-rw-r--r--   0     1001      123     6085 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/helpers.rs
+-rw-r--r--   0     1001      123     6863 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/io/mod.rs
+-rw-r--r--   0     1001      123      371 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/lib.rs
+-rw-r--r--   0     1001      123    11951 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/measure.rs
+-rw-r--r--   0     1001      123     3362 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/overrides.rs
+-rw-r--r--   0     1001      123      222 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/prelude.rs
+-rw-r--r--   0     1001      123       64 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/reports/mod.rs
+-rw-r--r--   0     1001      123     3332 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/src/reports/report.rs
+-rw-r--r--   0     1001      123     1870 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/add_row.rs
+-rw-r--r--   0     1001      123      734 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/agg_request.rs
+-rw-r--r--   0     1001      123     1441 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/aggregations.rs
+-rw-r--r--   0     1001      123        1 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/cache.rs
+-rw-r--r--   0     1001      123     2210 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/common/mod.rs
+-rw-r--r--   0     1001      123       95 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/bad_config.toml
+-rw-r--r--   0     1001      123      553 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml
+-rw-r--r--   0     1001      123      116 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/test_config.toml
+-rw-r--r--   0     1001      123      354 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/testset.csv
+-rw-r--r--   0     1001      123     1269 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/datasource.rs
+-rw-r--r--   0     1001      123     3094 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/dependants.rs
+-rw-r--r--   0     1001      123     1417 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/filters.rs
+-rw-r--r--   0     1001      123     1056 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/overrides.rs
+-rw-r--r--   0     1001      123     1144 2023-07-22 15:33:29.000000 ultibi-0.4.0/local_dependencies/ultibi_core/tests/source.rs
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123      728 2023-07-22 15:33:29.000000 ultibi-0.4.0/.gitignore
+-rw-r--r--   0     1001      123     5129 2023-07-22 15:33:29.000000 ultibi-0.4.0/LICENSE
+-rw-r--r--   0     1001      123     2405 2023-07-22 15:33:29.000000 ultibi-0.4.0/Makefile
+-rw-r--r--   0     1001      123     7071 2023-07-22 15:33:29.000000 ultibi-0.4.0/README.md
+-rw-r--r--   0     1001      123     1559 2023-07-22 15:33:29.000000 ultibi-0.4.0/example.py
+-rw-r--r--   0     1001      123     2098 2023-07-22 15:33:29.000000 ultibi-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123       36 2023-07-22 15:33:29.000000 ultibi-0.4.0/requirements-lint.txt
+-rw-r--r--   0     1001      123      307 2023-07-22 15:33:29.000000 ultibi-0.4.0/requirements.txt
+-rw-r--r--   0     1001      123     3922 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/calculator.rs
+-rw-r--r--   0     1001      123       48 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/conversions/mod.rs
+-rw-r--r--   0     1001      123     3570 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/conversions/series.rs
+-rw-r--r--   0     1001      123     3049 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/conversions/wrappers.rs
+-rw-r--r--   0     1001      123     9008 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/dataset.rs
+-rw-r--r--   0     1001      123     1786 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/datasource.rs
+-rw-r--r--   0     1001      123     3833 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/errors.rs
+-rw-r--r--   0     1001      123      693 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/filter.rs
+-rw-r--r--   0     1001      123     2170 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123     2521 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/measure.rs
+-rw-r--r--   0     1001      123     1353 2023-07-22 15:33:29.000000 ultibi-0.4.0/src/requests.rs
+-rw-r--r--   0     1001      123     1762 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/data/datasource_config.toml
+-rw-r--r--   0     1001      123     4042 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/docs/run_doc_examples.py
+-rw-r--r--   0     1001      123     1613 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_compute.py
+-rw-r--r--   0     1001      123     1692 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_ds.py
+-rw-r--r--   0     1001      123      826 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_filters.py
+-rw-r--r--   0     1001      123     2658 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_measure.py
+-rw-r--r--   0     1001      123      878 2023-07-22 15:33:29.000000 ultibi-0.4.0/tests/unit/test_source.py
+-rw-r--r--   0     1001      123      918 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/__init__.py
+-rw-r--r--   0     1001      123     1145 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/__init__.py
+-rw-r--r--   0     1001      123     7999 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/dataset.py
+-rw-r--r--   0     1001      123     2749 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/datasource.py
+-rw-r--r--   0     1001      123     3257 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/filters.py
+-rw-r--r--   0     1001      123     8407 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/measure.py
+-rw-r--r--   0     1001      123     2950 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/internals/requests.py
+-rw-r--r--   0     1001      123        0 2023-07-22 15:33:29.000000 ultibi-0.4.0/ultibi/rust_module/__init__.py
+-rw-r--r--   0        0        0   121894 2023-07-22 15:35:01.000000 ultibi-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     7979 1970-01-01 00:00:00.000000 ultibi-0.4.0/PKG-INFO
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/Cargo.toml` & `ultibi-0.4.0/local_dependencies/frtb_engine/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 [package]
 name = "frtb_engine"
-version= "0.3.4"
+version= "0.4.0"
 edition = "2021"
 publish = false
 license-file= "LICENSE"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 ultibi = {path = "../ultibi" }
-polars = { version = "0.28.0", features = [
+polars = { version = "0.31.1", features = [
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
-    "csv-file",
     "diagonal_concat",
     "serde-lazy" 
 ,"strings", "ndarray", "lazy", "is_in", "dtype-categorical", "performant", "partition_by", "concat_str"] }
 serde = { version = "1.0", features = ["derive","derive"] }
 serde_json = "1.0"
 once_cell = "1.12"
 ndarray = {version = "0.15.6", features = ["matrixmultiply-threading", "rayon", "serde"] }
 rayon = "1.5.3"
 strum = {version="0.24", features = ["derive"] }
 log = "0.4"
 yearfrac = "0.1.4"
 smartstring = "*"
 
-[dev-dependencies]
-
 [features]
 CRR2 = []
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/Delta.csv` & `ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/Delta.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv` & `ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/datasource_config.toml` & `ultibi-0.4.0/local_dependencies/frtb_engine/data/frtb/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/calc_params.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/calc_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/docs/optional_params.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/docs/optional_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/common.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             // Do you want to aggregate as per  22.19?
             // Note, the algorithm is O(N), but we loose Negative GrossJTD position changes,
             // (and might end up with a different Credit Quality, but same obligor)
             // This shouldn't be a problem since we sum positions (netShort netLong) anyway,
             // And THEN apply CreditQuality weights, BECAUSE Obligor - CreditQuality should be 1to1 map
             if offset {
                 lf = lf
-                    .sort_by_exprs(&[col("rft")], [false], false)
+                    .sort_by_exprs(&[col("rft")], [false], false, true)
                     .groupby(["b", "rf"])
                     .apply(
                         |mut df| {
                             let mut neg = 0.;
                             let mut neg_flag = false; //flags if we have any negative values
                             let mut res: Vec<f64> = Vec::with_capacity(df["scaled_jtd"].len());
                             df["scaled_jtd"].f64()?.into_no_null_iter().for_each(|x| {
@@ -218,15 +218,15 @@
         },
         &[
             col("RiskClass"),
             col("BucketBCBS"),
             col("RiskFactor"),
             col("SeniorityRank"),
             col("GrossJTD"),
-            weights.arr().get(lit(0)),
+            weights.list().get(lit(0)),
             col("ScaleFactor"),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         &[
             col("RiskClass"),
             col("BucketBCBS"),
             col("RiskFactor"),
             col("RiskFactorType"), //Seniority
             col("Tranche"),
             col("GrossJTD"),
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
             col("ScaleFactor"),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_weights.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/drc_weights.rs`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         "Key" => key,
         "RiskWeightDRC" => weight,
         "RiskClass" => vec!["DRC_Sec_nonCTP"; len],
         "RiskCategory" => vec!["DRC"; len],
     ]
     .unwrap() // We must not fail on default frame
     .lazy()
-    .with_column(concat_lst([col("RiskWeightDRC")]).unwrap())
+    .with_column(concat_list([col("RiskWeightDRC")]).unwrap())
     .collect()
     .unwrap() // we should never fail on default frame
 }
 
 ///CreditQuality_Seniority - Weight
 pub(crate) fn drc_secnonctp_weights_frame() -> DataFrame {
     let (key, weight): (Vec<String>, Vec<f64>) = drc_secnonctp_weights_raw()
@@ -231,9 +231,9 @@
         "RiskClass" => vec!["DRC_nonSec"; 6],
         "RiskCategory" => vec!["DRC"; 6],
     ]
     .unwrap() // We must not fail on default frame
     .lazy();
 
     let join_on = [col("RiskClass"), col("RiskCategory"), col("RiskFactorType")];
-    lf.join(drc_sen, join_on.clone(), join_on, JoinType::Left)
+    lf.join(drc_sen, join_on.clone(), join_on, JoinType::Left.into())
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/drc/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/helpers.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/lib.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/lib.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 //! FRTB job entry point
 #![allow(clippy::unnecessary_lazy_evaluations)]
 #![doc(html_no_source)]
 
 mod drc;
+mod reports;
 mod rrao;
 mod sbm;
 mod totals;
 
 pub mod calc_params;
 pub mod docs;
 mod helpers;
@@ -14,206 +15,214 @@
 pub mod prelude;
 mod risk_weights;
 #[cfg(feature = "CRR2")]
 mod risk_weights_crr2;
 pub mod statics;
 mod validate;
 
-use ultibi::cache::{Cache, CacheableDataSet};
-use ultibi::{CalcParameter, DataSet, Measure, MeasuresMap, ValidateSet, CPM};
-//use crate::drc::drc_weights;
 use prelude::calc_params::FRTB_CALC_PARAMS;
+use ultibi::cache::{Cache, CacheableDataSet};
+use ultibi::datasource::DataSource;
+use ultibi::errors::{UltiResult, UltimaErr};
+use ultibi::new::NewSourcedDataSet;
 use ultibi::polars::prelude::{
     col, lit, when, AnyValue, Expr, LazyFrame, Literal, LiteralValue, NamedFrom, PolarsResult,
     Series, NULL,
 };
+use ultibi::reports::report::ReportersMap;
+use ultibi::{overridable_columns, CalcParameter, DataSet, Measure, MeasuresMap, CPM};
 //use polars:: series::Series, lazy::dsl::when};
 use prelude::{drc::common::drc_scalinng, frtb_measure_vec};
 use risk_weights::*;
 use sbm::buckets;
 
 use std::collections::{BTreeMap, HashSet};
 
 pub struct FRTBDataSet {
-    pub frame: LazyFrame,
+    pub source: DataSource,
     pub measures: MeasuresMap,
-    pub build_params: BTreeMap<String, String>,
+    pub config: BTreeMap<String, String>,
     pub cache: Cache,
 }
 impl FRTBDataSet {
     /// Helper function which appends bespoke measures to self.measures
     fn with_measures(&mut self, bespoke: Vec<Measure>)
     where
         Self: Sized,
     {
         let self_measures = &mut self.measures;
         self_measures.extend(bespoke.into_iter().map(|m| (m.name().clone(), m)));
     }
 }
 
+impl NewSourcedDataSet for FRTBDataSet {
+    /// Here we add FRTB measures
+    /// We do it here, since [new] will be called one only
+    fn new(source: DataSource, mm: MeasuresMap, _: ReportersMap, config: CPM) -> Self {
+        let mut res = Self {
+            source,
+            measures: mm,
+            config,
+            cache: Cache::default(),
+        };
+        res.with_measures(frtb_measure_vec());
+        res
+    }
+}
+
 impl DataSet for FRTBDataSet {
+    /// FRTBDataSet has a cache
     fn as_cacheable(&self) -> Option<&dyn CacheableDataSet> {
         Some(self)
     }
 
-    fn get_lazyframe(&self) -> &LazyFrame {
-        &self.frame
+    fn get_datasource(&self) -> &DataSource {
+        &self.source
     }
-    /// Modify lf in place
-    fn set_lazyframe_inplace(&mut self, lf: LazyFrame) {
-        self.frame = lf;
+    /// Modify lf in place - applicable only to InMemory DataSource
+    fn set_lazyframe_inplace(&mut self, lf: LazyFrame) -> UltiResult<()> {
+        if let DataSource::InMemory(_) = self.source {
+            self.source = DataSource::InMemory(lf.collect()?)
+        } else {
+            return Err(UltimaErr::Other("Can't set data inplace with this Source. Currently can only set In Memory Dataframe".to_string()));
+        }
+        Ok(())
     }
     fn get_measures(&self) -> &MeasuresMap {
         &self.measures
     }
+    /// TODO - this should be done once only
     fn calc_params(&self) -> Vec<CalcParameter> {
         let mut res = vec![];
 
         for measure in self.get_measures().values() {
             res.extend_from_slice(measure.calc_params())
         }
 
         res.extend_from_slice(FRTB_CALC_PARAMS.as_ref());
 
         let hash_res: HashSet<CalcParameter> = res.into_iter().collect();
 
         hash_res.into_iter().collect()
     }
 
-    fn new(frame: LazyFrame, mm: MeasuresMap, build_params: CPM) -> Self {
-        let mut res = Self {
-            frame,
-            measures: mm,
-            build_params,
-            cache: Cache::default(),
-        };
-        res.with_measures(frtb_measure_vec());
-        res
-    }
-
     /// Adds: BCBS buckets, CRR2 Buckets
     /// Adds: SensWeights, CurvatureRiskWeight, SensWeightsCRR2, SeniorityRank
-    fn prepare_frame(&self, _lf: Option<LazyFrame>) -> PolarsResult<LazyFrame> {
-        let mut lf1 = if let Some(lf) = _lf {
-            lf
-        } else {
-            self.get_lazyframe().clone()
-        };
-
+    fn prepare_frame(&self, lf: LazyFrame) -> UltiResult<LazyFrame> {
         //First, where possible (FX and GIRR) - assign buckets
         //this really is an optional step
-        lf1 = lf1.with_column(buckets::sbm_buckets(&self.build_params).alias("BucketBCBS"));
+        let mut lf1 = lf.with_column(buckets::sbm_buckets(&self.config).alias("BucketBCBS"));
         //dbg!(lf1.clone().filter(col("RiskClass").eq(lit("FX"))).select([col("BucketBCBS")]).collect());
 
         // Then assign SensWeights(BCBS) based on buckets
-        lf1 = weights_assign(lf1, &self.build_params)?;
+        lf1 = weights_assign(lf1, &self.config)?;
 
         // TODO Remove after this issue
         // workaround for https://github.com/pola-rs/polars/issues/5812
         let a = Expr::Literal(
             LiteralValue::try_from(AnyValue::List(Series::new("NewVal", [0.]))).unwrap(),
         );
         lf1 = lf1.with_column(
             when(col("SensWeights").is_null())
-                .then(a.list())
+                .then(a.implode())
                 .otherwise(col("SensWeights"))
                 .alias("SensWeights"),
         );
         //dbg!(lf1.clone().filter(col("RiskClass").eq(lit("FX"))).select([col("BucketBCBS"), col("SensWeights")]).collect());
 
         // Curvature risk weight
         //lf1 = tmp_frame.lazy()
         lf1 = lf1.with_column(
             when(
                 col("PnL_Up")
                     .is_not_null()
                     .or(col("PnL_Down").is_not_null()),
             )
-            .then(col("SensWeights").arr().max().alias("CurvatureRiskWeight"))
+            .then(col("SensWeights").list().max().alias("CurvatureRiskWeight"))
             .otherwise(NULL.lit()),
         );
         //dbg!(lf1.clone().filter(col("RiskClass").eq(lit("FX"))).select([col("BucketBCBS"), col("SensWeights"), col("CurvatureRiskWeight")]).collect());
 
         // Now,  ammend weights if required. ie has to be done after main assignment of risk weights
         let mut other_cols: Vec<Expr> = vec![];
         // 21.53 Footnote 17
         let csrnonsec_covered_bond_15 = self
-            .build_params
+            .config
             .get("csrnonsec_covered_bond_15")
             .and_then(|s| s.parse::<bool>().ok())
             .unwrap_or_else(|| false);
 
         if csrnonsec_covered_bond_15 {
             other_cols.push(
                 when(
                     col("RiskClass")
                         .eq(lit("CSR_nonSec"))
                         .and(col("RiskCategory").eq(lit("Delta")))
                         .and(col("BucketBCBS").eq(lit("8")))
                         .and(col("CoveredBondReducedWeight").eq(lit::<bool>(true))),
                 )
-                .then(Series::new("", &[0.015]).lit().list())
+                .then(Series::new("", &[0.015]).lit().implode())
                 .otherwise(col("SensWeights"))
                 .alias("SensWeights"),
             )
         };
 
         if !other_cols.is_empty() {
             lf1 = lf1.with_columns(&other_cols)
         };
 
         // If CRR2 config, we need to derive SensWeightsCRR2
         #[cfg(feature = "CRR2")]
         if cfg!(feature = "CRR2") {
             lf1 = lf1.with_column(buckets::sbm_buckets_crr2());
             //other_cols.push(weights_assign_crr2().alias("SensWeightsCRR2"))
-            lf1 = crate::risk_weights_crr2::weights_assign_crr2(lf1, &self.build_params)?;
+            lf1 = crate::risk_weights_crr2::weights_assign_crr2(lf1, &self.config)?;
 
             // Now, we need to also ammend CRR2 weights
             // Bucket 10 as per
             // https://www.eba.europa.eu/regulation-and-policy/single-rulebook/interactive-single-rulebook/108776
             let mut with_cols = vec![when(
                 col("PnL_Up")
                     .is_not_null()
                     .or(col("PnL_Down").is_not_null()),
             )
             .then(
                 col("SensWeightsCRR2")
-                    .arr()
+                    .list()
                     .max()
                     .alias("CurvatureRiskWeightCRR2"),
             )
             .otherwise(NULL.lit())];
 
             if csrnonsec_covered_bond_15 {
                 with_cols.push(
                     when(
                         col("RiskClass")
                             .eq(lit("CSR_nonSec"))
                             .and(col("RiskCategory").eq(lit("Delta")))
                             .and(col("BucketCRR2").eq(lit("10")))
                             .and(col("CoveredBondReducedWeight").eq(lit::<bool>(true))),
                     )
-                    .then(Series::new("", &[0.015]).lit().list())
+                    .then(Series::new("", &[0.015]).lit().implode())
                     .otherwise(col("SensWeightsCRR2"))
                     .alias("SensWeightsCRR2"),
                 )
             }
 
             lf1 = lf1.with_columns(with_cols)
         }
 
         // Have to collect into a tmp df, as the code panics otherwise
         //let tmp_frame = lf1
         //    .collect()
         //    .expect("Failed to unwrap tmp_frame while .prepare()");
         //lf1 = tmp_frame.lazy()
         lf1 = lf1.with_columns(&[drc_scalinng(
-            self.build_params.get("DayCountConvention"),
-            self.build_params.get("DateFormat"),
+            self.config.get("DayCountConvention"),
+            self.config.get("DateFormat"),
         )
         .alias("ScaleFactor")]);
 
         // DRC Seniority
         lf1 = drc::drc_weights::with_drc_seniority(lf1);
         //let tmp2_frame = lf1
         //    .collect()
@@ -235,27 +244,51 @@
     // Equity bucket can be strictly an int in 1..13 inclusive (and non empty)
     // Equity Risk Factor Type has to be one of: EqSpot, EqRepo (and non empty) for Delta
     //
     // CSR_nonSec BCBS buckets
     // CSR_nonSec CRR2 buckets
     // if csrnonsec_covered_bond_15 == true in build config then
     // If DRC validate CreditQuality
-    fn validate_frame(&self, lf: Option<&LazyFrame>, v: ValidateSet) -> PolarsResult<()> {
+    fn validate_frame(&self, lf: Option<&LazyFrame>, set: u8) -> UltiResult<()> {
         let csrnonsec_covered_bond_15 = self
-            .build_params
+            .config
             .get("csrnonsec_covered_bond_15")
             .and_then(|s| s.parse::<bool>().ok())
             .unwrap_or_else(|| false);
 
         if let Some(lf) = lf {
-            validate::validate_frame(lf, csrnonsec_covered_bond_15, v)
+            validate::validate_frtb_frame(lf, csrnonsec_covered_bond_15, set)
         } else {
-            validate::validate_frame(self.get_lazyframe(), csrnonsec_covered_bond_15, v)
+            validate::validate_frtb_frame(
+                &self.get_lazyframe(&vec![]),
+                csrnonsec_covered_bond_15,
+                set,
+            )
         }
     }
+
+    /// We manually add "prepared" columns here
+    /// Good usecase: add prepared
+    fn overridable_columns(&self) -> Vec<String> {
+        let mut standard_cols = self
+            .get_schema()
+            .map(overridable_columns)
+            .unwrap_or_default();
+
+        // TODO add CRR2
+        standard_cols.extend([
+            "SensWeights".to_string(),
+            "ScaleFactor".to_string(),
+            "CurvatureRiskWeight".to_string(),
+        ]);
+
+        let hash_res: HashSet<String> = standard_cols.into_iter().collect();
+
+        hash_res.into_iter().collect()
+    }
 }
 
 impl CacheableDataSet for FRTBDataSet {
     fn get_cache(&self) -> &Cache {
         &self.cache
     }
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/measures.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/measures.rs`

 * *Files 4% similar despite different names*

```diff
@@ -46,23 +46,35 @@
 
 use crate::drc::totals::drc_total_measures;
 
 use crate::rrao::rrao_measures;
 
 use crate::totals::sa_total_measures;
 
+use crate::prelude::total_delta_sens;
+use ultibi::CPM;
+
 /// Exporting Measures
 pub(crate) fn frtb_measure_vec() -> Vec<Measure> {
-    let non_rc_specific = vec![Measure::Base(BaseMeasure {
-        name: "RiskWeights".to_string(),
-        calculator: std::sync::Arc::new(sens_weights),
-        aggregation: Some("first".into()),
-        precomputefilter: None,
-        calc_params: vec![],
-    })];
+    let non_rc_specific = vec![
+        Measure::Base(BaseMeasure {
+            name: "RiskWeights".to_string(),
+            calculator: std::sync::Arc::new(sens_weights),
+            aggregation: Some("first".into()),
+            precomputefilter: None,
+            calc_params: vec![],
+        }),
+        Measure::Base(BaseMeasure {
+            name: "Total DeltaSens".to_string(),
+            calculator: std::sync::Arc::new(|_: &CPM| Ok(total_delta_sens())),
+            aggregation: None,
+            precomputefilter: None,
+            calc_params: vec![],
+        }),
+    ];
 
     let mut res = vec![];
     res.extend(fx_delta_measures());
     res.extend(fx_vega_measures());
     res.extend(fx_curv_measures());
     res.extend(fx_total_measures());
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 //! This module includes complete weights allocation logic (pre build mode). SBM and DRC weights and Scale Factors
 //! It follows the logic prescribed by the text https://www.bis.org/bcbs/publ/d457.pdf
 //! TODO Weights column is a list. We can't read it as list from a csv. frame_from_path_or_str must concat_lst columns which have Sens in the name
 
 use crate::drc::drc_weights;
 use once_cell::sync::OnceCell;
 use std::collections::BTreeMap;
+use ultibi::polars::prelude::diag_concat_lf;
 use ultibi::polars::prelude::{
-    col, concat_lst, concat_str, df, lit, CsvReader, DataFrame, DataType, Expr, GetOutput,
+    col, concat_list, concat_str, df, lit, CsvReader, DataFrame, DataType, Expr, GetOutput,
     IntoLazy, IntoSeries, JoinType, LazyFrame, NamedFrom, PolarsError, PolarsResult, SerReader,
     Series, Utf8NameSpaceImpl,
 };
-use ultibi::prelude::helpers::diag_concat_lf;
 
 static FX_SPECIAL_DELTA_FULL_RW: OnceCell<LazyFrame> = OnceCell::new();
 static FX_SPECIAL_DELTA_PARTIAL_RW: OnceCell<LazyFrame> = OnceCell::new();
 static FX_BASE_DELRA_RW: OnceCell<LazyFrame> = OnceCell::new();
 
 /// 21.44 specified currencies
 pub static REDUCED_IR_WEIGHT: &str = "EUR|USD|GBP|AUD|JPY|SEK|CAD";
@@ -534,33 +534,33 @@
         col("RiskFactorType"),
         col("BucketBCBS"),
     ];
     let mut lf1 = lf.join(
         weights.rc_rcat_rtype_b_weights,
         join_on.clone(),
         join_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     // tmp workaround, since .rename() panics
     // TODO remove
     // Adding here to check if weights were assigned, if not - create a dummy column
     if !lf1.schema()?.iter_names().any(|col| col == "Weights") {
-        lf1 = lf1.with_column(lit(0.).list().alias("SensWeights"))
+        lf1 = lf1.with_column(lit(0.).implode().alias("SensWeights"))
     } else {
         lf1 = lf1.rename(["Weights"], ["SensWeights"])
     }
 
     //dbg!(lf1.clone().filter(col("RiskClass").eq(lit("FX"))).select([col("BucketBCBS"), col("RiskFactor"), col("SensWeights")]).collect());
 
     let join_on = [col("RiskClass"), col("RiskCategory"), col("BucketBCBS")];
     lf1 = lf1.join(
         weights.rc_rcat_b_weights,
         join_on.clone(),
         join_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights"])]);
 
     // FX SECOND HERE
     lf1 = lf1.with_column(
@@ -572,37 +572,37 @@
             .alias("Bucket"),
     );
     let right_on = [col("RiskClass"), col("RiskCategory"), col("Bucket")];
     lf1 = lf1.join(
         weights.rc_rcat_b_weights_second,
         right_on.clone(),
         right_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights", "Bucket"])]);
 
     let join_on = [col("RiskClass"), col("RiskCategory"), col("RiskFactorType")];
     lf1 = lf1.join(
         weights.rc_rcat_rtype_weights,
         join_on.clone(),
         join_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights"])]);
 
     let join_on = [col("RiskClass"), col("RiskCategory")];
     let mut lf1 = lf1.join(
         weights.rc_rcat_weights,
         join_on.clone(),
         join_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights"])]);
 
     let join_on = [
         col("RiskClass"),
@@ -612,15 +612,15 @@
             GetOutput::from_type(DataType::Utf8),
         ),
     ];
     let mut lf1 = lf1.join(
         weights.drc_nonsec_weights_frame,
         join_on.clone(),
         join_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1
         .with_column(col("SensWeights").fill_null(col("Weights")))
         .select([col("*").exclude(["Weights"])]);
 
     //drc_secnonctp_weights
     lf1 = lf1.with_column(
@@ -642,15 +642,15 @@
 
     let left_on = [col("RiskClass"), col("RiskCategory"), col("Key")];
     let right_on = [col("RiskClass"), col("RiskCategory"), col("Key")];
     let mut lf1 = lf1.join(
         weights.drc_secnonctp_weights,
         left_on,
         right_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1
         .with_column(col("SensWeights").fill_null(col("RiskWeightDRC")))
         .select([col("*").exclude(["RiskWeightDRC", "Key"])]);
 
     Ok(lf1)
 }
@@ -746,15 +746,15 @@
         "Weights" => vec![xccy_weights, infl_weights, yield_weights],
         "RiskFactorType" => ["XCCY", "Inflation", "Yield"],
         "RiskClass" => vec!["GIRR"; 3],
         "RiskCategory" => vec!["Delta"; 3],
     ]
     .unwrap() // We must not fail on default frame
     .lazy()
-    .with_column(concat_lst([col("Weights")]).unwrap()) // don't expect to fail on default
+    .with_column(concat_list([col("Weights")]).unwrap()) // don't expect to fail on default
     .collect()
     .expect("failed on IR Delta weights") // We must not fail on default frame
 }
 
 /// Checks if `some_str` is a path
 /// If not tries to serialise it
 /// Checks for expected columns
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights_crr2.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/risk_weights_crr2.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 //! This module is for CRR2 specific Risk weights
 //! https://www.eba.europa.eu/regulation-and-policy/single-rulebook/interactive-single-rulebook/108255 325ae onward
 use std::collections::BTreeMap;
 
 use once_cell::sync::OnceCell;
+use ultibi::polars::prelude::diag_concat_lf;
 use ultibi::polars::prelude::{
     col, DataType, GetOutput, IntoLazy, IntoSeries, JoinType, LazyFrame, NamedFrom, PolarsResult,
     Series, Utf8NameSpaceImpl,
 };
-use ultibi::prelude::helpers::diag_concat_lf;
 
 use crate::{
     drc::drc_weights,
     prelude::{frame_from_path_or_str, rcat_rc_b_weights_frame},
 };
 
 static CSR_NONSEC_RW_CRR2: OnceCell<LazyFrame> = OnceCell::new();
@@ -130,15 +130,15 @@
 ) -> PolarsResult<LazyFrame> {
     // First, left join one by one
     let join_on = [col("RiskClass"), col("RiskCategory"), col("BucketCRR2")];
     let mut lf1 = lf.join(
         weights.rc_rcat_b_weights_crr2,
         join_on.clone(),
         join_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1.rename(["WeightsCRR2"], ["SensWeightsCRR2"]);
 
     let join_on = [
         col("RiskClass"),
         col("RiskCategory"),
         col("CreditQuality").map(
@@ -146,15 +146,15 @@
             GetOutput::from_type(DataType::Utf8),
         ),
     ];
     let mut lf1 = lf1.join(
         weights.drc_nonsec_weights_frame_crr2,
         join_on.clone(),
         join_on,
-        JoinType::Left,
+        JoinType::Left.into(),
     );
     lf1 = lf1
         .with_column(col("SensWeightsCRR2").fill_null(col("WeightsCRR2")))
         .select([col("*").exclude(["WeightsCRR2"])]);
 
     // Finally, fill with default weights of BCBS
     lf1 = lf1.with_column(col("SensWeightsCRR2").fill_null(col("SensWeights")));
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/rrao/mod.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/rrao/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/buckets.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/buckets.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
-use crate::{prelude::*, sbm::equity::curvature::eq_curvature_charge};
-use polars::prelude::*;
-use ultibi::{prelude::CPM, BaseMeasure};
+use crate::{
+    prelude::{
+        get_optional_parameter, get_optional_parameter_array, ReturnMetric, ScenarioConfig,
+        HIGH_CORR_SCENARIO, LOW_CORR_SCENARIO, MEDIUM_CORR_SCENARIO,
+    },
+    sbm::{
+        common::rc_rcat_sens,
+        common_curv::{curv_delta_total, rc_cvr, Cvr},
+        equity::curvature::eq_curvature_charge,
+    },
+};
+use ultibi::lit;
+use ultibi::polars::lazy::dsl::{col, max_horizontal, Expr};
+use ultibi::{prelude::CPM, BaseMeasure, Measure, PolarsResult};
 
 pub fn com_curv_delta(_: &CPM) -> PolarsResult<Expr> {
     Ok(curv_delta_total("Commodity"))
 }
 /// Helper functions
 pub fn com_curv_delta_weighted(op: &CPM) -> PolarsResult<Expr> {
     com_curv_delta(op).map(|expr| expr * col("CurvatureRiskWeight"))
@@ -100,15 +111,15 @@
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn com_curv_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         com_curvature_charge_low(op)?,
         com_curvature_charge_medium(op)?,
         com_curvature_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 //! Commodity Delta Risk Charge
 //! TODO Commodity RiskFactor should be of the form ...CCY (same as FX, where CCY is the reporting CCY)
 
 use crate::prelude::*;
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput, MeltArgs},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput, MeltArgs},
     BaseMeasure, DataFrame, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
 pub fn total_commodity_delta_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Delta", "Commodity", total_delta_sens()))
 }
 
 /// Total Commodity Delta
 pub(crate) fn commodity_delta_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    total_commodity_delta_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
+    total_commodity_delta_sens(op).map(|expr| expr * col("SensWeights").list().get(lit(0)))
 }
 
 /// Interm Result: Commodity Delta Sb <--> Sb Low == Sb Medium == Sb High
 pub(crate) fn commodity_delta_sb(op: &CPM) -> PolarsResult<Expr> {
     commodity_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
 }
 /// Interm Result: Commodity Kb Low
@@ -176,25 +176,25 @@
                 .filter(
                     col("rc")
                         .eq(lit("Commodity"))
                         .and(col("rcat").eq(lit("Delta"))),
                 )
                 .groupby(grp_by)
                 .agg([
-                    (col("y0") * col("w").arr().get(lit(0))).sum(),
-                    (col("y025") * col("w").arr().get(lit(1))).sum(),
-                    (col("y05") * col("w").arr().get(lit(2))).sum(),
-                    (col("y1") * col("w").arr().get(lit(3))).sum(),
-                    (col("y2") * col("w").arr().get(lit(4))).sum(),
-                    (col("y3") * col("w").arr().get(lit(5))).sum(),
-                    (col("y5") * col("w").arr().get(lit(6))).sum(),
-                    (col("y10") * col("w").arr().get(lit(7))).sum(),
-                    (col("y15") * col("w").arr().get(lit(8))).sum(),
-                    (col("y20") * col("w").arr().get(lit(9))).sum(),
-                    (col("y30") * col("w").arr().get(lit(10))).sum(),
+                    (col("y0") * col("w").list().get(lit(0))).sum(),
+                    (col("y025") * col("w").list().get(lit(1))).sum(),
+                    (col("y05") * col("w").list().get(lit(2))).sum(),
+                    (col("y1") * col("w").list().get(lit(3))).sum(),
+                    (col("y2") * col("w").list().get(lit(4))).sum(),
+                    (col("y3") * col("w").list().get(lit(5))).sum(),
+                    (col("y5") * col("w").list().get(lit(6))).sum(),
+                    (col("y10") * col("w").list().get(lit(7))).sum(),
+                    (col("y15") * col("w").list().get(lit(8))).sum(),
+                    (col("y20") * col("w").list().get(lit(9))).sum(),
+                    (col("y30") * col("w").list().get(lit(10))).sum(),
                 ])
                 // No need to fill null here
                 .collect()?;
 
             let mut ma = MeltArgs {
                 streamable: false,
                 id_vars: vec!["b".into(), "rf".into(), "loc".into()],
@@ -254,15 +254,15 @@
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn com_delta_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         commodity_delta_charge_low(op)?,
         commodity_delta_charge_medium(op)?,
         commodity_delta_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pub(crate) fn com_total_high(_: &CPM) -> PolarsResult<Expr> {
     Ok(col("Commodity DeltaCharge High")
         + col("Commodity VegaCharge High")
         + col("Commodity CurvatureCharge High"))
 }
 /// Not a real measure. Used for analysis only
 fn com_total_max(_: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         col("Commodity TotalCharge Low"),
         col("Commodity TotalCharge Medium"),
         col("Commodity TotalCharge High"),
     ]))
 }
 
 pub(crate) fn com_total_measures() -> Vec<Measure> {
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use crate::{prelude::*, sbm::equity::vega::equity_vega_charge};
-use ultibi::{polars::prelude::max_exprs, BaseMeasure, CPM};
+use ultibi::{polars::prelude::max_horizontal, BaseMeasure, CPM};
 
 pub fn total_com_vega_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Vega", "Commodity", total_vega_curv_sens()))
 }
 
 pub fn total_com_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    total_com_vega_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
+    total_com_vega_sens(op).map(|expr| expr * col("SensWeights").list().get(lit(0)))
 }
 ///Interm Result
 pub(crate) fn com_vega_sb(op: &CPM) -> PolarsResult<Expr> {
     com_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Sb)
 }
 pub(crate) fn com_vega_kb_low(op: &CPM) -> PolarsResult<Expr> {
     com_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
@@ -77,15 +77,15 @@
 }
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn com_vega_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         com_vega_charge_low(op)?,
         com_vega_charge_medium(op)?,
         com_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 //#![allow(clippy::unnecessary_lazy_evaluations)]
 
+use ultibi::polars::prelude::IndexOrder;
 use ultibi::prelude::*;
 
 use ndarray::{s, Array1, Array2, ArrayView1, Axis, Zip};
 use ultibi::polars::export::num::Signed;
 use ultibi::polars::prelude::{
     apply_multiple, AnyValue, ChunkAgg, ChunkCompare, ChunkSet, DataType, FillNullStrategy,
     Float64Type, GetOutput, IntoSeries, NamedFrom, NumOpsDispatch, PolarsError, Series, TakeRandom,
@@ -103,15 +104,15 @@
 
             let x = delta.multiply(&columns[2])?;
             Ok(Some(x))
         },
         &[
             col("RiskClass"),
             col(delta_tenor),
-            col(weights_col).arr().get(lit(weight_idx)),
+            col(weights_col).list().get(lit(weight_idx)),
             col("RiskCategory"),
         ],
         GetOutput::from_type(DataType::Float64),
         false,
     )
 }
 
@@ -212,55 +213,57 @@
     let mut reskbs_sbs: Vec<PolarsResult<(f64, f64)>> = Vec::with_capacity(n_buckets);
     for _ in 0..n_buckets {
         reskbs_sbs.push(Ok((0., 0.)))
     }
 
     let arc_mtx = std::sync::Arc::new(Mutex::new(reskbs_sbs));
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
-    df.partition_by(["b"])?.par_iter().for_each(|bucket_df| {
-        // Safety: since partition, we must have at least one member
-        let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
-        // validating also bucket is not greater than max index of bucket_rho_diff_rf
-        let b_as_idx_plus_1 = match b_as_idx_plus_1 {
-            AnyValue::Utf8(st) => st.parse::<usize>().ok().and_then(|b_id| {
-                if (1..=n_buckets).contains(&b_id) {
-                    Some(b_id)
-                } else {
-                    None
-                }
-            }),
-
-            _ => None,
-        };
+    df.partition_by(["b"], true)?
+        .par_iter()
+        .for_each(|bucket_df| {
+            // Safety: since partition, we must have at least one member
+            let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
+            // validating also bucket is not greater than max index of bucket_rho_diff_rf
+            let b_as_idx_plus_1 = match b_as_idx_plus_1 {
+                AnyValue::Utf8(st) => st.parse::<usize>().ok().and_then(|b_id| {
+                    if (1..=n_buckets).contains(&b_id) {
+                        Some(b_id)
+                    } else {
+                        None
+                    }
+                }),
 
-        // CALCULATE Kb Sb for a bucket
-        if let Some(b_as_idx_plus_1) = b_as_idx_plus_1 {
-            // Above we check len of bucket_rho_diff_rf via n_buckets, so we won't panic here
-            let name_rho = bucket_rho_diff_rf[b_as_idx_plus_1 - 1];
+                _ => None,
+            };
 
             // CALCULATE Kb Sb for a bucket
-            let is_special_bucket = Some(b_as_idx_plus_1) == special_bucket;
-            let a = bucket_kb_sb_onsq(
-                bucket_df,
-                tenor_col,
-                rho_diff_tenor,
-                name_col,
-                name_rho,
-                basis_col,
-                rho_diff_rft,
-                risk_col,
-                scenario_fn,
-                is_special_bucket,
-                rho_overwrite,
-            );
+            if let Some(b_as_idx_plus_1) = b_as_idx_plus_1 {
+                // Above we check len of bucket_rho_diff_rf via n_buckets, so we won't panic here
+                let name_rho = bucket_rho_diff_rf[b_as_idx_plus_1 - 1];
 
-            let mut res = arc_mtx.lock().unwrap();
-            res[b_as_idx_plus_1 - 1] = a;
-        }
-    });
+                // CALCULATE Kb Sb for a bucket
+                let is_special_bucket = Some(b_as_idx_plus_1) == special_bucket;
+                let a = bucket_kb_sb_onsq(
+                    bucket_df,
+                    tenor_col,
+                    rho_diff_tenor,
+                    name_col,
+                    name_rho,
+                    basis_col,
+                    rho_diff_rft,
+                    risk_col,
+                    scenario_fn,
+                    is_special_bucket,
+                    rho_overwrite,
+                );
+
+                let mut res = arc_mtx.lock().unwrap();
+                res[b_as_idx_plus_1 - 1] = a;
+            }
+        });
     let reskbs_sbs: PolarsResult<Vec<(f64, f64)>> = Arc::try_unwrap(arc_mtx)
         .map_err(|_| PolarsError::ComputeError("Couldn't unwrap Arc".into()))?
         .into_inner()
         .map_err(|_| PolarsError::ComputeError("Couldn't get Mutex inner".into()))?
         .into_iter()
         .collect();
     reskbs_sbs
@@ -415,15 +418,15 @@
     for _ in 0..n_buckets {
         reskbs_sbs.push(Ok((0., 0.)))
     }
 
     let arc_mtx = std::sync::Arc::new(Mutex::new(reskbs_sbs));
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
     df.fill_null(FillNullStrategy::Zero)?
-        .partition_by(["b"])?
+        .partition_by(["b"], true)?
         .par_iter()
         .for_each(|bucket_df| {
             // Ok to go unsafe here becaause we validate length in [equity_delta_charge_distributor]
             let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
             // validating also bucket is not greater than max index of bucket_rho_diff_rf
             let b_as_idx_plus_1 = match b_as_idx_plus_1 {
                 AnyValue::Utf8(st) => st.parse::<usize>().ok().and_then(|b_id| {
@@ -520,23 +523,25 @@
         };
         // First, check dtenor was provided
         if let Some(dt) = dtenor {
             let rho_case4 = scenario_fn(dt);
             let rho_case5 = scenario_fn(dt * rho_diff_rft);
             let rho_case6 = scenario_fn(dt * rho_name_bucket);
             let rho_case7 = scenario_fn(dt * rho_diff_rft * rho_name_bucket);
-            let mut arr_tenor = df.select([*c1, *c2])?.to_ndarray::<Float64Type>()?; // Nulls must've been filled
+            let mut arr_tenor = df
+                .select([*c1, *c2])?
+                .to_ndarray::<Float64Type>(IndexOrder::Fortran)?; // Nulls must've been filled
             let dim = arr_tenor.raw_dim();
 
             let mut next_tenors_sum = Array2::<f64>::zeros(dim);
             for (c3, c4) in cols_by_tenor[(t + 1)..].iter() {
                 let next_tenor = df
                     .select([*c3, *c4])?
                     //.fill_null(FillNullStrategy::Zero)?
-                    .to_ndarray::<Float64Type>()?; // Nulls must've been filled
+                    .to_ndarray::<Float64Type>(IndexOrder::Fortran)?; // Nulls must've been filled
                 next_tenors_sum = next_tenors_sum + next_tenor;
             }
             let type0_sum = next_tenors_sum.slice(s![.., 0]).sum();
             let type1_sum = next_tenors_sum.slice(s![.., 1]).sum();
             arr_tenor
                 .indexed_iter_mut()
                 .par_bridge()
@@ -652,50 +657,51 @@
     let mut reskbs_sbs: Vec<PolarsResult<(String, (f64, f64))>> = Vec::with_capacity(n_buckets);
     for _ in 0..n_buckets {
         reskbs_sbs.push(Ok(("".to_string(), (0., 0.))))
     }
 
     let arc_mtx = std::sync::Arc::new(Mutex::new(reskbs_sbs));
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
-    df.partition_by(["b"])?.par_iter().for_each(|bucket_df| {
-        // Safety: since we are in partition, bucket_df["b"] has at least one element
-        let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
-        let b_as_idx_plus_1 =
-            match b_as_idx_plus_1 {
+    df.partition_by(["b"], true)?
+        .par_iter()
+        .for_each(|bucket_df| {
+            // Safety: since we are in partition, bucket_df["b"] has at least one element
+            let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
+            let b_as_idx_plus_1 = match b_as_idx_plus_1 {
                 AnyValue::Utf8(st) => st.parse::<usize>().ok().and_then(|b_id| {
                     if b_id <= n_buckets {
                         Some(b_id)
                     } else {
                         None
                     }
                 }),
                 _ => None,
             };
 
-        // For example if CSR BCBS bucket is 19, then we would have None here
-        // Now, if b_as_idx_plus_1 is None then we simply do nothing
-        if let Some(b_as_idx_plus_1) = b_as_idx_plus_1 {
-            let rho_diff_curve = rho_diff_curve
-                .get(b_as_idx_plus_1 - 1)
-                .unwrap_or_else(|| &0.);
+            // For example if CSR BCBS bucket is 19, then we would have None here
+            // Now, if b_as_idx_plus_1 is None then we simply do nothing
+            if let Some(b_as_idx_plus_1) = b_as_idx_plus_1 {
+                let rho_diff_curve = rho_diff_curve
+                    .get(b_as_idx_plus_1 - 1)
+                    .unwrap_or_else(|| &0.);
 
-            // CALCULATE Kb Sb for a bucket
-            let buck_kb_sb = bucket_kb_sb_single_type(
-                bucket_df,
-                rho_same_curve,
-                *rho_diff_curve,
-                scenario_fn,
-                columns,
-                None,
-                special_bucket,
-            );
-            let mut res = arc_mtx.lock().unwrap();
-            res[b_as_idx_plus_1 - 1] = buck_kb_sb;
-        }
-    });
+                // CALCULATE Kb Sb for a bucket
+                let buck_kb_sb = bucket_kb_sb_single_type(
+                    bucket_df,
+                    rho_same_curve,
+                    *rho_diff_curve,
+                    scenario_fn,
+                    columns,
+                    None,
+                    special_bucket,
+                );
+                let mut res = arc_mtx.lock().unwrap();
+                res[b_as_idx_plus_1 - 1] = buck_kb_sb;
+            }
+        });
 
     let reskbs_sbs: PolarsResult<Vec<(String, (f64, f64))>> = Arc::try_unwrap(arc_mtx)
         .map_err(|_| PolarsError::ComputeError("Couldn't unwrap Arc".into()))?
         .into_inner()
         .map_err(|_| PolarsError::ComputeError("Couldn't get Mutex inner".into()))?
         .into_iter()
         .collect();
@@ -738,15 +744,15 @@
     // as per 21.94. This can be achieved by passing an additional Vega flag.
     // However, does this make sence? Every rho in the text is less than or equal to(in case of opt mat same tenor) 1
     // Hence, can we ever have rho over 1? Doesn't seem so.
     let case1 = scenario_fn(rho_diff_curve); //Same tenor, diff curve
     let yield_df = bucket_df
         .select(columns)?
         .fill_null(FillNullStrategy::Zero)?;
-    let all_yield_arr = yield_df.to_ndarray::<Float64Type>()?;
+    let all_yield_arr = yield_df.to_ndarray::<Float64Type>(IndexOrder::Fortran)?;
 
     // EQ Vega, take care of special bucket
     match special_bucket {
         Some(x) if x == bucket.as_str() => {
             let abs_sum = all_yield_arr.iter().map(|x| x.abs()).sum::<f64>();
             return Ok((x.to_string(), (abs_sum, abs_sum)));
         }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common_curv.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/common_curv.rs`

 * *Files 1% similar despite different names*

```diff
@@ -165,43 +165,44 @@
     for _ in 0..n_buckets {
         res_kb_cvr.push((Ok((0., 0.)), Ok((0., 0.))))
     }
 
     let arc_mtx_kbpm_cvr = std::sync::Arc::new(Mutex::new(res_kb_cvr));
 
     // Do not iterate over each bukcet. Instead, only iterate over unique buckets
-    df.partition_by(["b"])?.par_iter().for_each(|bucket_df| {
-        // Ok to go unsafe here becaause we validate length in [equity_delta_charge_distributor]
-        let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
-        let b_as_idx_plus_1 =
-            match b_as_idx_plus_1 {
+    df.partition_by(["b"], true)?
+        .par_iter()
+        .for_each(|bucket_df| {
+            // Ok to go unsafe here becaause we validate length in [equity_delta_charge_distributor]
+            let b_as_idx_plus_1 = unsafe { bucket_df["b"].get_unchecked(0) };
+            let b_as_idx_plus_1 = match b_as_idx_plus_1 {
                 AnyValue::Utf8(st) => st.parse::<usize>().ok().and_then(|b_id| {
                     if b_id <= n_buckets {
                         Some(b_id)
                     } else {
                         None
                     }
                 }),
                 _ => None,
             };
 
-        if let Some(b_as_idx_plus_1) = b_as_idx_plus_1 {
-            let is_special_bucket = matches!(special_bucket, Some(b) if b == b_as_idx_plus_1);
+            if let Some(b_as_idx_plus_1) = b_as_idx_plus_1 {
+                let is_special_bucket = matches!(special_bucket, Some(b) if b == b_as_idx_plus_1);
 
-            let rho = bucket_rho[b_as_idx_plus_1 - 1];
-            // CALCULATE Kb Sb for a bucket
-            let buck_kb_plus_cvr_up_sum =
-                kb_plus_minus(&bucket_df["cvr_up"], rho, is_special_bucket);
-            let buck_kb_minus_cvr_down_sum =
-                kb_plus_minus(&bucket_df["cvr_down"], rho, is_special_bucket);
-            let res = (buck_kb_plus_cvr_up_sum, buck_kb_minus_cvr_down_sum);
-            let mut r = arc_mtx_kbpm_cvr.lock().unwrap(); //[b_as_idx_plus_1-1];// = res;
-            r[b_as_idx_plus_1 - 1] = res;
-        }
-    });
+                let rho = bucket_rho[b_as_idx_plus_1 - 1];
+                // CALCULATE Kb Sb for a bucket
+                let buck_kb_plus_cvr_up_sum =
+                    kb_plus_minus(&bucket_df["cvr_up"], rho, is_special_bucket);
+                let buck_kb_minus_cvr_down_sum =
+                    kb_plus_minus(&bucket_df["cvr_down"], rho, is_special_bucket);
+                let res = (buck_kb_plus_cvr_up_sum, buck_kb_minus_cvr_down_sum);
+                let mut r = arc_mtx_kbpm_cvr.lock().unwrap(); //[b_as_idx_plus_1-1];// = res;
+                r[b_as_idx_plus_1 - 1] = res;
+            }
+        });
     //Result<Vec<(f64, f64)>>
     let (res_kbp_cvrup, res_kbm_cvrdown): (
         Vec<PolarsResult<(f64, f64)>>,
         Vec<PolarsResult<(f64, f64)>>,
     ) = Arc::try_unwrap(arc_mtx_kbpm_cvr)
         .map_err(|_| PolarsError::ComputeError("Couldn't unwrap Arc".into()))?
         .into_inner()
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #![allow(clippy::type_complexity)]
 
 use crate::prelude::*;
 use ndarray::Array2;
 use ultibi::{prelude::CPM, BaseMeasure, IntoLazy};
 //use polars::lazy::dsl::apply_multiple;
-use ultibi::polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput};
+use ultibi::polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput};
 
 pub fn csrnonsec_curv_delta(_: &CPM) -> PolarsResult<Expr> {
     Ok(curv_delta_5("CSR_nonSec"))
 }
 /// Helper functions
 pub fn csrnonsec_curv_delta_weighted(op: &CPM) -> PolarsResult<Expr> {
     let juri: Jurisdiction = get_jurisdiction(op)?;
@@ -234,15 +234,15 @@
     )
 }
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrnonsec_curv_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csrnonsec_curvature_charge_low(op)?,
         csrnonsec_curvature_charge_medium(op)?,
         csrnonsec_curvature_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 //! CSR non-Sec Delta Calculations
 use crate::helpers::*;
 use crate::sbm::common::*;
 use ndarray::Array2;
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput},
     BaseMeasure, IntoLazy, CPM,
 };
 
 use crate::prelude::*;
 
 pub fn total_csr_nonsec_delta_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Delta", "CSR_nonSec", total_vega_curv_sens()))
@@ -145,34 +145,34 @@
 ) -> PolarsResult<Expr> {
     let juri: Jurisdiction = get_jurisdiction(op)?;
     let _suffix = scenario.as_str();
     let (weight, bucket_col, name_rho_vec, gamma, n_buckets, special_bucket) = match juri {
         #[cfg(feature = "CRR2")]
         Jurisdiction::CRR2 => (
             [
-                col("SensWeightsCRR2").arr().get(lit(0)),
-                col("SensWeightsCRR2").arr().get(lit(1)),
-                col("SensWeightsCRR2").arr().get(lit(2)),
-                col("SensWeightsCRR2").arr().get(lit(3)),
-                col("SensWeightsCRR2").arr().get(lit(4)),
+                col("SensWeightsCRR2").list().get(lit(0)),
+                col("SensWeightsCRR2").list().get(lit(1)),
+                col("SensWeightsCRR2").list().get(lit(2)),
+                col("SensWeightsCRR2").list().get(lit(3)),
+                col("SensWeightsCRR2").list().get(lit(4)),
             ],
             col("BucketCRR2"),
             Vec::from(scenario.csr_nonsec_delta_diff_name_rho_per_bucket_base_crr2),
             &scenario.csr_nonsec_delta_vega_gamma_crr2,
             20usize,
             Some(18usize),
         ),
 
         Jurisdiction::BCBS => (
             [
-                col("SensWeights").arr().get(lit(0)),
-                col("SensWeights").arr().get(lit(1)),
-                col("SensWeights").arr().get(lit(2)),
-                col("SensWeights").arr().get(lit(3)),
-                col("SensWeights").arr().get(lit(4)),
+                col("SensWeights").list().get(lit(0)),
+                col("SensWeights").list().get(lit(1)),
+                col("SensWeights").list().get(lit(2)),
+                col("SensWeights").list().get(lit(3)),
+                col("SensWeights").list().get(lit(4)),
             ],
             col("BucketBCBS"),
             Vec::from(scenario.csr_nonsec_delta_vega_diff_name_rho_per_bucket_base_bcbs),
             &scenario.csr_nonsec_delta_vega_gamma_bcbs,
             18,
             Some(16),
         ),
@@ -374,15 +374,15 @@
 }
 
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrnonsec_delta_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csr_nonsec_delta_charge_low(op)?,
         csr_nonsec_delta_charge_medium(op)?,
         csr_nonsec_delta_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Ok(col("CSR nonSec DeltaCharge High")
         + col("CSR nonSec VegaCharge High")
         + col("CSR nonSec CurvatureCharge High"))
 }
 
 /// Not a real measure. Used for analysis only
 fn csrnonsec_total_max(_: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         col("CSR nonSec TotalCharge Low"),
         col("CSR nonSec TotalCharge Medium"),
         col("CSR nonSec TotalCharge High"),
     ]))
 }
 
 pub(crate) fn csrnonsec_total_measures() -> Vec<Measure> {
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use crate::prelude::*;
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput},
     BaseMeasure, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
 pub fn total_csrnonsec_vega_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Vega", "CSR_nonSec", total_vega_curv_sens()))
@@ -12,17 +12,17 @@
 
 pub fn total_csrnonsec_vega_sens_weighted_bcbs(op: &CPM) -> PolarsResult<Expr> {
     let juri: Jurisdiction = get_jurisdiction(op)?;
 
     match juri {
         #[cfg(feature = "CRR2")]
         Jurisdiction::CRR2 => total_csrnonsec_vega_sens(op)
-            .map(|expr| expr * col("SensWeightsCRR2").arr().get(lit(0))),
+            .map(|expr| expr * col("SensWeightsCRR2").list().get(lit(0))),
         Jurisdiction::BCBS => {
-            total_csrnonsec_vega_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
+            total_csrnonsec_vega_sens(op).map(|expr| expr * col("SensWeights").list().get(lit(0)))
         }
     }
 }
 
 ///calculate CSR Non Sec Interm Result
 pub(crate) fn csr_nonsec_vega_sb(op: &CPM) -> PolarsResult<Expr> {
     csr_nonsec_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Sb)
@@ -67,24 +67,24 @@
 ) -> PolarsResult<Expr> {
     let juri: Jurisdiction = get_jurisdiction(op)?;
     let _suffix = scenario.as_str();
 
     let (weight, bucket_col, name_rho_vec, rho_opt, gamma, special_bucket) = match juri {
         #[cfg(feature = "CRR2")]
         Jurisdiction::CRR2 => (
-            col("SensWeightsCRR2").arr().get(lit(0)),
+            col("SensWeightsCRR2").list().get(lit(0)),
             col("BucketCRR2"),
             Vec::from(scenario.csr_nonsec_delta_diff_name_rho_per_bucket_base_crr2),
             &scenario.base_vega_rho,
             &scenario.csr_nonsec_delta_vega_gamma_crr2,
             Some("18"),
         ),
 
         Jurisdiction::BCBS => (
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
             col("BucketBCBS"),
             Vec::from(scenario.csr_nonsec_delta_vega_diff_name_rho_per_bucket_base_bcbs),
             &scenario.base_vega_rho,
             &scenario.csr_nonsec_delta_vega_gamma_bcbs,
             Some("16"),
         ),
     };
@@ -208,15 +208,15 @@
     )
 }
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrnonsec_vega_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csr_nonsec_vega_charge_low(op)?,
         csr_nonsec_vega_charge_medium(op)?,
         csr_nonsec_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 }
 
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrsecctp_curv_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csrsecctp_curvature_charge_low(op)?,
         csrsecctp_curvature_charge_medium(op)?,
         csrsecctp_curvature_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 //! CSR Sec CTP Delta Calculations
 
 use crate::helpers::*;
 use sbm::csr_nonsec::delta::csr_nonsec_delta_charge;
-use ultibi::{polars::prelude::max_exprs, BaseMeasure, CPM};
+use ultibi::{polars::prelude::max_horizontal, BaseMeasure, CPM};
 
 use crate::prelude::*;
 
 pub fn total_csr_sec_ctp_delta_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Delta", "CSR_Sec_CTP", total_delta_sens()))
 }
 /// Helper functions
@@ -145,33 +145,33 @@
     let juri: Jurisdiction = get_jurisdiction(op)?;
 
     // First, obtaining parameters specific to jurisdiciton
     let (weight, bucket_col, name_rho_vec, gamma, n_buckets, special_bucket) = match juri {
         #[cfg(feature = "CRR2")]
         Jurisdiction::CRR2 => (
             [
-                col("SensWeightsCRR2").arr().get(lit(0)),
-                col("SensWeightsCRR2").arr().get(lit(1)),
-                col("SensWeightsCRR2").arr().get(lit(2)),
-                col("SensWeightsCRR2").arr().get(lit(3)),
-                col("SensWeightsCRR2").arr().get(lit(4)),
+                col("SensWeightsCRR2").list().get(lit(0)),
+                col("SensWeightsCRR2").list().get(lit(1)),
+                col("SensWeightsCRR2").list().get(lit(2)),
+                col("SensWeightsCRR2").list().get(lit(3)),
+                col("SensWeightsCRR2").list().get(lit(4)),
             ],
             col("BucketCRR2"),
             Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_crr2),
             &scenario.csr_ctp_delta_vega_gamma_crr2,
             18usize,
             Option::<usize>::None,
         ),
         Jurisdiction::BCBS => (
             [
-                col("SensWeights").arr().get(lit(0)),
-                col("SensWeights").arr().get(lit(1)),
-                col("SensWeights").arr().get(lit(2)),
-                col("SensWeights").arr().get(lit(3)),
-                col("SensWeights").arr().get(lit(4)),
+                col("SensWeights").list().get(lit(0)),
+                col("SensWeights").list().get(lit(1)),
+                col("SensWeights").list().get(lit(2)),
+                col("SensWeights").list().get(lit(3)),
+                col("SensWeights").list().get(lit(4)),
             ],
             col("BucketBCBS"),
             Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_bcbs),
             &scenario.csr_ctp_delta_vega_gamma_bcbs,
             16usize,
             Option::<usize>::None,
         ),
@@ -217,15 +217,15 @@
 }
 
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrsecctp_delta_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csr_sec_ctp_delta_charge_low(op)?,
         csr_sec_ctp_delta_charge_medium(op)?,
         csr_sec_ctp_delta_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 use crate::{prelude::*, sbm::csr_nonsec::vega::csr_nonsec_vega_charge};
-use ultibi::{polars::prelude::max_exprs, BaseMeasure, CPM};
+use ultibi::{polars::prelude::max_horizontal, BaseMeasure, CPM};
 
 pub fn total_csrsecctp_vega_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Vega", "CSR_Sec_CTP", total_vega_curv_sens()))
 }
 
 pub fn total_csrsecctp_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
     let juri: Jurisdiction = get_jurisdiction(op)?;
 
     match juri {
         #[cfg(feature = "CRR2")]
         Jurisdiction::CRR2 => total_csrsecctp_vega_sens(op)
-            .map(|expr| expr * col("SensWeightsCRR2").arr().get(lit(0))),
+            .map(|expr| expr * col("SensWeightsCRR2").list().get(lit(0))),
         Jurisdiction::BCBS => {
-            total_csrsecctp_vega_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
+            total_csrsecctp_vega_sens(op).map(|expr| expr * col("SensWeights").list().get(lit(0)))
         }
     }
 }
 
 ///calculate CSR Sec CTP Interm Result
 pub(crate) fn csrsecctp_vega_sb(op: &CPM) -> PolarsResult<Expr> {
     csrsecctp_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Sb)
@@ -62,24 +62,24 @@
 ) -> PolarsResult<Expr> {
     let juri: Jurisdiction = get_jurisdiction(op)?;
     let _suffix = scenario.as_str();
 
     let (weight, bucket_col, name_rho_vec, rho_opt, gamma, special_bucket) = match juri {
         #[cfg(feature = "CRR2")]
         Jurisdiction::CRR2 => (
-            col("SensWeightsCRR2").arr().get(lit(0)),
+            col("SensWeightsCRR2").list().get(lit(0)),
             col("BucketCRR2"),
             Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_crr2),
             &scenario.base_vega_rho,
             &scenario.csr_ctp_delta_vega_gamma_crr2,
             None,
         ),
 
         Jurisdiction::BCBS => (
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
             col("BucketBCBS"),
             Vec::from(scenario.csr_ctp_delta_vega_diff_name_rho_per_bucket_base_bcbs),
             &scenario.base_vega_rho,
             &scenario.csr_ctp_delta_vega_gamma_bcbs,
             None,
         ),
     };
@@ -108,15 +108,15 @@
 }
 
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrsecctp_vega_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csrsecctp_vega_charge_low(op)?,
         csrsecctp_vega_charge_medium(op)?,
         csrsecctp_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 }
 
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrsecnonctp_curv_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csr_sec_nonctp_curvature_charge_low(op)?,
         csr_sec_nonctp_curvature_charge_medium(op)?,
         csr_sec_nonctp_curvature_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 //! CSR Sec non-CTP Delta Calculations
 
 use crate::prelude::*;
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput, MeltArgs},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput, MeltArgs},
     BaseMeasure, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
 pub fn total_csr_sec_nonctp_delta_sens(_: &CPM) -> PolarsResult<Expr> {
-    Ok(rc_rcat_sens("CSR_Sec_nonCTP", "Delta", total_delta_sens()))
+    Ok(rc_rcat_sens("Delta", "CSR_Sec_nonCTP", total_delta_sens()))
 }
 /// Helper functions
 
 fn csr_sec_nonctp_delta_sens_weighted_05y_bcbs() -> Expr {
     rc_tenor_weighted_sens(
         "Delta",
         "CSR_Sec_nonCTP",
@@ -251,28 +251,28 @@
             col("Tranche"),
             col("BucketBCBS"),
             col("Sensitivity_05Y"),
             col("Sensitivity_1Y"),
             col("Sensitivity_3Y"),
             col("Sensitivity_5Y"),
             col("Sensitivity_10Y"),
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
             col("RiskCategory"),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
 
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrsecnonctp_delta_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csr_sec_nonctp_delta_charge_low(op)?,
         csr_sec_nonctp_delta_charge_medium(op)?,
         csr_sec_nonctp_delta_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 use crate::{prelude::*, sbm::equity::vega::equity_vega_charge};
-use ultibi::{polars::prelude::max_exprs, BaseMeasure, CPM};
+use ultibi::{polars::prelude::max_horizontal, BaseMeasure, CPM};
 
 pub fn total_csr_sec_nonctp_vega_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens(
         "Vega",
         "CSR_Sec_nonCTP",
         total_vega_curv_sens(),
     ))
 }
 
 pub fn total_csr_sec_nonctp_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    total_csr_sec_nonctp_vega_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
+    total_csr_sec_nonctp_vega_sens(op).map(|expr| expr * col("SensWeights").list().get(lit(0)))
 }
 ///Interm Result
 pub(crate) fn csr_sec_nonctp_vega_sb(op: &CPM) -> PolarsResult<Expr> {
     csr_sec_nonctp_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Sb)
 }
 pub(crate) fn csr_sec_nonctp_vega_kb_low(op: &CPM) -> PolarsResult<Expr> {
     csr_sec_nonctp_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
@@ -82,15 +82,15 @@
 }
 
 /// Returns max of three scenarios
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn csrsecnonctp_vega_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         csr_sec_nonctp_vega_charge_low(op)?,
         csr_sec_nonctp_vega_charge_medium(op)?,
         csr_sec_nonctp_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #![allow(clippy::type_complexity)]
 
 use crate::prelude::*;
 use ndarray::Array2;
-use ultibi::polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput};
+use ultibi::polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput};
 use ultibi::prelude::CPM;
 use ultibi::{BaseMeasure, IntoLazy};
 
 pub fn eq_curv_delta(_: &CPM) -> PolarsResult<Expr> {
     Ok(curv_delta_spot("Equity"))
 }
 /// Helper functions
@@ -188,15 +188,15 @@
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn eq_curv_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         eq_curvature_charge_low(op)?,
         eq_curvature_charge_medium(op)?,
         eq_curvature_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/delta.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/delta.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 //! is 1*0.25 because spot == spot (1) and Goog != App (0.25)
 //! Apprepo Googspot is 0.999*0.25 because repo != spot and App != Goog (0.25)
 //! Hence, it's sufficient to build two matrixes:
 //! 1 based on rft and 2 based on rf
 
 use crate::prelude::*;
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput},
     BaseMeasure, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
 /// Total Equity Delta Sens
 pub(crate) fn equity_delta_sens(_: &CPM) -> PolarsResult<Expr> {
@@ -120,14 +120,15 @@
             df = df
                 .lazy()
                 .filter(
                     col("rc")
                         .eq(lit("Equity"))
                         .and(col("rcat").eq(lit("Delta"))),
                 )
+                // TODO Fill empty bucket with 11 here
                 .with_columns([
                     when(col("rft").eq(lit("EqSpot")))
                         .then((col("d") * col("w")).alias("Spot"))
                         .otherwise(NULL.lit()),
                     when(col("rft").eq(lit("EqRepo")))
                         .then((col("d") * col("w")).alias("Repo"))
                         .otherwise(NULL.lit()),
@@ -167,28 +168,28 @@
         &[
             col("RiskCategory"),
             col("RiskClass"),
             col("BucketBCBS"),
             col("RiskFactor"),
             col("RiskFactorType"),
             col("SensitivitySpot"),
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn eq_delta_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         equity_delta_charge_low(op)?,
         equity_delta_charge_medium(op)?,
         equity_delta_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/vega.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/equity/vega.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 use crate::prelude::*;
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput},
     BaseMeasure, IntoLazy, CPM,
 };
 
 use ndarray::Array2;
 
 pub fn total_eq_vega_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Vega", "Equity", total_vega_curv_sens()))
 }
 
 pub fn total_eq_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    total_eq_vega_sens(op).map(|expr| expr * col("SensWeights").arr().get(lit(0)))
+    total_eq_vega_sens(op).map(|expr| expr * col("SensWeights").list().get(lit(0)))
 }
 ///Interm Result
 pub(crate) fn equity_vega_sb(op: &CPM) -> PolarsResult<Expr> {
     equity_vega_charge_distributor(op, &MEDIUM_CORR_SCENARIO, ReturnMetric::Sb)
 }
 pub(crate) fn equity_vega_kb_low(op: &CPM) -> PolarsResult<Expr> {
     equity_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Kb)
@@ -156,27 +156,27 @@
             col("BucketBCBS"),
             col("RiskFactor"),
             col("Sensitivity_05Y"),
             col("Sensitivity_1Y"),
             col("Sensitivity_3Y"),
             col("Sensitivity_5Y"),
             col("Sensitivity_10Y"),
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn eq_vega_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         equity_vega_charge_low(op)?,
         equity_vega_charge_medium(op)?,
         equity_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use crate::prelude::*;
 use ndarray::{Array1, Array2};
 use ultibi::{
     polars::prelude::{
-        apply_multiple, df, max_exprs, ChunkFillNullValue, ChunkSet, DataType, Float64Chunked,
+        apply_multiple, df, max_horizontal, ChunkFillNullValue, ChunkSet, DataType, Float64Chunked,
         GetOutput, IntoSeries, NumOpsDispatch, Utf8NameSpaceImpl,
     },
     BaseMeasure, IntoLazy, CPM,
 };
 
 use super::delta::ccy_regex;
 
@@ -222,15 +222,15 @@
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn fx_curv_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         fx_curvature_charge_low(op)?,
         fx_curvature_charge_medium(op)?,
         fx_curvature_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/delta.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/delta.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 use crate::{
     helpers::get_jurisdiction,
     prelude::*,
     sbm::common::{across_bucket_agg, SBMChargeType},
 };
 use ultibi::{
     polars::prelude::{
-        apply_multiple, df, max_exprs, ChunkCompare, ChunkSet, DataType, GetOutput, IntoSeries,
-        PolarsError, Utf8NameSpaceImpl,
+        apply_multiple, df, max_horizontal, ChunkCompare, ChunkSet, DataType, GetOutput,
+        IntoSeries, PolarsError, Utf8NameSpaceImpl,
     },
     BaseMeasure, IntoLazy, CPM,
 };
 
 /// This works for cases like GBP reporting with BCBS params
 pub(crate) fn ccy_regex(op: &CPM) -> PolarsResult<String> {
     let juri: Jurisdiction = get_jurisdiction(op)?;
@@ -65,15 +65,15 @@
         GetOutput::from_type(DataType::Float64),
         false,
     ))
 }
 
 /// takes CalcParams because we need to know reporting CCY
 pub(crate) fn fx_delta_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    Ok(fx_delta_sens_repccy(op)? * col("SensWeights").arr().get(lit(0)))
+    Ok(fx_delta_sens_repccy(op)? * col("SensWeights").list().get(lit(0)))
 }
 ///calculate FX Delta Sb, same for all scenarios
 pub(crate) fn fx_delta_sb(op: &CPM) -> PolarsResult<Expr> {
     fx_delta_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
 }
 
 ///calculate FX Delta Kb, same for all scenarios
@@ -127,15 +127,15 @@
                 "rc"   => &columns[1],
                 "b"    => &columns[2],
                 "d"    => &columns[3],
                 "w"    => &columns[4],
             ]?;
 
             let ccy_regex = ccy_regex.clone();
-            let mut df = df
+            let df = df
                 .lazy()
                 .filter(
                     col("rc")
                         .eq(lit("FX"))
                         .and(col("rcat").eq(lit("Delta")))
                         .and(col("b").apply(
                             move |col| {
@@ -146,15 +146,16 @@
                 )
                 .groupby([col("b")])
                 .agg([(col("d") * col("w")).sum().alias("dw_sum")])
                 // Drop nulls (ie other reporting ccys)
                 .drop_nulls(Some(vec![col("dw_sum")]))
                 .collect()?;
 
-            df.rechunk();
+            // Not needed anymore
+            //df.rechunk();
 
             if df.height() == 0 {
                 return Ok(Some(Series::new("res", [0.])));
             };
 
             //21.4.4 |dw_sum| == kb for FX
             //21.4.5.a sb == dw_sum
@@ -184,27 +185,27 @@
             )
         },
         &[
             col("RiskCategory"),
             col("RiskClass"),
             col("BucketBCBS"),
             col("SensitivitySpot"),
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     ))
 }
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn fx_delta_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         fx_delta_charge_low(op)?,
         fx_delta_charge_medium(op)?,
         fx_delta_charge_high(op)?,
     ]))
 }
 /// Exporting Measures
 pub(crate) fn fx_delta_measures() -> Vec<Measure> {
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/vega.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/fx/vega.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 use crate::helpers::{get_optional_parameter, get_optional_parameter_array, ReturnMetric};
 use crate::prelude::*;
 use crate::sbm::common::{across_bucket_agg, rc_rcat_sens, total_vega_curv_sens, SBMChargeType};
 use ndarray::{Array1, Array2, Axis};
+use polars::prelude::IndexOrder;
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, Float64Type, GetOutput},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, Float64Type, GetOutput},
     CPM,
 };
 use ultibi::{BaseMeasure, IntoLazy};
 
 pub fn total_fx_vega_sens(_: &CPM) -> PolarsResult<Expr> {
     Ok(rc_rcat_sens("Vega", "FX", total_vega_curv_sens()))
 }
 
 pub fn total_fx_vega_sens_weighted(op: &CPM) -> PolarsResult<Expr> {
-    Ok(total_fx_vega_sens(op)? * col("SensWeights").arr().get(lit(0)))
+    Ok(total_fx_vega_sens(op)? * col("SensWeights").list().get(lit(0)))
 }
 
 /// Sb Low == Sb Medium == Sb High
 /// FX Vega Sb is identical to total_fx_vega_sens_weighted
 pub(crate) fn fx_vega_sb(op: &CPM) -> PolarsResult<Expr> {
     fx_vega_charge_distributor(op, &LOW_CORR_SCENARIO, ReturnMetric::Sb)
 }
@@ -109,15 +110,15 @@
 
             let res_len = columns[0].len();
 
             if df.height() == 0 {
                 return Ok(Some(Series::new("res", [0.])));
             };
 
-            let sens = df.to_ndarray::<Float64Type>()?;
+            let sens = df.to_ndarray::<Float64Type>(IndexOrder::Fortran)?;
 
             let sbs = sens.sum_axis(Axis(1));
 
             // Early return Kb or Sb, ie the required metric
             if let ReturnMetric::Sb = rtrn {
                 return Ok(Some(Series::new("res", [sbs.sum()])));
             }
@@ -148,28 +149,28 @@
             col("RiskClass"),
             col("BucketBCBS"),
             col("Sensitivity_05Y"),
             col("Sensitivity_1Y"),
             col("Sensitivity_3Y"),
             col("Sensitivity_5Y"),
             col("Sensitivity_10Y"),
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     ))
 }
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn fx_vega_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         fx_vega_charge_low(op)?,
         fx_vega_charge_medium(op)?,
         fx_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use crate::{
     prelude::*,
     sbm::common::{across_bucket_agg, rc_rcat_sens, SBMChargeType},
 };
 use ndarray::{Array1, Array2};
 use ultibi::{
-    polars::prelude::{apply_multiple, df, max_exprs, DataType, GetOutput},
+    polars::prelude::{apply_multiple, df, max_horizontal, DataType, GetOutput},
     BaseMeasure, IntoLazy, CPM,
 };
 
 #[cfg(feature = "CRR2")]
 use super::delta::build_girr_crr2_gamma;
 use crate::helpers::ReturnMetric;
 
@@ -218,15 +218,15 @@
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn girr_curv_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         girr_curvature_charge_low(op)?,
         girr_curvature_charge_medium(op)?,
         girr_curvature_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/delta.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/delta.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::prelude::*;
 use ultibi::{
     polars::prelude::{
-        apply_multiple, col, df, lit, max_exprs, when, DataType, GetOutput, PolarsError,
+        apply_multiple, col, df, lit, max_horizontal, when, DataType, GetOutput, PolarsError,
     },
     BaseMeasure, IntoLazy, CPM,
 };
 
 //use polars::lazy::dsl::{apply_multiple, col, lit, when};
 use rayon::prelude::IntoParallelIterator;
 
@@ -296,15 +296,15 @@
                 .select([col("*").exclude(["rft"])])
                 .collect()?;
 
             if df.height() == 0 {
                 return Ok(Some(Series::new("res", [0.])));
             };
 
-            let part = df.partition_by(["b"])?;
+            let part = df.partition_by(["b"], true)?;
 
             let res_buckets_kbs_sbs: PolarsResult<Vec<(String, (f64, f64))>> = part
                 .into_par_iter()
                 .map(|bdf| {
                     bucket_kb_sb_single_type(
                         &bdf,
                         &girr_delta_rho_same_curve,
@@ -367,25 +367,25 @@
             col("Sensitivity_5Y"),
             col("Sensitivity_10Y"),
             col("Sensitivity_15Y"),
             col("Sensitivity_20Y"),
             col("Sensitivity_30Y"),
             col("RiskCategory"),
             //col("SensWeights"),
-            col("SensWeights").arr().get(lit(0)),
-            col("SensWeights").arr().get(lit(1)),
-            col("SensWeights").arr().get(lit(2)),
-            col("SensWeights").arr().get(lit(3)),
-            col("SensWeights").arr().get(lit(4)),
-            col("SensWeights").arr().get(lit(5)),
-            col("SensWeights").arr().get(lit(6)),
-            col("SensWeights").arr().get(lit(7)),
-            col("SensWeights").arr().get(lit(8)),
-            col("SensWeights").arr().get(lit(9)),
-            col("SensWeights").arr().get(lit(10)),
+            col("SensWeights").list().get(lit(0)),
+            col("SensWeights").list().get(lit(1)),
+            col("SensWeights").list().get(lit(2)),
+            col("SensWeights").list().get(lit(3)),
+            col("SensWeights").list().get(lit(4)),
+            col("SensWeights").list().get(lit(5)),
+            col("SensWeights").list().get(lit(6)),
+            col("SensWeights").list().get(lit(7)),
+            col("SensWeights").list().get(lit(8)),
+            col("SensWeights").list().get(lit(9)),
+            col("SensWeights").list().get(lit(10)),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
 
 /// 325ag
@@ -441,15 +441,15 @@
 
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn girr_delta_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         girr_delta_charge_low(op)?,
         girr_delta_charge_medium(op)?,
         girr_delta_charge_high(op)?,
     ]))
 }
 /// Exporting Measures
 pub(crate) fn girr_delta_measures() -> Vec<Measure> {
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/vega.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/girr/vega.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 use crate::helpers::{get_optional_parameter, get_optional_parameter_array, ReturnMetric};
 use crate::prelude::*;
 use crate::sbm::common::{
     across_bucket_agg, option_maturity_rho, rc_rcat_sens, rc_tenor_weighted_sens,
     total_vega_curv_sens, SBMChargeType,
 };
+use ultibi::polars::prelude::IndexOrder;
 use ultibi::{
     polars::prelude::{
-        apply_multiple, col, df, lit, max_exprs, ChunkCompare, DataType, Float64Type, GetOutput,
-        TakeRandom,
+        apply_multiple, col, df, lit, max_horizontal, ChunkCompare, DataType, Float64Type,
+        GetOutput, TakeRandom,
     },
     CPM,
 };
 use ultibi::{BaseMeasure, DataFrame, IntoLazy};
 
 #[cfg(feature = "CRR2")]
 use super::delta::build_girr_crr2_gamma;
@@ -162,15 +163,15 @@
                 .fill_null(lit::<f64>(0.))
                 .collect()?;
 
             if df.height() == 0 {
                 return Ok(Some(Series::new("res", [0.])));
             };
 
-            let part = df.partition_by(["b"])?;
+            let part = df.partition_by(["b"], true)?;
             let res_buckets_kbs_sbs: PolarsResult<Vec<((&str, f64), f64)>> = part
                 .par_iter()
                 .map(|bdf| girr_vega_bucket_kb_sb(bdf, &girr_vega_opt_rho))
                 .collect();
 
             let buckets_kbs_sbs = res_buckets_kbs_sbs?;
             let (buckets_kbs, sbs): (Vec<(&str, f64)>, Vec<f64>) =
@@ -206,15 +207,15 @@
             col("BucketBCBS"),
             col("GirrVegaUnderlyingMaturity"),
             col("Sensitivity_05Y"),
             col("Sensitivity_1Y"),
             col("Sensitivity_3Y"),
             col("Sensitivity_5Y"),
             col("Sensitivity_10Y"),
-            col("SensWeights").arr().get(lit(0)),
+            col("SensWeights").list().get(lit(0)),
             col("RiskFactorType"),
         ],
         GetOutput::from_type(DataType::Float64),
         true,
     )
 }
 
@@ -274,15 +275,15 @@
     mat: &str,
     _: &str,
 ) -> PolarsResult<Array1<f64>> {
     let mask = df["um"].equal(mat)?;
     Ok(df
         .filter(&mask)?
         .select(["y05", "y1", "y3", "y5", "y10"])?
-        .to_ndarray::<Float64Type>()?
+        .to_ndarray::<Float64Type>(IndexOrder::Fortran)?
         .into_shape(5)
         .unwrap_or_else(|_| Array1::<f64>::zeros(5)))
 }
 
 pub(crate) fn girr_vega_rho() -> Array2<f64> {
     let base = option_maturity_rho();
     let mut arr = Array2::<f64>::uninit((35, 35));
@@ -315,15 +316,15 @@
 }
 /// Returns max of three scenarios
 ///
 /// !Note This is not a real measure, as MAX should be taken as
 /// MAX(ir_delta_low+ir_vega_low+eq_curv_low, ..._medium, ..._high).
 /// This is for convienience view only.
 fn girr_vega_max(op: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         girr_vega_charge_low(op)?,
         girr_vega_charge_medium(op)?,
         girr_vega_charge_high(op)?,
     ]))
 }
 
 /// Exporting Measures
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/sbm/totals.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //! Totals across different Risk Classes
 
-use ultibi::polars::lazy::dsl::{col, max_exprs, Expr};
+use ultibi::polars::lazy::dsl::{col, max_horizontal, Expr};
 use ultibi::{DependantMeasure, Measure, PolarsResult, CPM};
 
 // Testing Dependant Measures
 fn sbm_charge_low_dep(_: &CPM) -> PolarsResult<Expr> {
     Ok(col("FX TotalCharge Low")
         + col("GIRR TotalCharge Low")
         + col("EQ TotalCharge Low")
@@ -30,15 +30,15 @@
         + col("CSR Sec nonCTP TotalCharge High")
         + col("CSR nonSec TotalCharge High")
         + col("CSR Sec CTP TotalCharge High")
         + col("Commodity TotalCharge High"))
 }
 
 pub(crate) fn sbm_charge_dep(_: &CPM) -> PolarsResult<Expr> {
-    Ok(max_exprs(&[
+    Ok(max_horizontal(&[
         col("SBM Charge High"),
         col("SBM Charge Medium"),
         col("SBM Charge Low"),
     ]))
 }
 
 pub(crate) fn sbm_total_measures() -> Vec<Measure> {
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/statics.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/statics.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/src/validate.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/src/validate.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 use ultibi::{
-    polars::prelude::{LazyFrame, PolarsError, PolarsResult},
-    ValidateSet,
+    errors::{UltiResult, UltimaErr},
+    polars::prelude::{LazyFrame, PolarsError},
 };
 
-pub(crate) fn validate_frame(
-    lf: &LazyFrame,
-    covered_bond: bool,
-    v: ValidateSet,
-) -> PolarsResult<()> {
+pub(crate) fn validate_frtb_frame(lf: &LazyFrame, covered_bond: bool, v: u8) -> UltiResult<()> {
     let arc_schema = lf.schema()?;
 
     // Buckets and weights assignments
     let mut must_have = vec![
         "RiskClass",
         "RiskCategory",
         "RiskFactor",
         "RiskFactorType",
         "BucketBCBS",
         "CreditQuality",
         "PnL_Up",
         "PnL_Down",
         "COB",
         "MaturityDate",
-        "BucketCRR2",
     ];
 
     if covered_bond {
         must_have.push("CoveredBondReducedWeight")
     }
 
     if cfg!(feature = "CRR2") {
         must_have.push("BucketCRR2")
     }
 
-    if matches!(v, ValidateSet::ALL) {
+    if matches!(v, 0) {
         // RRAO
         must_have.push("TradeId");
         must_have.push("EXOTIC_RRAO");
         must_have.push("OTHER_RRAO");
 
         // SBM + DRC
         must_have.push("GrossJTD");
@@ -56,16 +51,16 @@
         must_have.push("Sensitivity_15Y");
         must_have.push("Sensitivity_20Y");
         must_have.push("Sensitivity_30Y");
     }
 
     for must_have_col in must_have {
         if !arc_schema.iter_names().any(|col| col == must_have_col) {
-            return Err(PolarsError::NoData(
+            return Err(UltimaErr::from(PolarsError::NoData(
                 format!("{must_have_col} is missing. It is a required column. Check your data")
                     .into(),
-            ));
+            )));
         }
     }
 
     Ok(())
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/tests/common/mod.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/tests/common/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+use std::sync::Arc;
+
 use once_cell::sync::Lazy;
-use polars::prelude::*;
 
 use frtb_engine::prelude::FRTBDataSet;
 use ultibi::{
+    new::NewSourcedDataSet,
     prelude::{read_toml2, DataSet, DataSourceConfig},
-    ComputeRequest, ValidateSet,
+    ComputeRequest, IntoLazy,
 };
 
+use ultibi::polars::prelude::{col, Float64Type, IndexOrder};
+
 pub static LAZY_DASET: Lazy<Arc<FRTBDataSet>> = Lazy::new(|| {
     let conf_path = r"data/frtb/datasource_config.toml";
     let conf = read_toml2::<DataSourceConfig>(conf_path)
         .expect("Can not proceed without valid Data Set Up"); //Unrecovarable error
-    let mut data: FRTBDataSet = DataSet::from_config(conf);
-    data.validate_frame(None, ValidateSet::ALL)
-        .expect("failed to validate");
+    let mut data: FRTBDataSet = FRTBDataSet::from_config(conf);
+    data.validate_frame(None, 0).expect("failed to validate");
     data.prepare().expect("Failed to prepare");
     std::sync::Arc::new(data)
 });
 
 #[ignore]
 #[allow(dead_code)]
 pub fn assert_results(req: &str, expected_sum: f64, epsilon: Option<f64>) {
@@ -27,22 +30,22 @@
         agg_req.groupby().clone()
     } else {
         unreachable!()
     };
     //let excl = data_req.groupby().clone();
     let a = LAZY_DASET.as_ref();
     let res = a
-        .compute(data_req, false)
+        .compute(data_req)
         .expect("Error while calculating results");
     let res_numeric = res
         .lazy()
         .select([col("*").exclude(excl)])
         .collect()
         .expect("Could not remove column");
     let res_arr = res_numeric
-        .to_ndarray::<Float64Type>()
+        .to_ndarray::<Float64Type>(IndexOrder::Fortran)
         .expect("Could not convert result to nd_array");
     // Slightly naive, but we assume if the sum is equivallent then the result is accurate
     dbg!(res_arr.sum());
     dbg!(expected_sum);
     assert!((res_arr.sum() - expected_sum).abs() < ep);
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/tests/dependant.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/tests/dependant.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use ultibi::{AggregationRequest, ComputeRequest, DataSet};
 mod common;
 use common::LAZY_DASET;
-use polars::prelude::Float64Type;
+use ultibi::polars::prelude::{Float64Type, IndexOrder};
 
 /// Note in later(post 25.1) versions of polars cannot call max_expr on
 /// an aggregated Expr. See this:
 /// https://github.com/pola-rs/polars/issues/6115
 /// Hence if fails it's ok to drop this test
 #[test]
 fn dependant_sbm() {
@@ -25,19 +25,19 @@
     }"#;
 
     let req_deps = serde_json::from_str::<AggregationRequest>(request_as_dependants)
         .expect("Could not parse request");
 
     let a = &*LAZY_DASET;
     let mut res1 = a
-        .compute(ComputeRequest::Aggregation(req_deps), false)
+        .compute(ComputeRequest::Aggregation(req_deps))
         .expect("Error while calculating dependant results");
     let _ = res1.drop_in_place("Desk").unwrap();
     let sum1 = res1
-        .to_ndarray::<Float64Type>()
+        .to_ndarray::<Float64Type>(IndexOrder::Fortran)
         .expect("Couldn't convert result 1 to ndarray")
         .sum();
 
     // This number is not derived from a Spread Sheet
     // Instead it was derived via measures which were derived from a SS
     let expected = 2267954.452798342;
     assert!((sum1 - expected).abs() < 1e-4);
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/tests/drc.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/tests/drc.rs`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,11 @@
             
     }"#;
     let data_req =
         serde_json::from_str::<AggregationRequest>(request).expect("Could not parse request");
 
     let compute_req = ComputeRequest::Aggregation(data_req);
 
-    let res = common::LAZY_DASET
-        .as_ref()
-        .compute(compute_req, false)
-        .unwrap();
+    let res = common::LAZY_DASET.as_ref().compute(compute_req).unwrap();
 
     assert!(dbg!(res.column("DRC Charge")).is_ok());
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm.rs`

 * *Files 1% similar despite different names*

```diff
@@ -613,14 +613,15 @@
     "calc_params": {"jurisdiction": "BCBS"}
     }"#;
     assert_results(request, expected_res.sum(), None)
 }
 
 #[test]
 /// User sets prepare to true but none of the required columns matches weights assignments
+/// so the weight of this sensi should be [0.0]
 fn add_rows_nothing_to_match_prepare() {
     let expected_res = arr1(&[-250.0]);
     let request = r#"
     {"measures": [
         ["Commodity DeltaSens", "sum"]
             ],
     "groupby": ["Desk"],
```

### Comparing `ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm_totals.rs` & `ultibi-0.4.0/local_dependencies/frtb_engine/tests/sbm_totals.rs`

 * *Files 21% similar despite different names*

```diff
@@ -18,14 +18,11 @@
             
     }"#;
     let data_req =
         serde_json::from_str::<AggregationRequest>(request).expect("Could not parse request");
 
     let compute_req = ComputeRequest::Aggregation(data_req);
 
-    let res = common::LAZY_DASET
-        .as_ref()
-        .compute(compute_req, false)
-        .unwrap();
+    let res = common::LAZY_DASET.as_ref().compute(compute_req).unwrap();
 
     assert!(dbg!(res.column("SA Charge")).is_ok());
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_server/Cargo.toml` & `ultibi-0.4.0/local_dependencies/ultibi_server/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_server"
-version= "0.3.4"
+version= "0.4.0"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
@@ -18,12 +18,12 @@
 tokio = { version = "1.21.0", features = ["full"] }
 tracing = { version = "0.1", features = ["log"] }
 pretty_env_logger = "0.4"
 log = "0.4"
 mime = "0.3"
 actix-web-static-files = "4.0"
 static-files = "0.2.1"
-utoipa = { git="https://github.com/juhaku/utoipa", features = ["actix_extras"] }
-utoipa-swagger-ui = { git="https://github.com/juhaku/utoipa", features = ["actix-web"] }
+utoipa = { version="3.3.0", features = ["actix_extras"] }
+utoipa-swagger-ui = { version="3.1.4", features = ["actix-web"] }
 
 [build-dependencies]
 static-files = "0.2.1"
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_server/src/api/open_api.rs` & `ultibi-0.4.0/local_dependencies/ultibi_server/src/api/open_api.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_server/src/api/routers.rs` & `ultibi-0.4.0/local_dependencies/ultibi_server/src/api/routers.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,20 @@
     web::{self, Data, ServiceConfig},
     HttpRequest, HttpResponse, Responder, Result,
 };
 use anyhow::Context;
 use serde::Deserialize;
 use tokio::task;
 use ultibi_core::{
-    aggregations::BASE_CALCS, polars::lazy::dsl::col, AggregationRequest, ComputeRequest,
-    DataFrame, DataSet, PolarsResult,
+    aggregations::BASE_CALCS, errors::UltiResult, AggregationRequest, ComputeRequest, DataFrame,
+    DataSet,
 };
+use utoipa::IntoParams;
 
-#[derive(Deserialize)]
+#[derive(Deserialize, IntoParams)]
 struct Pagination {
     page: usize,
     pattern: String,
 }
 const PER_PAGE: u16 = 100;
 
 #[get("/health_check")]
@@ -32,26 +33,24 @@
     path: web::Path<String>,
     page: web::Query<Pagination>,
     data: Data<RwLock<dyn DataSet>>,
 ) -> Result<HttpResponse> {
     let column_name = path.into_inner();
     let (page, pat) = (page.page, page.pattern.clone());
     let res = task::spawn_blocking(move || {
-        let lf = data
+        let srs = data
             .read()
             .expect("Poisonned RwLock")
-            .get_lazyframe()
-            .clone();
-        let df = lf.select([col(&column_name)]).collect()?;
-        let srs = df.column(&column_name)?;
-        let search = ultibi_core::helpers::searches::filter_contains_unique(srs, &pat)?;
+            .get_column(&column_name)?;
+
+        let search = ultibi_core::helpers::searches::filter_contains_unique(&srs, &pat)?;
         let first = page * PER_PAGE as usize;
         let last = first + PER_PAGE as usize;
         let s = search.slice(first as i64, last);
-        PolarsResult::Ok(s)
+        UltiResult::Ok(s)
     })
     .await
     .context("Failed to spawn blocking task.")
     .map_err(actix_web::error::ErrorInternalServerError)?;
 
     match res {
         Ok(srs) => Ok(HttpResponse::Ok().json(Vec::from(
@@ -113,26 +112,21 @@
     )
 )]
 #[tracing::instrument(name = "Request Execution", skip(data))]
 #[post("")]
 pub(crate) async fn execute(
     data: Data<RwLock<dyn DataSet>>,
     req: web::Json<ComputeRequest>,
-    streaming: Data<bool>,
 ) -> Result<HttpResponse> {
     let r = req.into_inner();
     // TODO kill this OS thread if it is hanging (see spawn_blocking docs for ideas)
-    let res = task::spawn_blocking(move || {
-        data.read()
-            .expect("Poisonned RwLock")
-            .compute(r, **streaming) //TODO streaming mode
-    })
-    .await
-    .context("Failed to spawn blocking task.")
-    .map_err(actix_web::error::ErrorInternalServerError)?;
+    let res = task::spawn_blocking(move || data.read().expect("Poisonned RwLock").compute(r))
+        .await
+        .context("Failed to spawn blocking task.")
+        .map_err(actix_web::error::ErrorInternalServerError)?;
 
     match res {
         Ok(df) => Ok(HttpResponse::Ok().json(df)),
         Err(e) => {
             tracing::error!("Failed to execute query: {:?}", e);
             Err(actix_web::error::ErrorExpectationFailed(e))
         }
@@ -145,15 +139,15 @@
 }
 #[utoipa::path(get)]
 #[get("/overrides")]
 async fn overridable_columns(data: Data<RwLock<dyn DataSet>>) -> impl Responder {
     web::Json(data.read().expect("Poisonned RwLock").overridable_columns())
 }
 
-pub(crate) fn configure() -> impl FnOnce(&mut ServiceConfig) {
+pub fn configure() -> impl FnOnce(&mut ServiceConfig) {
     |config: &mut ServiceConfig| {
         config.service(
             web::scope("/api")
                 .service(aggtypes)
                 .service(describe)
                 .service(health_check)
                 //TODO change FRTB to DataSet
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_server/src/app.rs` & `ultibi-0.4.0/local_dependencies/ultibi_server/src/app.rs`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 include!(concat!(env!("OUT_DIR"), "/generated.rs"));
 
 use crate::api::{open_api::ApiDoc, routers};
 pub fn build_app(
     listener: TcpListener,
     ds: Arc<RwLock<dyn DataSet>>,
     _templates: Vec<AggregationRequest>,
-    streaming: bool,
 ) -> std::io::Result<Server> {
     let ds = Data::from(ds);
-    let streaming = Data::new(streaming);
+    //let streaming = Data::new(streaming);
     let openapi = ApiDoc::openapi();
 
     let _templates = Data::new(_templates);
 
     let server = HttpServer::new(move || {
         let generated = generate();
 
@@ -34,13 +33,13 @@
             .configure(routers::configure())
             .service(
                 SwaggerUi::new("/swagger-ui/{_:.*}").url("/api-doc/openapi.json", openapi.clone()),
             )
             .service(ResourceFiles::new("/", generated))
             .app_data(ds.clone())
             .app_data(_templates.clone())
-            .app_data(streaming.clone())
+        //.app_data(streaming.clone())
     })
     .listen(listener)?
     .run();
     Ok(server)
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_server/src/helpers.rs` & `ultibi-0.4.0/local_dependencies/ultibi_server/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_server/src/lib.rs` & `ultibi-0.4.0/local_dependencies/ultibi_server/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+#![doc(html_no_source)]
+
 use std::sync::RwLock;
 use std::{net::SocketAddr, sync::Arc};
 
 use std::env;
 use std::net::TcpListener;
 use tokio::runtime::Builder;
 use ultibi_core::DataSet;
 
 use log::info;
 
-mod api;
+pub mod api;
 mod app;
 mod helpers;
 mod visual;
 
 pub use visual::VisualDataSet;
 
 #[allow(unused_must_use)]
-fn run_server(ds: Arc<RwLock<dyn DataSet>>, streaming: bool) {
+fn run_server(ds: Arc<RwLock<dyn DataSet>>) {
     // Read .env
     dotenv::dotenv().ok();
     // Allow pretty logs
     pretty_env_logger::init();
 
     let runtime = Builder::new_multi_thread().enable_all().build().unwrap();
 
@@ -44,11 +46,9 @@
 
     // We retrieve the port assigned to us by the OS
     let port = listener.local_addr().unwrap().port();
     info!("http://localhost:{port}");
     let url = format!("http://localhost:{port}");
     dbg!(url);
 
-    runtime.block_on(
-        crate::app::build_app(listener, ds, vec![], streaming).expect("Failed to bind address"),
-    );
+    runtime.block_on(crate::app::build_app(listener, ds, vec![]).expect("Failed to bind address"));
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/Cargo.toml` & `ultibi-0.4.0/local_dependencies/ultibi_core/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 [package]
 name = "ultibi_core"
-version= "0.3.4"
+version= "0.4.0"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 serde = { version = "1.0", features = ["derive","derive"] }
-polars = { version = "0.28.0", features = [
+polars = { version = "0.31.1", features = [
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
-    "csv-file",
     "diagonal_concat",
     "serde-lazy" 
 ,
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
-    "csv-file",
     "diagonal_concat",
     "describe"] }
 serde_json = "1.0"
 toml = "0.7.2"
 once_cell = "1.12"
 derivative = "2.2"
 thiserror = "*"
 #AWS S3
 aws-config = { version = "0.49.0", optional = true }
 aws-sdk-s3 = { version = "0.19.0", optional = true }
 tokio = { version = "1.21.2", features = ["rt-multi-thread"], optional = true }
 futures = { version = "0.3", optional = true }
 #Cache
-#May be make optional
 dashmap = "5.4.0"
 # Open API Swagger
 quote = "1.0.26" # Needs to be specified for utoipa to build
-utoipa = { git="https://github.com/juhaku/utoipa", optional = true} # TODO change to version
+utoipa = { version="3.3.0", optional = true} # TODO change to version
+# DB
+connectorx = { git = "https://github.com/AnatolyBuga/connector-x.git", branch="polars_dtype_u8", optional = true, features=["dst_arrow2", "src_mysql"]}
+
 
 
 [features]
 default = []
 aws_s3 = ["dep:aws-config", "dep:aws-sdk-s3", "dep:tokio", "dep:futures"]
 openapi = ["dep:utoipa"]
+db = ["dep:connectorx"]
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/add_row.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/aggregations.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/cache.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/datarequest.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/datarequest.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+//! TODO rename to compute request and move to a separate module
+
 use std::collections::BTreeMap;
 
 use crate::aggregations::AggregationName;
 use crate::filters::FilterE;
 use crate::overrides::Override;
 use crate::MeasureName;
 use crate::{add_row::AdditionalRows, filters::AndOrFltrChain};
@@ -17,14 +19,16 @@
 /// Otherwise, ii) Apply the same procedure to every group and get multiple numbers (ie a Breakdown)
 // TODO #[cfg_attr(feature = "openapi", derive(utoipa::ToSchema))]
 #[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Eq, Hash)]
 #[serde(untagged)]
 pub enum ComputeRequest {
     /// Measures will be called in GroupBy-Aggregate context
     Aggregation(AggregationRequest),
+    /// Converted into a Vec<AggregationRequest/Breakdown) to produce a report
+    Report(ReportRequest),
     /// TODO Measures will be called in groupby-Apply Context
     Breakdown,
 }
 
 impl From<AggregationRequest> for ComputeRequest {
     fn from(item: AggregationRequest) -> Self {
         ComputeRequest::Aggregation(item)
@@ -90,14 +94,15 @@
 pub enum CacheableComputeRequest {
     /// Measures will be called in GroupBy-Aggregate context
     Aggregation(CacheableAggregationRequest),
     /// TODO Measures will be called in groupby-Apply Context
     Breakdown,
 }
 
+/// Similar to AggregationRequest, but Measure is only one
 #[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Eq, Hash)]
 #[serde(tag = "type")]
 pub struct CacheableAggregationRequest {
     // general fields
     #[serde(default)]
     pub name: Option<String>,
     /// Measure: (Name, Action) where Name will be looked up in
@@ -130,7 +135,17 @@
                 add_row: item.add_row.clone(),
                 calc_params: item.calc_params.clone(),
                 totals: item.totals,
             })
             .collect::<Vec<CacheableAggregationRequest>>()
     }
 }
+
+#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Eq, Hash)]
+#[serde(tag = "type")]
+pub struct ReportRequest {
+    /// Report Name
+    pub report_name: String,
+    /// This should Deserialise into report specific request
+    /// For example [GroupbyAggReportRequest]
+    pub report_body: String,
+}
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/dataset.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/dataset/mod.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,142 @@
+pub mod datasource;
+pub mod new;
+
 use std::collections::{BTreeMap, HashSet};
 
 use polars::prelude::*;
 use serde::{ser::SerializeMap, Serialize, Serializer};
 
 use crate::cache::{Cache, CacheableDataSet};
-use crate::{derive_basic_measures_vec, execute, Measure, CPM};
-use crate::{CalcParameter, ComputeRequest, DataSourceConfig, MeasuresMap};
+use crate::errors::{UltiResult, UltimaErr};
+use crate::execute;
+use crate::filters::AndOrFltrChain;
+use crate::reports::report::ReportersMap;
+use crate::{CalcParameter, ComputeRequest, MeasuresMap};
+use once_cell::sync::Lazy;
+
+use self::datasource::DataSource;
+pub static EMPTY_REPORTS_MAP: Lazy<ReportersMap> = Lazy::new(Default::default);
 
 /// This is the default struct which implements Dataset
 /// Usually a client/user would overwrite it with their own DataSet
 #[derive(Default)]
 pub struct DataSetBase {
     /// Data
-    pub frame: LazyFrame,
+    pub source: DataSource,
     /// Stores measures map, ie what you want to calculate
     pub measures: MeasuresMap,
-    /// build_params are passed into .prepare() - if streaming or add_row
+    ///Similar to measures, but stores Reports
+    pub reports: ReportersMap,
+    /// build_params can be used in .prepare() - if streaming or add_row
     ///  this happens during the execution. Hence we can't remove and pass to .prepare() directly
-    pub build_params: BTreeMap<String, String>,
+    pub config: BTreeMap<String, String>,
     /// Cache
     pub cache: Cache,
 }
 
 /// The main Trait
 ///
 /// If you have your own DataSet, implement this
 pub trait DataSet: Send + Sync {
     #[cfg(feature = "ui")]
     fn ui(&self) {
         ultibi_server::run_server(self)
     }
-    /// Polars DataFrame clone is cheap:
-    /// https://stackoverflow.com/questions/72320911/how-to-avoid-deep-copy-when-using-groupby-in-polars-rust
-    /// This method gets the main LazyFrame of the Dataset
-    fn get_lazyframe(&self) -> &LazyFrame;
 
-    /// Modify lf in place
-    fn set_lazyframe_inplace(&mut self, lf: LazyFrame);
+    /// Since we support a limited number of data sources, each [DataSet] must contain a source.
+    /// Since many of the [DataSet] methods' logic depends on the variant of the source, we implement those there    
+    fn get_datasource(&self) -> &DataSource;
 
-    /// Get all measures associated with the DataSet
+    /// Get all Measures associated with the DataSet
+    /// TODO by default coauld be numeric columns accessed via [get_lazyframe]
     fn get_measures(&self) -> &MeasuresMap;
 
-    /// See [DataSetBase] and [CalcParameter] for description of the parameters
-    fn new(frame: LazyFrame, mm: MeasuresMap, params: CPM) -> Self
-    where
-        Self: Sized;
-
-    /// Cannot be defined since returns Self which is a Struct.
-    /// Not possible to call [DataSet::new] either since it's not on self
-    fn from_config(conf: DataSourceConfig) -> Self
-    where
-        Self: Sized,
-    {
-        let (frame, measure_cols, bp) = conf.build();
-        let mm: MeasuresMap = MeasuresMap::from_iter(measure_cols);
-        Self::new(frame, mm, bp)
+    /// Clones but clone is cheap
+    /// Polars DataFrame clone is cheap:
+    /// https://stackoverflow.com/questions/72320911/how-to-avoid-deep-copy-when-using-groupby-in-polars-rust
+    /// This method gets the main LazyFrame of the Dataset
+    fn get_lazyframe(&self, filters: &AndOrFltrChain) -> LazyFrame {
+        self.get_datasource().get_lazyframe(filters)
     }
 
-    /// Either place your desired numeric columns and bespokes in
-    /// *ms and set include_numeric_cols_as_measures = False
-    /// or set your bespokes in *ms and include_numeric_cols_as_measures = True
-    /// See [DataSetBase] and [CalcParameter] for description of the parameters
-    fn from_vec(
-        frame: LazyFrame,
-        mut ms: Vec<Measure>,
-        include_numeric_cols_as_measures: bool,
-        params: CPM,
-    ) -> Self
-    where
-        Self: Sized,
-    {
-        if include_numeric_cols_as_measures {
-            let num_cols = frame
-                .schema()
-                .map(numeric_columns)
-                .expect("Failed to obtain numeric columns");
+    /// Get Schema (Column Names and DataTypes) of the underlying Data
+    /// !Default implementation calls `.get_lazyframe(&vec![])`, so if `get_lazyframe` materialises/loads data (eg from DB via a connector)
+    /// Be careful, this might break your app.
+    fn get_schema(&self) -> UltiResult<Arc<Schema>> {
+        self.get_datasource().get_schema()
+    }
 
-            let numeric_cols_as_measures = derive_basic_measures_vec(num_cols);
-            ms.extend(numeric_cols_as_measures);
-        }
+    /// !Default implementation assumes the DataSet is an InMemory DataSet, and has been prepared.
+    /// Therefore by default we don't prepare on each compute request.
+    /// * `streaming` - See polars streaming. Use when your LazyFrame is a Scan if you don't want to load whole frame
+    /// into memory. See: https://www.rhosignal.com/posts/polars-dont-fear-streaming/
+    fn compute(&self, r: ComputeRequest) -> UltiResult<DataFrame> {
+        execute(self, r, self.get_datasource().prepare_on_each_request())
+    }
 
-        let mm: MeasuresMap = MeasuresMap::from_iter(ms);
-        Self::new(frame, mm, params)
+    /// Get a column. Potentially this will be removed in favour of get_columns
+    /// !Default implementation calls `.get_lazyframe(&vec![])`, so if `get_lazyframe` materialises/loads data (eg from DB via a connector)
+    /// Be careful, this might break your app.
+    fn get_column(&self, col_name: &str) -> UltiResult<Series> {
+        self.get_lazyframe(&vec![])
+            .select([col(col_name)])
+            .collect()?
+            .pop() //above select guaranteed one column
+            .ok_or(UltimaErr::Other(format!("Column {col_name} doesn't exist")))
+    }
+
+    /// Get all Reporters associated with the DataSet
+    fn get_reporters(&self) -> &ReportersMap {
+        &EMPTY_REPORTS_MAP
+    }
+
+    /// Modify lf in place - applicable only to InMemory DataSet
+    /// Common use case - prepare, and then set_inplace
+    fn set_lazyframe_inplace(&mut self, _: LazyFrame) -> UltiResult<()> {
+        Err(UltimaErr::Other(
+            "set_lazyframe_inplace is Not implemented for your Data Set".to_string(),
+        ))
     }
 
     /// Collects the (main) LazyFrame of the DataSet
-    fn collect(&mut self) -> PolarsResult<()>
-    where
-        Self: Sized,
-    {
-        let lf = self.get_lazyframe().clone().collect()?.lazy();
-        self.set_lazyframe_inplace(lf);
+    /// Will return an error if [DataSet::set_lazyframe_inplace] is not implemented
+    fn collect(&mut self) -> UltiResult<()> {
+        let lf = self.get_lazyframe(&vec![]).collect()?.lazy();
+        self.set_lazyframe_inplace(lf).map_err(|err| {
+            UltimaErr::Other(format!(
+                "Error calling .collect(), followed by
+            an attempt to set Data inplace: {err}. Does it make sence to collect you Datasource?",
+            ))
+        })?;
         Ok(())
     }
 
-    // These methods could be overwritten.
-
-    /// Clones
-    fn frame(&self) -> PolarsResult<DataFrame> {
-        self.get_lazyframe().clone().collect()
-    }
-
     /// Prepare runs BEFORE any calculations. In eager mode it runs ONCE
     /// Any pre-computations which are common to all queries could go in here.
-    /// Calls [DataSet::prepare_frame] insternally
-    fn prepare(&mut self) -> PolarsResult<()>
-    where
-        Self: Sized,
+    /// Calls [DataSet::prepare_frame]
+    /// Will return an error if [DataSet::set_lazyframe_inplace] is not implemented
+    fn prepare(&mut self) -> UltiResult<()>
+//where
+    //    Self: Sized,
     {
-        let new_frame = self.prepare_frame(None)?;
-        self.set_lazyframe_inplace(new_frame);
+        let new_frame = self.prepare_frame(self.get_lazyframe(&vec![]))?;
+        self.set_lazyframe_inplace(new_frame).map_err(|err| {
+            UltimaErr::Other(format!(
+                "Error calling .prepare(), followed by
+            an attempt to set Data inplace: {err}. Does it make sence to prepare you Datasource? Has your DataSet already been prepared?"
+            ))
+        })?;
         Ok(())
     }
 
     /// By returning a Frame this method can be used on a
     /// *lf - buffer. if None, function "prepares" self.lazy_frame()
-    fn prepare_frame(&self, _lf: Option<LazyFrame>) -> PolarsResult<LazyFrame> {
-        if let Some(lf) = _lf {
-            Ok(lf)
-        } else {
-            Ok(self.get_lazyframe().clone())
-        }
+    fn prepare_frame(&self, lf: LazyFrame) -> UltiResult<LazyFrame> {
+        Ok(lf)
     }
 
     /// Calc params are used for the UI and hence are totally optional
     fn calc_params(&self) -> Vec<CalcParameter> {
         let mut res = vec![];
 
         for measure in self.get_measures().values() {
@@ -134,79 +146,58 @@
         let hash_res: HashSet<CalcParameter> = res.into_iter().collect();
 
         hash_res.into_iter().collect()
     }
 
     /// Limits overridable columns which you can override in
     /// See [AggregationRequest::overrides]
+    /// Good usecase: add prepared
     fn overridable_columns(&self) -> Vec<String> {
-        self.get_lazyframe()
-            .schema()
-            .map(overrides_columns)
+        self.get_schema()
+            .map(overridable_columns)
             .unwrap_or_default()
     }
     /// Validate DataSet
     /// Runs once, making sure all the required columns, their contents, types etc are valid
     /// Should contain an optional flag for analysis(ie displaying statistics of filtered out items, saving those as CSVs)
-    fn validate_frame(&self, _: Option<&LazyFrame>, _: ValidateSet) -> PolarsResult<()> {
+    /// *_validation_set - at different points in the runtime it makes sence to validate different subsets of the data
+    /// eg FRTB validate before or after .prepare(). User can control that through _validation_set param
+    fn validate_frame(&self, _: Option<&LazyFrame>, _validation_set: u8) -> UltiResult<()> {
         Ok(())
     }
 
-    /// * `streaming` - See polars streaming. Use when your LazyFrame is a Scan if you don't want to load whole frame
-    /// into memory. See: https://www.rhosignal.com/posts/polars-dont-fear-streaming/
-    fn compute(&self, r: ComputeRequest, streaming: bool) -> PolarsResult<DataFrame> {
-        execute(self, r, streaming)
-    }
-
     /// Indicates if your DataSet has a cache or not
     /// It is recommended that you implement CacheableDataSet
     /// make sure to return Some(&self)
     fn as_cacheable(&self) -> Option<&dyn CacheableDataSet> {
         None
     }
 }
 
 impl DataSet for DataSetBase {
     /// Polars DataFrame clone is cheap:
     /// https://stackoverflow.com/questions/72320911/how-to-avoid-deep-copy-when-using-groupby-in-polars-rust
-    fn get_lazyframe(&self) -> &LazyFrame {
-        &self.frame
+    fn get_datasource(&self) -> &DataSource {
+        &self.source
     }
-    /// Modify lf in place
-    fn set_lazyframe_inplace(&mut self, lf: LazyFrame) {
-        self.frame = lf;
+
+    /// Modify lf in place - applicable only to InMemory DataSource
+    fn set_lazyframe_inplace(&mut self, lf: LazyFrame) -> UltiResult<()> {
+        if let DataSource::InMemory(_) = self.source {
+            self.source = DataSource::InMemory(lf.collect()?)
+        } else {
+            return Err(UltimaErr::Other("Can't set data inplace with this Source. Currently can only set In Memory Dataframe".to_string()));
+        }
+        Ok(())
     }
 
     fn get_measures(&self) -> &MeasuresMap {
         &self.measures
     }
 
-    //fn new(frame: LazyFrame, mm: MeasuresMap, build_params: BTreeMap<String, String>) -> Self {
-    //    Self {
-    //        frame,
-    //        measures: mm,
-    //        build_params,
-    //        ..Default::default()
-    //    }
-    //}
-
-    fn new(frame: LazyFrame, mm: MeasuresMap, build_params: CPM) -> Self {
-        Self {
-            frame,
-            measures: mm,
-            build_params,
-            ..Default::default()
-        }
-    }
-
-    //fn collect(self) -> PolarsResult<Self> {
-    //    let lf = self.frame.collect()?.lazy();
-    //    Ok(Self { frame: lf, ..self })
-    //}
-
     //    /// Validate Dataset contains columns
     //    /// files_join_attributes and attributes_join_hierarchy
     //    /// numeric_cols and TODO dimensions(groups and filters)
     //    /// !only! numeric_col can be a measure
     //    ///  and therefore <numeric_col> should be only one across DataSet
     //    /// see how to validate dtype:
     //    /// https://stackoverflow.com/questions/72372821/how-to-apply-a-function-to-multiple-columns-of-a-polars-dataframe-in-rust
@@ -245,15 +236,15 @@
             )
         })
         .map(|field| field.name.to_string())
         .collect::<Vec<String>>()
 }
 
 /// DataTypes supported for overrides are defined in [overrides::string_to_lit]
-pub(crate) fn overrides_columns(schema: Arc<Schema>) -> Vec<String> {
+pub fn overridable_columns(schema: Arc<Schema>) -> Vec<String> {
     schema
         .iter_fields()
         .filter(|c| match c.data_type() {
             DataType::Utf8 | DataType::Boolean | DataType::Float64 => true,
             DataType::List(x) => {
                 matches!(x.as_ref(), DataType::Float64)
             }
@@ -264,34 +255,26 @@
 }
 
 impl Serialize for dyn DataSet {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
+        // For measures we are only interested in their agg method
         let measures = self
             .get_measures()
             .iter()
             .map(|(x, m)| (x, m.aggregation()))
             .collect::<BTreeMap<&String, &Option<String>>>();
-
         let ordered_measures: BTreeMap<_, _> = measures.iter().collect();
-        let utf8_cols = self
-            .get_lazyframe()
-            .schema()
-            .map(fields_columns)
-            .unwrap_or_default();
+
+        let utf8_cols = self.get_schema().map(fields_columns).unwrap_or_default();
         let calc_params = self.calc_params();
 
         let mut seq = serializer.serialize_map(Some(4))?;
 
         seq.serialize_entry("fields", &utf8_cols)?;
         seq.serialize_entry("measures", &ordered_measures)?;
         seq.serialize_entry("calc_params", &calc_params)?;
         seq.end()
     }
 }
-
-pub enum ValidateSet {
-    ALL,
-    SUBSET1,
-}
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/awss3.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/io/awss3.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/helpers.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/io/helpers.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-use std::collections::BTreeMap;
+use std::{collections::BTreeMap, time::Instant};
 
 use polars::{
     prelude::{
-        col, concat, DataFrame, DataType, Expr, Field, JoinType, LazyCsvReader, LazyFileListReader,
-        LazyFrame, Literal, NamedFrom, PolarsResult, Schema, NULL,
+        col, DataFrame, DataType, Expr, Field, JoinType, LazyCsvReader, LazyFileListReader,
+        LazyFrame, NamedFrom, Schema,
     },
     series::Series,
 };
 
-use crate::{derive_basic_measures_vec, numeric_columns, Measure};
+use crate::{
+    datasource::{DataSource, SourceVariant},
+    derive_basic_measures_vec, numeric_columns, Measure,
+};
 
 /// creates an empty frame with columns
 pub fn empty_frame(with_columns: &[String]) -> DataFrame {
     let mut x: Vec<Series> = Vec::with_capacity(with_columns.len());
     let y: [String; 0] = [];
     for c in with_columns {
         x.push(Series::new(c, &y));
@@ -49,27 +52,28 @@
     a2h: Vec<String>,
     f2a: Vec<String>,
     measures: Vec<String>,
     mut df_attr: LazyFrame,
     df_hms: LazyFrame,
     mut concatinated_frame: LazyFrame,
     build_params: BTreeMap<String, String>,
-) -> (LazyFrame, Vec<Measure>, BTreeMap<String, String>) {
+    source_type: SourceVariant,
+) -> (DataSource, Vec<Measure>, BTreeMap<String, String>) {
     // join with hms if a2h was provided
     if !a2h.is_empty() {
         let a2h_expr = a2h.iter().map(|c| col(c)).collect::<Vec<Expr>>();
-        df_attr = df_attr.join(df_hms, a2h_expr.clone(), a2h_expr, JoinType::Left)
+        df_attr = df_attr.join(df_hms, a2h_expr.clone(), a2h_expr, JoinType::Left.into())
         //.collect()
         //.expect("Could not join attributes to hms. Review attributes_join_hierarchy field in the setup");
     }
     // if files to attributes was provided
     if !f2a.is_empty() {
         let f2a_expr = f2a.iter().map(|c| col(c)).collect::<Vec<Expr>>();
         concatinated_frame =
-            concatinated_frame.join(df_attr, f2a_expr.clone(), f2a_expr, JoinType::Outer)
+            concatinated_frame.join(df_attr, f2a_expr.clone(), f2a_expr, JoinType::Outer.into())
         //.collect()
         //.expect("Could not join files with attributes-hms. Review files_join_attributes field in the setup");
     }
 
     // if measures were provided
     let measures = if !measures.is_empty() {
         let schema = concatinated_frame
@@ -85,75 +89,89 @@
             if !fields.contains(col) {
                 panic!("Measure: {col}, is not part of the fields: {fields:?}",)
             }
         });
         derive_basic_measures_vec(measures)
     }
     // If not provided return all numeric columns
-    // TODO move inside the DataSet see FRTBDataSetWrapper::new
     else {
         let num_cols = concatinated_frame
             .schema()
             .map(numeric_columns)
             .expect("Check numeric columns in the config");
         derive_basic_measures_vec(num_cols)
     };
 
-    (concatinated_frame, measures, build_params)
-}
-
-/// TODO contribute to Polars
-/// Concat [LazyFrame]s diagonally.
-/// Calls [concat] internally.
-pub fn diag_concat_lf<L: AsRef<[LazyFrame]>>(
-    lfs: L,
-    rechunk: bool,
-    parallel: bool,
-) -> PolarsResult<LazyFrame> {
-    let lfs = lfs.as_ref().to_vec();
-    let schemas = lfs
-        .iter()
-        .map(|lf| lf.schema())
-        .collect::<PolarsResult<Vec<_>>>()?;
-
-    let upper_bound_width = schemas.iter().map(|sch| sch.len()).sum();
-
-    // Use Vec to preserve order
-    let mut column_names = Vec::with_capacity(upper_bound_width);
-    let mut total_schema = Vec::with_capacity(upper_bound_width);
-
-    for sch in schemas.iter() {
-        sch.iter().for_each(|(name, dtype)| {
-            if !column_names.contains(name) {
-                column_names.push(name.clone());
-                total_schema.push((name.clone(), dtype.clone()));
-            }
-        });
-    }
+    #[allow(unreachable_patterns)]
+    let source = match source_type {
+        SourceVariant::InMemory => {
+            let now = Instant::now();
+            let df = concatinated_frame
+                .collect()
+                .expect("Failed to read frame from config");
+            println!("Time to Read/Aggregate DF: {:.6?}", now.elapsed());
+            DataSource::InMemory(df)
+        }
+        SourceVariant::Scan => DataSource::Scan(concatinated_frame),
+        // only InMemory or Scan is supported for DataSourceConfig::CSV
+        _ => panic!("only InMemory or Scan for CSV Config"),
+    };
 
-    //Append column if missing
-    let lfs_with_all_columns = lfs
-        .into_iter()
-        // Zip Frames with their Schemas
-        .zip(schemas.into_iter())
-        .map(|(mut lf, lf_schema)| {
-            for (name, dtype) in total_schema.iter() {
-                // If a name from Total Schema is not present - append
-                if lf_schema.get_field(name).is_none() {
-                    lf = lf.with_column(NULL.lit().cast(dtype.clone()).alias(name))
-                }
-            }
+    (source, measures, build_params)
+}
 
-            // Now, reorder to match schema
-            let reordered_lf = lf.select(
-                column_names
-                    .iter()
-                    .map(|col_name| col(col_name))
-                    .collect::<Vec<Expr>>(),
-            );
-
-            Ok(reordered_lf)
-        })
-        .collect::<PolarsResult<Vec<_>>>()?;
+// /// TODO contribute to Polars
+// /// Concat [LazyFrame]s diagonally.
+// /// Calls [concat] internally.
+// pub fn diag_concat_lf<L: AsRef<[LazyFrame]>>(
+//     lfs: L,
+//     rechunk: bool,
+//     parallel: bool,
+// ) -> PolarsResult<LazyFrame> {
+//     let lfs = lfs.as_ref().to_vec();
+//     let schemas = lfs
+//         .iter()
+//         .map(|lf| lf.schema())
+//         .collect::<PolarsResult<Vec<_>>>()?;
+
+//     let upper_bound_width = schemas.iter().map(|sch| sch.len()).sum();
+
+//     // Use Vec to preserve order
+//     let mut column_names = Vec::with_capacity(upper_bound_width);
+//     let mut total_schema = Vec::with_capacity(upper_bound_width);
+
+//     for sch in schemas.iter() {
+//         sch.iter().for_each(|(name, dtype)| {
+//             if !column_names.contains(name) {
+//                 column_names.push(name.clone());
+//                 total_schema.push((name.clone(), dtype.clone()));
+//             }
+//         });
+//     }
+
+//     //Append column if missing
+//     let lfs_with_all_columns = lfs
+//         .into_iter()
+//         // Zip Frames with their Schemas
+//         .zip(schemas.into_iter())
+//         .map(|(mut lf, lf_schema)| {
+//             for (name, dtype) in total_schema.iter() {
+//                 // If a name from Total Schema is not present - append
+//                 if lf_schema.get_field(name).is_none() {
+//                     lf = lf.with_column(NULL.lit().cast(dtype.clone()).alias(name))
+//                 }
+//             }
+
+//             // Now, reorder to match schema
+//             let reordered_lf = lf.select(
+//                 column_names
+//                     .iter()
+//                     .map(|col_name| col(col_name))
+//                     .collect::<Vec<Expr>>(),
+//             );
+
+//             Ok(reordered_lf)
+//         })
+//         .collect::<PolarsResult<Vec<_>>>()?;
 
-    concat(lfs_with_all_columns, rechunk, parallel)
-}
+//     concat(lfs_with_all_columns, rechunk, parallel)
+// }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/mod.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/io/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-use std::{collections::BTreeMap, path::PathBuf};
+//! Ultibi IO operations
+//! This potentially will be moved to a separate crate
+
+pub mod acquire;
+pub mod helpers;
+
+#[cfg(feature = "aws_s3")]
+pub mod awss3;
 
-//use log::error;
 #[cfg(feature = "aws_s3")]
 use polars::functions::diag_concat_df;
+
 use polars::prelude::*;
 use serde::{Deserialize, Serialize};
+use std::collections::BTreeMap;
 
-use crate::Measure;
-pub mod acquire;
-pub mod helpers;
+use crate::{
+    datasource::{DataSource, SourceVariant},
+    Measure,
+};
 use helpers::{empty_frame, finish, path_to_lf};
 
-use self::helpers::diag_concat_lf;
-
-#[cfg(feature = "aws_s3")]
-pub mod awss3;
-
 /// reads setup.toml
 /// # Panics
 /// When path or file is invalid
 pub fn read_toml2<T>(path: &str) -> std::result::Result<T, Box<dyn std::error::Error>>
 where
     T: serde::de::DeserializeOwned,
 {
@@ -29,14 +33,16 @@
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 #[serde(tag = "type")]
 #[non_exhaustive]
 pub enum DataSourceConfig {
     CSV {
+        #[serde(default)]
+        source_type: SourceVariant,
         #[serde(default, rename = "files")]
         file_paths: Vec<String>,
         #[serde(default, rename = "attributes_path")]
         attr: Option<String>,
         #[serde(default, rename = "hierarchy_path")]
         hms: Option<String>,
         #[serde(default)]
@@ -80,26 +86,27 @@
 
 impl DataSourceConfig {
     /// build's DataSet
     ///
     /// Returns:
     ///
     /// (joined concatinated DataFrame, vec of base measures, build params)
-    pub fn build(self) -> (LazyFrame, Vec<Measure>, BTreeMap<String, String>) {
+    pub fn build(self) -> (DataSource, Vec<Measure>, BTreeMap<String, String>) {
         match self {
             DataSourceConfig::CSV {
                 file_paths: files,
                 attr: ta,
                 hms,
                 files_join_attributes: f2a,
                 attributes_join_hierarchy: a2h,
                 measures,
                 f1_cast_to_str: mut str_cols,
                 f1_numeric_cols: f64_cols,
                 build_params,
+                source_type,
             } => {
                 for s in f2a.iter() {
                     if !str_cols.contains(s) {
                         str_cols.push(s.to_string())
                     }
                 }
 
@@ -136,14 +143,15 @@
                     a2h,
                     f2a,
                     measures,
                     df_attr,
                     df_hms,
                     concatinated_frame,
                     build_params,
+                    source_type,
                 )
             }
             #[cfg(feature = "aws_s3")]
             DataSourceConfig::AwsCSV {
                 bucket,
                 file_paths: files,
                 attr: ta,
@@ -189,34 +197,14 @@
                     a2h,
                     f2a,
                     measures,
                     df_attr.lazy(),
                     df_hms.lazy(),
                     concatinated_frame.lazy(),
                     build_params,
+                    // Currently AWS doesn't support Scan
+                    SourceVariant::InMemory,
                 )
             }
         }
     }
-
-    /// Checks relative path, if file not exists then tries to find file by abs path.
-    /// Panics if failed.
-    pub fn change_path_on_abs_if_not_exist(&mut self, path_to_file_location: &str) {
-        match self {
-            DataSourceConfig::CSV { file_paths, .. } => {
-                file_paths.iter_mut().for_each(|path_str| {
-                    if !PathBuf::from(&path_str).exists() {
-                        let mut new_path_str = String::from(path_to_file_location);
-                        new_path_str.push_str(path_str);
-                        std::mem::swap(path_str, &mut new_path_str);
-
-                        if !PathBuf::from(&path_str).exists() {
-                            panic!("Non existend path: {path_str}");
-                        }
-                    }
-                });
-            }
-            #[cfg(feature = "aws_s3")]
-            _ => panic!("Only allowed for CSV data source"),
-        }
-    }
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/errors.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 //! Main logic of execution in aggregate context
 
 use std::collections::{HashMap, HashSet};
 
-use polars::prelude::PolarsError;
+use polars::prelude::{diag_concat_lf, PolarsError};
 pub use polars::{
     functions::diag_concat_df,
     prelude::{col, lit, DataFrame, Expr, IntoLazy, Literal, PolarsResult, NULL},
 };
 
 use crate::{
     add_row::{df_from_maps_and_schema, AdditionalRows},
     agg_measure_lookup, agg_measure_to_expr,
     aggregations::{Aggregation, AggregationName, BASE_CALCS},
+    errors::UltiResult,
     execute_agg_with_cache::_exec_agg_with_cache,
-    filters::{fltr_chain, AndOrFltrChain},
+    filters::AndOrFltrChain,
     lookup_dependants_with_depth,
     overrides::Override,
-    prelude::helpers::diag_concat_lf,
     AggregationRequest, DataSet, Measure, MeasureName, ProcessedBaseMeasure, ProcessedMeasure,
-    ValidateSet,
 };
 
 /// Looks up measures and calls calculator on those returning an Expr
 /// Breaks down requested measures into Basic and Dependents
 /// Sends Basics to [ultibi::_exec_agg_with_cache] or [ultibi::_exec_agg_base]
 /// Executes Dependents in .with_columns() context
 pub fn exec_agg<DS: DataSet + ?Sized>(
     data: &DS,
     req: AggregationRequest,
-    streaming: bool,
-) -> PolarsResult<DataFrame> {
+    prepare: bool,
+) -> UltiResult<DataFrame> {
     // Step 0: Lookup and return Expr
     let all_requested_measures = req.measures();
     if all_requested_measures.is_empty() {
         return Err(PolarsError::InvalidOperation(
             "Select measures. What do you want to aggregate?".into(),
-        ));
+        )
+        .into());
     }
 
     let op = req.calc_params(); // Optional params of the request
 
     let dataset_measure_map = data.get_measures(); // all availiable measures
 
     // Step 1.0 Lookup requested measures in the DataSet
@@ -100,24 +100,24 @@
         if let (measure_name, aggregation_name, ProcessedMeasure::Base(pbm)) = m {
             base_measures.push((measure_name, aggregation_name, pbm))
         }
     }
 
     // Step 2 Compute basics
     let mut res = match data.as_cacheable() {
-        Some(cacheable) => _exec_agg_with_cache(cacheable, req.clone(), base_measures, streaming),
+        Some(cacheable) => _exec_agg_with_cache(cacheable, req.clone(), base_measures, prepare),
         _ => _exec_agg_base(
             data,
             req.filters(),
             &req.add_row,
             &req.overrides,
             &req.groupby,
             req.totals,
             base_measures.into_iter().map(|(_, _, pbm)| pbm).collect(),
-            streaming,
+            prepare,
         ),
     }?;
 
     // Step 3 compute dependants
     for i in processed_dependants.into_iter() {
         res = res.lazy().with_columns(i).collect()?
     }
@@ -160,31 +160,24 @@
     Ok(res)
 }
 
 /// main function which returns a Result of the calculation
 /// Executes base measures on your DataSet
 pub(crate) fn _exec_agg_base<DS: DataSet + ?Sized>(
     data: &DS,
-    //req: AggregationRequest,
     filters: &AndOrFltrChain,
     add_rows: &AdditionalRows,
     overrides: &[Override],
     groupby: &[String],
     totals: bool,
     processed_base_measures: Vec<ProcessedBaseMeasure>,
-    streaming: bool,
-) -> PolarsResult<DataFrame> {
-    // Step 0.1 - get existing frame - first building block
-    let mut f1 = data.get_lazyframe().clone();
-
-    // Step 1.0 Applying FILTERS:
-    // TODO check if column is present in DF - (is this "second line of defence" even needed?)
-    if let Some(f) = fltr_chain(filters) {
-        f1 = f1.filter(f)
-    }
+    prepare: bool,
+) -> UltiResult<DataFrame> {
+    // Step 1.0 and 1.1 - get existing Filtered frame - first building block
+    let mut f1 = data.get_lazyframe(filters);
 
     // Step 2.1
     // Unpack - (New Column Name, AggExpr, MeasureSpecificFilter)
     let (_, (aggregateions, fltrs)): (Vec<String>, (Vec<Expr>, Vec<Option<Expr>>)) =
         processed_base_measures
             .into_iter()
             .map(|m| (m.name, (m.calculator, m.precomputefilter)))
@@ -211,48 +204,54 @@
 
     // Step 2.3 Applying (Mesure)FILTER
     if let Some(fltr) = measure_filter_opt {
         f1 = f1.filter(fltr)
     }
 
     // If streaming then prepare (assign weights) NOW (ie post filtering)
-    if streaming {
-        f1 = data.prepare_frame(Some(f1))?
+    if prepare {
+        f1 = data.prepare_frame(f1)?
     }
 
     // Step 2.4 Applying Overwrites
     for ow in overrides {
         f1 = ow.lf_with_overwrite(f1)?
     }
 
     // Step 2.5 Add Row
     if !add_rows.rows.is_empty() {
         let current_schema = f1.schema()?;
         let mut extra_frame = df_from_maps_and_schema(&add_rows.rows, current_schema)?.lazy();
 
         if add_rows.prepare {
             // Validating only a subset required for prepare()
-            data.validate_frame(Some(&extra_frame), ValidateSet::SUBSET1)?;
-            extra_frame = data.prepare_frame(Some(extra_frame))?;
+            data.validate_frame(Some(&extra_frame), 1)?;
+            extra_frame = data.prepare_frame(extra_frame)?;
+            // Collect now to reduce pressure on the logical plan
+            // Totally Fine since extra_frame is always relatively small
+            extra_frame = extra_frame.collect()?.lazy();
         }
         f1 = diag_concat_lf([f1, extra_frame], true, true)?;
     }
 
-    //dbg!(f1.clone().select([col("TradeId"), col("RiskClass"), col("RiskFactor"),col("BucketBCBS"), col("SensWeightsCRR2"), col("SensWeights")]).collect());
+    //dbg!(f1.clone().select([col("TradeId"), col("Desk"), col("RiskFactor"),col("BucketBCBS"), col("SensWeightsCRR2"), col("SensWeights")]).collect());
     //dbg!(f1.clone().select([col("*")]).collect());
+    //dbg!(&groupby);
 
     // Step 3.1 Build GROUPBY
     let groups: Vec<Expr> = groupby.iter().map(|x| col(x)).collect();
     // fill nulls with a "null" - needed for better totals views
     let groups_fill_nulls: Vec<Expr> = groups
         .clone()
         .into_iter()
         .map(|e| e.fill_null(lit(" ")))
         .collect();
 
+    //let f1 = f1.collect()?.lazy();
+
     // Step 3.2 Apply GroupBy and Agg
     // Note .limit doesn't work with standard groupby on large frames
     // hence use groupby_stable
     let mut aggregated_df = f1
         .clone()
         .with_streaming(true) // Set streaming to True anyway - no performance penalty
         .groupby_stable(&groups)
@@ -293,15 +292,15 @@
             .clone()
             .into_iter()
             .map(|e| e.fill_null(lit("Total")))
             .collect();
 
         aggregated_df = aggregated_df
             .lazy()
-            .sort_by_exprs(&groups, vec![false; groups.len()], false)
+            .sort_by_exprs(&groups, vec![false; groups.len()], false, true)
             .select(ordered_cols.iter().map(|c| col(c)).collect::<Vec<Expr>>())
             .with_columns(groups_totals)
             .collect()?;
     }
 
     Ok(aggregated_df)
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-use polars::prelude::{col, DataFrame, Expr, IntoLazy, JoinType, PolarsResult};
+use polars::prelude::{col, DataFrame, Expr, IntoLazy, JoinType};
 
 use crate::cache::CacheableDataSet;
+use crate::errors::UltiResult;
 use crate::{
     AggregationRequest, CacheableAggregationRequest, CacheableComputeRequest, ProcessedBaseMeasure,
 };
 
 /// TODO work in progress
 /// Looks up from Cache
 /// Whatever is not found is sent to [_exec_agg]
 /// Whatever was sent to [_exec_agg] is then saved to Cache
 /// Then results are joined
 pub(crate) fn _exec_agg_with_cache<DS: CacheableDataSet + ?Sized>(
     data: &DS,
     req: AggregationRequest,
     processed_base_measures: Vec<(&String, &String, ProcessedBaseMeasure)>,
     streaming: bool,
-) -> PolarsResult<DataFrame> {
+) -> UltiResult<DataFrame> {
     let requested_groupby = req.groupby().clone();
     let grp_by_expr = req.groupby().iter().map(|x| col(x)).collect::<Vec<Expr>>();
 
     // have already been calculated
     let mut cached_results = vec![];
     // Need to be calculated
     let mut yet_to_calculate = vec![];
@@ -57,15 +58,15 @@
         for df in it {
             res = res
                 .lazy()
                 .join(
                     df.lazy(),
                     grp_by_expr.clone(),
                     grp_by_expr.clone(),
-                    JoinType::Outer,
+                    JoinType::Outer.into(),
                 )
                 .collect()?
         }
         Some(res)
     } else {
         None
     };
@@ -111,20 +112,20 @@
         Some(new_res)
     } else {
         None
     };
 
     // Finally join cached and new if needed and return
     match (_chached_df, _new_res) {
-        (Some(cached), Some(new)) => cached
+        (Some(cached), Some(new)) => Ok(cached
             .lazy()
             .join(
                 new.lazy(),
                 grp_by_expr.clone(),
                 grp_by_expr,
-                JoinType::Outer,
+                JoinType::Outer.into(),
             )
-            .collect(),
+            .collect()?),
         (None, Some(df)) | (Some(df), None) => Ok(df),
         _ => unreachable!(),
     }
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/filters.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/helpers/searches.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/helpers/searches.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-use polars::{
-    prelude::{PolarsResult, Utf8NameSpaceImpl},
-    series::Series,
-};
+use polars::{prelude::Utf8NameSpaceImpl, series::Series};
+
+use crate::errors::{UltiResult, UltimaErr};
 
 /// Helper function - used for search within a column
 /// Filters Series by `pat`
 /// Returns unique values
 /// TODO cache function
-pub fn filter_contains_unique(srs: &Series, pat: &str) -> PolarsResult<Series> {
+pub fn filter_contains_unique(srs: &Series, pat: &str) -> UltiResult<Series> {
     let mask = srs
         .utf8()?
         .to_lowercase()
         .contains(pat.to_lowercase().as_str(), false)?;
     let filtered = srs.filter(&mask)?;
     // Stable in order to preserve the order for pagination
-    filtered.unique_stable()
+    filtered.unique_stable().map_err(UltimaErr::Polars)
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/src/measure.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/src/measure.rs`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 use std::{collections::BTreeMap, sync::Arc};
 
 use crate::{
     aggregations::{Aggregation, AggregationName},
     CPM,
 };
 
-//pub type OCPM = BTreeMap<String, String>;
-
 /// Each [DataSet] has measures accessed via get_measures()
 /// This alias to represent a measure name, a unique string
 pub type MeasureName = String;
 
 /// (Measure Name, Measure)
 pub type MeasuresMap = BTreeMap<MeasureName, Measure>;
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/add_row.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/add_row.rs`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                             "groupby": ["State"],
                             "filters": [[{"op": "Eq", "field": "State", "value": "NY"}]],
                             "add_row": {"prepare": true, "rows": [{"State": "NY", "Balance": "10"}, {"State": "NY", "Balance": "10"}]}}"#;
         let data_req =
             serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
         let res = common::TEST_DASET
             .as_ref()
-            .compute(data_req, false)
+            .compute(data_req)
             .expect("Calculation failed");
 
         let res_sum = dbg!(res)
             .column("Balance_sum")
             .expect("Couldn't get column Balance_sum")
             .sum::<f64>()
             .expect("Couldn't sum");
@@ -34,15 +34,15 @@
                             "filters": [[{"op": "Eq", "field": "State", "value": "NY"}]],
                             "add_row": {"prepare": true, "rows": [{"State": "NY", "Balance": "10"}, {"State": "NY", "Age": "29"}]}}"#;
         let data_req =
             serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
 
         let res = common::TEST_DASET
             .as_ref()
-            .compute(data_req, false)
+            .compute(data_req)
             .expect("Calculation failed");
 
         let res_sum = dbg!(res)
             .column("Balance_sum")
             .expect("Couldn't get column Balance_sum")
             .sum::<f64>()
             .expect("Couldn't sum");
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/agg_request.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/agg_request.rs`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         ["Balance", "sum"]
             ],
     "groupby": ["State"],
     "filters": [[{"op": "Eq", "field": "State", "value": "NY"}]]         
     }"#;
     let data_req = serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
     let a = (*common::TEST_DASET).as_ref();
-    let res = a.compute(data_req, false).expect("Calculation failed");
+    let res = a.compute(data_req).expect("Calculation failed");
 
     let res_sum = res
         .column("Balance_sum")
         .expect("Couldn't get column Balance_sum")
         .sum::<f64>()
         .expect("Couldn't sum");
     assert_eq!(res_sum, 25.0)
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/aggregations.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/aggregations.rs`

 * *Files 19% similar despite different names*

```diff
@@ -11,18 +11,15 @@
         ["Balance", "sum"]
             ],
     "groupby": ["State"],
     "filters": [[{"op": "Eq", "field": "State", "value": "NY"}]]         
     }"#;
     let data_req = serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
 
-    let res = common::TEST_DASET
-        .as_ref()
-        .compute(data_req, false)
-        .unwrap();
+    let res = common::TEST_DASET.as_ref().compute(data_req).unwrap();
 
     let expected = df!(
         "State" => ["NY"],
         "Balance_sum" => [25.0]
     )
     .unwrap();
 
@@ -38,18 +35,15 @@
             ],
     "groupby": ["State"],
     "filters": []         
     }"#;
 
     let data_req = serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
 
-    common::TEST_DASET
-        .as_ref()
-        .compute(data_req, false)
-        .unwrap();
+    common::TEST_DASET.as_ref().compute(data_req).unwrap();
 }
 
 #[test]
 #[should_panic(expected = "No action NoSuchAction")]
 fn non_existent_action() {
     let req = r#"
     {"measures": [
@@ -57,12 +51,9 @@
             ],
     "groupby": ["State"],
     "filters": []         
     }"#;
 
     let data_req = serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
 
-    common::TEST_DASET
-        .as_ref()
-        .compute(data_req, false)
-        .unwrap();
+    common::TEST_DASET.as_ref().compute(data_req).unwrap();
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/common/mod.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/common/mod.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use std::{env, path::PathBuf};
 
 use once_cell::sync::Lazy;
 use polars::prelude::*;
 
 use ultibi_core::{
+    datasource::DataSource,
+    new::NewSourcedDataSet,
     prelude::{read_toml2, DataSet, DataSetBase, DataSourceConfig},
     DependantMeasure, Measure, CPM,
 };
 
 #[allow(dead_code)] // Not dead code actually, but clippy complains
 pub static TEST_DASET: Lazy<Arc<DataSetBase>> = Lazy::new(|| {
     let path: PathBuf = [
@@ -17,15 +19,16 @@
         "test_config.toml",
     ]
     .iter()
     .collect();
     let conf = read_toml2::<DataSourceConfig>(path.to_str().unwrap())
         .expect("Can not proceed without valid Data Set Up"); //Unrecovarable error
 
-    let mut data: DataSetBase = DataSet::from_config(conf);
+    let mut data: DataSetBase = DataSetBase::from_config(conf);
+
     data.prepare().unwrap();
     Arc::new(data)
 });
 
 #[allow(dead_code)] // Not dead code actually, but clippy complains
 pub static TEST_DASET_WITH_DEPENDANTS: Lazy<Arc<DataSetBase>> = Lazy::new(|| {
     let path: PathBuf = [env!("CARGO_MANIFEST_DIR"), "tests", "data", "testset.csv"]
@@ -52,12 +55,18 @@
             }),
             depends_upon: vec![("NoSuchMeasure".to_string(), "sum".to_string())],
             calc_params: vec![],
         }
         .into(),
     ];
 
-    let mut data: DataSetBase = DataSet::from_vec(df, measures, true, Default::default());
+    let data: DataSetBase = DataSetBase::from_vec(
+        DataSource::Scan(df),
+        measures,
+        true,
+        vec![],
+        Default::default(),
+    );
 
-    data.prepare().unwrap();
+    // Not preparing here, since scan
     Arc::new(data)
 });
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/bad_config2.toml` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/data/bad_config2.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/datasource.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/datasource.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::path::PathBuf;
 
-use ultibi_core::{read_toml2, DataSet, DataSetBase, DataSourceConfig};
+use ultibi_core::{new::NewSourcedDataSet, read_toml2, DataSetBase, DataSourceConfig};
 
 #[test]
 fn toml2config() {
     let path = String::from(env!("CARGO_MANIFEST_DIR"));
     let conf_path = path + "/tests/data/bad_config.toml";
     read_toml2::<DataSourceConfig>(conf_path.as_str()).unwrap();
 }
@@ -13,15 +13,15 @@
 #[should_panic(expected = "Error reading file")]
 fn config_build() {
     let mut path = PathBuf::from(env!("CARGO_MANIFEST_DIR"));
     path.extend(["tests", "data", "bad_config.toml"]);
 
     let conf = read_toml2::<DataSourceConfig>(path.to_str().unwrap())
         .expect("Can not proceed without valid Data Set Up");
-    let _data: DataSetBase = DataSet::from_config(conf);
+    let _data: DataSetBase = DataSetBase::from_config(conf);
 }
 
 /// In this config, files_join_attributes was provided but no such column is present
 #[test]
 #[should_panic(expected = "Check numeric columns in the config")]
 fn config_build2() {
     let mut path = PathBuf::from(env!("CARGO_MANIFEST_DIR"));
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/dependants.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/dependants.rs`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     let data_req =
         serde_json::from_str::<AggregationRequest>(req).expect("Could not parse request");
     let compute_req = ComputeRequest::Aggregation(data_req);
 
     let res = common::TEST_DASET_WITH_DEPENDANTS
         .as_ref()
-        .compute(compute_req, false)
+        .compute(compute_req)
         .unwrap();
 
     let res_sum = res
         .column("DivAge")
         .expect("Couldn't get column Dalance_sum")
         .sum::<f64>()
         .expect("Couldn't sum");
@@ -74,15 +74,15 @@
 
     let data_req =
         serde_json::from_str::<AggregationRequest>(req).expect("Could not parse request");
     let compute_req = ComputeRequest::Aggregation(data_req);
 
     let res = common::TEST_DASET_WITH_DEPENDANTS
         .as_ref()
-        .compute(compute_req, false)
+        .compute(compute_req)
         .unwrap();
 
     let res_sum = res
         .column("DivAge")
         .expect("Couldn't get column Dalance_sum")
         .sum::<f64>()
         .expect("Couldn't sum");
@@ -103,10 +103,10 @@
 
     let data_req =
         serde_json::from_str::<AggregationRequest>(req).expect("Could not parse request");
     let compute_req = ComputeRequest::Aggregation(data_req);
 
     let _ = common::TEST_DASET_WITH_DEPENDANTS
         .as_ref()
-        .compute(compute_req, false)
+        .compute(compute_req)
         .unwrap();
 }
```

### Comparing `ultibi-0.3.4/local_dependencies/ultibi_core/tests/filters.rs` & `ultibi-0.4.0/local_dependencies/ultibi_core/tests/filters.rs`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,15 @@
             ],
     "groupby": ["State"],
     "filters": [[{"op": "In", "field": "City", "value": ["NY", "New York", "Forks"]}], [{"op": "Eq","field": "State", "value": "Washington"}]]            
     }"#;
 
     let data_req = serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
 
-    let res = common::TEST_DASET
-        .as_ref()
-        .compute(data_req, false)
-        .unwrap();
+    let res = common::TEST_DASET.as_ref().compute(data_req).unwrap();
 
     let res_sum = res
         .column("Balance_sum")
         .expect("Couldn't get column Dalance_sum")
         .sum::<f64>()
         .expect("Couldn't sum");
     assert_eq!(res_sum, 20.0)
@@ -35,18 +32,15 @@
             ],
     "groupby": ["State"],
     "filters": [[{"op": "Eq", "field": "City", "value": "Sun Diego"}, {"op": "Eq", "field": "State", "value": "Washington"}], [{"op": "Eq", "field": "Sex", "value": "female"}]]            
     }"#;
 
     let data_req = serde_json::from_str::<ComputeRequest>(req).expect("Could not parse request");
 
-    let res = common::TEST_DASET
-        .as_ref()
-        .compute(data_req, false)
-        .unwrap();
+    let res = common::TEST_DASET.as_ref().compute(data_req).unwrap();
 
     let res_sum = res
         .column("Balance_mean")
         .expect("Couldn't get column Balance_mean")
         .mean()
         .expect("Couldn't find mean");
     assert_eq!(res_sum, 30.0)
```

### Comparing `ultibi-0.3.4/Cargo.toml` & `ultibi-0.4.0/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [package]
 name = "pyultima"
-version= "0.3.4"
+version= "0.4.0"
 edition = "2021"
 publish = false
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ultibi"
 crate-type = ["cdylib"]
 
 [package.metadata.maturin]
 name = "ultibi.rust_module.ultibi_engine"
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["extension-module", "abi3-py37"] }
-polars = { version = "0.28.0", features = [
+polars = { version = "0.31.1", features = [
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
     "serde",
-    "csv-file",
     "diagonal_concat",
     "serde-lazy" 
 ] }
-polars-arrow = "0.28.0"
-ultibi = { path = "local_dependencies/ultibi", features=["ui"] }
+#polars-arrow = { workspace = true }
+ultibi = { path = "local_dependencies/ultibi", features=["ui", "aws_s3"] }
 frtb_engine = { path = "local_dependencies/frtb_engine", features=["CRR2"] }
 serde_json = "1.0"
 thiserror = "1.0.38"
 once_cell = "1.17.1"
 ciborium = "0.2"
 
 [features]
```

### Comparing `ultibi-0.3.4/.gitignore` & `ultibi-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/LICENSE` & `ultibi-0.4.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Parameters
 
 Licensor:             Ultibi Ltd.
 Licensed Work:        Ultima
                       The Licensed Work is (c) 2023 Ultibi Ltd.
 
 Abstract
-Ultibi users can run it as a service, make availiable to their employees, contractors, and subsidiary companies. They can  extend Ultibi with their own Measures applied to their DataSets. They can use Ultibi to present their data to their consumers. The only thing that Ultibi users will not be able to do is offer a commercial version of Ultibi as Analytics as a Service without buying a license. For information about alternative licensing arrangements for the Software,
-please visit: https://ultimabi.uk/
+`ultibi` python library is made available exclusively for the purpose of demonstrating the possibilities offered by the Software so users can evaluate the possibilities and potential of the Software. You may use the library for non comercial, non for profit activity. You may not use this library in production, but you can purchase an alternative license for doing so. 
 
-`Ultibi as Analytics as a Service` is a commercial offering that allows third parties (other than your employees andcontractors) to make use of the setup and Measures defined by that who makes the offer or other third parties.
+Our `licenses` are extremely affordable, and you can check out the options by reaching out to us directly, via anatoly at ultimabi dot uk.
 
 Acceptance
 By using the software, you agree to all of the terms and conditions below.
 
 Copyright License
 The licensor grants you a non-exclusive, royalty-free, worldwide, non-sublicensable, non-transferable license to use, copy, distribute, make available, and tailor derivative works of the software, in each case subject to the limitations and conditions below.
 
 Limitations
+You may use the library for non comercial, non for profit activity. You may not use this library in production, but you can purchase an alternative license for doing so.
+
 You may not make the functionality of the software or a modified version available to third parties as a service, or distribute the software or a modified version in a manner that makes the functionality of the software available to third parties.
 
 Making the functionality of the software or modified version available to third parties includes, without limitation, enabling third parties to interact with the functionality of the software or modified version in distributed form or remotely through a computer network, offering a product or service the value of which entirely or primarily derives from the value of the software or modified version, or offering a product or service that accomplishes for users the primary purpose of the software or modified version.
 
 You may not alter, remove, or obscure any licensing, copyright, or other notices of the licensor in the software. Any use of the licensor’s trademarks is subject to applicable law.
 
 Patents
```

### Comparing `ultibi-0.3.4/Makefile` & `ultibi-0.4.0/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 venv:  ## Set up virtual environment
 	python3 -m venv $(VENV)
 	$(VENV_BIN)/python -m pip install --upgrade pip
 	$(VENV_BIN)/pip install -r requirements.txt
 	$(VENV_BIN)/pip install -r requirements-lint.txt
 
 .PHONY: develop
-build: venv  ## Compile and install Polars for development
+develop: venv  ## Compile and install Polars for development
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate && maturin develop
 
 .PHONY: build
 build: venv  ## Build whl
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate && maturin build -i=$(PY311) --release
 
 .PHONY: develop-release
```

### Comparing `ultibi-0.3.4/README.md` & `ultibi-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -42,22 +42,24 @@
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
 
 # Read Data
 # for more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html
 df = pl.read_csv("titanic.csv")
 
 # Convert it into an Ultibi DataSet
-ds = ul.DataSet.from_frame(df, bespoke_measures=measures)
+ds = ul.DataSet.from_frame(df)
 
 # By default (might change in the future)
 # Fields are Utf8 (non numerics) and integers
 # Measures are numeric columns.
 ds.ui() 
 ```
 
+Then navigate to `http://localhost:8000` or checkout `http://localhost:8000/swagger-ui` for the OpenAPI documentation.
+
 ### More flexible - custom measures
 ```python
 import ultibi as ul
 import polars as pl
 import os
 os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
@@ -134,12 +136,40 @@
 
 # By default (might change in the future)
 # Fields are Utf8 (non numerics) and integers
 # Measures are numeric columns.
 ds.ui() 
 ```
 
-Then navigate to `http://localhost:8000` or checkout `http://localhost:8000/swagger-ui` for the OpenAPI documentation.
+### DataSources
+We provide aim to support different sources of the data. 
+```python
+scan = pl.read_csv("../frtb_engine/data/frtb/Delta.csv", 
+                           dtypes={"SensitivitySpot": pl.Float64})
+dsource = ul.DataSource.inmemory(scan)
+ds = ul.DataSet.from_source(dsource)
+ds.prepare() # .prepare() is only relevant to FRTB dataset currently
+ds.ui()
+```
+If you don't want to/can't hold all your data in the process memory, you can sacrifise performance for memory with Scan/DataBase
+```python
+import polars as pl
+import ultibi as ul
+# Note that the LazyFrame query must start with scan_
+# and must've NOT been collected
+scan = pl.scan_csv("../frtb_engine/data/frtb/Delta.csv", 
+                    dtypes={"SensitivitySpot": pl.Float64})
+dsource = ul.DataSource.scan(scan)
+ds = ul.DataSet.from_source(dsource)
+ds.ui()
+```
+
+Note: Naturally the later two options will be slower, because prior to computing your measures we will need to read the relevant bits of the data into the process memory. 
 
 ### FRTB SA
 [FRTB SA](https://en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a great usecase for `ultibi`. FRTB SA is a set of standardised, computationally intensive rules established by the regulator. High business impact of these rules manifests in need for **analysis** and **visibility** thoroughout an organisation. Note: Ultima is not a certified aggregator. Always benchmark the results against your own interpretation of the rules.
-See python frtb [userguide](https://ultimabi.uk/ultibi-frtb-book/).
+See python frtb [userguide](https://ultimabi.uk/ultibi-frtb-book/).
+
+### License 
+`ultibi` python library is made available exclusively for the purpose of demonstrating the possibilities offered by the Software so users can evaluate the possibilities and potential of the Software. You may use the library for non comercial, non for profit activity. You may not use this library in production, but you can purchase an alternative license for doing so. 
+
+Our `licenses` are extremely affordable, and you can check out the options by reaching out to us directly, via anatoly at ultimabi dot uk.
```

#### html2text {}

```diff
@@ -15,53 +15,72 @@
 We use TypeScript for the frontend. # Examples Our userguide is under
 development. In the mean time refer to FRTB [userguide](https://ultimabi.uk/
 ultibi-frtb-book/). ## Python ### Quickstart ```python import ultibi as ul
 import polars as pl import os os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address # Read Data # for
 more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/
 polars.read_csv.html df = pl.read_csv("titanic.csv") # Convert it into an
-Ultibi DataSet ds = ul.DataSet.from_frame(df, bespoke_measures=measures) # By
-default (might change in the future) # Fields are Utf8 (non numerics) and
-integers # Measures are numeric columns. ds.ui() ``` ### More flexible - custom
-measures ```python import ultibi as ul import polars as pl import os os.environ
-["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] = "0.0.0.0:8000" #
-host on this address # Read Data # for more details: https://pola-rs.github.io/
-polars/py-polars/html/reference/api/polars.read_csv.html df = pl.read_csv
-("titanic.csv") # Let's add some Custom/Bespoke Calculations to our UI #
-Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -> pl.Expr:
-"""Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age") * pl.col
-("survived") - age of survived person, otherwise 0 pl.col("survived").sum() -
-number of survived """ return pl.col("age") * pl.col("survived") / pl.col
-("survived").sum() # Also a Standard Calculator def example_dep_calc(kwargs:
-dict[str, str]) -> pl.Expr: return pl.col("SurvivalMeanAge_sum") + pl.col
-("SouthamptonFareDivAge_sum") # When we need more involved calculations we go
-for a Custom Calculator def custom_calculator( srs: list[pl.Series], kwargs:
-dict[str, str] ) -> pl.Series: """ Southampton Fare/Age*multiplier """ df =
-pl.DataFrame({"age": srs[0], "fare": srs[1], "e": srs[2]}) # Add Indicator
-Column for Southampton df = df.with_columns(pl.when(pl.col("e")=="S").then
-(1).otherwise(0).alias("S")) multiplier = float(kwargs.get("multiplier", 1))
-res = df["S"] * df["fare"] / df["age"] * multiplier return res # inputs for the
-custom_calculator srs param inputs = ["age", "fare", "embarked"] # We return
-Floats res_type = pl.Float64 # We return a Series, not a scalar (which
-otherwise would be auto exploded) returns_scalar = False measures =
-[ ul.BaseMeasure( "SouthamptonFareDivAge", ul.CustomCalculator
-( custom_calculator, res_type, inputs, returns_scalar ), # (Optional) - we are
-only interested in Southampton, so # unless other measures requested we might
-as well filter for Southampton only # However, if if multiple measures
-requested, their precompute_filters will be joined as OR. [[ul.EqFilter
-("embarked", "S")]], # PARAMS tab of the UI calc_params=[ul.CalcParam("mltplr",
-"1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge", ul.StandardCalculator
-(survival_mean_age), aggregation_restriction="sum", ), ul.DependantMeasure
-( "A_Dependant_Measure", ul.StandardCalculator(example_dep_calc), [
-("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge", "sum")], ), ] # Convert
-it into an Ultibi DataSet ds = ul.DataSet.from_frame(df,
-bespoke_measures=measures) # By default (might change in the future) # Fields
-are Utf8 (non numerics) and integers # Measures are numeric columns. ds.ui()
-``` Then navigate to `http://localhost:8000` or checkout `http://localhost:
-8000/swagger-ui` for the OpenAPI documentation. ### FRTB SA [FRTB SA](https://
+Ultibi DataSet ds = ul.DataSet.from_frame(df) # By default (might change in the
+future) # Fields are Utf8 (non numerics) and integers # Measures are numeric
+columns. ds.ui() ``` Then navigate to `http://localhost:8000` or checkout
+`http://localhost:8000/swagger-ui` for the OpenAPI documentation. ### More
+flexible - custom measures ```python import ultibi as ul import polars as pl
+import os os.environ["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] =
+"0.0.0.0:8000" # host on this address # Read Data # for more details: https://
+pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html df =
+pl.read_csv("titanic.csv") # Let's add some Custom/Bespoke Calculations to our
+UI # Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -
+> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age")
+* pl.col("survived") - age of survived person, otherwise 0 pl.col
+("survived").sum() - number of survived """ return pl.col("age") * pl.col
+("survived") / pl.col("survived").sum() # Also a Standard Calculator def
+example_dep_calc(kwargs: dict[str, str]) -> pl.Expr: return pl.col
+("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") # When we need
+more involved calculations we go for a Custom Calculator def custom_calculator
+( srs: list[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton
+Fare/Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e":
+srs[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
+(pl.col("e")=="S").then(1).otherwise(0).alias("S")) multiplier = float
+(kwargs.get("multiplier", 1)) res = df["S"] * df["fare"] / df["age"] *
+multiplier return res # inputs for the custom_calculator srs param inputs =
+["age", "fare", "embarked"] # We return Floats res_type = pl.Float64 # We
+return a Series, not a scalar (which otherwise would be auto exploded)
+returns_scalar = False measures = [ ul.BaseMeasure( "SouthamptonFareDivAge",
+ul.CustomCalculator( custom_calculator, res_type, inputs, returns_scalar ), #
+(Optional) - we are only interested in Southampton, so # unless other measures
+requested we might as well filter for Southampton only # However, if if
+multiple measures requested, their precompute_filters will be joined as OR. [
+[ul.EqFilter("embarked", "S")]], # PARAMS tab of the UI calc_params=
+[ul.CalcParam("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
+ul.StandardCalculator(survival_mean_age), aggregation_restriction="sum", ),
+ul.DependantMeasure( "A_Dependant_Measure", ul.StandardCalculator
+(example_dep_calc), [("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge",
+"sum")], ), ] # Convert it into an Ultibi DataSet ds = ul.DataSet.from_frame
+(df, bespoke_measures=measures) # By default (might change in the future) #
+Fields are Utf8 (non numerics) and integers # Measures are numeric columns.
+ds.ui() ``` ### DataSources We provide aim to support different sources of the
+data. ```python scan = pl.read_csv("../frtb_engine/data/frtb/Delta.csv",
+dtypes={"SensitivitySpot": pl.Float64}) dsource = ul.DataSource.inmemory(scan)
+ds = ul.DataSet.from_source(dsource) ds.prepare() # .prepare() is only relevant
+to FRTB dataset currently ds.ui() ``` If you don't want to/can't hold all your
+data in the process memory, you can sacrifise performance for memory with Scan/
+DataBase ```python import polars as pl import ultibi as ul # Note that the
+LazyFrame query must start with scan_ # and must've NOT been collected scan =
+pl.scan_csv("../frtb_engine/data/frtb/Delta.csv", dtypes={"SensitivitySpot":
+pl.Float64}) dsource = ul.DataSource.scan(scan) ds = ul.DataSet.from_source
+(dsource) ds.ui() ``` Note: Naturally the later two options will be slower,
+because prior to computing your measures we will need to read the relevant bits
+of the data into the process memory. ### FRTB SA [FRTB SA](https://
 en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a great
 usecase for `ultibi`. FRTB SA is a set of standardised, computationally
 intensive rules established by the regulator. High business impact of these
 rules manifests in need for **analysis** and **visibility** thoroughout an
 organisation. Note: Ultima is not a certified aggregator. Always benchmark the
 results against your own interpretation of the rules. See python frtb
-[userguide](https://ultimabi.uk/ultibi-frtb-book/).
+[userguide](https://ultimabi.uk/ultibi-frtb-book/). ### License `ultibi` python
+library is made available exclusively for the purpose of demonstrating the
+possibilities offered by the Software so users can evaluate the possibilities
+and potential of the Software. You may use the library for non comercial, non
+for profit activity. You may not use this library in production, but you can
+purchase an alternative license for doing so. Our `licenses` are extremely
+affordable, and you can check out the options by reaching out to us directly,
+via anatoly at ultimabi dot uk.
```

### Comparing `ultibi-0.3.4/example.py` & `ultibi-0.4.0/example.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/pyproject.toml` & `ultibi-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 description = "Flexible DataFrame Operations via UI"
 readme = "README.md"
 authors = [
   { name = "Anatoly Bugakov", email = "anatoly@ultimabi.uk" },
 ]
 license = { file = "LICENSE" }
 dependencies = [
-#  "typing_extensions >= 4.0.0; python_version <= '3.9'",
-  "polars",
-  "pyarrow"
+  "polars >= 0.18.7",
 ]
 keywords = ["dataframe", "visualization", "aggregation", "calculation", 
   "chart", "data", "dataviz", "pivot-table", "frtb", "risk"]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
-    "License :: Free for non-commercial use",
+    "License :: Free To Use But Restricted",
     "Topic :: Scientific/Engineering",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
@@ -51,14 +49,15 @@
   "redundant-expr",
   "truthy-bool",
   "ignore-without-code",
 ]
 disable_error_code = [
   "empty-body",
 ]
+python_version = 3.9 # MRV of Python for Ultibi is 3.9
 
 [[tool.mypy.overrides]]
 module = [
   "pyarrow.*",
   "ultibi.rust_module.ultibi_engine",
 ]
 ignore_missing_imports = true
```

### Comparing `ultibi-0.3.4/src/calculator.rs` & `ultibi-0.4.0/src/calculator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     .call(py, (op.into_py_dict(py),), None)
                     .map_err(|e| PolarsError::ComputeError(e.value(py).to_string().into()))?;
                 let b = out.call_method(py, "__getstate__", (), None).unwrap(); // should never fail
                 let as_pybytes = b.downcast::<PyBytes>(py).unwrap(); // should never fail
                 let rustbytes = as_pybytes.as_bytes();
                 //let e = serde_json::from_slice::<Expr>(rustbytes).unwrap(); // should never fail
                 let e: Expr = ciborium::de::from_reader(rustbytes).map_err(|e| {
-                    PolarsError::ComputeError(format!("{}. Try using Custom calculator", e).into())
+                    PolarsError::ComputeError(format!("Error deserializing expression. This could be due to differenet Polars version. Try using Custom calculator. {}", e).into())
                 })?;
                 Ok(e)
             })
         };
         let calculator = Arc::new(calculator);
         Ok(Self { inner: calculator })
     }
```

### Comparing `ultibi-0.3.4/src/conversions/series.rs` & `ultibi-0.4.0/src/conversions/series.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #![allow(dead_code)]
 
 use std::collections::HashMap;
-
+use polars::export::arrow;
 use arrow::ffi;
 use polars::prelude::*;
-use polars_arrow::export::arrow;
+//use polars_arrow::export::arrow;
 use pyo3::exceptions::PyValueError;
 use pyo3::ffi::Py_uintptr_t;
 use pyo3::prelude::*;
 use pyo3::types::IntoPyDict;
 use pyo3::{PyAny, PyObject, PyResult};
 
 /// Take an arrow array from python and convert it to a rust arrow array.
```

### Comparing `ultibi-0.3.4/src/conversions/wrappers.rs` & `ultibi-0.4.0/src/conversions/wrappers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/src/dataset.rs` & `ultibi-0.4.0/src/dataset.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,69 @@
 use frtb_engine::FRTBDataSet;
 use pyo3::exceptions::PyFileNotFoundError;
 use pyo3::{prelude::*, types::PyType, PyTypeInfo};
 use std::collections::BTreeMap;
 use std::path::Path;
 use std::sync::Arc;
+use ultibi::datasource::DataSource;
+use ultibi::filters::FilterE;
+use ultibi::new::NewSourcedDataSet;
 //use std::sync::Mutex;
 use crate::conversions::series::{py_series_to_rust_series, rust_series_to_py_series};
+use crate::datasource::DataSourceWrapper;
 use crate::errors::PyUltimaErr;
+use crate::filter::FilterWrapper;
 use crate::measure::MeasureWrapper;
 use crate::requests;
 use std::sync::RwLock;
 use ultibi::polars::prelude::Series;
 use ultibi::VisualDataSet;
 use ultibi::{
-    self, derive_basic_measures_vec, numeric_columns, DataFrame, DataSet, DataSetBase, IntoLazy,
-    MeasuresMap, ValidateSet,
+    self, derive_basic_measures_vec, numeric_columns, DataFrame, DataSet, DataSetBase, MeasuresMap,
 };
 
 #[pyclass]
 pub struct DataSetWrapper {
     dataset: Arc<RwLock<dyn DataSet>>,
 }
 
 /// Part of config is limit of numeric cols
-fn from_conf<T: DataSet + 'static>(
+fn from_conf<T: NewSourcedDataSet + 'static>(
     conf_path: String,
-    collect: bool,
-    prepare: bool,
     bespoke_measures: MeasuresMap,
 ) -> PyResult<DataSetWrapper> {
     // This is now done in build_validate_prepare
     // TODO build_validate_prepare to return result and errors to be mapped
     // Like this:
     if !Path::new(&conf_path).exists() {
         return Err(PyFileNotFoundError::new_err("Config file doesn't exist"));
     }
 
-    let ds = ultibi::acquire::config_build_validate_prepare::<T>(
-        conf_path.as_str(),
-        collect,
-        prepare,
-        bespoke_measures,
-    );
+    let ds =
+        ultibi::acquire::config_build_validate_prepare::<T>(conf_path.as_str(), bespoke_measures);
     //let dataset = Box::new(ds);
     Ok(DataSetWrapper {
         dataset: Arc::new(RwLock::new(ds)),
     })
 }
 
-fn from_frame<T: DataSet + 'static>(
-    py: Python,
-    seriess: Vec<Py<PyAny>>,
+fn from_source<T: NewSourcedDataSet + 'static>(
+    _: Python,
+    source: DataSource,
     measures: Option<Vec<String>>,
     build_params: BTreeMap<String, String>,
     bespoke_measures: MeasuresMap,
 ) -> PyResult<DataSetWrapper> {
-    let df = DataFrame::new(
-        seriess
-            .into_iter()
-            .map(|x| py_series_to_rust_series(x.as_ref(py)))
-            .collect::<PyResult<Vec<Series>>>()?,
-    )
-    .map_err(PyUltimaErr::Polars)?;
-
-    let schema = df.schema();
-    let arc_schema = Arc::new(schema);
-    // TODO function arg should be add_numeric_columns_as_measures, defaulted to true
+    let arc_schema = source.get_schema().map_err(PyUltimaErr::Ultima)?;
     let measures = measures.unwrap_or_else(|| numeric_columns(arc_schema));
     let mv = derive_basic_measures_vec(measures);
     let mut mm: MeasuresMap = MeasuresMap::from_iter(mv);
     mm.extend(bespoke_measures);
 
-    let ds: T = DataSet::new(df.lazy(), mm, build_params);
+    let ds: T = T::new(source, mm, Default::default(), build_params);
 
     Ok(DataSetWrapper {
         dataset: Arc::new(RwLock::new(ds)),
     })
 }
 
 #[pymethods]
@@ -87,113 +75,147 @@
         Self::from_frame(pyself, py, vec![], None, None, None).unwrap()
     }
 
     #[classmethod]
     fn from_config_path(
         _: &PyType,
         conf_path: String,
-        collect: Option<bool>,
-        prepare: Option<bool>,
         bespoke_measures: Option<Vec<MeasureWrapper>>,
     ) -> PyResult<Self> {
-        let collect = collect.unwrap_or_else(|| true);
-        let prepare = prepare.unwrap_or_else(|| false);
         let bespoke_measures = bespoke_measures.unwrap_or_default();
         let mm = bespoke_measures
             .into_iter()
             .map(|x| {
                 let m = x._inner;
                 (m.name().clone(), m)
             })
             .collect::<MeasuresMap>();
-        from_conf::<DataSetBase>(conf_path, collect, prepare, mm)
+        from_conf::<DataSetBase>(conf_path, mm)
     }
 
     #[classmethod]
     fn frtb_from_config_path(
         _: &PyType,
         conf_path: String,
-        collect: Option<bool>,
-        prepare: Option<bool>,
+        bespoke_measures: Option<Vec<MeasureWrapper>>,
     ) -> PyResult<Self> {
-        let collect = collect.unwrap_or_else(|| true);
-        let prepare = prepare.unwrap_or_else(|| false);
-        let empty = BTreeMap::default();
-        from_conf::<FRTBDataSet>(conf_path, collect, prepare, empty)
+        let bespoke_measures = bespoke_measures.unwrap_or_default();
+        let mm = bespoke_measures
+            .into_iter()
+            .map(|x| x._inner)
+            .collect::<MeasuresMap>();
+
+        from_conf::<FRTBDataSet>(conf_path, mm)
     }
 
     #[classmethod]
     fn from_frame(
         _: &PyType,
         py: Python,
         seriess: Vec<Py<PyAny>>,
         measures: Option<Vec<String>>,
         build_params: Option<BTreeMap<String, String>>,
         bespoke_measures: Option<Vec<MeasureWrapper>>,
     ) -> PyResult<Self> {
+        let df = DataFrame::new(
+            seriess
+                .into_iter()
+                .map(|x| py_series_to_rust_series(x.as_ref(py)))
+                .collect::<PyResult<Vec<Series>>>()?,
+        )
+        .map_err(PyUltimaErr::Polars)?;
+        let source = DataSource::InMemory(df);
         let build_params = build_params.unwrap_or_default();
         let mm = bespoke_measures
             .unwrap_or_default()
             .into_iter()
             .map(|x| {
                 let m = x._inner;
                 (m.name().clone(), m)
             })
             .collect::<MeasuresMap>();
-        from_frame::<DataSetBase>(py, seriess, measures, build_params, mm)
+        from_source::<DataSetBase>(py, source, measures, build_params, mm)
     }
 
     #[classmethod]
     fn frtb_from_frame(
         _: &PyType,
         py: Python,
-        series: Vec<Py<PyAny>>,
+        seriess: Vec<Py<PyAny>>,
+        measures: Option<Vec<String>>,
+        build_params: Option<BTreeMap<String, String>>,
+        bespoke_measures: Option<Vec<MeasureWrapper>>,
+    ) -> PyResult<Self> {
+        let df = DataFrame::new(
+            seriess
+                .into_iter()
+                .map(|x| py_series_to_rust_series(x.as_ref(py)))
+                .collect::<PyResult<Vec<Series>>>()?,
+        )
+        .map_err(PyUltimaErr::Polars)?;
+        let source = DataSource::InMemory(df);
+        let build_params = build_params.unwrap_or_default();
+        let mm = bespoke_measures
+            .unwrap_or_default()
+            .into_iter()
+            .map(|x| {
+                let m = x._inner;
+                (m.name().clone(), m)
+            })
+            .collect::<MeasuresMap>();
+        from_source::<FRTBDataSet>(py, source, measures, build_params, mm)
+    }
+
+    #[classmethod]
+    fn from_source(
+        _: &PyType,
+        py: Python,
+        source: DataSourceWrapper,
         measures: Option<Vec<String>>,
         build_params: Option<BTreeMap<String, String>>,
+        bespoke_measures: Option<Vec<MeasureWrapper>>,
     ) -> PyResult<Self> {
         let build_params = build_params.unwrap_or_default();
-        let empty = BTreeMap::default();
-        from_frame::<FRTBDataSet>(py, series, measures, build_params, empty)
+        let mm = bespoke_measures
+            .unwrap_or_default()
+            .into_iter()
+            .map(|x| {
+                let m = x._inner;
+                (m.name().clone(), m)
+            })
+            .collect::<MeasuresMap>();
+        from_source::<DataSetBase>(py, source.inner, measures, build_params, mm)
     }
 
-    pub fn ui(&self, py: Python, streaming: bool) -> PyResult<()> {
+    pub fn ui(&self, py: Python) -> PyResult<()> {
         let a = Arc::clone(&self.dataset);
-        py.allow_threads(|| a.ui(streaming));
+        py.allow_threads(|| a.ui());
         Ok(())
     }
 
     pub fn prepare(&mut self, collect: Option<bool>) -> PyResult<()> {
-        let ds = self.dataset.read().expect("Poisonned RwLock");
-        let lf = ds.get_lazyframe().clone();
-        let collect = collect.unwrap_or_else(|| true);
-
-        let mut new_frame = ds.prepare_frame(Some(lf)).map_err(PyUltimaErr::Polars)?;
-
-        if collect {
-            new_frame = new_frame.collect().map_err(PyUltimaErr::Polars)?.lazy()
-        }
-        std::mem::drop(ds);
-
         let mut ds = self.dataset.write().expect("Poisonned RwLock");
-        ds.set_lazyframe_inplace(new_frame);
+        ds.prepare().map_err(PyUltimaErr::Ultima)?;
+        if let Some(true) = collect {
+            ds.collect().map_err(PyUltimaErr::Ultima)?;
+        }
         Ok(())
     }
 
     pub fn compute(
         &self,
         py: Python,
         request: requests::ComputeRequestWrapper,
-        streaming: bool,
     ) -> PyResult<Vec<PyObject>> {
         py.allow_threads(|| {
             self.dataset
                 .read()
                 .expect("Poisonned RwLock")
-                .compute(request.ar, streaming)
-                .map_err(PyUltimaErr::Polars)?
+                .compute(request.ar)
+                .map_err(PyUltimaErr::Ultima)?
                 .iter()
                 .map(rust_series_to_py_series)
                 .collect()
         })
     }
 
     pub fn measures(&self) -> BTreeMap<String, Option<String>> {
@@ -201,51 +223,64 @@
             .read()
             .expect("Poisonned RwLock")
             .get_measures()
             .iter()
             .map(|(x, m)| (x.to_string(), m.aggregation().clone()))
             .collect::<BTreeMap<String, Option<String>>>()
     }
-    pub fn frame(&self) -> PyResult<Vec<PyObject>> {
+    pub fn frame(&self, fltrs: Option<Vec<Vec<FilterWrapper>>>) -> PyResult<Vec<PyObject>> {
+        let fltrs = if let Some(f) = fltrs {
+            f.into_iter()
+                .map(|inner| {
+                    inner
+                        .into_iter()
+                        .map(|fltr_wrap| fltr_wrap.inner)
+                        .collect::<Vec<FilterE>>()
+                })
+                .collect::<Vec<Vec<FilterE>>>()
+        } else {
+            Default::default()
+        };
+
         self.dataset
             .read()
             .expect("Poisonned RwLock")
-            .get_lazyframe()
-            .clone()
+            .get_lazyframe(&fltrs)
             .collect()
             .map_err(PyUltimaErr::Polars)?
             .iter()
             .map(rust_series_to_py_series)
             .collect()
     }
+
     pub fn fields(&self) -> PyResult<Vec<String>> {
         let schema = self
             .dataset
             .read()
             .expect("Poisonned RwLock")
-            .get_lazyframe()
-            .schema()
-            .map_err(PyUltimaErr::Polars)?;
+            .get_schema()
+            .map_err(PyUltimaErr::Ultima)?;
 
         Ok(ultibi::prelude::fields_columns(schema))
     }
     pub fn calc_params(&self) -> Vec<(String, Option<String>, Option<String>)> {
         self.dataset
             .read()
             .expect("Poisonned RwLock")
             .calc_params()
             .iter()
             .cloned()
             .map(|calc_param| (calc_param.name, calc_param.type_hint, calc_param.default))
             .collect()
     }
 
-    pub fn validate(&self) -> PyResult<()> {
+    pub fn validate(&self, subset: Option<u8>) -> PyResult<()> {
+        let subset = if let Some(u) = subset { u } else { 0 };
         self.dataset
             .read()
             .expect("Poisonned RwLock")
-            .validate_frame(None, ValidateSet::ALL)
-            .map_err(PyUltimaErr::Polars)?;
+            .validate_frame(None, subset)
+            .map_err(PyUltimaErr::Ultima)?;
 
         Ok(())
     }
 }
```

### Comparing `ultibi-0.3.4/src/errors.rs` & `ultibi-0.4.0/src/errors.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 use std::fmt::{Debug, Formatter};
 use std::io::Error;
 
 use polars::prelude::PolarsError;
-use pyo3::exceptions::{PyException, PyIOError};
+use pyo3::exceptions::PyException;
 use pyo3::{create_exception, PyErr};
 //use pyo3::prelude::*;
 use thiserror::Error;
+use ultibi::errors::UltimaErr;
 
 #[derive(Error)]
 pub enum PyUltimaErr {
     #[error(transparent)]
     Polars(#[from] PolarsError),
     #[error(transparent)]
     SerdeJson(#[from] serde_json::Error),
+    #[error(transparent)]
+    Ultima(#[from] UltimaErr),
     #[error("{0}")]
     Other(String),
 }
 
 impl std::convert::From<std::io::Error> for PyUltimaErr {
     fn from(value: Error) -> Self {
         PyUltimaErr::Other(format!("{value}"))
@@ -25,47 +28,51 @@
 
 impl std::convert::From<PyUltimaErr> for PyErr {
     fn from(err: PyUltimaErr) -> PyErr {
         //let default = || PyRuntimeError::new_err(format!("{:?}", &err));
 
         use PyUltimaErr::*;
         match &err {
-            Polars(err) => match err {
-                PolarsError::ColumnNotFound(name) => NotFoundError::new_err(name.to_string()),
-                PolarsError::ComputeError(err) => ComputeError::new_err(err.to_string()),
-                PolarsError::SchemaFieldNotFound(err) => {
-                    SchemaFieldNotFound::new_err(err.to_string())
-                }
-                PolarsError::StructFieldNotFound(err) => {
-                    StructFieldNotFound::new_err(err.to_string())
-                }
-                PolarsError::NoData(err) => NoDataError::new_err(err.to_string()),
-                PolarsError::ShapeMismatch(err) => ShapeError::new_err(err.to_string()),
-                PolarsError::SchemaMismatch(err) => SchemaError::new_err(err.to_string()),
-                PolarsError::Io(err) => PyIOError::new_err(err.to_string()),
-                PolarsError::ArrowError(err) => ArrowErrorException::new_err(format!("{err}")),
-                PolarsError::Duplicate(err) => DuplicateError::new_err(err.to_string()),
-                PolarsError::InvalidOperation(err) => {
-                    InvalidOperationError::new_err(err.to_string())
-                }
-            },
+            Polars(err) => UltiPolarsError::new_err(err.to_string()),
+            // Polars(err) => match err {
+            //     PolarsError::ColumnNotFound(name) => NotFoundError::new_err(name.to_string()),
+            //     PolarsError::ComputeError(err) => ComputeError::new_err(err.to_string()),
+            //     PolarsError::SchemaFieldNotFound(err) => {
+            //         SchemaFieldNotFound::new_err(err.to_string())
+            //     }
+            //     PolarsError::StructFieldNotFound(err) => {
+            //         StructFieldNotFound::new_err(err.to_string())
+            //     }
+            //     PolarsError::NoData(err) => NoDataError::new_err(err.to_string()),
+            //     PolarsError::ShapeMismatch(err) => ShapeError::new_err(err.to_string()),
+            //     PolarsError::SchemaMismatch(err) => SchemaError::new_err(err.to_string()),
+            //     PolarsError::Io(err) => PyIOError::new_err(err.to_string()),
+            //     PolarsError::ArrowError(err) => ArrowErrorException::new_err(format!("{err}")),
+            //     PolarsError::Duplicate(err) => DuplicateError::new_err(err.to_string()),
+            //     PolarsError::InvalidOperation(err) => {
+            //         InvalidOperationError::new_err(err.to_string())
+            //     },
+            //     PolarsError::StringCacheMismatch(err) => Other(err.to_string())
+            //},
             SerdeJson(err) => SerdeJsonError::new_err(format!(
                 "Couldn't (de)serialise input. Check format. {err}"
             )),
+            Ultima(err) => UltimaError::new_err(err.to_string()),
             Other(_str) => OtherError::new_err(_str.to_string()),
         }
     }
 }
 
 impl Debug for PyUltimaErr {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         use PyUltimaErr::*;
         match self {
             Polars(err) => write!(f, "{err}"),
             SerdeJson(err) => write!(f, "Couldn't serialize string. Check format. {err}"),
+            Ultima(err) => write!(f, "Ultima error. {err}"),
             Other(err) => write!(f, "BindingsError: {err}"),
         }
     }
 }
 
 create_exception!(exceptions, NotFoundError, PyException);
 create_exception!(exceptions, ComputeError, PyException);
@@ -75,7 +82,9 @@
 create_exception!(exceptions, SchemaError, PyException);
 create_exception!(exceptions, DuplicateError, PyException);
 create_exception!(exceptions, InvalidOperationError, PyException);
 create_exception!(exceptions, SerdeJsonError, PyException);
 create_exception!(exceptions, OtherError, PyException);
 create_exception!(exceptions, SchemaFieldNotFound, PyException);
 create_exception!(exceptions, StructFieldNotFound, PyException);
+create_exception!(exceptions, UltimaError, PyException);
+create_exception!(exceptions, UltiPolarsError, PyException);
```

### Comparing `ultibi-0.3.4/src/filter.rs` & `ultibi-0.4.0/src/filter.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/src/lib.rs` & `ultibi-0.4.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #![allow(clippy::unnecessary_lazy_evaluations)]
 extern crate ultibi as ultibi_rs;
 
 use errors::{
     ArrowErrorException, ComputeError, DuplicateError, InvalidOperationError, NoDataError,
-    NotFoundError, OtherError, SchemaError, SerdeJsonError, ShapeError,
+    NotFoundError, OtherError, SchemaError, SerdeJsonError, ShapeError, UltimaError,
 };
 use pyo3::{pyfunction, pymodule, types::PyModule, wrap_pyfunction, PyResult, Python};
 
 mod calculator;
 mod conversions;
 mod dataset;
+mod datasource;
 mod errors;
 mod filter;
 mod measure;
 mod requests;
 
 #[pyfunction]
 fn agg_ops() -> Vec<&'static str> {
@@ -28,19 +29,22 @@
 #[pymodule]
 fn ultibi_engine(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(agg_ops, m)?)?;
     //m.add_function(wrap_pyfunction!(exec_agg, m)?)?;
     m.add_class::<requests::AggregationRequestWrapper>()?;
     m.add_class::<requests::ComputeRequestWrapper>()?;
     m.add_class::<dataset::DataSetWrapper>()?;
+    m.add_class::<datasource::DataSourceWrapper>()?;
     m.add_class::<measure::MeasureWrapper>()?;
     m.add_class::<filter::FilterWrapper>()?;
     m.add_class::<calculator::CalculatorWrapper>()?;
     m.add_class::<measure::CalcParamWrapper>()?;
 
+    m.add("UltimaError", _py.get_type::<UltimaError>()).unwrap();
+
     m.add("NotFoundError", _py.get_type::<NotFoundError>())
         .unwrap();
     m.add("ComputeError", _py.get_type::<ComputeError>())
         .unwrap();
     m.add("OtherError", _py.get_type::<OtherError>()).unwrap();
     m.add("NoDataError", _py.get_type::<NoDataError>()).unwrap();
     m.add("ArrowErrorException", _py.get_type::<ArrowErrorException>())
```

### Comparing `ultibi-0.3.4/src/measure.rs` & `ultibi-0.4.0/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/src/requests.rs` & `ultibi-0.4.0/src/requests.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/tests/data/datasource_config.toml` & `ultibi-0.4.0/tests/data/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/tests/docs/run_doc_examples.py` & `ultibi-0.4.0/tests/docs/run_doc_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     # __file__ returns the __init__.py, so grab the parent
     src_dir = Path(ultibi.__file__).parent
 
     with TemporaryDirectory() as tmpdir:
         # collect all tests
         tests = [
             doctest.DocTestSuite(
-                m, extraglobs={"pl": ultibi, "dirpath": Path(tmpdir)}, optionflags=1
+                m, extraglobs={"ul": ultibi, "dirpath": Path(tmpdir)}, optionflags=1
             )
             for m in modules_in_path(src_dir)
         ]
         test_suite = unittest.TestSuite(tests)
 
         # run doctests and report
         result = unittest.TextTestRunner().run(test_suite)
```

### Comparing `ultibi-0.3.4/tests/unit/test_ds.py` & `ultibi-0.4.0/tests/unit/test_ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import polars as pl
 
 import ultibi as ul
 
 
 class TestCreation(unittest.TestCase):
+    # TODO add tast for Scan
     def test_frtbds_from_config(self) -> None:
         dataset = ul.FRTBDataSet.from_config_path("./tests/data/datasource_config.toml")
 
         frame = dataset.frame()
 
         dataset.validate()
 
-        dataset.prepare()
-
+        # Has already been prepared via the config
+        self.assertRaises(ul.internals.UltimaError, dataset.prepare)
         assert "jurisdiction" in [cp[0] for cp in dataset.calc_params]
         assert "FX Curvature KbMinus" in dataset.measures
         assert isinstance(frame, pl.DataFrame)
         assert "TradeId" in frame
 
     def test_ds_from_frame(self) -> None:
         data = {"a": [1, 2, 3], "b": [4, 5, 6], "c": ["a", "a", "b"]}
@@ -30,19 +31,20 @@
         assert ds.frame().frame_equal(expected)
         assert {"a", "b"}.issubset(ds.measures.keys())
 
     def test_ds_validate(self) -> None:
         data = {"a": [1, 2, 3], "b": [4, 5, 6], "c": ["a", "a", "b"]}
         df = pl.DataFrame(data)
         ds = ul.FRTBDataSet.from_frame(df)
-        self.assertRaises(ul.internals.NoDataError, ds.validate)
+        self.assertRaises(ul.internals.UltimaError, ds.validate)
 
+    # TODO this will be turned into prepare_for_each_request
     def test_ds_already_prepared(self) -> None:
         data = {"a": [1, 2, 3], "b": [4, 5, 6], "c": ["a", "a", "b"]}
         df = pl.DataFrame(data)
         ds = ul.DataSet.from_frame(df)
         ds.validate()
-        self.assertRaises(ul.internals.OtherError, ds.prepare)
+        # self.assertRaises(ul.internals.OtherError, ds.prepare)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ultibi-0.3.4/tests/unit/test_measure.py` & `ultibi-0.4.0/tests/unit/test_measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/ultibi/__init__.py` & `ultibi-0.4.0/ultibi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 from .internals import (
     AggRequest,
     BaseMeasure,
     CalcParam,
     ComputeRequest,
     CustomCalculator,
     DataSet,
+    DataSource,
     DependantMeasure,
     EqFilter,
     FRTBDataSet,
     InFilter,
     NeqFilter,
     NoDataError,
     NotInFilter,
     OtherError,
     StandardCalculator,
+    UltimaError,
     aggregation_ops,
 )
 
 __all__ = [
     "AggRequest",
     "ComputeRequest",
     "FRTBDataSet",
     "DataSet",
+    "DataSource",
     "aggregation_ops",
     "OtherError",
     "NoDataError",
     "polars",
     "pyarrow",
     "Filter",
     "FilterType",
@@ -43,8 +46,9 @@
     "Measure",
     "BaseMeasure",
     "DependantMeasure",
     "Calculator",
     "CustomCalculator",
     "StandardCalculator",
     "CalcParam",
+    "UltimaError",
 ]
```

### Comparing `ultibi-0.3.4/ultibi/internals/__init__.py` & `ultibi-0.4.0/ultibi/internals/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 Core Ultima functionality.
 
 The modules within `ultima.internals` are interdependent. To prevent cyclical imports,
 they all import from each other via this __init__ file using
 `import ultibi.internals as uli`. The imports below are being shared across this module.
 """
 
-from ..rust_module.ultibi_engine import NoDataError, OtherError
+from ..rust_module.ultibi_engine import NoDataError, OtherError, UltimaError
 from .dataset import DS, DataSet, FRTBDataSet
+from .datasource import DataSource
 from .filters import EqFilter, Filter, InFilter, NeqFilter, NotInFilter
 from .measure import (
     BaseMeasure,
     CalcParam,
     Calculator,
     CustomCalculator,
     DependantMeasure,
@@ -22,17 +23,19 @@
 
 __all__ = [
     "AggRequest",
     "ComputeRequest",
     "aggregation_ops",
     "FRTBDataSet",
     "DataSet",
+    "DataSource",
     "DS",
     "NoDataError",
     "OtherError",
+    "UltimaError",
     "EqFilter",
     "NeqFilter",
     "InFilter",
     "NotInFilter",
     "Filter",
     "Measure",
     "BaseMeasure",
```

### Comparing `ultibi-0.3.4/ultibi/internals/dataset.py` & `ultibi-0.4.0/ultibi/internals/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,84 @@
 from __future__ import annotations
 
-from typing import Any, Type, TypeVar
+from typing import Any, Type, TypeVar, no_type_check
 
 import polars as pl
 
 import ultibi.internals as uli
+from ultibi.internals.filters import AnyFilter
 from ultibi.internals.measure import Measure
 
 from ..rust_module.ultibi_engine import DataSetWrapper
 
 TMeasure = TypeVar("TMeasure", bound=Measure)
 
 
 # Create a generic variable that can be 'Parent', or any subclass.
 DS = TypeVar("DS", bound="DataSet")
 
 
 class DataSet:
     """
-    Main DataSet class
+    Main DataSet class. Holds data source info, optionally validates and prepares Data,
+     and executes request.
+
+    Creation:
+        Preffer `DataSet.from_source`
+        `DataSet.from_config_path`
+        `DataSet.from_frame`
+
+    Examples
+    --------
+    Usage:
+
+    >>> import ultibi as ul
+    >>> import polars as pl
+    >>> df = pl.DataFrame(
+    ...     {
+    ...         "a": [1, 2, -3],
+    ...         "b": [4, 5, 6],
+    ...         "c": ["z", "z", "w"],
+    ...         "d": ["k", "y", "s"],
+    ...     }
+    ... )
+    >>> ds = ul.DataSet.from_frame(df)
+    >>> request = dict(
+    ...     measures=[["a", "sum"], ["b", "max"]],
+    ...     groupby=["c"],
+    ...     filters=[  # c==a OR b in (5,6)
+    ...         [
+    ...             {"op": "Eq", "field": "c", "value": "z"},
+    ...             {"op": "In", "field": "b", "value": ["6", "5"]},
+    ...         ],
+    ...         # AND k!=c
+    ...         [{"op": "Neq", "field": "d", "value": "y"}],
+    ...     ],
+    ...     overrides=[
+    ...         {
+    ...             "field": "a",
+    ...             "value": "100",
+    ...             "filters": [
+    ...                 [{"op": "Eq", "field": "b", "value": "4"}],
+    ...             ],
+    ...         }
+    ...     ],
+    ... )
+    >>> result = ds.compute(request)
 
-    Holds data, optionally validates and prepares Data,
-     and finally executes request.
     """
 
     inner: DataSetWrapper
-    prepared: bool
 
-    def __init__(self, ds: DataSetWrapper, prepared: bool = False) -> None:
+    def __init__(self, ds: DataSetWrapper) -> None:
         """
         Class constructor - not to br called directly.
         call .from_frame() or .from_config()
         """
         self.inner = ds
-        self.prepared = prepared
 
         """All column which you can group by. Currently those are string 
             and bool columns
         """
         self.fields: list[str] = self.inner.fields()
 
         """{measureName: "aggtype restriction(if any, otherwise
@@ -54,39 +95,34 @@
             passed to the request, "hint": type hint of the param}
         """
         self.calc_params: "list[tuple[str, str|None, str|None]]" = (
             self.inner.calc_params()
         )
 
     @classmethod
-    def from_config_path(
-        cls: Type[DS], path: str, collect: bool = True, prepare: bool = False
-    ) -> DS:
+    def from_config_path(cls: Type[DS], path: str) -> DS:
         """
         Reads path to <config>.toml
         Converts into DataSourceConfig
         Builds DataSet from DataSourceConfig
 
         Args:
             path (str): path to <config>.toml
-            collect (str): non-lazy evaluation
-            prepare (str): calls prepare
 
         Returns:
             T: Self
         """
-        return cls(DataSetWrapper.from_config_path(path, collect, prepare), prepare)
+        return cls(DataSetWrapper.from_config_path(path))
 
     @classmethod
     def from_frame(
         cls: Type[DS],
         df: pl.DataFrame,
         measures: "list[str] | None" = None,
         build_params: "dict[str, str] | None" = None,
-        prepared: bool = True,
         bespoke_measures: "list[TMeasure] | None" = None,
     ) -> DS:
         """
         Build DataSet directly from df
 
         Args:
             cls (Type[T]): _description_
@@ -103,49 +139,64 @@
             T: Self
         """
         bespoke_measures = (
             [m.inner for m in bespoke_measures] if bespoke_measures else None
         )
         return cls(
             DataSetWrapper.from_frame(df, measures, build_params, bespoke_measures),
-            prepared,
+        )
+
+    @classmethod
+    def from_source(
+        cls: Type[DS],
+        ds: uli.DataSource,
+        measures: "list[str] | None" = None,
+        build_params: "dict[str, str] | None" = None,
+        bespoke_measures: "list[TMeasure] | None" = None,
+    ) -> DS:
+        bespoke_measures = (
+            [m.inner for m in bespoke_measures] if bespoke_measures else None
+        )
+        return cls(
+            DataSetWrapper.from_source(
+                ds.inner, measures, build_params, bespoke_measures
+            ),
         )
 
     def prepare(self, collect: bool = True) -> None:
         """Does nothing unless overriden. To be used for one of computations.
             eg Weights Assignments
+            #TODO throws exception if Scan or DB
 
         Args:
             collect (cool): non-lazy mode. Evaluates.
 
         Raises:
             OtherError: Calling prepare on an already prepared dataset
         """
-        if not self.prepared:
-            self.inner.prepare(collect)
-            self.prepared = True
-        else:
-            raise uli.OtherError("Calling prepare on an already prepared dataset")
+        self.inner.prepare(collect)
 
     def validate(self) -> None:
         """Raises:
            uli.NoDataError: Calling prepare on an already prepared dataset
 
         Note: If you can guarantee your particular calculation would not require
         the missing columns you can proceed at your own risk!
         """
         self.inner.validate()
 
-    def frame(self) -> pl.DataFrame:
-        vec_srs = self.inner.frame()
+    @no_type_check
+    def frame(self, fltrs: "list[list[AnyFilter]] | None" = None) -> pl.DataFrame:
+        "Use with caution. The returned frame might be very large"
+        if fltrs is not None:  # extract inner
+            fltrs = [[a_fltr.inner for a_fltr in or_fltrs] for or_fltrs in fltrs]
+        vec_srs = self.inner.frame(fltrs)
         return pl.DataFrame(vec_srs)
 
-    def compute(
-        self, req: "dict[Any, Any]|uli.ComputeRequest", streaming: bool = False
-    ) -> pl.DataFrame:
+    def compute(self, req: "dict[Any, Any]|uli.ComputeRequest") -> pl.DataFrame:
         """Make sure that requested groupby and filters exist in self.columns,
         Make sure that requested measures exist in self.measures
         Make sure that aggregation type for a measure is selected properly
 
         Args:
             req (dict[Any, Any]|uli.ComputeRequest): Request, to be converted
                 into AggRequest.
@@ -156,53 +207,43 @@
         Returns:
             pl.DataFrame: If your request and data were constructed properly.
         """
 
         if isinstance(req, dict):
             req = uli.ComputeRequest(req)
 
-        vec_srs = self.inner.compute(req._ar, streaming)
+        vec_srs = self.inner.compute(req._ar)
 
         return pl.DataFrame(vec_srs)
 
-    def execute(
-        self, req: "dict[Any, Any]|uli.ComputeRequest", streaming: bool = False
-    ) -> pl.DataFrame:
-        from warnings import warn
-
-        warn("use .compute() instead")
-        return self.compute(req, streaming)
-
     def ui(self) -> None:
         """Spins up a localhost.
         You can control level of logging and the address like this:
         >>> import os
         >>> os.environ["RUST_LOG"] = "info"
         >>> os.environ["ADDRESS"] = "0.0.0.0:8000"
         """
         # Streaming mode calls prepare on each request
         # If already prepared we don't want to call it again
-        streaming = not self.prepared
-        self.inner.ui(streaming)
+        self.inner.ui()
 
 
 class FRTBDataSet(DataSet):
     """FRTB flavour of DataSet"""
 
     @classmethod
     def from_config_path(
-        cls: Type[DS], path: str, collect: bool = True, prepare: bool = False
+        cls: Type[DS], path: str, bespoke_measures: "list[TMeasure] | None" = None
     ) -> DS:
-        return cls(
-            DataSetWrapper.frtb_from_config_path(path, collect, prepare), prepare
-        )
+        return cls(DataSetWrapper.frtb_from_config_path(path, bespoke_measures))
 
     @classmethod
     def from_frame(
         cls: Type[DS],
         df: pl.DataFrame,
         measures: "list[str] | None" = None,
         build_params: "dict[str, str] | None" = None,
-        prepared: bool = False,
         bespoke_measures: "list[TMeasure] | None" = None,
     ) -> DS:
-        return cls(DataSetWrapper.frtb_from_frame(df, measures, build_params), prepared)
+        return cls(
+            DataSetWrapper.frtb_from_frame(df, measures, build_params, bespoke_measures)
+        )
```

### Comparing `ultibi-0.3.4/ultibi/internals/filters.py` & `ultibi-0.4.0/ultibi/internals/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import json
-from typing import Any
+from typing import Any, TypeVar
 
 from ..rust_module.ultibi_engine import FilterWrapper
 
+# Create a generic variable that can be 'Parent', or any subclass.
+AnyFilter = TypeVar("AnyFilter", bound="Filter")
+
 
 class Filter:
     """
     This is Filter to be applied on the data with your request
 
     Examples
     --------
```

### Comparing `ultibi-0.3.4/ultibi/internals/requests.py` & `ultibi-0.4.0/ultibi/internals/requests.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.4/Cargo.lock` & `ultibi-0.4.0/Cargo.lock`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [[package]]
 name = "actix-codec"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "617a8268e3537fe1d8c9ead925fca49ef6400927ee7bc26750e90ecee14ce4b8"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "bytes",
  "futures-core",
  "futures-sink",
  "memchr",
  "pin-project-lite",
  "tokio",
  "tokio-util",
@@ -26,15 +26,15 @@
 checksum = "d832782fac6ca7369a70c9ee9a20554623c5e51c76e190ad151780ebea1cf689"
 dependencies = [
  "actix-http",
  "actix-service",
  "actix-utils",
  "actix-web",
  "askama_escape",
- "bitflags",
+ "bitflags 1.3.2",
  "bytes",
  "derive_more",
  "futures-core",
  "http-range",
  "log",
  "mime",
  "mime_guess",
@@ -50,15 +50,15 @@
 dependencies = [
  "actix-codec",
  "actix-rt",
  "actix-service",
  "actix-utils",
  "ahash 0.8.3",
  "base64 0.21.2",
- "bitflags",
+ "bitflags 1.3.2",
  "brotli",
  "bytes",
  "bytestring",
  "derive_more",
  "encoding_rs",
  "flate2",
  "futures-core",
@@ -79,20 +79,20 @@
  "tokio-util",
  "tracing",
  "zstd",
 ]
 
 [[package]]
 name = "actix-macros"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "465a6172cf69b960917811022d8f29bc0b7fa1398bc4f78b3c466673db1213b6"
+checksum = "e01ed3140b2f8d422c68afa1ed2e85d996ea619c988ac834d255db32138655cb"
 dependencies = [
  "quote",
- "syn 1.0.109",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "actix-router"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d66ff4d247d2b160861fa2866457e85706833527840e4133f8f49aa423a38799"
@@ -123,15 +123,15 @@
  "actix-rt",
  "actix-service",
  "actix-utils",
  "futures-core",
  "futures-util",
  "mio",
  "num_cpus",
- "socket2",
+ "socket2 0.4.9",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "actix-service"
 version = "2.0.2"
@@ -185,16 +185,16 @@
  "once_cell",
  "pin-project-lite",
  "regex",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "smallvec",
- "socket2",
- "time 0.3.22",
+ "socket2 0.4.9",
+ "time 0.3.23",
  "url",
 ]
 
 [[package]]
 name = "actix-web-codegen"
 version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -230,14 +230,23 @@
  "actix-web",
  "derive_more",
  "futures-util",
  "static-files",
 ]
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
@@ -283,14 +292,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -314,73 +329,88 @@
  "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
+checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "anstyle-wincon"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
+
+[[package]]
+name = "argminmax"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "202108b46429b765ef483f8a24d5c46f48c14acfdacc086dd4ab6dddf6bcdbd2"
+dependencies = [
+ "num-traits",
+]
 
 [[package]]
 name = "array-init-cursor"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
 
 [[package]]
+name = "arrayvec"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
+
+[[package]]
 name = "arrow-format"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07884ea216994cdc32a2d5f8274a8bee979cfe90274b83f86f440866ee3132c7"
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15ae0428d69ab31d7b2adad22a752d6f11fef2e901d2262d0cad4f5cb08b7093"
+checksum = "e44f27e89e3edd8738a07c5e2c881efaa25e69be97a816d2df051685d460670c"
 dependencies = [
  "ahash 0.8.3",
  "arrow-format",
  "bytemuck",
  "chrono",
  "dyn-clone",
  "either",
@@ -389,35 +419,37 @@
  "futures",
  "getrandom",
  "hash_hasher",
  "lexical-core",
  "lz4",
  "multiversion",
  "num-traits",
+ "regex",
+ "regex-syntax 0.6.29",
  "rustc_version",
  "simdutf8",
  "strength_reduce",
  "zstd",
 ]
 
 [[package]]
 name = "askama_escape"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "619743e34b5ba4e9703bba34deac3427c72507c7159f5fd030aea8cac0cfe341"
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "cc6dde6e4ed435a4c1ee4e73592f5ba9da2151af10076cc04858746af9352d09"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -459,15 +491,15 @@
  "aws-smithy-types",
  "aws-types",
  "bytes",
  "hex",
  "http",
  "hyper",
  "ring",
- "time 0.3.22",
+ "time 0.3.23",
  "tokio",
  "tower",
  "tracing",
  "zeroize",
 ]
 
 [[package]]
@@ -600,15 +632,15 @@
  "form_urlencoded",
  "hex",
  "http",
  "once_cell",
  "percent-encoding",
  "regex",
  "ring",
- "time 0.3.22",
+ "time 0.3.23",
  "tracing",
 ]
 
 [[package]]
 name = "aws-smithy-async"
 version = "0.49.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -648,15 +680,15 @@
 checksum = "ec39585f8274fa543ad5c63cc09cbd435666be16b2cf99e4e07be5cf798bc050"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-http-tower",
  "aws-smithy-types",
  "bytes",
- "fastrand",
+ "fastrand 1.9.0",
  "http",
  "http-body",
  "hyper",
  "hyper-rustls",
  "lazy_static",
  "pin-project-lite",
  "tokio",
@@ -736,15 +768,15 @@
 version = "0.49.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e93b0c93a3b963da946a0b8ef3853a7252298eb75cdbfb21dad60f5ed0ded861"
 dependencies = [
  "itoa",
  "num-integer",
  "ryu",
- "time 0.3.22",
+ "time 0.3.23",
 ]
 
 [[package]]
 name = "aws-smithy-xml"
 version = "0.49.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36b9efb4855b4acb29961a776d45680f3cbdd7c4783cbbae078da54c342575dd"
@@ -765,41 +797,149 @@
  "http",
  "rustc_version",
  "tracing",
  "zeroize",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
+name = "bigdecimal"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6773ddc0eafc0e509fb60e48dff7f450f8e674a0686ae8605e8d9901bd5eefa"
+dependencies = [
+ "num-bigint",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "bindgen"
+version = "0.59.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2bd2a9a458e8f4304c52c43ebb0cfbd520289f8379a52e329a38afda99bf8eb8"
+dependencies = [
+ "bitflags 1.3.2",
+ "cexpr",
+ "clang-sys",
+ "lazy_static",
+ "lazycell",
+ "peeking_take_while",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "rustc-hash",
+ "shlex",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
+
+[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
+name = "borsh"
+version = "0.10.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4114279215a005bc675e386011e594e1d9b800918cea18fcadadcce864a2046b"
+dependencies = [
+ "borsh-derive",
+ "hashbrown 0.13.2",
+]
+
+[[package]]
+name = "borsh-derive"
+version = "0.10.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0754613691538d51f329cce9af41d7b7ca150bc973056f1156611489475f54f7"
+dependencies = [
+ "borsh-derive-internal",
+ "borsh-schema-derive-internal",
+ "proc-macro-crate",
+ "proc-macro2",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "borsh-derive-internal"
+version = "0.10.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "afb438156919598d2c7bad7e1c0adf3d26ed3840dbc010db1a882a65583ca2fb"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "borsh-schema-derive-internal"
+version = "0.10.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "634205cc43f74a1b9046ef87c4540ebda95696ec0f315024860cad7c5b0f5ccd"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "brotli"
 version = "3.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1a0b1dbcc8ae29329621f8d4f0d835787c1c38bb1401979b49d13b0b305ff68"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
@@ -813,20 +953,48 @@
 checksum = "4b6561fd3f895a11e8f72af2cb7d22e08366bebc2b6b57f7744c4bda27034744"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
+name = "bufstream"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "40e38929add23cdf8a366df9b0e088953150724bcbe5fc330b0d8eb3b328eec8"
+
+[[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
+name = "bytecheck"
+version = "0.6.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b6372023ac861f6e6dc89c8344a8f398fb42aaba2b5dbc649ca0c0e9dbcb627"
+dependencies = [
+ "bytecheck_derive",
+ "ptr_meta",
+ "simdutf8",
+]
+
+[[package]]
+name = "bytecheck_derive"
+version = "0.6.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a7ec4c6f261935ad534c0c22dbef2201b45918860eb1c574b972bd213a76af61"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 dependencies = [
  "bytemuck_derive",
 ]
@@ -835,15 +1003,15 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
@@ -879,14 +1047,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 dependencies = [
  "jobserver",
 ]
 
 [[package]]
+name = "cexpr"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+dependencies = [
+ "nom",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "change-detection"
@@ -938,87 +1115,130 @@
 checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
+name = "clang-sys"
+version = "1.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c688fc74432808e3eb684cae8830a86be1d66a2bd58e1f248ed0960a590baf6f"
+dependencies = [
+ "glob",
+ "libc",
+ "libloading",
+]
+
+[[package]]
 name = "clap"
-version = "4.3.5"
+version = "4.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2686c4115cb0810d9a984776e197823d08ec94f176549a89a9efded477c456dc"
+checksum = "5fd304a20bff958a57f04c4e96a2e7594cc4490a0e809cbd48bb6437edaa452d"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.5"
+version = "4.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e53afce1efce6ed1f633cf0e57612fe51db54a1ee4fd8f8503d078fe02d69ae"
+checksum = "01c6a3f08f1fe5662a35cfe393aec09c4df95f60ee93b7556505260f75eee9e1"
 dependencies = [
  "anstream",
  "anstyle",
- "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.2"
+version = "4.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
+checksum = "54a9bb5758fc5dfe728d1019941681eccaf0cf8a4189b692a0ee2f2ecf90a050"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
+name = "cmake"
+version = "0.1.50"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "comfy-table"
-version = "6.2.0"
+version = "7.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e959d788268e3bf9d35ace83e81b124190378e4c91c9067524675e33394b8ba"
+checksum = "9ab77dbd8adecaf3f0db40581631b995f312a8a5ae3aa9993188bb8f23d83a5b"
 dependencies = [
  "crossterm",
  "strum",
- "strum_macros",
+ "strum_macros 0.24.3",
  "unicode-width",
 ]
 
 [[package]]
+name = "connectorx"
+version = "0.3.2-alpha.7"
+source = "git+https://github.com/AnatolyBuga/connector-x.git?branch=polars_dtype_u8#c5a559e77b7c4848e2a21f09b180bca41991438d"
+dependencies = [
+ "anyhow",
+ "chrono",
+ "fehler",
+ "itertools",
+ "log",
+ "mysql_common",
+ "num-traits",
+ "owning_ref",
+ "polars",
+ "r2d2",
+ "r2d2_mysql",
+ "rayon",
+ "rust_decimal",
+ "serde_json",
+ "sqlparser 0.11.0",
+ "thiserror",
+ "url",
+]
+
+[[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
 name = "cookie"
 version = "0.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e859cd57d0710d9e06c381b550c06e76992472a8c6d527aecd2fc673dcc231fb"
 dependencies = [
  "percent-encoding",
- "time 0.3.22",
+ "time 0.3.23",
  "version_check",
 ]
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1032,17 +1252,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32c"
 version = "0.6.3"
@@ -1058,14 +1278,28 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "crossbeam"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2801af0d36612ae591caa9568261fddce32ce6e08a7275ea334a06a4ad021a2c"
+dependencies = [
+ "cfg-if",
+ "crossbeam-channel",
+ "crossbeam-deque",
+ "crossbeam-epoch",
+ "crossbeam-queue",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-channel"
 version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
@@ -1092,29 +1326,39 @@
  "cfg-if",
  "crossbeam-utils",
  "memoffset",
  "scopeguard",
 ]
 
 [[package]]
+name = "crossbeam-queue"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d1cfb3ea8a53f37c40dea2c7bedcbd88bdfae54f5e2175d6ecaff1c988353add"
+dependencies = [
+ "cfg-if",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-utils"
 version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossterm"
 version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a84cda67535339806297f1b331d6dd6320470d2a0fe65381e79ee9e156dd3d13"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "crossterm_winapi",
  "libc",
  "mio",
  "parking_lot 0.12.1",
  "signal-hook",
  "signal-hook-mio",
  "winapi",
@@ -1146,20 +1390,20 @@
 checksum = "c1a816186fa68d9e426e3cb4ae4dff1fcd8e4a2c34b781bf7a822574a0d0aac8"
 dependencies = [
  "sct",
 ]
 
 [[package]]
 name = "dashmap"
-version = "5.4.0"
+version = "5.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+checksum = "6943ae99c34386c84a470c499d3414f66502a41340aa895406e0d2e4a207b91d"
 dependencies = [
  "cfg-if",
- "hashbrown 0.12.3",
+ "hashbrown 0.14.0",
  "lock_api",
  "once_cell",
  "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "derivative"
@@ -1182,21 +1426,33 @@
  "proc-macro2",
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "derive_utils"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "20ce151e1b790e3e36d767ae57691240feafe8b605e1c2fe081183d64ac1bff3"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.27",
+]
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
+ "subtle",
 ]
 
 [[package]]
 name = "dirs"
 version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
@@ -1219,43 +1475,43 @@
 name = "dotenv"
 version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77c90badedccf4105eca100756a0b1289e191f6fcbdadd3cee1d2f614f97da8f"
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+checksum = "304e6508efa593091e97a9abbc10f90aa7ca635b6d2784feff3c89d41dd12272"
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.11"
+version = "0.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f36e95862220b211a6e2aa5eca09b4fa391b13cd52ceb8035a24bf65a79de2"
+checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44533bbbb3bb3c1fa17d9f2e4e38bbbaf8396ba82193c4cb1b6445d711445d36"
@@ -1264,22 +1520,28 @@
  "humantime",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -1291,14 +1553,20 @@
 [[package]]
 name = "ethnum"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0198b9d0078e0f30dedc7acbb21c974e838fc8fae3ee170128658a98cb2c1c04"
 
 [[package]]
+name = "fallible-iterator"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4443176a9f2c162692bd3d352d745ef9413eec5782a80d8fd6f8a1ac692a07f7"
+
+[[package]]
 name = "fast-float"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
 
 [[package]]
 name = "fastrand"
@@ -1306,20 +1574,47 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
+name = "fastrand"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6999dc1837253364c2ebb0704ba97994bd874e8f195d665c50b7548f6ea92764"
+
+[[package]]
+name = "fehler"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5729fe49ba028cd550747b6e62cd3d841beccab5390aa398538c31a2d983635"
+dependencies = [
+ "fehler-macros",
+]
+
+[[package]]
+name = "fehler-macros"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ccb5acb1045ebbfa222e2c50679e392a71dd77030b78fb0189f2d9c5974400f9"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "flate2"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
+ "libz-sys",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1353,15 +1648,15 @@
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frtb_engine"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "log",
  "ndarray",
  "once_cell",
  "polars",
  "rayon",
  "serde",
@@ -1369,14 +1664,72 @@
  "smartstring",
  "strum",
  "ultibi",
  "yearfrac",
 ]
 
 [[package]]
+name = "frunk"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "11a351b59e12f97b4176ee78497dff72e4276fb1ceb13e19056aca7fa0206287"
+dependencies = [
+ "frunk_core",
+ "frunk_derives",
+ "frunk_proc_macros",
+]
+
+[[package]]
+name = "frunk_core"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af2469fab0bd07e64ccf0ad57a1438f63160c69b2e57f04a439653d68eb558d6"
+
+[[package]]
+name = "frunk_derives"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fa992f1656e1707946bbba340ad244f0814009ef8c0118eb7b658395f19a2e"
+dependencies = [
+ "frunk_proc_macro_helpers",
+ "quote",
+ "syn 2.0.27",
+]
+
+[[package]]
+name = "frunk_proc_macro_helpers"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "35b54add839292b743aeda6ebedbd8b11e93404f902c56223e51b9ec18a13d2c"
+dependencies = [
+ "frunk_core",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.27",
+]
+
+[[package]]
+name = "frunk_proc_macros"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "71b85a1d4a9a6b300b41c05e8e13ef2feca03e0334127f29eca9506a7fe13a93"
+dependencies = [
+ "frunk_core",
+ "frunk_proc_macro_helpers",
+ "quote",
+ "syn 2.0.27",
+]
+
+[[package]]
+name = "funty"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
+
+[[package]]
 name = "futures"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -1424,15 +1777,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1481,32 +1834,38 @@
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap",
+ "indexmap 1.9.3",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -1522,22 +1881,35 @@
 checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+dependencies = [
+ "ahash 0.7.6",
+]
 
 [[package]]
 name = "hashbrown"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
  "ahash 0.8.3",
+]
+
+[[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+dependencies = [
+ "ahash 0.8.3",
+ "allocator-api2",
  "rayon",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1550,34 +1922,43 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
+name = "hmac"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
+dependencies = [
+ "digest",
+]
+
+[[package]]
+name = "home"
+version = "0.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
 name = "http"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
@@ -1620,30 +2001,30 @@
 checksum = "df004cfca50ef23c36850aaaa59ad52cc70d0e90243c3c7737a4dd32dc7a3c4f"
 dependencies = [
  "quick-error",
 ]
 
 [[package]]
 name = "hyper"
-version = "0.14.26"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2",
+ "socket2 0.4.9",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -1717,14 +2098,25 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
  "serde",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.0",
+ "serde",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "instant"
@@ -1732,47 +2124,54 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.11"
+name = "io-enum"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
+checksum = "5305557fa27b460072ae15ce07617e999f5879f14d376c8449f0bfb9f9d8e91e"
 dependencies = [
- "hermit-abi 0.3.1",
- "libc",
- "windows-sys 0.48.0",
+ "derive_utils",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "ipnet"
-version = "2.7.2"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
+ "hermit-abi 0.3.2",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys",
+]
+
+[[package]]
+name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jemalloc-sys"
 version = "0.5.3+5.3.0-patched"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9bd5d616ea7ed58b571b2e209a65759664d7fb021a0819d7a790afc67e47ca1"
 dependencies = [
@@ -1817,14 +2216,20 @@
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
+name = "lazycell"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
+
+[[package]]
 name = "lexical"
 version = "6.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7aefb36fd43fef7003334742cbf77b243fcd36418a1d1bdd480d613a67968f6"
 dependencies = [
  "lexical-core",
 ]
@@ -1891,17 +2296,27 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
+
+[[package]]
+name = "libloading"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
+dependencies = [
+ "cfg-if",
+ "winapi",
+]
 
 [[package]]
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
@@ -1912,18 +2327,29 @@
 checksum = "f4ac0e912c8ef1b735e92369695618dc5b1819f5a7bf3f167301a3ba1cea515e"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
+name = "libz-sys"
+version = "1.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
+dependencies = [
+ "cc",
+ "pkg-config",
+ "vcpkg",
+]
+
+[[package]]
 name = "linux-raw-sys"
-version = "0.3.8"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
 
 [[package]]
 name = "local-channel"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f303ec0e94c6c54447f84f3b0ef7af769858a9c4ef56ef2a986d3dcd4c3fc9c"
 dependencies = [
@@ -1952,14 +2378,23 @@
 [[package]]
 name = "log"
 version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
+name = "lru"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6e8aaa3f231bb4bd57b84b2d5dc3ae7f350265df8aa96492e0bc394a1571909"
+dependencies = [
+ "hashbrown 0.12.3",
+]
+
+[[package]]
 name = "lz4"
 version = "1.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
 dependencies = [
  "libc",
  "lz4-sys",
@@ -2043,14 +2478,20 @@
 checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
+name = "minimal-lexical"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
+
+[[package]]
 name = "miniz_oxide"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
@@ -2060,15 +2501,15 @@
 version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "multiversion"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cda45dade5144c2c929bf2ed6c24bebbba784e9198df049ec87d722b9462bd1"
@@ -2086,14 +2527,87 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "target-features",
 ]
 
 [[package]]
+name = "mysql"
+version = "23.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f11339ca5c251941805d51362a07823605a80586ced92914ab7de84fba813f"
+dependencies = [
+ "bufstream",
+ "bytes",
+ "crossbeam",
+ "flate2",
+ "io-enum",
+ "libc",
+ "lru",
+ "mysql_common",
+ "named_pipe",
+ "native-tls",
+ "once_cell",
+ "pem",
+ "percent-encoding",
+ "serde",
+ "serde_json",
+ "socket2 0.4.9",
+ "twox-hash",
+ "url",
+]
+
+[[package]]
+name = "mysql_common"
+version = "0.29.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9006c95034ccf7b903d955f210469119f6c3477fc9c9e7a7845ce38a3e665c2a"
+dependencies = [
+ "base64 0.13.1",
+ "bigdecimal",
+ "bindgen",
+ "bitflags 1.3.2",
+ "bitvec",
+ "byteorder",
+ "bytes",
+ "cc",
+ "chrono",
+ "cmake",
+ "crc32fast",
+ "flate2",
+ "frunk",
+ "lazy_static",
+ "lexical",
+ "num-bigint",
+ "num-traits",
+ "rand",
+ "regex",
+ "rust_decimal",
+ "saturating",
+ "serde",
+ "serde_json",
+ "sha1",
+ "sha2",
+ "smallvec",
+ "subprocess",
+ "thiserror",
+ "time 0.3.23",
+ "uuid",
+]
+
+[[package]]
+name = "named_pipe"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad9c443cce91fc3e12f017290db75dde490d685cdaaf508d7159d7cf41f0eb2b"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
 dependencies = [
  "lazy_static",
  "libc",
@@ -2119,14 +2633,24 @@
  "num-traits",
  "rawpointer",
  "rayon",
  "serde",
 ]
 
 [[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
 name = "now"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d89e9874397a1f0a52fc1f197a8effd9735223cb2390e9dcc83ac6cd02923d0"
 dependencies = [
  "chrono",
 ]
@@ -2137,14 +2661,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "num-bigint"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-complex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
@@ -2157,45 +2692,54 @@
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi 0.3.2",
  "libc",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "openssl"
-version = "0.10.54"
+version = "0.10.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
+checksum = "345df152bc43501c5eb9e4654ff05f794effb78d4efe3d53abc158baddc0703d"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -2204,36 +2748,45 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.88"
+version = "0.9.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2ce0f250f34a308dcfdbb351f511359857d4ed2134ba715a4eadd46e1ffd617"
+checksum = "374533b0e45f3a7ced10fcaeccca020e66656bc03dac384f852e4e5a7a8104a6"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
+name = "owning_ref"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6ff55baddef9e4ad00f88b6c743a2a8062d4c6ade126c2a528644b8e444d52ce"
+dependencies = [
+ "stable_deref_trait",
+]
+
+[[package]]
 name = "parking_lot"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
  "instant",
  "lock_api",
@@ -2275,17 +2828,17 @@
  "redox_syscall 0.3.5",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "path-matchers"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36cd9b72a47679ec193a5f0229d9ab686b7bd45e1fbc59ccf953c9f3d83f7b2b"
 dependencies = [
@@ -2295,44 +2848,77 @@
 [[package]]
 name = "path-slash"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "498a099351efa4becc6a19c72aa9270598e8fd274ca47052e37455241c88b696"
 
 [[package]]
+name = "peeking_take_while"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
+
+[[package]]
+name = "pem"
+version = "1.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a8835c273a76a90455d7344889b0964598e3316e2a79ede8e36f16bdcf2228b8"
+dependencies = [
+ "base64 0.13.1",
+]
+
+[[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
+name = "phf"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
+dependencies = [
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
+dependencies = [
+ "siphasher",
+]
+
+[[package]]
 name = "pin-project"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -2349,56 +2935,57 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8f04742abbadbd348d73a803617e6df61464485a410361e9c6634e55a4bc01c"
+checksum = "7e072ca6b1c26e686b18d86b607a17b1f8baa5fb0a713a1fefe033f0aa527bfd"
 dependencies = [
  "getrandom",
  "polars-core",
  "polars-io",
  "polars-lazy",
  "polars-ops",
+ "polars-sql",
  "polars-time",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eacd179fe0cc7cf18e12a80cfda3e6d15ce907655203cc69277e883a925f9bd8"
+checksum = "d52f7b885c589dd7184c881be3dfb149feb1f405083fdd2fd9194e8f96104b76"
 dependencies = [
  "arrow2",
- "hashbrown 0.13.2",
+ "hashbrown 0.14.0",
  "multiversion",
  "num-traits",
  "polars-error",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04145d95791f31a0df3b2d3d600cbb5d0d43ccc105d74e871ffe7351a5e70cbe"
+checksum = "9f98d6b1ef5362f76063b4984634d371de72f4834f50892944d48fd7b7d5ae45"
 dependencies = [
  "ahash 0.8.3",
  "arrow2",
- "bitflags",
+ "bitflags 1.3.2",
  "chrono",
  "comfy-table",
  "either",
- "hashbrown 0.13.2",
- "indexmap",
+ "hashbrown 0.14.0",
+ "indexmap 2.0.0",
  "ndarray",
  "num-traits",
  "once_cell",
  "polars-arrow",
  "polars-error",
  "polars-row",
  "polars-utils",
@@ -2411,37 +2998,37 @@
  "thiserror",
  "wasm-timer",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fc2fb4ff74f7224b4096b3551b309c50bfd49bb0b66fb3948e70feffb1a8e51"
+checksum = "b1557cd24b1865194bac6979765cfec5e97ecd8af5dcb7858a17b31d1e7fbf70"
 dependencies = [
  "arrow2",
  "regex",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4d186157d427b39085f812e74eefb04608b7bd033ef3a7f848b93a5939c396d"
+checksum = "c44b1c6d7b2c04e459effb93bac050f90762687cb752c534967476c452478a65"
 dependencies = [
  "ahash 0.8.3",
  "arrow2",
  "async-trait",
  "bytes",
  "chrono",
- "dirs",
  "fast-float",
  "futures",
+ "home",
  "lexical",
  "lexical-core",
  "memchr",
  "memmap2",
  "num-traits",
  "once_cell",
  "polars-arrow",
@@ -2454,106 +3041,127 @@
  "serde",
  "simdutf8",
  "tokio",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "385b1beb0ae4f1c8fbe6aef9769b8e0a22a8b56ba494e382f17de82ce653702f"
+checksum = "494f1e75a035978339b06bdcc4d60523ec347243ac65f11794a7eeaba0507d4e"
 dependencies = [
  "ahash 0.8.3",
- "bitflags",
+ "bitflags 1.3.2",
  "glob",
+ "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-pipe",
  "polars-plan",
  "polars-time",
  "polars-utils",
  "rayon",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8beae89044ad6f5a2237103852d2650c7a52e7b339e356c1d707b9427b48ba7"
+checksum = "06dd95bc84a7bf17886670420097c5fb8b88906ebb16653153ce5f0cf71ffd6e"
 dependencies = [
+ "argminmax",
  "arrow2",
  "either",
+ "indexmap 2.0.0",
  "memchr",
  "polars-arrow",
  "polars-core",
  "polars-utils",
  "serde",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59c7fbda6ff77db1ae1a0d8f210b9729b2c0cb7c584345504a8282e3bd38e97d"
+checksum = "ff34c8f09c064ab26bc9283c13b6a1571083c30c4c3812301cd84cdd3982a2e0"
 dependencies = [
  "crossbeam-channel",
+ "crossbeam-queue",
  "enum_dispatch",
- "hashbrown 0.13.2",
+ "hashbrown 0.14.0",
  "num-traits",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-plan",
  "polars-row",
  "polars-utils",
  "rayon",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11b788cb03c651c9b92c2293b0adc07cb89ae64d7f187310cb7d62d688ccd9d8"
+checksum = "58f0837dac2b7064e04a2a37a2bff20f75a455d23b29f2dd82f0345de62d3bfb"
 dependencies = [
  "ahash 0.8.3",
  "arrow2",
  "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-time",
  "polars-utils",
  "rayon",
+ "regex",
  "serde",
  "smartstring",
+ "strum_macros 0.25.1",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bfcd216b7953321a6946c38d352fdfa67260a4d2125cbb4a1c3b46f03d0bebb"
+checksum = "46235f6f67005fff3fd8095b994e86f846b5affd6fc6f36f41099a4dbc27d714"
 dependencies = [
  "arrow2",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
+name = "polars-sql"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7f716671c8e8ed1db6ebdbfcc7ca0c98a599e92c340747c24072b86e8839bed"
+dependencies = [
+ "polars-arrow",
+ "polars-core",
+ "polars-lazy",
+ "polars-plan",
+ "serde",
+ "serde_json",
+ "sqlparser 0.34.0",
+]
+
+[[package]]
 name = "polars-time"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5384945cc104ba99683455760dcfe1048e4025bfaf78043e14450cc8c988a745"
+checksum = "02488938edfbff6efed56a4f90ebd6574ea16a7d32b6dc678134624031f7f3e9"
 dependencies = [
  "arrow2",
  "atoi",
  "chrono",
  "now",
  "once_cell",
  "polars-arrow",
@@ -2563,25 +3171,71 @@
  "regex",
  "serde",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.28.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c1823141ed08322d17e9717ddf652c42df92f0d9b0c52cc5a242c96bc845144"
+checksum = "69f04f6c127b8d20292b4d49b5fb0e47c652875b316274f74f52e77d50f6a459"
 dependencies = [
+ "ahash 0.8.3",
+ "hashbrown 0.14.0",
+ "num-traits",
  "once_cell",
  "rayon",
  "smartstring",
  "sysinfo",
 ]
 
 [[package]]
+name = "postgres"
+version = "0.19.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0bed5017bc2ff49649c0075d0d7a9d676933c1292480c1d137776fb205b5cd18"
+dependencies = [
+ "bytes",
+ "fallible-iterator",
+ "futures-util",
+ "log",
+ "tokio",
+ "tokio-postgres",
+]
+
+[[package]]
+name = "postgres-protocol"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "78b7fa9f396f51dffd61546fd8573ee20592287996568e6175ceb0f8699ad75d"
+dependencies = [
+ "base64 0.21.2",
+ "byteorder",
+ "bytes",
+ "fallible-iterator",
+ "hmac",
+ "md-5",
+ "memchr",
+ "rand",
+ "sha2",
+ "stringprep",
+]
+
+[[package]]
+name = "postgres-types"
+version = "0.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f028f05971fe20f512bcc679e2c10227e57809a3af86a7606304435bc8896cd6"
+dependencies = [
+ "bytes",
+ "fallible-iterator",
+ "postgres-protocol",
+]
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "pretty_env_logger"
@@ -2590,14 +3244,23 @@
 checksum = "926d36b9553851b8b0005f1275891b392ee4d2d833852c417ed025477350fb9d"
 dependencies = [
  "env_logger",
  "log",
 ]
 
 [[package]]
+name = "proc-macro-crate"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1d6ea3c4595b96363c13943497db34af4460fb474a95c43f4446ad341b8c9785"
+dependencies = [
+ "toml 0.5.11",
+]
+
+[[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
@@ -2615,112 +3278,158 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "ptr_meta"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0738ccf7ea06b608c10564b31debd4f5bc5e197fc8bfe088f68ae5ce81e7a4f1"
+dependencies = [
+ "ptr_meta_derive",
+]
+
+[[package]]
+name = "ptr_meta_derive"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "16b845dbfca988fa33db069c0e230574d15a3088f147a87b64c7589eb662c9ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyultima"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "ciborium",
  "frtb_engine",
  "once_cell",
  "polars",
- "polars-arrow",
  "pyo3",
  "serde_json",
  "thiserror",
  "ultibi",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "r2d2"
+version = "0.8.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51de85fb3fb6524929c8a2eb85e6b6d363de4e8c48f9e2c2eac4944abc181c93"
+dependencies = [
+ "log",
+ "parking_lot 0.12.1",
+ "scheduled-thread-pool",
+]
+
+[[package]]
+name = "r2d2_mysql"
+version = "23.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9733d738ce65959a744f387bae69aa690a867e18d48e5486b171c47bc7b0c575"
+dependencies = [
+ "mysql",
+ "r2d2",
+]
+
+[[package]]
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
@@ -2786,24 +3495,24 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
@@ -2811,28 +3520,55 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax 0.7.4",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.4",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
+
+[[package]]
+name = "rend"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "581008d2099240d37fb08d77ad713bcaec2c4d89d50b5b21a8bb1996bbab68ab"
+dependencies = [
+ "bytecheck",
+]
 
 [[package]]
 name = "reqwest"
 version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
@@ -2879,69 +3615,127 @@
  "spin",
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
+name = "rkyv"
+version = "0.7.42"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0200c8230b013893c0b2d6213d6ec64ed2b9be2e0e016682b7224ff82cff5c58"
+dependencies = [
+ "bitvec",
+ "bytecheck",
+ "hashbrown 0.12.3",
+ "ptr_meta",
+ "rend",
+ "rkyv_derive",
+ "seahash",
+ "tinyvec",
+ "uuid",
+]
+
+[[package]]
+name = "rkyv_derive"
+version = "0.7.42"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2e06b915b5c230a17d7a736d1e2e63ee753c256a8614ef3f5147b13a4f5541d"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "rust-embed"
-version = "6.7.0"
+version = "6.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b73e721f488c353141288f223b599b4ae9303ecf3e62923f40a492f0634a4dc3"
+checksum = "a36224c3276f8c4ebc8c20f158eca7ca4359c8db89991c4925132aaaf6702661"
 dependencies = [
  "rust-embed-impl",
  "rust-embed-utils",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-impl"
-version = "6.6.0"
+version = "6.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e22ce362f5561923889196595504317a4372b84210e6e335da529a65ea5452b5"
+checksum = "49b94b81e5b2c284684141a2fb9e2a31be90638caf040bf9afbc5a0416afe1ac"
 dependencies = [
  "proc-macro2",
  "quote",
  "rust-embed-utils",
  "shellexpand",
- "syn 2.0.18",
+ "syn 2.0.27",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-utils"
-version = "7.5.0"
+version = "7.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "512b0ab6853f7e14e3c8754acb43d6f748bb9ced66aa5915a6553ac8213f7731"
+checksum = "9d38ff6bf570dc3bb7100fce9f7b60c33fa71d80e88da3f2580df4ff2bdded74"
 dependencies = [
  "sha2",
  "walkdir",
 ]
 
 [[package]]
+name = "rust_decimal"
+version = "1.30.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d0446843641c69436765a35a5a77088e28c2e6a12da93e84aa3ab1cd4aa5a042"
+dependencies = [
+ "arrayvec",
+ "borsh",
+ "bytecheck",
+ "byteorder",
+ "bytes",
+ "num-traits",
+ "postgres",
+ "rand",
+ "rkyv",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.38.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
 dependencies = [
- "bitflags",
+ "bitflags 2.3.3",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35edb675feee39aec9c99fa5ff985081995a06d594114ae14cbe797ad7b7a6d7"
@@ -2963,123 +3757,144 @@
  "rustls",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "saturating"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ece8e78b2f38ec51c51f5d475df0a7187ba5111b2a28bdc761ee05b075d40a71"
+
+[[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
+name = "scheduled-thread-pool"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "3cbc66816425a074528352f5789333ecff06ca41b36b0b0efdfbb29edc391a19"
 dependencies = [
- "windows-sys 0.42.0",
+ "parking_lot 0.12.1",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "sct"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b362b83898e0e69f38515b82ee15aa80636befe47c3b6d3d89a911e78fc228ce"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
+name = "seahash"
+version = "4.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
+
+[[package]]
 name = "security-framework"
-version = "2.9.1"
+version = "2.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
+checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.0"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
+checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.174"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "3b88756493a5bd5e5395d53baa70b194b05764ab85b59e43e4b8f4e1192fa9b1"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.174"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "6e5c3a298c7f978e53536f95a63bdc4c4a64550582f31a0359a9afda6aede62e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.97"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.2"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93107647184f6027e3b7dcb2e11034cf95ffa1e3a682c67951963ac69c1c007d"
+checksum = "96426c9936fd7a0124915f9185ea1d20aa9445cc9821142f0a73bc9207a2e186"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -3120,18 +3935,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ccc8076840c4da029af4f87e4e8daeb0fca6b87bbb02e10cb60b791450e11e4"
 dependencies = [
  "dirs",
 ]
 
 [[package]]
+name = "shlex"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
+
+[[package]]
 name = "signal-hook"
-version = "0.3.15"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "732768f1176d21d09e076c23a93123d40bba92d50c4058da34d45c8de8e682b9"
+checksum = "8621587d4798caf8eb44879d42e56b9a93ea5dcd315a6487c357130095b62801"
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-mio"
@@ -3156,27 +3977,33 @@
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
+name = "siphasher"
+version = "0.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+
+[[package]]
 name = "slab"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
@@ -3193,20 +4020,54 @@
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "socket2"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2538b18701741680e0322a2302176d3253a35388e2e62f172f64f4f16605f877"
+dependencies = [
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
+name = "sqlparser"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "10e1ce16b71375ad72d28d111131069ce0d5f8603f4f86d8acd3456b41b57a51"
+dependencies = [
+ "log",
+]
+
+[[package]]
+name = "sqlparser"
+version = "0.34.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "37d3706eefb17039056234df6b566b0014f303f867f2656108334a55b8096f59"
+dependencies = [
+ "log",
+]
+
+[[package]]
+name = "stable_deref_trait"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
+
+[[package]]
 name = "static-files"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64712ea1e3e140010e1d9605872ba205afa2ab5bd38191cc6ebd248ae1f6a06b"
 dependencies = [
  "change-detection",
  "mime_guess",
@@ -3222,26 +4083,36 @@
 [[package]]
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
+name = "stringprep"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3737bde7edce97102e0e2b15365bf7a20bfdb5f60f4f9e8d7004258a51a8da"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "strum"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "063e6045c0e62079840579a7e47a355ae92f60eb74daaf156fb1e84ba164e63f"
 dependencies = [
- "strum_macros",
+ "strum_macros 0.24.3",
 ]
 
 [[package]]
 name = "strum_macros"
 version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
@@ -3250,78 +4121,112 @@
  "proc-macro2",
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "strum_macros"
+version = "0.25.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6069ca09d878a33f883cc06aaa9718ede171841d3832450354410b718b097232"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 2.0.27",
+]
+
+[[package]]
+name = "subprocess"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2e86926081dda636c546d8c5e641661049d7562a68f5488be4a1f7f66f6086"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
+name = "subtle"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.28.4"
+version = "0.29.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4c2f3ca6693feb29a89724516f016488e9aafc7f37264f898593ee4b942f31b"
+checksum = "c7cb97a5a85a136d84e75d5c3cf89655090602efb1be0d8d5337b7e386af2908"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "winapi",
 ]
 
 [[package]]
+name = "tap"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
+
+[[package]]
 name = "target-features"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06f6b473c37f9add4cf1df5b4d66a8ef58ab6c895f1a3b3f949cf3e21230140e"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "tempfile"
-version = "3.6.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+checksum = "5486094ee78b2e5038a6382ed7645bc084dc2ec433426ca4c3cb61e2007b8998"
 dependencies = [
- "autocfg",
  "cfg-if",
- "fastrand",
+ "fastrand 2.0.0",
  "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "template_drivers"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "actix-files",
  "actix-web",
  "actix-web-httpauth",
  "actix-web-static-files",
  "anyhow",
  "clap",
@@ -3333,15 +4238,15 @@
  "pretty_env_logger",
  "reqwest",
  "serde",
  "serde_json",
  "static-files",
  "thiserror",
  "tokio",
- "toml",
+ "toml 0.7.6",
  "tracing",
  "ultibi",
  "uuid",
 ]
 
 [[package]]
 name = "termcolor"
@@ -3350,30 +4255,30 @@
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "thread-tree"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ffbd370cb847953a25954d9f63e14824a36113f8c72eecf6eccef5dc4b45d630"
@@ -3390,17 +4295,17 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.22"
+version = "0.3.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+checksum = "59e399c068f43a5d116fedaf73b203fa4f9c519f17e2b34f63221d3792f81446"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
@@ -3408,17 +4313,17 @@
 name = "time-core"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+checksum = "96ba15a897f3c86766b757e5ac7221554c6750054d74d5b28844fce5fb36a6c4"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
@@ -3432,53 +4337,78 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2",
+ "socket2 0.4.9",
  "tokio-macros",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
+name = "tokio-postgres"
+version = "0.7.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e89f6234aa8fd43779746012fcf53603cdb91fdd8399aa0de868c2d56b6dde1"
+dependencies = [
+ "async-trait",
+ "byteorder",
+ "bytes",
+ "fallible-iterator",
+ "futures-channel",
+ "futures-util",
+ "log",
+ "parking_lot 0.12.1",
+ "percent-encoding",
+ "phf",
+ "pin-project-lite",
+ "postgres-protocol",
+ "postgres-types",
+ "socket2 0.5.3",
+ "tokio",
+ "tokio-util",
+]
+
+[[package]]
 name = "tokio-rustls"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc6844de72e57df1980054b38be3a9f4702aba4858be64dd700181a8a6d0e1b6"
 dependencies = [
  "rustls",
  "tokio",
@@ -3508,40 +4438,49 @@
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "toml"
-version = "0.7.4"
+version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6135d499e69981f9ff0ef2167955a5333c35e36f6937d382974566b3d5b94ec"
+checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "toml"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c17e963a819c331dcacd7ab957d80bc2b9a9c1e71c804826d2f283dd65306542"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.2"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
+checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.10"
+version = "0.19.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
+checksum = "f8123f27e969974a3dfba720fdb560be359f57b44302d280ba72e76a74480e8a"
 dependencies = [
- "indexmap",
+ "indexmap 2.0.0",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
@@ -3583,21 +4522,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.25"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8803eee176538f94ae9a14b55b2804eb7e1441f8210b1c31290b3bccdccff73b"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -3608,50 +4547,62 @@
 [[package]]
 name = "try-lock"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
 
 [[package]]
+name = "twox-hash"
+version = "1.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
+dependencies = [
+ "cfg-if",
+ "rand",
+ "static_assertions",
+]
+
+[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ultibi"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "ultibi_core",
  "ultibi_server",
 ]
 
 [[package]]
 name = "ultibi_core"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "aws-config",
  "aws-sdk-s3",
+ "connectorx",
  "dashmap",
  "derivative",
  "futures",
  "once_cell",
  "polars",
  "quote",
  "serde",
  "serde_json",
  "thiserror",
  "tokio",
- "toml",
+ "toml 0.7.6",
  "utoipa",
 ]
 
 [[package]]
 name = "ultibi_server"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "actix-web",
  "actix-web-static-files",
  "anyhow",
  "dotenv",
  "log",
  "mime",
@@ -3679,17 +4630,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -3723,68 +4674,71 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "urlencoding"
-version = "2.1.2"
+version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
+checksum = "daf8dba3b7eb870caf1ddeed7bc9d2a049f3cfdfae7cb521b087cc33ae4c49da"
 
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "utoipa"
 version = "3.3.0"
-source = "git+https://github.com/juhaku/utoipa#1774bb708c15dafcf34f28c0ec8b5b093dece7a9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68ae74ef183fae36d650f063ae7bde1cacbe1cd7e72b617cbe1e985551878b98"
 dependencies = [
- "indexmap",
+ "indexmap 1.9.3",
  "serde",
  "serde_json",
  "utoipa-gen",
 ]
 
 [[package]]
 name = "utoipa-gen"
 version = "3.3.0"
-source = "git+https://github.com/juhaku/utoipa#1774bb708c15dafcf34f28c0ec8b5b093dece7a9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7ea8ac818da7e746a63285594cce8a96f5e00ee31994e655bd827569cb8b137b"
 dependencies = [
  "lazy_static",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "utoipa-swagger-ui"
-version = "3.1.3"
-source = "git+https://github.com/juhaku/utoipa#1774bb708c15dafcf34f28c0ec8b5b093dece7a9"
+version = "3.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4602d7100d3cfd8a086f30494e68532402ab662fa366c9d201d677e33cee138d"
 dependencies = [
  "actix-web",
  "mime_guess",
  "regex",
  "rust-embed",
  "serde",
  "serde_json",
  "utoipa",
  "zip",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.4"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
+checksum = "79daa5ed5740825c40b389c5e50312b9c86df53fccd33f281df655642b43869d"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
@@ -3845,15 +4799,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3879,15 +4833,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -3967,154 +4921,106 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.4.7"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca0ace3845f0d96209f0375e6d367e3eb87eb65d27d445bdc9f1843a26f39448"
+checksum = "81fac9742fd1ad1bd9643b991319f72dd031016d44b77039a26977eb667141e7"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "wyz"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+dependencies = [
+ "tap",
+]
+
+[[package]]
 name = "xmlparser"
 version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "114ba2b24d2167ef6d67d7d04c8cc86522b87f490025f39f0303b7db5bf5e3d8"
 
 [[package]]
 name = "xxhash-rust"
@@ -4148,26 +5054,26 @@
  "crc32fast",
  "crossbeam-utils",
  "flate2",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.12.3+zstd.1.5.2"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
+checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.5+zstd.1.5.4"
+version = "6.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
+checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
```

### Comparing `ultibi-0.3.4/PKG-INFO` & `ultibi-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ultibi
-Version: 0.3.4
+Version: 0.4.0
 Classifier: Programming Language :: Rust
-Classifier: License :: Free for non-commercial use
+Classifier: License :: Free To Use But Restricted
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polars
-Requires-Dist: pyarrow
+Requires-Dist: polars >=0.18.7
 License-File: LICENSE
 Summary: Flexible DataFrame Operations via UI
 Keywords: dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-table,frtb,risk
 Author-email: Anatoly Bugakov <anatoly@ultimabi.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://ultimabi.uk/
-Project-URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book
 Project-URL: Documentation, https://ultimabi.uk/ultibi-frtb-book/
+Project-URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book
 
 <br>
 
 <p align="center">
     <a href="https://ultimabi.uk/" target="_blank">
     <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/logo.png" alt="Ultima Logo">
     </a>
@@ -64,22 +63,24 @@
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
 
 # Read Data
 # for more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html
 df = pl.read_csv("titanic.csv")
 
 # Convert it into an Ultibi DataSet
-ds = ul.DataSet.from_frame(df, bespoke_measures=measures)
+ds = ul.DataSet.from_frame(df)
 
 # By default (might change in the future)
 # Fields are Utf8 (non numerics) and integers
 # Measures are numeric columns.
 ds.ui() 
 ```
 
+Then navigate to `http://localhost:8000` or checkout `http://localhost:8000/swagger-ui` for the OpenAPI documentation.
+
 ### More flexible - custom measures
 ```python
 import ultibi as ul
 import polars as pl
 import os
 os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
@@ -156,12 +157,40 @@
 
 # By default (might change in the future)
 # Fields are Utf8 (non numerics) and integers
 # Measures are numeric columns.
 ds.ui() 
 ```
 
-Then navigate to `http://localhost:8000` or checkout `http://localhost:8000/swagger-ui` for the OpenAPI documentation.
+### DataSources
+We provide aim to support different sources of the data. 
+```python
+scan = pl.read_csv("../frtb_engine/data/frtb/Delta.csv", 
+                           dtypes={"SensitivitySpot": pl.Float64})
+dsource = ul.DataSource.inmemory(scan)
+ds = ul.DataSet.from_source(dsource)
+ds.prepare() # .prepare() is only relevant to FRTB dataset currently
+ds.ui()
+```
+If you don't want to/can't hold all your data in the process memory, you can sacrifise performance for memory with Scan/DataBase
+```python
+import polars as pl
+import ultibi as ul
+# Note that the LazyFrame query must start with scan_
+# and must've NOT been collected
+scan = pl.scan_csv("../frtb_engine/data/frtb/Delta.csv", 
+                    dtypes={"SensitivitySpot": pl.Float64})
+dsource = ul.DataSource.scan(scan)
+ds = ul.DataSet.from_source(dsource)
+ds.ui()
+```
+
+Note: Naturally the later two options will be slower, because prior to computing your measures we will need to read the relevant bits of the data into the process memory. 
 
 ### FRTB SA
 [FRTB SA](https://en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a great usecase for `ultibi`. FRTB SA is a set of standardised, computationally intensive rules established by the regulator. High business impact of these rules manifests in need for **analysis** and **visibility** thoroughout an organisation. Note: Ultima is not a certified aggregator. Always benchmark the results against your own interpretation of the rules.
 See python frtb [userguide](https://ultimabi.uk/ultibi-frtb-book/).
+
+### License 
+`ultibi` python library is made available exclusively for the purpose of demonstrating the possibilities offered by the Software so users can evaluate the possibilities and potential of the Software. You may use the library for non comercial, non for profit activity. You may not use this library in production, but you can purchase an alternative license for doing so. 
+
+Our `licenses` are extremely affordable, and you can check out the options by reaching out to us directly, via anatoly at ultimabi dot uk.
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ultibi Version: 0.3.4 Classifier: Programming
-Language :: Rust Classifier: License :: Free for non-commercial use Classifier:
+Metadata-Version: 2.1 Name: ultibi Version: 0.4.0 Classifier: Programming
+Language :: Rust Classifier: License :: Free To Use But Restricted Classifier:
 Topic :: Scientific/Engineering Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polars Requires-Dist: pyarrow License-File: LICENSE Summary:
-Flexible DataFrame Operations via UI Keywords:
+Requires-Dist: polars >=0.18.7 License-File: LICENSE Summary: Flexible
+DataFrame Operations via UI Keywords:
 dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-
 table,frtb,risk Author-email: Anatoly Bugakov
 ultimabi.uk> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: Homepage, https://ultimabi.uk/ Project-
-URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book Project-URL:
-Documentation, https://ultimabi.uk/ultibi-frtb-book/
+URL: Documentation, https://ultimabi.uk/ultibi-frtb-book/ Project-URL:
+Repository, https://github.com/ultima-ib/ultibi-frtb-book
                                  [Ultima_Logo]
 
                     **** the ultimate data analytics tool
          for no code visualisation and collaborative exploration. ****
          **** Present easier.   Dig deeper.   Review together.   ****
 # The Ultimate BI tool With `Ultibi` you can turn your `DataFrame` into a pivot
 table with a UI and share it across organisation. You can also define measures
@@ -27,53 +27,72 @@
 We use TypeScript for the frontend. # Examples Our userguide is under
 development. In the mean time refer to FRTB [userguide](https://ultimabi.uk/
 ultibi-frtb-book/). ## Python ### Quickstart ```python import ultibi as ul
 import polars as pl import os os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address # Read Data # for
 more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/
 polars.read_csv.html df = pl.read_csv("titanic.csv") # Convert it into an
-Ultibi DataSet ds = ul.DataSet.from_frame(df, bespoke_measures=measures) # By
-default (might change in the future) # Fields are Utf8 (non numerics) and
-integers # Measures are numeric columns. ds.ui() ``` ### More flexible - custom
-measures ```python import ultibi as ul import polars as pl import os os.environ
-["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] = "0.0.0.0:8000" #
-host on this address # Read Data # for more details: https://pola-rs.github.io/
-polars/py-polars/html/reference/api/polars.read_csv.html df = pl.read_csv
-("titanic.csv") # Let's add some Custom/Bespoke Calculations to our UI #
-Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -> pl.Expr:
-"""Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age") * pl.col
-("survived") - age of survived person, otherwise 0 pl.col("survived").sum() -
-number of survived """ return pl.col("age") * pl.col("survived") / pl.col
-("survived").sum() # Also a Standard Calculator def example_dep_calc(kwargs:
-dict[str, str]) -> pl.Expr: return pl.col("SurvivalMeanAge_sum") + pl.col
-("SouthamptonFareDivAge_sum") # When we need more involved calculations we go
-for a Custom Calculator def custom_calculator( srs: list[pl.Series], kwargs:
-dict[str, str] ) -> pl.Series: """ Southampton Fare/Age*multiplier """ df =
-pl.DataFrame({"age": srs[0], "fare": srs[1], "e": srs[2]}) # Add Indicator
-Column for Southampton df = df.with_columns(pl.when(pl.col("e")=="S").then
-(1).otherwise(0).alias("S")) multiplier = float(kwargs.get("multiplier", 1))
-res = df["S"] * df["fare"] / df["age"] * multiplier return res # inputs for the
-custom_calculator srs param inputs = ["age", "fare", "embarked"] # We return
-Floats res_type = pl.Float64 # We return a Series, not a scalar (which
-otherwise would be auto exploded) returns_scalar = False measures =
-[ ul.BaseMeasure( "SouthamptonFareDivAge", ul.CustomCalculator
-( custom_calculator, res_type, inputs, returns_scalar ), # (Optional) - we are
-only interested in Southampton, so # unless other measures requested we might
-as well filter for Southampton only # However, if if multiple measures
-requested, their precompute_filters will be joined as OR. [[ul.EqFilter
-("embarked", "S")]], # PARAMS tab of the UI calc_params=[ul.CalcParam("mltplr",
-"1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge", ul.StandardCalculator
-(survival_mean_age), aggregation_restriction="sum", ), ul.DependantMeasure
-( "A_Dependant_Measure", ul.StandardCalculator(example_dep_calc), [
-("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge", "sum")], ), ] # Convert
-it into an Ultibi DataSet ds = ul.DataSet.from_frame(df,
-bespoke_measures=measures) # By default (might change in the future) # Fields
-are Utf8 (non numerics) and integers # Measures are numeric columns. ds.ui()
-``` Then navigate to `http://localhost:8000` or checkout `http://localhost:
-8000/swagger-ui` for the OpenAPI documentation. ### FRTB SA [FRTB SA](https://
+Ultibi DataSet ds = ul.DataSet.from_frame(df) # By default (might change in the
+future) # Fields are Utf8 (non numerics) and integers # Measures are numeric
+columns. ds.ui() ``` Then navigate to `http://localhost:8000` or checkout
+`http://localhost:8000/swagger-ui` for the OpenAPI documentation. ### More
+flexible - custom measures ```python import ultibi as ul import polars as pl
+import os os.environ["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] =
+"0.0.0.0:8000" # host on this address # Read Data # for more details: https://
+pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html df =
+pl.read_csv("titanic.csv") # Let's add some Custom/Bespoke Calculations to our
+UI # Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -
+> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age")
+* pl.col("survived") - age of survived person, otherwise 0 pl.col
+("survived").sum() - number of survived """ return pl.col("age") * pl.col
+("survived") / pl.col("survived").sum() # Also a Standard Calculator def
+example_dep_calc(kwargs: dict[str, str]) -> pl.Expr: return pl.col
+("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") # When we need
+more involved calculations we go for a Custom Calculator def custom_calculator
+( srs: list[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton
+Fare/Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e":
+srs[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
+(pl.col("e")=="S").then(1).otherwise(0).alias("S")) multiplier = float
+(kwargs.get("multiplier", 1)) res = df["S"] * df["fare"] / df["age"] *
+multiplier return res # inputs for the custom_calculator srs param inputs =
+["age", "fare", "embarked"] # We return Floats res_type = pl.Float64 # We
+return a Series, not a scalar (which otherwise would be auto exploded)
+returns_scalar = False measures = [ ul.BaseMeasure( "SouthamptonFareDivAge",
+ul.CustomCalculator( custom_calculator, res_type, inputs, returns_scalar ), #
+(Optional) - we are only interested in Southampton, so # unless other measures
+requested we might as well filter for Southampton only # However, if if
+multiple measures requested, their precompute_filters will be joined as OR. [
+[ul.EqFilter("embarked", "S")]], # PARAMS tab of the UI calc_params=
+[ul.CalcParam("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
+ul.StandardCalculator(survival_mean_age), aggregation_restriction="sum", ),
+ul.DependantMeasure( "A_Dependant_Measure", ul.StandardCalculator
+(example_dep_calc), [("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge",
+"sum")], ), ] # Convert it into an Ultibi DataSet ds = ul.DataSet.from_frame
+(df, bespoke_measures=measures) # By default (might change in the future) #
+Fields are Utf8 (non numerics) and integers # Measures are numeric columns.
+ds.ui() ``` ### DataSources We provide aim to support different sources of the
+data. ```python scan = pl.read_csv("../frtb_engine/data/frtb/Delta.csv",
+dtypes={"SensitivitySpot": pl.Float64}) dsource = ul.DataSource.inmemory(scan)
+ds = ul.DataSet.from_source(dsource) ds.prepare() # .prepare() is only relevant
+to FRTB dataset currently ds.ui() ``` If you don't want to/can't hold all your
+data in the process memory, you can sacrifise performance for memory with Scan/
+DataBase ```python import polars as pl import ultibi as ul # Note that the
+LazyFrame query must start with scan_ # and must've NOT been collected scan =
+pl.scan_csv("../frtb_engine/data/frtb/Delta.csv", dtypes={"SensitivitySpot":
+pl.Float64}) dsource = ul.DataSource.scan(scan) ds = ul.DataSet.from_source
+(dsource) ds.ui() ``` Note: Naturally the later two options will be slower,
+because prior to computing your measures we will need to read the relevant bits
+of the data into the process memory. ### FRTB SA [FRTB SA](https://
 en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a great
 usecase for `ultibi`. FRTB SA is a set of standardised, computationally
 intensive rules established by the regulator. High business impact of these
 rules manifests in need for **analysis** and **visibility** thoroughout an
 organisation. Note: Ultima is not a certified aggregator. Always benchmark the
 results against your own interpretation of the rules. See python frtb
-[userguide](https://ultimabi.uk/ultibi-frtb-book/).
+[userguide](https://ultimabi.uk/ultibi-frtb-book/). ### License `ultibi` python
+library is made available exclusively for the purpose of demonstrating the
+possibilities offered by the Software so users can evaluate the possibilities
+and potential of the Software. You may use the library for non comercial, non
+for profit activity. You may not use this library in production, but you can
+purchase an alternative license for doing so. Our `licenses` are extremely
+affordable, and you can check out the options by reaching out to us directly,
+via anatoly at ultimabi dot uk.
```

