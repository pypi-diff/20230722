# Comparing `tmp/wtfis-0.6.1.tar.gz` & `tmp/wtfis-0.6.2.tar.gz`

## Comparing `wtfis-0.6.1.tar` & `wtfis-0.6.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wtfis-0.6.1/.env.wtfis.example
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wtfis-0.6.1/.flake8
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 wtfis-0.6.1/Dockerfile
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 wtfis-0.6.1/Makefile
--rw-r--r--   0        0        0    80106 2020-02-02 00:00:00.000000 wtfis-0.6.1/imgs/demo.gif
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 wtfis-0.6.1/imgs/example-greynoise.png
--rw-r--r--   0        0        0   112584 2020-02-02 00:00:00.000000 wtfis-0.6.1/imgs/example-no-color.png
--rw-r--r--   0        0        0   120658 2020-02-02 00:00:00.000000 wtfis-0.6.1/imgs/example-one-column.png
--rw-r--r--   0        0        0    96341 2020-02-02 00:00:00.000000 wtfis-0.6.1/imgs/example-shodan.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_cli.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_clients.py
--rw-r--r--   0        0        0    14739 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_handlers.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_models_vt.py
--rw-r--r--   0        0        0    44104 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_ui_domain_view.py
--rw-r--r--   0        0        0    18953 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_ui_ip_view.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_utils.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/greynoise_1.1.1.1.json
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/greynoise_1.1.1.1_malicious.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/greynoise_1.1.1.1_unknown.json
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/greynoise_one.json
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/ip2whois_whois_bbc.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/ip2whois_whois_hotmail.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/ipwhois_1.1.1.1.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/ipwhois_gist.json
--rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/pt_whois_1.1.1.1.json
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/pt_whois_gist.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/shodan_1.1.1.1.json
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/shodan_gist.json
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/shodan_gist_2.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/shodan_one.json
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/shodan_wired.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_domain_gist.json
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_domain_google.json
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_domain_tucows.json
--rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_ip_1.1.1.1.json
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_ip_142.251.220.110.json
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_resolutions_gist.json
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_resolutions_one.json
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_resolutions_wired.json
--rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_whois_1.1.1.1.json
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_whois_bbc.json
--rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_whois_example.json
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_whois_example_2.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_whois_foo.json
--rw-r--r--   0        0        0    18644 2020-02-02 00:00:00.000000 wtfis-0.6.1/tests/test_data/vt_whois_gist.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/__init__.py
--rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/main.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/__init__.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/base.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/greynoise.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/ip2whois.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/ipwhois.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/passivetotal.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/shodan.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/clients/virustotal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/handlers/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/handlers/base.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/handlers/domain.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/handlers/ip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/common.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/greynoise.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/ip2whois.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/ipwhois.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/passivetotal.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/shodan.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/models/virustotal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/ui/__init__.py
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/ui/base.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/ui/progress.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/ui/theme.py
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 wtfis-0.6.1/wtfis/ui/view.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 wtfis-0.6.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.6.1/LICENSE
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 wtfis-0.6.1/README.md
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 wtfis-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 wtfis-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wtfis-0.6.2/.env.wtfis.example
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wtfis-0.6.2/.flake8
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 wtfis-0.6.2/Dockerfile
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 wtfis-0.6.2/Makefile
+-rw-r--r--   0        0        0    80106 2020-02-02 00:00:00.000000 wtfis-0.6.2/imgs/demo.gif
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 wtfis-0.6.2/imgs/example-greynoise.png
+-rw-r--r--   0        0        0   112584 2020-02-02 00:00:00.000000 wtfis-0.6.2/imgs/example-no-color.png
+-rw-r--r--   0        0        0   120658 2020-02-02 00:00:00.000000 wtfis-0.6.2/imgs/example-one-column.png
+-rw-r--r--   0        0        0    96341 2020-02-02 00:00:00.000000 wtfis-0.6.2/imgs/example-shodan.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/conftest.py
+-rw-r--r--   0        0        0    16656 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_cli.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_clients.py
+-rw-r--r--   0        0        0    14885 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_handlers.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_models_vt.py
+-rw-r--r--   0        0        0    44226 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_ui_domain_view.py
+-rw-r--r--   0        0        0    19012 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_ui_ip_view.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_utils.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/greynoise_1.1.1.1.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/greynoise_1.1.1.1_malicious.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/greynoise_1.1.1.1_unknown.json
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/greynoise_one.json
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/ip2whois_whois_bbc.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/ip2whois_whois_hotmail.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/ipwhois_1.1.1.1.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/ipwhois_gist.json
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/pt_whois_1.1.1.1.json
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/pt_whois_gist.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/shodan_1.1.1.1.json
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/shodan_gist.json
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/shodan_gist_2.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/shodan_one.json
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/shodan_wired.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_domain_gist.json
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_domain_google.json
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_domain_tucows.json
+-rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_ip_1.1.1.1.json
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_ip_142.251.220.110.json
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_resolutions_gist.json
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_resolutions_one.json
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_resolutions_wired.json
+-rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_whois_1.1.1.1.json
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_whois_bbc.json
+-rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_whois_example.json
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_whois_example_2.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_whois_foo.json
+-rw-r--r--   0        0        0    18644 2020-02-02 00:00:00.000000 wtfis-0.6.2/tests/test_data/vt_whois_gist.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/__init__.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/main.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/__init__.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/base.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/greynoise.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/ip2whois.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/ipwhois.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/passivetotal.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/shodan.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/clients/virustotal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/handlers/__init__.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/handlers/base.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/handlers/domain.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/handlers/ip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/common.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/greynoise.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/ip2whois.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/ipwhois.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/passivetotal.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/shodan.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/models/virustotal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/ui/__init__.py
+-rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/ui/base.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/ui/progress.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/ui/theme.py
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 wtfis-0.6.2/wtfis/ui/view.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 wtfis-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.6.2/LICENSE
+-rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 wtfis-0.6.2/README.md
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 wtfis-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 wtfis-0.6.2/PKG-INFO
```

### Comparing `wtfis-0.6.1/Dockerfile` & `wtfis-0.6.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/imgs/demo.gif` & `wtfis-0.6.2/imgs/demo.gif`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/imgs/example-greynoise.png` & `wtfis-0.6.2/imgs/example-greynoise.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/imgs/example-no-color.png` & `wtfis-0.6.2/imgs/example-no-color.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/imgs/example-one-column.png` & `wtfis-0.6.2/imgs/example-one-column.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/imgs/example-shodan.png` & `wtfis-0.6.2/imgs/example-shodan.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/conftest.py` & `wtfis-0.6.2/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,25 +31,25 @@
     path = Path(__file__).parent.resolve() / "test_data" / fname
     with open(path) as f:
         return f.read()
 
 
 def greynoise_get(ip, pool) -> GreynoiseIp:
     """ Mock replacement for GreynoiseClient().get_ip() """
-    return GreynoiseIp.parse_obj(pool[ip])
+    return GreynoiseIp.model_validate(pool[ip])
 
 
 def ipwhois_get(ip, pool) -> IpWhois:
     """ Mock replacement for IpWhoisClient().get_ipwhois() """
-    return IpWhois.parse_obj(pool[ip])
+    return IpWhois.model_validate(pool[ip])
 
 
 def shodan_get_ip(ip, pool) -> ShodanIp:
     """ Mock replacement for ShodanClient().get_ip() """
-    return ShodanIp.parse_obj(pool[ip])
+    return ShodanIp.model_validate(pool[ip])
 
 
 def timestamp_text(ts) -> Optional[RenderableType]:
     """ Standard timestamp formatting """
     theme = TestTheme()
     return Text(
         ts,
```

### Comparing `wtfis-0.6.1/tests/test_clients.py` & `wtfis-0.6.2/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_handlers.py` & `wtfis-0.6.2/tests/test_handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     def test_entity_refang(self, domain_handler):
         handler = domain_handler()
         assert handler.entity == "www.example.com"
 
     def test_fetch_data_1(self, domain_handler, test_data):
         """ Test with max_resolutions = 3 (default) """
         handler = domain_handler()
-        handler.resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+        handler.resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
         handler._fetch_vt_domain = MagicMock()
         handler._fetch_vt_resolutions = MagicMock()
         handler._fetch_ip_enrichments = MagicMock()
         handler._fetch_whois = MagicMock()
         handler._fetch_greynoise = MagicMock()
 
@@ -131,30 +131,30 @@
 
             # Thorough test of first _fetch_* method
             with pytest.raises(SystemExit) as e:
                 handler._fetch_vt_domain()
 
             capture = capsys.readouterr()
 
-            assert capture.err == (
+            assert capture.err.startswith(
                 "Data model validation error: 1 validation error for Domain\ndata\n"
-                "  field required (type=value_error.missing)\n"
+                "  Field required [type=missing, input_value={'intentionally': 'wrong data'}, input_type=dict]\n"
             )
             assert e.type == SystemExit
             assert e.value.code == 1
 
             # Extra: just make sure program exits correctly
             with pytest.raises(SystemExit) as e:
                 handler._fetch_vt_resolutions()
             assert e.value.code == 1
 
     @patch.object(requests.Session, "get")
     def test_ipwhois_http_error(self, mock_requests_get, domain_handler, capsys, test_data):
         handler = domain_handler()
-        handler.resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+        handler.resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
         mock_resp = requests.models.Response()
 
         mock_resp.status_code = 500
         mock_requests_get.return_value = mock_resp
 
         with pytest.raises(SystemExit) as e:
@@ -227,15 +227,15 @@
         """
         handler = domain_handler()
         mock_resp = requests.models.Response()
 
         mock_resp.status_code = 429
         mock_requests_get.return_value = mock_resp
 
-        handler.resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+        handler.resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
         handler._fetch_greynoise()
         assert handler.warnings[0].startswith("Could not fetch Greynoise: 429 Client Error:")
 
         handler.print_warnings()
         capture = capsys.readouterr()
         assert capture.out.startswith("WARN: Could not fetch Greynoise: 429 Client Error:")
@@ -244,22 +244,22 @@
     def test_greynoise_404_error(self, mock_requests_get, domain_handler, test_data):
         """
         Test fail open behavior of Greynoise when no IP found (404) and no warning message
         """
         handler = domain_handler(3)
         mock_resp = requests.models.Response()
 
-        handler.resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+        handler.resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
         mock_resp.status_code = 404
         mock_requests_get.return_value = mock_resp
 
         handler._fetch_greynoise()
         assert len(handler.warnings) == 0
-        assert handler.greynoise == GreynoiseIpMap(__root__={})
+        assert handler.greynoise == GreynoiseIpMap.model_validate({})
 
 
 class TestIpAddressHandler:
     def test_entity_refang(self, ip_handler):
         handler = ip_handler()
         assert handler.entity == "1.1.1.1"
 
@@ -306,17 +306,17 @@
 
             # Thorough test of first _fetch_* method
             with pytest.raises(SystemExit) as e:
                 handler._fetch_vt_ip_address()
 
             capture = capsys.readouterr()
 
-            assert capture.err == (
+            assert capture.err.startswith(
                 "Data model validation error: 1 validation error for IpAddress\ndata\n"
-                "  field required (type=value_error.missing)\n"
+                "  Field required [type=missing, input_value={'intentionally': 'wrong data'}, input_type=dict]\n"
             )
             assert e.type == SystemExit
             assert e.value.code == 1
 
     @patch.object(requests.Session, "get")
     def test_ipwhois_http_error(self, mock_requests_get, ip_handler, capsys, test_data):
         handler = ip_handler()
@@ -399,8 +399,8 @@
         mock_resp = requests.models.Response()
 
         mock_resp.status_code = 404
         mock_requests_get.return_value = mock_resp
 
         handler._fetch_greynoise()
         assert len(handler.warnings) == 0
-        assert handler.greynoise == GreynoiseIpMap(__root__={})
+        assert handler.greynoise == GreynoiseIpMap.model_validate({})
```

### Comparing `wtfis-0.6.1/tests/test_models_vt.py` & `wtfis-0.6.2/tests/test_models_vt.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
     Domain,
     Resolutions,
 )
 
 
 class TestVirustotalModels:
     def test_domain_1(self, test_data):
-        domain = Domain.parse_obj(json.loads(test_data("vt_domain_gist.json")))
+        domain = Domain.model_validate(json.loads(test_data("vt_domain_gist.json")))
 
         assert domain.data.id_ == "gist.github.com"
         assert domain.data.type_ == "domain"
         assert domain.data.attributes.last_analysis_stats.malicious == 0
         assert domain.data.attributes.last_analysis_stats.suspicious == 0
         assert domain.data.attributes.last_analysis_stats.harmless == 84
         assert domain.data.attributes.last_analysis_stats.undetected == 10
-        assert list(domain.data.attributes.last_analysis_results.__root__.keys())[:2] == [
+        assert list(domain.data.attributes.last_analysis_results.root.keys())[:2] == [
             "CMC Threat Intelligence",
             "Snort IP sample list",
         ]
 
     def test_resolutions_1(self, test_data):
-        res = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+        res = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
         assert res.meta.count == 37
         assert len(res.data) == 10
         assert res.data[1].attributes.ip_address == "192.30.255.113"
         assert res.data[1].attributes.ip_address_last_analysis_stats.malicious == 1
         assert res.data[1].attributes.ip_address_last_analysis_stats.suspicious == 0
         assert res.data[1].attributes.ip_address_last_analysis_stats.harmless == 82
```

### Comparing `wtfis-0.6.1/tests/test_ui_domain_view.py` & `wtfis-0.6.2/tests/test_ui_domain_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,148 +21,148 @@
 )
 from wtfis.ui.view import DomainView
 
 
 @pytest.fixture()
 def view01(test_data, mock_ipwhois_get):
     """ gist.github.com with PT whois. Complete test of all panels. Also test print(). """
-    resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+    resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
     ipwhois_pool = json.loads(test_data("ipwhois_gist.json"))
     ipwhois_client = IpWhoisClient()
     ipwhois_client.get_ipwhois = MagicMock(side_effect=lambda ip: mock_ipwhois_get(ip, ipwhois_pool))
     ip_enrich = ipwhois_client.bulk_get_ip(resolutions, 3)
 
     return DomainView(
         console=Console(),
-        entity=Domain.parse_obj(json.loads(test_data("vt_domain_gist.json"))),
+        entity=Domain.model_validate(json.loads(test_data("vt_domain_gist.json"))),
         resolutions=resolutions,
-        whois=PTWhois.parse_obj(json.loads(test_data("pt_whois_gist.json"))),
+        whois=PTWhois.model_validate(json.loads(test_data("pt_whois_gist.json"))),
         ip_enrich=ip_enrich,
-        greynoise=GreynoiseIpMap(__root__={}),
+        greynoise=GreynoiseIpMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view02(test_data):
     """
     gist.github.com VT whois. Resolution and whois tests only. Test empty enrichment
     and max_resolutions=1
     """
     return DomainView(
         console=Console(),
         entity=MagicMock(),
-        resolutions=Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json"))),
-        whois=VTWhois.parse_obj(json.loads(test_data("vt_whois_gist.json"))),
-        ip_enrich=IpWhoisMap(__root__={}),
-        greynoise=GreynoiseIpMap(__root__={}),
+        resolutions=Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json"))),
+        whois=VTWhois.model_validate(json.loads(test_data("vt_whois_gist.json"))),
+        ip_enrich=IpWhoisMap.model_validate({}),
+        greynoise=GreynoiseIpMap.model_validate({}),
         max_resolutions=1,
     )
 
 
 @pytest.fixture()
 def view03(test_data):
     """ bbc.co.uk VT whois. Whois panel test only. Test whois with no domain field. """
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
-        whois=VTWhois.parse_obj(json.loads(test_data("vt_whois_bbc.json"))),
+        whois=VTWhois.model_validate(json.loads(test_data("vt_whois_bbc.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view04(test_data):
     """
     google.com domain. Domain and resolution test only. Test domain with 1 malicious
     analysis point, and empty resolutions.
     """
     return DomainView(
         console=Console(),
-        entity=Domain.parse_obj(json.loads(test_data("vt_domain_google.json"))),
+        entity=Domain.model_validate(json.loads(test_data("vt_domain_google.json"))),
         resolutions=None,
         whois=MagicMock(),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view05(test_data):
     """ tucows.com domain. Domain test only. Test domain with negative reputation and no popularity."""
     return DomainView(
         console=Console(),
-        entity=Domain.parse_obj(json.loads(test_data("vt_domain_tucows.json"))),
+        entity=Domain.model_validate(json.loads(test_data("vt_domain_tucows.json"))),
         resolutions=MagicMock(),
         whois=MagicMock(),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view06(test_data):
     """ exmple.com VT whois. Whois test only. Test empty whois_map."""
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
-        whois=VTWhois.parse_obj(json.loads(test_data("vt_whois_example_2.json"))),
+        whois=VTWhois.model_validate(json.loads(test_data("vt_whois_example_2.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view07(test_data, mock_shodan_get_ip):
     """ gist.github.com with Shodan. Only test resolution and IP enrich. """
-    resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+    resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
     shodan_pool = json.loads(test_data("shodan_gist.json"))
     shodan_client = ShodanClient(MagicMock())
     shodan_client.get_ip = MagicMock(side_effect=lambda ip: mock_shodan_get_ip(ip, shodan_pool))
     ip_enrich = shodan_client.bulk_get_ip(resolutions, 3)
 
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=resolutions,
         whois=MagicMock(),
         ip_enrich=ip_enrich,
-        greynoise=GreynoiseIpMap(__root__={}),
+        greynoise=GreynoiseIpMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view08(test_data, mock_shodan_get_ip):
     """ www.wired.com with Shodan. Only test resolution and IP enrich. """
-    resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_wired.json")))
+    resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_wired.json")))
 
     shodan_pool = json.loads(test_data("shodan_wired.json"))
     shodan_client = ShodanClient(MagicMock())
     shodan_client.get_ip = MagicMock(side_effect=lambda ip: mock_shodan_get_ip(ip, shodan_pool))
     ip_enrich = shodan_client.bulk_get_ip(resolutions, 1)
 
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=resolutions,
         whois=MagicMock(),
         ip_enrich=ip_enrich,
-        greynoise=GreynoiseIpMap(__root__={}),
+        greynoise=GreynoiseIpMap.model_validate({}),
         max_resolutions=1,
     )
 
 
 @pytest.fixture()
 def view09(test_data, mock_shodan_get_ip, mock_greynoise_get):
     """ one.one.one.one with Shodan. Only test resolution and IP enrich. """
-    resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_one.json")))
+    resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_one.json")))
 
     shodan_pool = json.loads(test_data("shodan_one.json"))
     shodan_client = ShodanClient(MagicMock())
     shodan_client.get_ip = MagicMock(side_effect=lambda ip: mock_shodan_get_ip(ip, shodan_pool))
     ip_enrich = shodan_client.bulk_get_ip(resolutions, 1)
 
     greynoise_pool = json.loads(test_data("greynoise_one.json"))
@@ -184,61 +184,61 @@
 @pytest.fixture()
 def view10(test_data):
     """ Dummy VT whois. Whois panel test only. Test whois with no data. """
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
-        whois=VTWhois.parse_obj(json.loads(test_data("vt_whois_foo.json"))),
+        whois=VTWhois.model_validate(json.loads(test_data("vt_whois_foo.json"))),
         ip_enrich=MagicMock(),
-        greynoise=GreynoiseIpMap(__root__={}),
+        greynoise=GreynoiseIpMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view11(test_data, mock_shodan_get_ip):
     """ gist.github.com with Shodan. Only test IP enrich. Test empty open ports. """
-    resolutions = Resolutions.parse_obj(json.loads(test_data("vt_resolutions_gist.json")))
+    resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json")))
 
     shodan_pool = json.loads(test_data("shodan_gist_2.json"))
     shodan_client = ShodanClient(MagicMock())
     shodan_client.get_ip = MagicMock(side_effect=lambda ip: mock_shodan_get_ip(ip, shodan_pool))
     ip_enrich = shodan_client.bulk_get_ip(resolutions, 3)
 
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=resolutions,
         whois=MagicMock(),
         ip_enrich=ip_enrich,
-        greynoise=GreynoiseIpMap(__root__={}),
+        greynoise=GreynoiseIpMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view12(test_data):
     """ Dummy IP2WHOIS whois. Whois panel test only. """
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
-        whois=Ip2Whois.parse_obj(json.loads(test_data("ip2whois_whois_hotmail.json"))),
+        whois=Ip2Whois.model_validate(json.loads(test_data("ip2whois_whois_hotmail.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view13(test_data):
     """ Dummy IP2WHOIS whois. Whois panel test only. Test null registrant. """
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
-        whois=Ip2Whois.parse_obj(json.loads(test_data("ip2whois_whois_bbc.json"))),
+        whois=Ip2Whois.model_validate(json.loads(test_data("ip2whois_whois_bbc.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
     )
 
 
 class TestView01:
     def test_domain_panel(self, view01, display_timestamp):
```

### Comparing `wtfis-0.6.1/tests/test_ui_ip_view.py` & `wtfis-0.6.2/tests/test_ui_ip_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     greynoise_pool = json.loads(test_data("greynoise_1.1.1.1.json"))
     greynoise_client = GreynoiseClient("dummykey")
     greynoise_client.get_ip = MagicMock(side_effect=lambda ip: mock_greynoise_get(ip, greynoise_pool))
     greynoise_enrich = greynoise_client.single_get_ip(ip)
 
     return IpAddressView(
         console=Console(),
-        entity=IpAddress.parse_obj(json.loads(test_data("vt_ip_1.1.1.1.json"))),
-        whois=PTWhois.parse_obj(json.loads(test_data("pt_whois_1.1.1.1.json"))),
+        entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
+        whois=PTWhois.model_validate(json.loads(test_data("pt_whois_1.1.1.1.json"))),
         ip_enrich=ip_enrich,
         greynoise=greynoise_enrich,
     )
 
 
 @pytest.fixture()
 def view02(test_data, mock_shodan_get_ip, mock_greynoise_get):
@@ -55,62 +55,62 @@
     greynoise_pool = json.loads(test_data("greynoise_1.1.1.1.json"))
     greynoise_client = GreynoiseClient("dummykey")
     greynoise_client.get_ip = MagicMock(side_effect=lambda ip: mock_greynoise_get(ip, greynoise_pool))
     greynoise_enrich = greynoise_client.single_get_ip(ip)
 
     return IpAddressView(
         console=Console(),
-        entity=IpAddress.parse_obj(json.loads(test_data("vt_ip_1.1.1.1.json"))),
+        entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
         whois=MagicMock(),
         ip_enrich=ip_enrich,
         greynoise=greynoise_enrich,
     )
 
 
 @pytest.fixture()
 def view03(test_data):
     """ 1.1.1.1 VT whois. Whois panel test only."""
     return IpAddressView(
         console=Console(),
         entity=MagicMock(),
-        whois=VTWhois.parse_obj(json.loads(test_data("vt_whois_1.1.1.1.json"))),
+        whois=VTWhois.model_validate(json.loads(test_data("vt_whois_1.1.1.1.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view04(test_data):
     """
     142.251.220.110. Test whole IP panel with 0 malicious, 0 reputation and no IP and
     Greynoise enrichment.
     """
     return IpAddressView(
         console=Console(),
-        entity=IpAddress.parse_obj(json.loads(test_data("vt_ip_142.251.220.110.json"))),
+        entity=IpAddress.model_validate(json.loads(test_data("vt_ip_142.251.220.110.json"))),
         whois=MagicMock(),
-        ip_enrich=IpWhoisMap(__root__={}),
-        greynoise=GreynoiseIpMap(__root__={}),
+        ip_enrich=IpWhoisMap.model_validate({}),
+        greynoise=GreynoiseIpMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view05(test_data, mock_greynoise_get):
     """ 1.1.1.1 with alt Greynoise results. Test Greynoise only. """
     ip = "1.1.1.1"
     greynoise_pool = json.loads(test_data("greynoise_1.1.1.1_malicious.json"))
     greynoise_client = GreynoiseClient("dummykey")
     greynoise_client.get_ip = MagicMock(side_effect=lambda ip: mock_greynoise_get(ip, greynoise_pool))
     greynoise_enrich = greynoise_client.single_get_ip(ip)
 
     return IpAddressView(
         console=Console(),
-        entity=IpAddress.parse_obj(json.loads(test_data("vt_ip_1.1.1.1.json"))),
+        entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
         whois=MagicMock(),
-        ip_enrich=IpWhoisMap(__root__={}),
+        ip_enrich=IpWhoisMap.model_validate({}),
         greynoise=greynoise_enrich,
     )
 
 
 @pytest.fixture()
 def view06(test_data, mock_greynoise_get):
     """ 1.1.1.1 with another alt Greynoise result (unknown class). Test Greynoise only. """
@@ -118,17 +118,17 @@
     greynoise_pool = json.loads(test_data("greynoise_1.1.1.1_unknown.json"))
     greynoise_client = GreynoiseClient("dummykey")
     greynoise_client.get_ip = MagicMock(side_effect=lambda ip: mock_greynoise_get(ip, greynoise_pool))
     greynoise_enrich = greynoise_client.single_get_ip(ip)
 
     return IpAddressView(
         console=Console(),
-        entity=IpAddress.parse_obj(json.loads(test_data("vt_ip_1.1.1.1.json"))),
+        entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
         whois=MagicMock(),
-        ip_enrich=IpWhoisMap(__root__={}),
+        ip_enrich=IpWhoisMap.model_validate({}),
         greynoise=greynoise_enrich,
     )
 
 
 class TestView01:
     def test_ip_panel(self, view01, theme, display_timestamp):
         ip = view01.ip_panel()
```

### Comparing `wtfis-0.6.1/tests/test_utils.py` & `wtfis-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/ip2whois_whois_bbc.json` & `wtfis-0.6.2/tests/test_data/ip2whois_whois_bbc.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/ip2whois_whois_hotmail.json` & `wtfis-0.6.2/tests/test_data/ip2whois_whois_hotmail.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/ipwhois_1.1.1.1.json` & `wtfis-0.6.2/tests/test_data/ipwhois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/ipwhois_gist.json` & `wtfis-0.6.2/tests/test_data/ipwhois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/pt_whois_1.1.1.1.json` & `wtfis-0.6.2/tests/test_data/pt_whois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/pt_whois_gist.json` & `wtfis-0.6.2/tests/test_data/pt_whois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/shodan_1.1.1.1.json` & `wtfis-0.6.2/tests/test_data/shodan_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/shodan_gist.json` & `wtfis-0.6.2/tests/test_data/shodan_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/shodan_gist_2.json` & `wtfis-0.6.2/tests/test_data/shodan_gist_2.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/shodan_one.json` & `wtfis-0.6.2/tests/test_data/shodan_one.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/shodan_wired.json` & `wtfis-0.6.2/tests/test_data/shodan_wired.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_domain_gist.json` & `wtfis-0.6.2/tests/test_data/vt_domain_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_domain_google.json` & `wtfis-0.6.2/tests/test_data/vt_domain_google.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_domain_tucows.json` & `wtfis-0.6.2/tests/test_data/vt_domain_tucows.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_ip_1.1.1.1.json` & `wtfis-0.6.2/tests/test_data/vt_ip_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_ip_142.251.220.110.json` & `wtfis-0.6.2/tests/test_data/vt_ip_142.251.220.110.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_resolutions_gist.json` & `wtfis-0.6.2/tests/test_data/vt_resolutions_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_resolutions_one.json` & `wtfis-0.6.2/tests/test_data/vt_resolutions_one.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_resolutions_wired.json` & `wtfis-0.6.2/tests/test_data/vt_resolutions_wired.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_whois_1.1.1.1.json` & `wtfis-0.6.2/tests/test_data/vt_whois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_whois_bbc.json` & `wtfis-0.6.2/tests/test_data/vt_whois_bbc.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_whois_example.json` & `wtfis-0.6.2/tests/test_data/vt_whois_example.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_whois_example_2.json` & `wtfis-0.6.2/tests/test_data/vt_whois_example_2.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/tests/test_data/vt_whois_gist.json` & `wtfis-0.6.2/tests/test_data/vt_whois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/wtfis/main.py` & `wtfis-0.6.2/wtfis/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import argparse
 import os
 
 from argparse import Namespace
 from dotenv import load_dotenv
 from pathlib import Path
 from rich.console import Console
+from rich.progress import Progress
+from typing import Union
 
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ip2whois import Ip2WhoisClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.shodan import ShodanClient
 from wtfis.clients.virustotal import VTClient
+from wtfis.handlers.base import BaseHandler
 from wtfis.handlers.domain import DomainHandler
 from wtfis.handlers.ip import IpAddressHandler
+from wtfis.models.virustotal import Domain, IpAddress
 from wtfis.utils import error_and_exit, is_ip
+from wtfis.ui.base import BaseView
 from wtfis.ui.progress import get_progress
 from wtfis.ui.view import DomainView, IpAddressView
 from wtfis.version import get_version
 
 
 def parse_env() -> None:
     DEFAULT_ENV_FILE = Path().home() / ".env.wtfis"
@@ -81,101 +86,128 @@
         argparse.ArgumentParser().error("GREYNOISE_API_KEY is not set")
     if is_ip(parsed.entity) and parsed.max_resolutions != DEFAULT_MAX_RESOLUTIONS:
         argparse.ArgumentParser().error("--max-resolutions is not applicable to IPs")
 
     return parsed
 
 
-def main():
-    # Load environment variables
-    parse_env()
-
-    # Args
-    args = parse_args()
-
-    # Instantiate the console
-    console = Console(no_color=True) if args.no_color else Console()
+def generate_entity_handler(
+    args: Namespace,
+    console: Console,
+    progress: Progress,
+) -> BaseHandler:
+    # Virustotal client
+    vt_client = VTClient(os.environ["VT_API_KEY"])
+
+    # IP enrichment client selector
+    enricher_client: Union[IpWhoisClient, ShodanClient] = (
+        ShodanClient(os.environ["SHODAN_API_KEY"])
+        if args.use_shodan
+        else IpWhoisClient()
+    )
 
-    # Progress animation controller
-    progress = get_progress(console)
+    # Whois client selector
+    # Order of use based on set envvars:
+    #    1. Passivetotal
+    #    2. IP2Whois (Domain only)
+    #    2. Virustotal (fallback)
+    if os.environ.get("PT_API_USER") and os.environ.get("PT_API_KEY"):
+        whois_client: Union[PTClient, Ip2WhoisClient, VTClient] = (
+            PTClient(os.environ["PT_API_USER"], os.environ["PT_API_KEY"])
+        )
+    elif os.environ.get("IP2WHOIS_API_KEY") and not is_ip(args.entity):
+        whois_client = Ip2WhoisClient(os.environ["IP2WHOIS_API_KEY"])
+    else:
+        whois_client = vt_client
 
-    # Fetch data
-    with progress:
-        # Virustotal client
-        vt_client = VTClient(os.environ.get("VT_API_KEY"))
+    # Greynoise client (optional)
+    greynoise_client = (
+        GreynoiseClient(os.environ["GREYNOISE_API_KEY"])
+        if args.use_greynoise
+        else None
+    )
 
-        # IP enrichment client selector
-        enricher_client = (
-            ShodanClient(os.environ.get("SHODAN_API_KEY"))
-            if args.use_shodan
-            else IpWhoisClient()
+    # Domain / FQDN handler
+    if not is_ip(args.entity):
+        entity: BaseHandler = DomainHandler(
+            entity=args.entity,
+            console=console,
+            progress=progress,
+            vt_client=vt_client,
+            ip_enricher_client=enricher_client,
+            whois_client=whois_client,
+            greynoise_client=greynoise_client,
+            max_resolutions=args.max_resolutions,
         )
-
-        # Whois client selector
-        # Order of use based on set envvars:
-        #    1. Passivetotal
-        #    2. IP2Whois (Domain only)
-        #    2. Virustotal (fallback)
-        if os.environ.get("PT_API_USER") and os.environ.get("PT_API_KEY"):
-            whois_client = PTClient(os.environ.get("PT_API_USER"), os.environ.get("PT_API_KEY"))
-        elif os.environ.get("IP2WHOIS_API_KEY") and not is_ip(args.entity):
-            whois_client = Ip2WhoisClient(os.environ.get("IP2WHOIS_API_KEY"))
-        else:
-            whois_client = vt_client
-
-        # Greynoise client (optional)
-        greynoise_client = (
-            GreynoiseClient(os.environ.get("GREYNOISE_API_KEY"))
-            if args.use_greynoise
-            else None
+    # IP address handler
+    else:
+        entity = IpAddressHandler(
+            entity=args.entity,
+            console=console,
+            progress=progress,
+            vt_client=vt_client,
+            ip_enricher_client=enricher_client,
+            whois_client=whois_client,
+            greynoise_client=greynoise_client,
         )
 
-        # Domain / FQDN handler
-        if not is_ip(args.entity):
-            entity = DomainHandler(
-                entity=args.entity,
-                console=console,
-                progress=progress,
-                vt_client=vt_client,
-                ip_enricher_client=enricher_client,
-                whois_client=whois_client,
-                greynoise_client=greynoise_client,
-                max_resolutions=args.max_resolutions,
-            )
-        # IP address handler
-        else:
-            entity = IpAddressHandler(
-                entity=args.entity,
-                console=console,
-                progress=progress,
-                vt_client=vt_client,
-                ip_enricher_client=enricher_client,
-                whois_client=whois_client,
-                greynoise_client=greynoise_client,
-            )
-
-        # Data fetching proper
-        entity.fetch_data()
+    return entity
 
-    # Print warnings, if any
-    entity.print_warnings()
 
+def generate_view(
+    args: Namespace,
+    console: Console,
+    entity: BaseHandler,
+) -> BaseView:
     # Output display
-    if isinstance(entity, DomainHandler):
-        view = DomainView(
+    if isinstance(entity, DomainHandler) and isinstance(entity.vt_info, Domain):
+        view: BaseView = DomainView(
             console,
             entity.vt_info,
             entity.resolutions,
             entity.whois,
             entity.ip_enrich,
             entity.greynoise,
             max_resolutions=args.max_resolutions,
         )
-    else:
+    elif isinstance(entity, IpAddressHandler) and isinstance(entity.vt_info, IpAddress):
         view = IpAddressView(
             console,
             entity.vt_info,
             entity.whois,
             entity.ip_enrich,
             entity.greynoise,
         )
+    else:
+        raise Exception("Unsupported entity!")
+
+    return view
+
+
+def main():
+    # Load environment variables
+    parse_env()
+
+    # Args
+    args = parse_args()
+
+    # Instantiate the console
+    console = Console(no_color=True) if args.no_color else Console()
+
+    # Progress animation controller
+    progress = get_progress(console)
+
+    # Entity handler
+    entity = generate_entity_handler(args, console, progress)
+
+    # Fetch data
+    with progress:
+        entity.fetch_data()
+
+    # Print fetch warnings, if any
+    entity.print_warnings()
+
+    # Output display
+    view = generate_view(args, console, entity)
+
+    # Finally, print output
     view.print(one_column=args.one_column)
```

### Comparing `wtfis-0.6.1/wtfis/utils.py` & `wtfis-0.6.2/wtfis/utils.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/wtfis/clients/base.py` & `wtfis-0.6.2/wtfis/clients/base.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/wtfis/clients/greynoise.py` & `wtfis-0.6.2/wtfis/clients/greynoise.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.api_key = api_key
 
     @property
     def name(self) -> str:
         return "Greynoise"
 
     def get_ip(self, ip: str) -> GreynoiseIp:
-        return GreynoiseIp.parse_obj(
+        return GreynoiseIp.model_validate(
             self._get(f"/{ip}", headers={"key": self.api_key})
         )
 
     def bulk_get_ip(
         self,
         resolutions: Resolutions,
         max_ips_to_enrich: int
@@ -30,15 +30,15 @@
         greynoise_map = {}
         for idx, ip in enumerate(resolutions.data):
             if idx == max_ips_to_enrich:
                 break
             ip_data = self.get_ip(ip.attributes.ip_address)
             if ip_data:
                 greynoise_map[ip_data.ip] = ip_data
-        return GreynoiseIpMap(__root__=greynoise_map)
+        return GreynoiseIpMap.model_validate(greynoise_map)
 
     def single_get_ip(self, ip: str) -> GreynoiseIpMap:
         greynoise_map = {}
         ip_data = self.get_ip(ip)
         if ip_data:
             greynoise_map[ip] = ip_data
-        return GreynoiseIpMap(__root__=greynoise_map)
+        return GreynoiseIpMap.model_validate(greynoise_map)
```

### Comparing `wtfis-0.6.1/wtfis/clients/ip2whois.py` & `wtfis-0.6.2/wtfis/clients/ip2whois.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         params = {
             "key": self.api_key,
             "domain": refang(domain),
         }
 
         # Let a 404 or invalid domain pass
         try:
-            return Whois.parse_obj(self._get("/", params))
+            return Whois.model_validate(self._get("/", params))
         except HTTPError as e:
             if (
                 e.response.status_code == 404 or
                 (e.response.status_code == 400 and
                  e.response.json().get("error", {})["error_code"] == 10007)
             ):
-                return Whois.parse_obj({})
+                return Whois.model_validate({})
             raise
```

### Comparing `wtfis-0.6.1/wtfis/clients/ipwhois.py` & `wtfis-0.6.2/wtfis/clients/ipwhois.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     IPWhois client
     """
     baseurl = "https://ipwho.is"
 
     def get_ipwhois(self, ip: str) -> Optional[IpWhois]:
         result = self._get(f"/{ip}")
-        return IpWhois.parse_obj(result) if result.get("success") is True else None
+        return IpWhois.model_validate(result) if result.get("success") is True else None
 
     @property
     def name(self) -> str:
         return "IPWhois"
 
     def bulk_get_ip(
         self,
@@ -27,15 +27,15 @@
         ipwhois_map = {}
         for idx, ip in enumerate(resolutions.data):
             if idx == max_ips_to_enrich:
                 break
             ipwhois = self.get_ipwhois(ip.attributes.ip_address)
             if ipwhois:
                 ipwhois_map[ipwhois.ip] = ipwhois
-        return IpWhoisMap(__root__=ipwhois_map)
+        return IpWhoisMap.model_validate(ipwhois_map)
 
     def single_get_ip(self, ip: str) -> IpWhoisMap:
         ipwhois_map = {}
         ipwhois = self.get_ipwhois(ip)
         if ipwhois:
             ipwhois_map[ip] = ipwhois
-        return IpWhoisMap(__root__=ipwhois_map)
+        return IpWhoisMap.model_validate(ipwhois_map)
```

### Comparing `wtfis-0.6.1/wtfis/clients/shodan.py` & `wtfis-0.6.2/wtfis/clients/shodan.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     @property
     def name(self) -> str:
         return "Shodan"
 
     def get_ip(self, ip: str) -> Optional[ShodanIp]:
         try:
-            return ShodanIp.parse_obj(self.s.host(ip, minify=False))
+            return ShodanIp.model_validate(self.s.host(ip, minify=False))
         except APIError as e:
             if str(e) == "Invalid API key":
                 raise APIError("Invalid Shodan API key")
             else:
                 return None
 
     def bulk_get_ip(
@@ -34,15 +34,15 @@
         shodan_map = {}
         for idx, ip in enumerate(resolutions.data):
             if idx == max_ips_to_enrich:
                 break
             ip_data = self.get_ip(ip.attributes.ip_address)
             if ip_data:
                 shodan_map[ip_data.ip_str] = ip_data
-        return ShodanIpMap(__root__=shodan_map)
+        return ShodanIpMap.model_validate(shodan_map)
 
     def single_get_ip(self, ip: str) -> ShodanIpMap:
         shodan_map = {}
         ip_data = self.get_ip(ip)
         if ip_data:
             shodan_map[ip] = ip_data
-        return ShodanIpMap(__root__=shodan_map)
+        return ShodanIpMap.model_validate(shodan_map)
```

### Comparing `wtfis-0.6.1/wtfis/handlers/base.py` & `wtfis-0.6.2/wtfis/handlers/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ip2whois import Ip2WhoisClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.shodan import ShodanClient
 from wtfis.clients.virustotal import VTClient
-from wtfis.models.common import WhoisType
+from wtfis.models.common import WhoisBase
 from wtfis.models.greynoise import GreynoiseIpMap
 from wtfis.models.ipwhois import IpWhoisMap
 from wtfis.models.shodan import ShodanIpMap
 from wtfis.models.virustotal import Domain, IpAddress
 from wtfis.ui.theme import Theme
 from wtfis.utils import error_and_exit, refang
 
@@ -56,17 +56,17 @@
         # Clients
         self._vt = vt_client
         self._enricher = ip_enricher_client
         self._whois = whois_client
         self._greynoise = greynoise_client
 
         # Dataset containers
-        self.vt_info:   Union[Domain, IpAddress] = None        # type: ignore
-        self.ip_enrich: Union[IpWhoisMap, ShodanIpMap] = None  # type: ignore
-        self.whois:     WhoisType = None                       # type: ignore
+        self.vt_info:   Union[Domain, IpAddress]
+        self.ip_enrich: Union[IpWhoisMap, ShodanIpMap]
+        self.whois:     WhoisBase
         self.greynoise: GreynoiseIpMap = GreynoiseIpMap.empty()
 
         # Warning messages container
         self.warnings: List[str] = []
 
     @abc.abstractmethod
     def fetch_data(self) -> None:
```

### Comparing `wtfis-0.6.1/wtfis/handlers/domain.py` & `wtfis-0.6.2/wtfis/handlers/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,31 +69,31 @@
             # No warning message
             elif e.response.status_code == 404:
                 self.greynoise = GreynoiseIpMap.empty()
             else:
                 raise
 
     def fetch_data(self):
-        task1 = self.progress.add_task("Fetching data from Virustotal")
-        self.progress.update(task1, advance=33)
+        task_v = self.progress.add_task("Fetching data from Virustotal")
+        self.progress.update(task_v, advance=33)
         self._fetch_vt_domain()
         if self.max_resolutions != 0:
-            self.progress.update(task1, advance=33)
+            self.progress.update(task_v, advance=33)
             self._fetch_vt_resolutions()
-        self.progress.update(task1, completed=100)
+        self.progress.update(task_v, completed=100)
 
         if self.resolutions and self.resolutions.data:
-            task2 = self.progress.add_task(f"Fetching IP enrichments from {self._enricher.name}")
-            self.progress.update(task2, advance=50)
+            task_r = self.progress.add_task(f"Fetching IP enrichments from {self._enricher.name}")
+            self.progress.update(task_r, advance=50)
             self._fetch_ip_enrichments()
-            self.progress.update(task2, completed=100)
+            self.progress.update(task_r, completed=100)
 
         if self._greynoise:
-            task3 = self.progress.add_task(f"Fetching IP enrichments from {self._greynoise.name}")
-            self.progress.update(task3, advance=50)
+            task_g = self.progress.add_task(f"Fetching IP enrichments from {self._greynoise.name}")
+            self.progress.update(task_g, advance=50)
             self._fetch_greynoise()
-            self.progress.update(task3, completed=100)
+            self.progress.update(task_g, completed=100)
 
-        task4 = self.progress.add_task(f"Fetching domain whois from {self._whois.name}")
-        self.progress.update(task4, advance=50)
+        task_w = self.progress.add_task(f"Fetching domain whois from {self._whois.name}")
+        self.progress.update(task_w, advance=50)
         self._fetch_whois()
-        self.progress.update(task4, completed=100)
+        self.progress.update(task_w, completed=100)
```

### Comparing `wtfis-0.6.1/wtfis/handlers/ip.py` & `wtfis-0.6.2/wtfis/handlers/ip.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,27 +30,27 @@
             # No warning message
             elif e.response.status_code == 404:
                 self.greynoise = GreynoiseIpMap.empty()
             else:
                 raise
 
     def fetch_data(self):
-        task1 = self.progress.add_task("Fetching data from Virustotal")
-        self.progress.update(task1, advance=50)
+        task_v = self.progress.add_task("Fetching data from Virustotal")
+        self.progress.update(task_v, advance=50)
         self._fetch_vt_ip_address()
-        self.progress.update(task1, completed=100)
+        self.progress.update(task_v, completed=100)
 
-        task2 = self.progress.add_task(f"Fetching IP enrichments from {self._enricher.name}")
-        self.progress.update(task2, advance=50)
+        task_i = self.progress.add_task(f"Fetching IP enrichments from {self._enricher.name}")
+        self.progress.update(task_i, advance=50)
         self._fetch_ip_enrichments()
-        self.progress.update(task2, completed=100)
+        self.progress.update(task_i, completed=100)
 
         if self._greynoise:
-            task3 = self.progress.add_task(f"Fetching IP enrichments from {self._greynoise.name}")
-            self.progress.update(task3, advance=50)
+            task_g = self.progress.add_task(f"Fetching IP enrichments from {self._greynoise.name}")
+            self.progress.update(task_g, advance=50)
             self._fetch_greynoise()
-            self.progress.update(task3, completed=100)
+            self.progress.update(task_g, completed=100)
 
-        task4 = self.progress.add_task(f"Fetching IP whois from {self._whois.name}")
-        self.progress.update(task4, advance=50)
+        task_w = self.progress.add_task(f"Fetching IP whois from {self._whois.name}")
+        self.progress.update(task_w, advance=50)
         self._fetch_whois()
-        self.progress.update(task4, completed=100)
+        self.progress.update(task_w, completed=100)
```

### Comparing `wtfis-0.6.1/wtfis/models/ipwhois.py` & `wtfis-0.6.2/wtfis/models/ipwhois.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from pydantic import BaseModel
+from pydantic import BaseModel, Field, RootModel
 from typing import Dict
 
+from wtfis.models.common import LaxStr
+
 
 class Flag(BaseModel):
     img: str
     emoji: str
     emoji_unicode: str
 
 
 class Connection(BaseModel):
-    asn: str
+    asn: LaxStr
     org: str
     isp: str
     domain: str
 
 
 class IpWhois(BaseModel):
     ip: str
     success: bool
-    type_: str
+    type_: str = Field(alias="type")
     continent: str
     continent_code: str
     country: str
     country_code: str
     region: str
     region_code: str
     city: str
@@ -30,15 +32,10 @@
     postal: str
     calling_code: str
     capital: str
     borders: str
     flag: Flag
     connection: Connection
 
-    class Config:
-        fields = {
-            "type_": "type",
-        }
-
 
-class IpWhoisMap(BaseModel):
-    __root__: Dict[str, IpWhois]
+class IpWhoisMap(RootModel):
+    root: Dict[str, IpWhois]
```

### Comparing `wtfis-0.6.1/wtfis/models/shodan.py` & `wtfis-0.6.2/wtfis/models/shodan.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from collections import defaultdict, namedtuple
-from pydantic import BaseModel
+from pydantic import BaseModel, RootModel
 from typing import Dict, List, Optional
 
+from wtfis.models.common import LaxStr
+
 
 class PortData(BaseModel):
     port: int
-    product: Optional[str]
+    product: Optional[str] = None
     transport: str
 
 
 class ShodanIp(BaseModel):
-    asn: Optional[str]
-    city: Optional[str]
+    asn: Optional[LaxStr] = None
+    city: Optional[str] = None
     country_code: str
     country_name: str
     data: List[PortData]
     ip_str: str
-    isp: Optional[str]
+    isp: Optional[str] = None
     last_update: str
-    org: Optional[str]
-    os: Optional[str]
-    ports: Optional[List[int]]
-    region_name: Optional[str]
-    tags: Optional[List[str]]
+    org: Optional[str] = None
+    os: Optional[str] = None
+    ports: Optional[List[int]] = None
+    region_name: Optional[str] = None
+    tags: Optional[List[str]] = None
 
     def group_ports_by_product(self) -> dict:
         PortProtocol = namedtuple("PortProtocol", "port transport")
         result = defaultdict(list)
         unknown = []  # Save ports with no product for adding later as last result item
         for port in self.data:
             port_data = PortProtocol(port.port, port.transport)
@@ -35,9 +37,9 @@
             else:
                 unknown.append(port_data)
         if unknown:
             result["Other"] = unknown
         return result
 
 
-class ShodanIpMap(BaseModel):
-    __root__: Dict[str, ShodanIp]
+class ShodanIpMap(RootModel):
+    root: Dict[str, ShodanIp]
```

### Comparing `wtfis-0.6.1/wtfis/models/virustotal.py` & `wtfis-0.6.2/wtfis/models/virustotal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-from pydantic import BaseModel, root_validator, validator
+from pydantic import BaseModel, Field, RootModel, field_validator, model_validator
 from typing import Any, Dict, List, Optional
 
-from wtfis.models.common import WhoisBase
+from wtfis.models.common import LaxStr, WhoisBase
 
 
 class BaseData(BaseModel):
-    attributes: Any
-    id_: str
-    type_: str
-
-    class Config:
-        fields = {
-            "id_": "id",
-            "type_": "type",
-        }
+    attributes: Any = None
+    id_: str = Field(alias="id")
+    type_: str = Field(alias="type")
 
 
 class Meta(BaseModel):
     count: int
 
 
 class AnalysisResult(BaseModel):
     category: str
     engine_name: str
     method: str
     result: str
 
 
-class LastAnalysisResults(BaseModel):
-    __root__: Dict[str, AnalysisResult]
+class LastAnalysisResults(RootModel):
+    root: Dict[str, AnalysisResult]
 
 
 class LastAnalysisStats(BaseModel):
     harmless: int
     malicious: int
     suspicious: int
     timeout: int
@@ -40,37 +34,38 @@
 
 
 class Popularity(BaseModel):
     rank: int
     timestamp: int
 
 
-class PopularityRanks(BaseModel):
-    __root__: Dict[str, Popularity]
+class PopularityRanks(RootModel):
+    root: Dict[str, Popularity]
 
 
 class BaseAttributes(BaseModel):
-    jarm: Optional[str]
+    jarm: Optional[str] = None
     last_analysis_results: LastAnalysisResults
     last_analysis_stats: LastAnalysisStats
-    last_https_certificate_date: Optional[int]
-    last_modification_date: Optional[int]
+    last_https_certificate_date: Optional[int] = None
+    last_modification_date: Optional[int] = None
     reputation: int
     tags: List[str]
 
 
 class DomainAttributes(BaseAttributes):
     categories: List[str]
-    creation_date: Optional[int]
-    last_dns_records_date: Optional[int]
-    last_update_date: Optional[int]
+    creation_date: Optional[int] = None
+    last_dns_records_date: Optional[int] = None
+    last_update_date: Optional[int] = None
     popularity_ranks: PopularityRanks
-    registrar: Optional[str]
+    registrar: Optional[str] = None
 
-    @validator("categories", pre=True)
+    @field_validator("categories", mode="before")
+    @classmethod
     def transform_categories(cls, v):
         cats = set()
         for category in v.values():
             for delimiter in [", ", ",", "/", " / "]:
                 if delimiter in category:
                     cats = cats | set(category.lower().split(delimiter))
                     break
@@ -84,18 +79,18 @@
 
 
 class Domain(BaseModel):
     data: DomainData
 
 
 class IpAttributes(BaseAttributes):
-    asn: Optional[int]
-    continent: Optional[str]
-    country: Optional[str]
-    network: Optional[str]
+    asn: Optional[LaxStr] = None
+    continent: Optional[str] = None
+    country: Optional[str] = None
+    network: Optional[str] = None
 
 
 class IpData(BaseData):
     attributes: IpAttributes
 
 
 class IpAddress(BaseModel):
@@ -118,46 +113,33 @@
 class Resolutions(BaseModel):
     meta: Meta
     data: List[ResolutionData]
 
 
 class Whois(WhoisBase):
     source: str = "virustotal"
-    domain: str = ""
-    registrar: Optional[str]
-    organization: Optional[str]
-    name: Optional[str]
-    email: Optional[str]
-    phone: Optional[str]
-    street: Optional[str]
-    city: Optional[str]
-    state: Optional[str]
-    country: Optional[str]
-    postal_code: Optional[str]
-    name_servers: List[str] = []
-    date_created: Optional[str]
-    date_changed: Optional[str]
-    date_expires: Optional[str]
-    dnssec: Optional[str]
-
-    class Config:
-        fields = {
-            "domain": "Domain Name",
-            "organization": "Registrant Organization",
-            "email": "Registrant Email",
-            "phone": "Registrant Phone",
-            "street": "Registrant Street",
-            "city": "Registrant City",
-            "state": "Registrant State/Province",
-            "postal_code": "Registrant Postal Code",
-            "name_servers": "Name Server",
-            "dnssec": "DNSSEC",
-        }
+    domain: str = Field("", alias="Domain Name")
+    registrar: Optional[str] = None
+    organization: Optional[str] = Field(None, alias="Registrant Organization")
+    name: Optional[str] = None
+    email: Optional[str] = Field(None, alias="Registrant Email")
+    phone: Optional[str] = Field(None, alias="Registrant Phone")
+    street: Optional[str] = Field(None, alias="Registrant Street")
+    city: Optional[str] = Field(None, alias="Registrant City")
+    state: Optional[str] = Field(None, alias="Registrant State/Province")
+    country: Optional[str] = None
+    postal_code: Optional[str] = Field(None, alias="Registrant Postal Code")
+    name_servers: List[str] = Field([], alias="Name Server")
+    date_created: Optional[str] = None
+    date_changed: Optional[LaxStr] = None
+    date_expires: Optional[str] = None
+    dnssec: Optional[str] = Field(None, alias="DNSSEC")
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def get_latest_whois_record_and_transform(cls, v):
         data = v.pop("data")
         if not data:
             return {}
         transformed = data[0].get("attributes", {})
 
         # Flatten
@@ -191,20 +173,23 @@
                 transformed.pop("registrar_name", None) or
                 transformed.pop("Registrar", None)
             ),
         }
 
         return {**transformed, **fields_w_multiple_possible_sources}
 
-    @validator("name_servers", pre=True)
+    @field_validator("name_servers", mode="before")
+    @classmethod
     def transform_nameservers(cls, v):
         return v.lower().split(" | ")
 
-    @validator("domain", pre=True)
+    @field_validator("domain", mode="before")
+    @classmethod
     def lowercase_domain(cls, v):
         return v.lower()
 
-    @validator("*")
+    @field_validator("*")
+    @classmethod
     def dedupe_values(cls, v):
         if v is not None and "|" in v:
             return v.split(" | ")[0]
         return v
```

### Comparing `wtfis-0.6.1/wtfis/ui/base.py` & `wtfis-0.6.2/wtfis/ui/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     group,
 )
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 from typing import Any, Generator, List, Optional, Tuple, Union
 
-from wtfis.models.common import WhoisType
+from wtfis.models.common import WhoisBase
 from wtfis.models.greynoise import GreynoiseIp, GreynoiseIpMap
 from wtfis.models.ipwhois import IpWhois, IpWhoisMap
 from wtfis.models.shodan import ShodanIp, ShodanIpMap
 from wtfis.models.virustotal import (
     LastAnalysisStats,
     PopularityRanks,
 )
@@ -32,28 +32,28 @@
     pt_gui_baseurl = "https://community.riskiq.com/search"
     shodan_gui_baseurl = "https://www.shodan.io/host"
 
     def __init__(
         self,
         console: Console,
         entity: Any,
-        whois: Optional[WhoisType],
+        whois: Optional[WhoisBase],
         ip_enrich: Union[IpWhoisMap, ShodanIpMap],
         greynoise: GreynoiseIpMap,
     ) -> None:
         self.console = console
         self.entity = entity
         self.whois = whois
         self.ip_enrich = ip_enrich
         self.greynoise = greynoise
         self.theme = Theme()
 
     def _vendors_who_flagged_malicious(self) -> List[str]:
         vendors = []
-        for key, result in self.entity.data.attributes.last_analysis_results.__root__.items():
+        for key, result in self.entity.data.attributes.last_analysis_results.root.items():
             if result.category == "malicious":
                 vendors.append(key)
         return vendors
 
     def _gen_heading_text(self, heading: str, hyperlink: Optional[str] = None) -> Text:
         text = Text(justify="center", end="\n")
         style = f"{self.theme.heading} link {hyperlink}" if hyperlink else self.theme.heading
@@ -126,24 +126,24 @@
             elif reputation < 0:
                 return self.theme.error
             return "default"
 
         return Text(str(reputation), style=rep_style(reputation))
 
     def _gen_vt_popularity(self, popularity_ranks: PopularityRanks) -> Optional[Text]:
-        if len(popularity_ranks.__root__) == 0:
+        if len(popularity_ranks.root) == 0:
             return None
 
         text = Text()
-        for source, popularity in popularity_ranks.__root__.items():
+        for source, popularity in popularity_ranks.root.items():
             text.append(source, style=self.theme.popularity_source)
             text.append(" (")
             text.append(str(popularity.rank), style=self.theme.inline_stat)
             text.append(")")
-            if source != list(popularity_ranks.__root__.keys())[-1]:
+            if source != list(popularity_ranks.root.keys())[-1]:
                 text.append("\n")
         return text
 
     def _gen_shodan_services(self, ip: ShodanIp) -> Optional[Union[Text, str]]:
         if len(ip.data) == 0:
             return None
 
@@ -241,18 +241,18 @@
 
         text = Text(f"{asn.replace('AS', '')} (")
         text.append(str(org), style=self.theme.asn_org)
         text.append(")")
         return text
 
     def _get_ip_enrichment(self, ip: str) -> Optional[Union[IpWhois, ShodanIp]]:
-        return self.ip_enrich.__root__[ip] if ip in self.ip_enrich.__root__.keys() else None
+        return self.ip_enrich.root[ip] if ip in self.ip_enrich.root.keys() else None
 
     def _get_greynoise_enrichment(self, ip: str) -> Optional[GreynoiseIp]:
-        return self.greynoise.__root__[ip] if ip in self.greynoise.__root__.keys() else None
+        return self.greynoise.root[ip] if ip in self.greynoise.root.keys() else None
 
     def whois_panel(self) -> Optional[Panel]:
         # Do nothing if no whois
         if self.whois is None:
             return None
 
         if self.whois.source == "passivetotal":  # PT
```

### Comparing `wtfis-0.6.1/wtfis/ui/theme.py` & `wtfis-0.6.2/wtfis/ui/theme.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/wtfis/ui/view.py` & `wtfis-0.6.2/wtfis/ui/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     RenderableType,
 )
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.text import Text
 from typing import List, Optional, Tuple, Union
 
-from wtfis.models.common import WhoisType
+from wtfis.models.common import WhoisBase
 from wtfis.models.greynoise import GreynoiseIpMap
 from wtfis.models.ipwhois import IpWhois, IpWhoisMap
 from wtfis.models.shodan import ShodanIpMap
 from wtfis.models.virustotal import (
     Domain,
     IpAddress,
     Resolutions,
@@ -27,15 +27,15 @@
     Handler for FQDN and domain lookup output
     """
     def __init__(
         self,
         console: Console,
         entity: Domain,
         resolutions: Optional[Resolutions],
-        whois: WhoisType,
+        whois: WhoisBase,
         ip_enrich: Union[IpWhoisMap, ShodanIpMap],
         greynoise: GreynoiseIpMap,
         max_resolutions: int = 3,
     ) -> None:
         super().__init__(console, entity, whois, ip_enrich, greynoise)
         self.resolutions = resolutions
         self.max_resolutions = max_resolutions
@@ -192,15 +192,15 @@
     """
     Handler for IP Address lookup output
     """
     def __init__(
         self,
         console: Console,
         entity: IpAddress,
-        whois: WhoisType,
+        whois: WhoisBase,
         ip_enrich: Union[IpWhoisMap, ShodanIpMap],
         greynoise: GreynoiseIpMap,
     ) -> None:
         super().__init__(console, entity, whois, ip_enrich, greynoise)
 
     def ip_panel(self) -> Panel:
         attributes = self.entity.data.attributes
```

### Comparing `wtfis-0.6.1/.gitignore` & `wtfis-0.6.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -158,9 +158,12 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # VSCode
 .vscode/
 
+# hatch virtualenvs
+.hatch/
+
 # Custom env
 .env.wtfis
```

### Comparing `wtfis-0.6.1/LICENSE` & `wtfis-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfis-0.6.1/README.md` & `wtfis-0.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 
 ## Install
 
 ```
 $ pip install wtfis
 ```
 
+To install via `conda` (from conda-forge), see [wtfis-feedstock](https://github.com/conda-forge/wtfis-feedstock).
+
 
 ## Setup
 
 wtfis uses these environment variables:
 
 * `VT_API_KEY` (required) - Virustotal API key
 * `PT_API_KEY` (optional) - Passivetotal API key
@@ -118,24 +120,25 @@
 
 Alternatively, create a file in your home directory `~/.env.wtfis` with the above declarations. See [.env.wtfis.example](./.env.wtfis.example) for a template. **NOTE: Don't forget to `chmod 400` the file!**
 
 
 ## Usage
 
 ```
-usage: wtfis [-h] [-m N] [-s] [-n] [-1] [-V] entity
+usage: wtfis [-h] [-m N] [-s] [-g] [-n] [-1] [-V] entity
 
 positional arguments:
   entity                Hostname, domain or IP
 
 optional arguments:
   -h, --help            show this help message and exit
   -m N, --max-resolutions N
                         Maximum number of resolutions to show (default: 3)
   -s, --use-shodan      Use Shodan to enrich IPs
+  -g, --use-greynoise   Enable Greynoise for IPs
   -n, --no-color        Show output without colors
   -1, --one-column      Display results in one column
   -V, --version         Print version number
 ```
 
 Basically:
```

### Comparing `wtfis-0.6.1/pyproject.toml` & `wtfis-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Security",
 ]
 dependencies = [
-    "pydantic~=1.10.2",
+    "pydantic~=2.0.3",
     "python-dotenv~=0.21.0",
     "requests~=2.28.1",
     "rich~=12.6.0",
     "shodan~=1.28.0",
 ]
 dynamic = ["version"]
 
@@ -55,14 +55,16 @@
 
 [tool.hatch.publish.index]
 disable = true
 
 # Hatch default env
 [tool.hatch.envs.default]
 dependencies = [
+    "bandit",
+    "flake8>=6.0.0",
     "freezegun",
     "mypy",
     "pytest",
     "pytest-cov",
     "types-requests~=2.28.1",
 ]
 [tool.hatch.envs.default.scripts]
@@ -72,20 +74,20 @@
 test-all = [
     "typecheck",
     "test-cov",
 ]
 
 # Hatch test env
 [[tool.hatch.envs.test.matrix]]
-python = ["38", "39", "310"]
+python = ["38", "39", "310", "311"]
 
 # Hatch lint env
 [tool.hatch.envs.lint]
 detached = true
-dependencies = [
+dependencies = [  # Make sure the respective versions are synced with default!
     "bandit",
     "flake8>=6.0.0",
 ]
 [tool.hatch.envs.lint.scripts]
 flake = "flake8 {args:wtfis}"
 security = "bandit --quiet -r {args:wtfis}"
 all = [
```

### Comparing `wtfis-0.6.1/PKG-INFO` & `wtfis-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wtfis
-Version: 0.6.1
+Version: 0.6.2
 Summary: Passive hostname, domain and IP lookup tool for non-robots
 Project-URL: Homepage, https://github.com/pirxthepilot/wtfis
 Author-email: pirxthepilot <pirxthepilot@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ipinfo,osint,passive lookup,passivetotal,security,shodan,virustotal,whois
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Requires-Python: >=3.8
-Requires-Dist: pydantic~=1.10.2
+Requires-Dist: pydantic~=2.0.3
 Requires-Dist: python-dotenv~=0.21.0
 Requires-Dist: requests~=2.28.1
 Requires-Dist: rich~=12.6.0
 Requires-Dist: shodan~=1.28.0
 Description-Content-Type: text/markdown
 
 # wtfis
@@ -119,14 +119,16 @@
 
 ## Install
 
 ```
 $ pip install wtfis
 ```
 
+To install via `conda` (from conda-forge), see [wtfis-feedstock](https://github.com/conda-forge/wtfis-feedstock).
+
 
 ## Setup
 
 wtfis uses these environment variables:
 
 * `VT_API_KEY` (required) - Virustotal API key
 * `PT_API_KEY` (optional) - Passivetotal API key
@@ -140,24 +142,25 @@
 
 Alternatively, create a file in your home directory `~/.env.wtfis` with the above declarations. See [.env.wtfis.example](./.env.wtfis.example) for a template. **NOTE: Don't forget to `chmod 400` the file!**
 
 
 ## Usage
 
 ```
-usage: wtfis [-h] [-m N] [-s] [-n] [-1] [-V] entity
+usage: wtfis [-h] [-m N] [-s] [-g] [-n] [-1] [-V] entity
 
 positional arguments:
   entity                Hostname, domain or IP
 
 optional arguments:
   -h, --help            show this help message and exit
   -m N, --max-resolutions N
                         Maximum number of resolutions to show (default: 3)
   -s, --use-shodan      Use Shodan to enrich IPs
+  -g, --use-greynoise   Enable Greynoise for IPs
   -n, --no-color        Show output without colors
   -1, --one-column      Display results in one column
   -V, --version         Print version number
 ```
 
 Basically:
```

