# Comparing `tmp/nebari-2023.5.1rc1.tar.gz` & `tmp/nebari-2023.7.1rc1.tar.gz`

## Comparing `nebari-2023.5.1rc1.tar` & `nebari-2023.7.1rc1.tar`

### file list

```diff
@@ -1,505 +1,405 @@
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.cirun.yml
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.readthedocs.yml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/MANIFEST.in
--rw-r--r--   0        0        0    56020 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/RELEASE.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/flake.lock
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/flake.nix
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/noxfile.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/contributor.yaml
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/infracost.yml
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/kubernetes_test.yaml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/markdown.links.config.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/release.yaml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/.gitignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/.gitmodules
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/README.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/conf.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/index.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/requirements.txt
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/_templates/announcement.html
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/_templates/layout.html
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/ext/substitute.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/output/.nojekyll
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/argo-workflows.md
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/awss3curl.md
--rw-r--r--   0        0        0     9441 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/backup.md
--rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/breaking-upgrade.md
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/clearml.md
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/cost.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/custom-helm-charts.md
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/faq.md
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/gpu.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/index.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/jupyterhub.md
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/keycloak.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/monitoring.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/preemptible-spot-instances.md
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/prefect.md
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/system_maintenance.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/traefik.md
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/troubleshooting.md
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/upgrade.md
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/architecture.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/changelog.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/contribution.md
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/index.md
--rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/keycloak.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/logo.md
--rw-r--r--   0        0        0    20441 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/minikube.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/release.md
--rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/testing.md
--rw-r--r--   0        0        0    64293 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/argo-server-landing-page.png
--rw-r--r--   0        0        0   102104 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/argo-workflows-user-tab.png
--rw-r--r--   0        0        0   221390 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudfare_update_screenshot.png
--rw-r--r--   0        0        0    17170 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_account_resources_scr.png
--rw-r--r--   0        0        0   108690 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_auth_1.png
--rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_permissions_2.1.1.png
--rw-r--r--   0        0        0    75331 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_summary.png
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_zone_resources.png
--rw-r--r--   0        0        0   277092 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/dev_postman_for_keycloak.png
--rw-r--r--   0        0        0   154819 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/grafana_manage_dashboards.png
--rw-r--r--   0        0        0    75305 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/grafana_networking_dashboard.png
--rw-r--r--   0        0        0    92141 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/grafana_node_cpu_usage.png
--rw-r--r--   0        0        0    94475 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/high_level_architecture.png
--rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/init_cli_output.png
--rw-r--r--   0        0        0    65086 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/k9s_UI.png
--rw-r--r--   0        0        0   156751 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_add_users.png
--rw-r--r--   0        0        0   161065 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_adduser.png
--rw-r--r--   0        0        0   131930 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_groups.png
--rw-r--r--   0        0        0   132035 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_master_login.png
--rw-r--r--   0        0        0    25405 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_new_group1.png
--rw-r--r--   0        0        0    94386 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_new_group2.png
--rw-r--r--   0        0        0   100928 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_new_group3.png
--rw-r--r--   0        0        0   317402 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_qhub_login.png
--rw-r--r--   0        0        0    97778 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_account_security.png
--rw-r--r--   0        0        0   157913 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_manage_account.png
--rw-r--r--   0        0        0   143079 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_update_password.png
--rw-r--r--   0        0        0   163577 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_user_password.png
--rw-r--r--   0        0        0    88640 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/labs_logo_white.png
--rw-r--r--   0        0        0    71430 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_api_token.png
--rw-r--r--   0        0        0    86104 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_api_token_generated.png
--rw-r--r--   0        0        0   185838 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_aws_architecture.png
--rw-r--r--   0        0        0   126188 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_notebook.png
--rw-r--r--   0        0        0    63407 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_resources.png
--rw-r--r--   0        0        0    56065 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_simple.png
--rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dask_cluster_options.png
--rw-r--r--   0        0        0    30695 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dask_cluster_start.png
--rw-r--r--   0        0        0   136024 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_do_architecture.png
--rw-r--r--   0        0        0   136194 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_gcp_architecture.png
--rw-r--r--   0        0        0    75740 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_kernel_selection.png
--rw-r--r--   0        0        0   102949 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_login_screen.png
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_logo.png
--rw-r--r--   0        0        0    44399 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_main_hub_page.png
--rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_new_dashboard.png
--rw-r--r--   0        0        0    61425 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_new_dashboard_filled_in.png
--rw-r--r--   0        0        0    45358 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_notebook.png
--rw-r--r--   0        0        0    69000 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_select_profile.png
--rw-r--r--   0        0        0    57906 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_server_start.png
--rw-r--r--   0        0        0   106710 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_vscode.png
--rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/quansight_logo_white.png
--rw-r--r--   0        0        0    20987 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/render_cli_output.png
--rw-r--r--   0        0        0    91557 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/tech_stack_diagram.png
--rw-r--r--   0        0        0    50197 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_env.png
--rw-r--r--   0        0        0    47961 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_instances.png
--rw-r--r--   0        0        0    57399 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_login_1.png
--rw-r--r--   0        0        0    53867 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_login_2.png
--rw-r--r--   0        0        0    25284 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_server_start.png
--rw-r--r--   0        0        0    38893 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/conda_icon.png
--rw-r--r--   0        0        0    26130 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/dask_icon.png
--rw-r--r--   0        0        0    62475 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/jupyter_hub_icon.png
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/nginx_icon.png
--rw-r--r--   0        0        0    34775 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/configuration.md
--rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/existing.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/index.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/installation.md
--rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/login.md
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/management.md
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/setup.md
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/usage.md
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/introduction/index.md
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/introduction/qhub-101.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/argo_workflows.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/code_server.md
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/dashboard.md
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/dask_gateway.md
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/environments.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/experimental.md
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/faq.md
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/getting_started.md
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/idle_culler.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/index.md
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/ssh.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/training.md
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/troubleshooting.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/__main__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/_version.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/constants.py
--rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cost.py
--rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/deprecate.py
--rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/destroy.py
--rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/initialize.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/keycloak.py
--rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/render.py
--rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/schema.py
--rw-r--r--   0        0        0    16652 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/upgrade.py
--rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/utils.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/dev.py
--rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/init.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/keycloak.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/git.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/common.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/__init__.py
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/checks.py
--rw-r--r--   0        0        0    14771 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/input_vars.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/state_imports.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/tf_objects.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/main.tf
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/main.tf
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/locals.tf
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/main.tf
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/outputs.tf
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/providers.tf
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/versions.tf
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/existing/main.tf
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/outputs.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/provider.tf
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/main.tf
--rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/metallb.yaml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/outputs.tf
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/variables.tf
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/main.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/versions.tf
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
--rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/versions.tf
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/outputs.tf
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/versions.tf
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0   358918 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/argo-workflows.tf
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/clearml.tf
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/conda-store.tf
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/forward-auth.tf
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/kbatch.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/locals.tf
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/outputs.tf
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/prefect.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/providers.tf
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/versions.tf
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
--rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
--rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
--rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
--rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10511 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
--rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
--rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
--rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/versions.tf
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0    14303 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/conftest.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_cli.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_commons.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_dependencies.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_init.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_links.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_render.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_schema.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_upgrade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/notebooks/test-ipython-basic.ipynb
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/scripts/minikube-loadbalancer-ip.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/vale/styles/vocab.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/constants.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/LICENSE
--rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/README.md
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/pyproject.toml
--rw-r--r--   0        0        0    11874 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.cirun.yml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/MANIFEST.in
+-rw-r--r--   0        0        0    60531 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/RELEASE.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/flake.lock
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/flake.nix
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/actions/publish-from-template/action.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/actions/publish-from-template/render_template.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/failed-workflow-issue-templates/test-provider.md
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/kubernetes_test.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/test_helm_charts.yaml
+-rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/helm-validate.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/_version.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/constants.py
+-rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/deprecate.py
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/destroy.py
+-rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/initialize.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/keycloak.py
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/render.py
+-rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/schema.py
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/upgrade.py
+-rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/utils.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/dev.py
+-rw-r--r--   0        0        0    22058 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/init.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/keycloak.py
+-rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/git.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/__init__.py
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/checks.py
+-rw-r--r--   0        0        0    15591 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/input_vars.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/state_imports.py
+-rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/main.tf
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/main.tf
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/locals.tf
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/main.tf
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/outputs.tf
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/main.tf
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/providers.tf
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/versions.tf
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/existing/main.tf
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/outputs.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/provider.tf
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/main.tf
+-rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/metallb.yaml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/outputs.tf
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/variables.tf
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/main.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/versions.tf
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/versions.tf
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/outputs.tf
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/versions.tf
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/__init__.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/argo-workflows.tf
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/clearml.tf
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/conda-store.tf
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/dask_gateway.tf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/forward-auth.tf
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/kbatch.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/locals.tf
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/outputs.tf
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/prefect.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/providers.tf
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/__init__.py
+-rw-r--r--   0        0        0    15836 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
+-rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
+-rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
+-rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/__init__.py
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/__init__.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/__init__.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    16472 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
+-rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
+-rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
+-rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/providers.tf
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/versions.tf
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/nebari/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/nebari/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_cli.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_commons.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_dependencies.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_init.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_links.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_render.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_schema.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_upgrade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/notebooks/test-ipython-basic.ipynb
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/scripts/minikube-loadbalancer-ip.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/vale/styles/vocab.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/.env.tpl
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/README.md
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/conftest.py
+-rw-r--r--   0        0        0    16199 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/navigator.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/run_notebook.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/test_playwright.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/test_data/test_notebook_output.ipynb
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/LICENSE
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/README.md
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/PKG-INFO
```

### Comparing `nebari-2023.5.1rc1/.cirun.yml` & `nebari-2023.7.1rc1/.cirun.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.pre-commit-config.yaml` & `nebari-2023.7.1rc1/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -25,43 +25,43 @@
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: check-json
       - id: check-yaml
         # jinja2 templates for helm charts
-        exclude: "nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/(clearml/chart/templates/.*|prefect/chart/templates/.*)"
+        exclude: "src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/(clearml/chart/templates/.*|prefect/chart/templates/.*)"
         args: [--allow-multiple-documents]
       - id: check-toml
       # Lint: Checks that non-binary executables have a proper shebang.
       - id: check-executables-have-shebangs
-        exclude: "^nebari/template/"
+        exclude: "^src/_nebari/template/"
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         args:
           [
             "--builtin=rare,clear,informal,names",
-            "--skip=_build,*/build/*,*/node_modules/*,nebari.egg-info,.nox,*.git,*.js,*.json,*.yaml,*.yml",
+            "--skip=_build,*/build/*,*/node_modules/*,nebari.egg-info,*.git,*.js,*.json,*.yaml,*.yml",
             "--ignore-words-list=AKS,aks",
             "--write",
           ]
         language: python
 
   # python
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
-        args: ["--line-length=88", "--exclude=/nebari/template/"]
+        args: ["--line-length=88", "--exclude=/src/_nebari/template/"]
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.276
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
@@ -69,26 +69,12 @@
         name: isort
         additional_dependencies: [toml]
         files: \.py$
         args: ["--profile", "black"]
 
   # terraform
   - repo: https://github.com/antonbabenko/pre-commit-terraform
-    rev: v1.78.0
+    rev: v1.81.0
     hooks:
       - id: terraform_fmt
         args:
           - --args=-write=true
-
-  # markdown
-  - repo: https://github.com/executablebooks/mdformat
-    rev: 0.7.16
-    hooks:
-      - id: mdformat
-        files: ^docs/
-        name: mdformat
-        entry: mdformat --wrap=120 --number --end-of-line=lf
-        language: python
-        types: [markdown]
-        minimum_pre_commit_version: "2.0.0"
-        additional_dependencies:
-          - mdformat-tables
```

### Comparing `nebari-2023.5.1rc1/CODE_OF_CONDUCT.md` & `nebari-2023.7.1rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/CONTRIBUTING.md` & `nebari-2023.7.1rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/RELEASE.md` & `nebari-2023.7.1rc1/RELEASE.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,72 @@
 If you want to update the release notes, open a PR against nebari-dev/nebari.
 This file is copied to nebari-dev/nebari-docs using a GitHub Action. -->
 
 ---
 
 ## Upcoming Release
 
+### Release 2023.5.1 - May 5, 2023
+
+### Feature changes and enhancements
+
+* Upgrade Argo-Workflows to version 3.4.4
+
+### Breaking Changes
+
+* The Argo-Workflows version upgrade will result in a breaking change if the existing Kubernetes CRDs are not deleted (see the NOTE below for more details).
+* There is a minor breaking change for the Nebari CLI version shorthand, previously it `nebari -v` and now to align with Python convention, it will be `nebari -V`.
+
+> NOTE: After installing the Nebari version `2023.5.1`, please run `nebari upgrade -c nebari-config.yaml` to upgrade
+> the `nebari-config.yaml`. This command will also prompt you to delete a few Kubernetes resources (specifically
+> the Argo-Workflows CRDS and service accounts) before you can upgrade.
+
+### What's Changed
+* Use --quiet flag for conda install in CI by @pmeier in https://github.com/nebari-dev/nebari/pull/1699
+* improve CLI tests by @pmeier in https://github.com/nebari-dev/nebari/pull/1710
+* Fix Existing dashboards by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1723
+* Fix dashboards by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1727
+* Typo in the conda-store <-> conda_store key by @costrouc in https://github.com/nebari-dev/nebari/pull/1740
+* use -V (upper case) for --version short form by @pmeier in https://github.com/nebari-dev/nebari/pull/1720
+* [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/nebari-dev/nebari/pull/1692
+* improve pytest configuration by @pmeier in https://github.com/nebari-dev/nebari/pull/1700
+* fix upgrade command to look for nebari_version instead of qhub_version by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1693
+* remove lazy import by @pmeier in https://github.com/nebari-dev/nebari/pull/1721
+* fix nebari invocation through python by @pmeier in https://github.com/nebari-dev/nebari/pull/1711
+* Update Argo Workflows to latest version by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1639
+* Update secret token in release-notes-sync action by @pavithraes in https://github.com/nebari-dev/nebari/pull/1753
+* Typo fix in release-notes-sync action by @pavithraes in https://github.com/nebari-dev/nebari/pull/1756
+* 🔄 Synced file(s) with nebari-dev/.github by @nebari-sensei in https://github.com/nebari-dev/nebari/pull/1758
+* Update path in release-notes-sync action by @pavithraes in https://github.com/nebari-dev/nebari/pull/1757
+* Updating heading format in release notes by @pavithraes in https://github.com/nebari-dev/nebari/pull/1761
+* Update vault url by @costrouc in https://github.com/nebari-dev/nebari/pull/1752
+* Fix? contributor test trigger by @pmeier in https://github.com/nebari-dev/nebari/pull/1734
+* Consistent user Experience with y/N. by @AM-O7 in https://github.com/nebari-dev/nebari/pull/1747
+* Fix contributor trigger by @pmeier in https://github.com/nebari-dev/nebari/pull/1765
+* add more debug output to contributor test trigger by @pmeier in https://github.com/nebari-dev/nebari/pull/1766
+* fix copy-paste error by @pmeier in https://github.com/nebari-dev/nebari/pull/1767
+* add instructions insufficient permissions of contributor trigger by @pmeier in https://github.com/nebari-dev/nebari/pull/1772
+* fix invalid escape sequence by @pmeier in https://github.com/nebari-dev/nebari/pull/1770
+* Update AMI  in `.cirun.yml` for nebari-dev-ci AWS account by @aktech in https://github.com/nebari-dev/nebari/pull/1776
+* [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/nebari-dev/nebari/pull/1768
+* turn warnings into errors with pytest by @pmeier in https://github.com/nebari-dev/nebari/pull/1774
+* purge setup.cfg by @pmeier in https://github.com/nebari-dev/nebari/pull/1781
+* improve pre-commit run on GHA by @pmeier in https://github.com/nebari-dev/nebari/pull/1782
+* Upgrade to k8s 1.24 by @iameskild in https://github.com/nebari-dev/nebari/pull/1760
+* Overloaded dask gateway fix by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1777
+* Add option to specify GKE release channel by @iameskild in https://github.com/nebari-dev/nebari/pull/1648
+* Update upgrade command, add RELEASE notes by @iameskild in https://github.com/nebari-dev/nebari/pull/1789
+
+### New Contributors
+* @pmeier made their first contribution in https://github.com/nebari-dev/nebari/pull/1699
+* @AM-O7 made their first contribution in https://github.com/nebari-dev/nebari/pull/1747
+
+**Full Changelog**: https://github.com/nebari-dev/nebari/compare/2023.4.1...2023.5.1
+
+
 ## Release 2023.4.1 - April 12, 2023
 
 > NOTE: Nebari requires Kubernetes version 1.23 and Digital Ocean now requires new clusters to run Kubernetes version 1.24. This means that if you are currently running on Digital Ocean, you should be fine but deploying on a new cluster on Digital Ocean is not possible until we upgrade Kubernetes version (see [issue 1622](https://github.com/nebari-dev/nebari/issues/1622) for more details).
 
 
 ### Feature changes and enhancements
```

### Comparing `nebari-2023.5.1rc1/flake.lock` & `nebari-2023.7.1rc1/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/flake.nix` & `nebari-2023.7.1rc1/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2023.7.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/workflows/kubernetes_test.yaml` & `nebari-2023.7.1rc1/.github/workflows/kubernetes_test.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -4,40 +4,39 @@
   pull_request:
     paths:
       - ".github/workflows/kubernetes_test.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
-      - "nebari/**"
+      - "src/**"
       - "pyproject.toml"
       - "pytest.ini"
   push:
     branches:
       - main
       - develop
       - release/\d{4}.\d{1,2}.\d{1,2}
     paths:
       - ".github/workflows/kubernetes_test.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
-      - "nebari/**"
+      - "src/**"
       - "pyproject.toml"
       - "pytest.ini"
   workflow_call:
     inputs:
       pr_number:
         required: true
         type: string
 
 jobs:
   test-kubernetes:
-    if: github.event.pull_request.head.repo.full_name == github.repository || github.event_name != 'pull_request'
     name: "Kubernetes Tests"
     runs-on: "cirun-runner--${{ github.run_id }}"
     defaults:
       run:
         shell: bash -l {0}
     steps:
 
@@ -66,14 +65,15 @@
         with:
           python-version: 3.8
           miniconda-version: "latest"
       - name: Install Nebari
         run: |
           conda install --quiet --yes -c anaconda pip
           pip install .[dev]
+          playwright install
       - name: Download and Install Kubectl
         run: |
           mkdir -p bin
           pushd bin
 
           curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.19.0/bin/linux/amd64/kubectl
           chmod +x kubectl
@@ -86,17 +86,14 @@
           sudo usermod -aG docker $USER && newgrp docker
 
           docker info
           docker ps
       - name: Get routing table for docker pods
         run: |
           ip route
-      - name: Add DNS entry to hosts
-        run: |
-          sudo echo "172.18.1.100  github-actions.nebari.dev" | sudo tee -a /etc/hosts
       - name: Initialize Nebari Cloud
         run: |
           mkdir -p local-deployment
           cd local-deployment
           nebari init local --project=thisisatest --domain github-actions.nebari.dev --auth-provider=password
 
           # Need smaller profiles on Local Kind
@@ -149,22 +146,35 @@
       - name: Cypress run
         uses: cypress-io/github-action@v4
         env:
           CYPRESS_BASE_URL: https://github-actions.nebari.dev/
         with:
           working-directory: tests_e2e
 
+      - name: Playwright Tests
+        env:
+          KEYCLOAK_USERNAME: ${{ env.CYPRESS_EXAMPLE_USER_NAME }}
+          KEYCLOAK_PASSWORD: ${{ env.CYPRESS_EXAMPLE_USER_PASSWORD }}
+          NEBARI_FULL_URL: https://github-actions.nebari.dev/
+        working-directory: tests_e2e/playwright
+        run: |
+          # create environment file
+          envsubst < .env.tpl > .env
+          # run playwright pytest tests in headed mode with the chromium browser
+          xvfb-run pytest --browser chromium
+
       - name: Save Cypress screenshots and videos
         if: always()
         uses: actions/upload-artifact@v3
         with:
           name: e2e-cypress
           path: |
             ./tests_e2e/cypress/screenshots/
             ./tests_e2e/cypress/videos/
+            ./tests_e2e/playwright/videos/
 
       - name: Deployment Pytests
         run: |
           export KEYCLOAK_USERNAME=${CYPRESS_EXAMPLE_USER_NAME}
           export KEYCLOAK_PASSWORD=${CYPRESS_EXAMPLE_USER_PASSWORD}
           pytest tests_deployment/ -v -s
```

### Comparing `nebari-2023.5.1rc1/.github/workflows/release-notes-sync.yaml` & `nebari-2023.7.1rc1/.github/workflows/release-notes-sync.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/workflows/release.yaml` & `nebari-2023.7.1rc1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/workflows/run-precommit.yaml` & `nebari-2023.7.1rc1/.github/workflows/run-precommit.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.github/workflows/test-provider.yaml` & `nebari-2023.7.1rc1/.github/workflows/test-provider.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,46 @@
+# This is only workflow that requires cloud credentials and therefore will not run on PRs coming from forks.
 name: "Test Nebari Provider"
 
 on:
+  schedule:
+    - cron: "0 3 * * *"
   pull_request:
     paths:
       - ".github/workflows/test-provider.yaml"
+      - ".github/failed-workflow-issue-templates/test-provider.md"
+      - ".github/actions/publish-from-template"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
-      - "nebari/**"
+      - "src/**"
       - "pyproject.toml"
   push:
     branches:
       - main
       - develop
       - release/\d{4}.\d{1,2}.\d{1,2}
     paths:
       - ".github/workflows/test-provider.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
-      - "nebari/**"
+      - "src/**"
       - "pyproject.toml"
   workflow_call:
     inputs:
       pr_number:
         required: true
         type: string
 
 jobs:
   test-render-providers:
+    # avoid running on PRs coming from a fork
     if: github.event.pull_request.head.repo.full_name == github.repository || github.event_name != 'pull_request'
     name: "Test Nebari Provider"
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: read
       pull-requests: write
@@ -47,14 +53,15 @@
           - gcp
           - local
           - existing
         cicd:
           - none
           - github-actions
           - gitlab-ci
+      fail-fast: false
     steps:
       - name: "Checkout Infrastructure"
         uses: actions/checkout@v3
 
       - name: Checkout the branch from the PR that triggered the job
         if: ${{ github.event_name == 'issue_comment' }}
         run: hub pr checkout ${{ inputs.pr_number }}
@@ -129,7 +136,17 @@
           cp "nebari-config.yaml" "nebari-${{ matrix.provider }}-${{ matrix.cicd }}-deployment/nebari-config.yaml"
 
       - name: Nebari Render Artifact
         uses: actions/upload-artifact@master
         with:
           name: "nebari-${{ matrix.provider }}-${{ matrix.cicd }}-artifact"
           path: "nebari-${{ matrix.provider }}-${{ matrix.cicd }}-deployment"
+
+      - if: failure() || github.event_name == 'pull_request'
+        name: Publish information from template
+        uses: ./.github/actions/publish-from-template
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          PROVIDER: ${{ matrix.provider }}
+          CICD: ${{ matrix.cicd }}
+        with:
+          filename: .github/failed-workflow-issue-templates/test-provider.md
```

### Comparing `nebari-2023.5.1rc1/.github/workflows/test.yaml` & `nebari-2023.7.1rc1/.github/workflows/test.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -2,45 +2,46 @@
 
 on:
   pull_request:
     paths:
       - ".github/workflows/test.yaml"
       - "tests/**"
       - "tests_deployment/**"
-      - "tests_e2e/**"
+      - "tests_e2e/cypress/**"
       - "scripts/**"
-      - "nebari/**"
+      - "src/**"
       - "pyproject.toml"
       - "pytest.ini"
   push:
     branches:
       - main
       - develop
       - release/\d{4}.\d{1,2}.\d{1,2}
     paths:
       - ".github/workflows/test.yaml"
       - "tests/**"
       - "tests_deployment/**"
-      - "tests_e2e/**"
+      - "tests_e2e/cypress/**"
       - "scripts/**"
-      - "nebari/**"
+      - "src/**"
       - "pyproject.toml"
       - "pytest.ini"
 
 jobs:
   test-general:
     name: "Pytest"
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
+      fail-fast: false
     steps:
       - name: "Checkout Infrastructure"
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup miniconda
         uses: conda-incubator/setup-miniconda@v2
@@ -51,8 +52,8 @@
       - name: Install Nebari
         run: |
           pip install .[dev]
           conda install --quiet --yes conda-build
       - name: Test Nebari
         run: |
           pytest --version
-          pytest --ignore=tests_deployment
+          pytest --ignore=tests_deployment --ignore=tests_e2e/playwright
```

### Comparing `nebari-2023.5.1rc1/nebari/deploy.py` & `nebari-2023.7.1rc1/src/_nebari/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
-import os
 import subprocess
 import textwrap
+from pathlib import Path
 
-from nebari.provider import terraform
-from nebari.provider.dns.cloudflare import update_record
-from nebari.stages import checks, input_vars, state_imports
-from nebari.utils import (
+from _nebari.provider import terraform
+from _nebari.provider.dns.cloudflare import update_record
+from _nebari.stages import checks, input_vars, state_imports
+from _nebari.utils import (
     check_cloud_credentials,
     keycloak_provider_context,
     kubernetes_provider_context,
     timer,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def provision_01_terraform_state(stage_outputs, config):
-    directory = "stages/01-terraform-state"
+    directory = Path("stages/01-terraform-state")
 
     if config["provider"] in {"existing", "local"}:
         stage_outputs[directory] = {}
     else:
         stage_outputs[directory] = terraform.deploy(
             terraform_import=True,
-            directory=os.path.join(directory, config["provider"]),
+            directory=directory / config["provider"],
             input_vars=input_vars.stage_01_terraform_state(stage_outputs, config),
             state_imports=state_imports.stage_01_terraform_state(stage_outputs, config),
         )
 
 
 def provision_02_infrastructure(stage_outputs, config, disable_checks=False):
     """Generalized method to provision infrastructure.
@@ -44,15 +44,15 @@
 
     At a high level this stage is expected to provision a kubernetes
     cluster on a given provider.
     """
     directory = "stages/02-infrastructure"
 
     stage_outputs[directory] = terraform.deploy(
-        os.path.join(directory, config["provider"]),
+        Path(directory) / config["provider"],
         input_vars=input_vars.stage_02_infrastructure(stage_outputs, config),
     )
 
     if not disable_checks:
         checks.stage_02_infrastructure(stage_outputs, config)
 
 
@@ -231,15 +231,15 @@
         ):
             provision_06_kubernetes_keycloak_configuration(
                 stage_outputs, config, disable_checks
             )
             provision_07_kubernetes_services(stage_outputs, config, disable_checks)
             provision_08_nebari_tf_extensions(stage_outputs, config, disable_checks)
 
-            print("Nebari deployed successfully")
+        print("Nebari deployed successfully")
 
     print("Services:")
     for service_name, service in stage_outputs["stages/07-kubernetes-services"][
         "service_urls"
     ]["value"].items():
         print(f" - {service_name} -> {service['url']}")
```

### Comparing `nebari-2023.5.1rc1/nebari/destroy.py` & `nebari-2023.7.1rc1/src/_nebari/destroy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 import logging
-import os
+from pathlib import Path
 
-from nebari.provider import terraform
-from nebari.stages import input_vars, state_imports
-from nebari.utils import (
+from _nebari.provider import terraform
+from _nebari.stages import input_vars, state_imports
+from _nebari.utils import (
     check_cloud_credentials,
     keycloak_provider_context,
     kubernetes_provider_context,
     timer,
 )
 
 logger = logging.getLogger(__name__)
@@ -26,21 +26,21 @@
     )
 
     if (
         config["provider"] not in {"existing", "local"}
         and config["terraform_state"]["type"] == "remote"
     ):
         stage_outputs["stages/01-terraform-state"] = _terraform_init_output(
-            directory=os.path.join("stages/01-terraform-state", config["provider"]),
+            directory=Path("stages/01-terraform-state") / config["provider"],
             input_vars=input_vars.stage_01_terraform_state(stage_outputs, config),
             state_imports=state_imports.stage_01_terraform_state(stage_outputs, config),
         )
 
     stage_outputs["stages/02-infrastructure"] = _terraform_init_output(
-        directory=os.path.join("stages/02-infrastructure", config["provider"]),
+        directory=Path("stages/02-infrastructure") / config["provider"],
         input_vars=input_vars.stage_02_infrastructure(stage_outputs, config),
     )
 
     stage_outputs["stages/03-kubernetes-initialize"] = _terraform_init_output(
         directory="stages/03-kubernetes-initialize",
         input_vars=input_vars.stage_03_kubernetes_initialize(stage_outputs, config),
     )
@@ -142,28 +142,28 @@
         status["stages/03-kubernetes-initialize"] = _terraform_destroy(
             directory="stages/03-kubernetes-initialize",
             input_vars=input_vars.stage_03_kubernetes_initialize(stage_outputs, config),
             ignore_errors=True,
         )
 
     status["stages/02-infrastructure"] = _terraform_destroy(
-        directory=os.path.join("stages/02-infrastructure", config["provider"]),
+        directory=Path("stages/02-infrastructure") / config["provider"],
         input_vars=input_vars.stage_02_infrastructure(stage_outputs, config),
         ignore_errors=True,
     )
 
     if (
         config["provider"] not in {"existing", "local"}
         and config["terraform_state"]["type"] == "remote"
     ):
         status["stages/01-terraform-state"] = _terraform_destroy(
             # acl and force_destroy do not import properly
             # and only get refreshed properly with an apply
             terraform_apply=True,
-            directory=os.path.join("stages/01-terraform-state", config["provider"]),
+            directory=Path("stages/01-terraform-state") / config["provider"],
             input_vars=input_vars.stage_01_terraform_state(stage_outputs, config),
             ignore_errors=True,
         )
 
     return status
```

### Comparing `nebari-2023.5.1rc1/nebari/initialize.py` & `nebari-2023.7.1rc1/src/_nebari/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import os
 import random
 import re
 import secrets
 import string
 import tempfile
+from pathlib import Path
 
 import requests
 
-from nebari.provider import git
-from nebari.provider.cicd import github
-from nebari.provider.oauth.auth0 import create_client
-from nebari.utils import (
+from _nebari.provider import git
+from _nebari.provider.cicd import github
+from _nebari.provider.oauth.auth0 import create_client
+from _nebari.utils import (
     check_cloud_credentials,
     namestr_regex,
     set_docker_image_tag,
     set_kubernetes_version,
     set_nebari_dask_version,
 )
 
@@ -371,20 +372,18 @@
 
     # Generate default password for Keycloak root user and also example-user if using password auth
     default_password = "".join(
         secrets.choice(string.ascii_letters + string.digits) for i in range(16)
     )
 
     # Save default password to file
-    default_password_filename = os.path.join(
-        tempfile.gettempdir(), "NEBARI_DEFAULT_PASSWORD"
-    )
+    default_password_filename = Path(tempfile.gettempdir()) / "NEBARI_DEFAULT_PASSWORD"
     with open(default_password_filename, "w") as f:
         f.write(default_password)
-    os.chmod(default_password_filename, 0o700)
+    default_password_filename.chmod(0o700)
 
     config["theme"]["jupyterhub"]["hub_title"] = f"Nebari - { project_name }"
     config["theme"]["jupyterhub"][
         "welcome"
     ] = """Welcome! Learn about Nebari's features and configurations in <a href="https://www.nebari.dev/docs">the documentation</a>. If you have any questions or feedback, reach the team on <a href="https://www.nebari.dev/docs/community#getting-support">Nebari's support forums</a>."""
 
     if auth_provider == "github":
```

### Comparing `nebari-2023.5.1rc1/nebari/keycloak.py` & `nebari-2023.7.1rc1/src/_nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/render.py` & `nebari-2023.7.1rc1/src/_nebari/render.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 import functools
 import hashlib
 import json
 import os
-import pathlib
 import shutil
 import sys
+from pathlib import Path
 from typing import Dict, List
 
 import yaml
 from rich import print
 from rich.table import Table
 from ruamel.yaml import YAML
 
-import nebari
-from nebari.deprecate import DEPRECATED_FILE_PATHS
-from nebari.provider.cicd.github import gen_nebari_linter, gen_nebari_ops
-from nebari.provider.cicd.gitlab import gen_gitlab_ci
-from nebari.stages import tf_objects
+import _nebari
+from _nebari.deprecate import DEPRECATED_FILE_PATHS
+from _nebari.provider.cicd.github import gen_nebari_linter, gen_nebari_ops
+from _nebari.provider.cicd.gitlab import gen_gitlab_ci
+from _nebari.stages import tf_objects
+from _nebari.utils import is_relative_to
 
 
-def render_template(output_directory, config_filename, force=False, dry_run=False):
+def render_template(output_directory, config_filename, dry_run=False):
     # get directory for nebari templates
-    template_directory = pathlib.Path(nebari.__file__).parent / "template"
+    template_directory = Path(_nebari.__file__).parent / "template"
 
     # would be nice to remove assumption that input directory
     # is in local filesystem and a directory
-    template_directory = pathlib.Path(template_directory)
     if not template_directory.is_dir():
         raise ValueError(f"template directory={template_directory} is not a directory")
 
-    output_directory = pathlib.Path(output_directory).resolve()
-
-    if output_directory == str(pathlib.Path.home()):
+    if output_directory == Path.home():
         print("ERROR: Deploying Nebari in home directory is not advised!")
         sys.exit(1)
 
     # mkdir all the way down to repo dir so we can copy .gitignore
     # into it in remove_existing_renders
     output_directory.mkdir(exist_ok=True, parents=True)
 
-    config_filename = pathlib.Path(config_filename)
     if not config_filename.is_file():
         raise ValueError(
             f"cookiecutter configuration={config_filename} is not filename"
         )
 
-    with config_filename.open() as f:
+    with open(config_filename) as f:
         yaml = YAML(typ="safe", pure=True)
         config = yaml.load(f)
 
     # For any config values that start with
     # NEBARI_SECRET_, set the values using the
     # corresponding env var.
     set_env_vars_in_config(config)
@@ -70,21 +67,21 @@
     ]
     if (
         config["provider"] not in {"existing", "local"}
         and config["terraform_state"]["type"] == "remote"
     ):
         directories.append(f"stages/01-terraform-state/{config['provider']}")
 
-    source_dirs = [os.path.join(str(template_directory), _) for _ in directories]
-    output_dirs = [os.path.join(str(output_directory), _) for _ in directories]
+    source_dirs = [template_directory / Path(directory) for directory in directories]
+    output_dirs = [output_directory / Path(directory) for directory in directories]
     new, untracked, updated, deleted = inspect_files(
         source_dirs,
         output_dirs,
-        source_base_dir=str(template_directory),
-        output_base_dir=str(output_directory),
+        source_base_dir=template_directory,
+        output_base_dir=output_directory,
         ignore_filenames=[
             "terraform.tfstate",
             ".terraform.lock.hcl",
             "terraform.tfstate.backup",
         ],
         ignore_directories=[
             ".terraform",
@@ -93,66 +90,65 @@
         deleted_paths=DEPRECATED_FILE_PATHS,
         contents=contents,
     )
 
     if new:
         table = Table("The following files will be created:", style="deep_sky_blue1")
         for filename in sorted(new):
-            table.add_row(filename, style="green")
+            table.add_row(str(filename), style="green")
         print(table)
     if updated:
         table = Table("The following files will be updated:", style="deep_sky_blue1")
         for filename in sorted(updated):
-            table.add_row(filename, style="green")
+            table.add_row(str(filename), style="green")
         print(table)
     if deleted:
         table = Table("The following files will be deleted:", style="deep_sky_blue1")
         for filename in sorted(deleted):
-            table.add_row(filename, style="green")
+            table.add_row(str(filename), style="green")
         print(table)
     if untracked:
         table = Table(
             "The following files are untracked (only exist in output directory):",
             style="deep_sky_blue1",
         )
         for filename in sorted(updated):
-            table.add_row(filename, style="green")
+            table.add_row(str(filename), style="green")
         print(table)
 
     if dry_run:
         print("dry-run enabled no files will be created, updated, or deleted")
     else:
         for filename in new | updated:
-            input_filename = os.path.join(str(template_directory), filename)
-            output_filename = os.path.join(str(output_directory), filename)
-            os.makedirs(os.path.dirname(output_filename), exist_ok=True)
+            input_filename = template_directory / filename
+            output_filename = output_directory / filename
+            output_filename.parent.mkdir(parents=True, exist_ok=True)
 
-            if os.path.exists(input_filename):
+            if input_filename.exists():
                 shutil.copy(input_filename, output_filename)
             else:
                 with open(output_filename, "w") as f:
                     f.write(contents[filename])
 
         for path in deleted:
-            abs_path = os.path.abspath(os.path.join(str(output_directory), path))
+            abs_path = (output_directory / path).resolve()
 
-            # be extra cautious that deleted path is within output_directory
-            if not abs_path.startswith(str(output_directory)):
+            if not is_relative_to(abs_path, output_directory):
                 raise Exception(
                     f"[ERROR] SHOULD NOT HAPPEN filename was about to be deleted but path={abs_path} is outside of output_directory"
                 )
 
-            if os.path.isfile(abs_path):
-                os.remove(abs_path)
-            elif os.path.isdir(abs_path):
+            if abs_path.is_file():
+                abs_path.unlink()
+            elif abs_path.is_dir():
                 shutil.rmtree(abs_path)
 
 
 def render_contents(config: Dict):
-    """Dynamically generated contents from Nebari configuration."""
+    """Dynamically generated contents from _nebari configuration."""
     contents = {
         **tf_objects.stage_01_terraform_state(config),
         **tf_objects.stage_02_infrastructure(config),
         **tf_objects.stage_03_kubernetes_initialize(config),
         **tf_objects.stage_04_kubernetes_ingress(config),
         **tf_objects.stage_05_kubernetes_keycloak(config),
         **tf_objects.stage_06_kubernetes_keycloak_configuration(config),
@@ -169,37 +165,37 @@
                 exclude_defaults=True,
             )
             workflow_yaml = yaml.dump(
                 json.loads(workflow_json), sort_keys=False, indent=2
             )
             contents.update({fn: workflow_yaml})
 
-    contents.update(gen_gitignore(config))
+    contents.update(gen_gitignore())
 
     return contents
 
 
-def gen_gitignore(config):
+def gen_gitignore():
     """
     Generate `.gitignore` file.
     Add files as needed.
     """
     from inspect import cleandoc
 
-    filestoignore = """
+    files_to_ignore = """
         # ignore terraform state
         .terraform
         terraform.tfstate
         terraform.tfstate.backup
         .terraform.tfstate.lock.info
 
         # python
         __pycache__
     """
-    return {".gitignore": cleandoc(filestoignore)}
+    return {Path(".gitignore"): cleandoc(files_to_ignore)}
 
 
 def gen_cicd(config):
     """
     Use cicd schema to generate workflow files based on the
     `ci_cd` key in the `config`.
 
@@ -207,88 +203,94 @@
     GiHub-Actions - nebari/providers/cicd/github.py
     GitLab-CI - nebari/providers/cicd/gitlab.py
     """
     cicd_files = {}
     cicd_provider = config["ci_cd"]["type"]
 
     if cicd_provider == "github-actions":
-        gha_dir = ".github/workflows/"
-        cicd_files[gha_dir + "nebari-ops.yaml"] = gen_nebari_ops(config)
-        cicd_files[gha_dir + "nebari-linter.yaml"] = gen_nebari_linter(config)
+        gha_dir = Path(".github") / "workflows"
+        cicd_files[gha_dir / "nebari-ops.yaml"] = gen_nebari_ops(config)
+        cicd_files[gha_dir / "nebari-linter.yaml"] = gen_nebari_linter(config)
 
     elif cicd_provider == "gitlab-ci":
-        cicd_files[".gitlab-ci.yml"] = gen_gitlab_ci(config)
+        cicd_files[Path(".gitlab-ci.yml")] = gen_gitlab_ci(config)
 
     else:
         raise ValueError(
             f"The ci_cd provider, {cicd_provider}, is not supported. Supported providers include: `github-actions`, `gitlab-ci`."
         )
 
     return cicd_files
 
 
 def inspect_files(
-    source_dirs: str,
-    output_dirs: str,
-    source_base_dir: str,
-    output_base_dir: str,
+    source_dirs: Path,
+    output_dirs: Path,
+    source_base_dir: Path,
+    output_base_dir: Path,
     ignore_filenames: List[str] = None,
     ignore_directories: List[str] = None,
-    deleted_paths: List[str] = None,
+    deleted_paths: List[Path] = None,
     contents: Dict[str, str] = None,
 ):
     """Return created, updated and untracked files by computing a checksum over the provided directory.
 
     Args:
-        source_dirs (str): The source dir used as base for comparssion
-        output_dirs (str): The destination dir which will be matched with
-        source_base_dir (str): Relative base path to source directory
-        output_base_dir (str): Relative base path to output directory
+        source_dirs (Path): The source dir used as base for comparison
+        output_dirs (Path): The destination dir which will be matched with
+        source_base_dir (Path): Relative base path to source directory
+        output_base_dir (Path): Relative base path to output directory
         ignore_filenames (list[str]): Filenames to ignore while comparing for changes
         ignore_directories (list[str]): Directories to ignore while comparing for changes
-        deleted_paths (list[str]): Paths that if exist in output directory should be deleted
+        deleted_paths (list[Path]): Paths that if exist in output directory should be deleted
         contents (dict): filename to content mapping for dynamically generated files
     """
     ignore_filenames = ignore_filenames or []
     ignore_directories = ignore_directories or []
     contents = contents or {}
 
     source_files = {}
     output_files = {}
 
     def list_files(
-        directory: str, ignore_filenames: List[str], ignore_directories: List[str]
+        directory: Path, ignore_filenames: List[str], ignore_directories: List[str]
     ):
-        for root, dirs, files in os.walk(directory):
-            dirs[:] = [d for d in dirs if d not in ignore_directories]
-            for file in files:
-                if file not in ignore_filenames:
-                    yield os.path.join(root, file)
-
-    for filename in contents:
-        source_files[filename] = hashlib.sha256(
-            contents[filename].encode("utf8")
-        ).hexdigest()
-        output_filename = os.path.join(output_base_dir, filename)
-        if os.path.isfile(output_filename):
+        for path in directory.rglob("*"):
+            if not path.is_file():
+                continue
+
+            if path.name in ignore_filenames:
+                continue
+
+            if any(
+                d in ignore_directories for d in path.relative_to(directory).parts[:-1]
+            ):
+                continue
+
+            yield path
+
+    for filename, content in contents.items():
+        source_files[filename] = hashlib.sha256(content.encode("utf8")).hexdigest()
+        output_filename = output_base_dir / filename
+        if output_filename.is_file():
             output_files[filename] = hash_file(filename)
 
-    deleted_paths = set()
+    deleted_files = set()
     for path in deleted_paths:
-        absolute_path = os.path.join(output_base_dir, path)
-        if os.path.exists(absolute_path):
-            deleted_paths.add(path)
+        absolute_path = output_base_dir / path
+        if absolute_path.exists():
+            deleted_files.add(path)
 
     for source_dir, output_dir in zip(source_dirs, output_dirs):
         for filename in list_files(source_dir, ignore_filenames, ignore_directories):
-            relative_path = os.path.relpath(filename, source_base_dir)
+            relative_path = filename.relative_to(source_base_dir)
             source_files[relative_path] = hash_file(filename)
 
         for filename in list_files(output_dir, ignore_filenames, ignore_directories):
-            relative_path = os.path.relpath(filename, output_base_dir)
+            relative_path = filename.relative_to(output_base_dir)
             output_files[relative_path] = hash_file(filename)
 
     new_files = source_files.keys() - output_files.keys()
     untracted_files = output_files.keys() - source_files.keys()
 
     updated_files = set()
     for prevalent_file in source_files.keys() & output_files.keys():
```

### Comparing `nebari-2023.5.1rc1/nebari/schema.py` & `nebari-2023.7.1rc1/src/_nebari/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import enum
 import typing
 from abc import ABC
 
 import pydantic
 from pydantic import root_validator, validator
 
-from nebari.utils import namestr_regex
+from _nebari.utils import namestr_regex
 
 from .version import __version__, rounded_ver_parse
 
 
 class CertificateEnum(str, enum.Enum):
     letsencrypt = "lets-encrypt"
     selfsigned = "self-signed"
@@ -82,17 +82,23 @@
     version: str
     overrides: typing.Optional[typing.Dict]
 
 
 # ============== Argo-Workflows =========
 
 
+class NebariWorkflowController(Base):
+    enabled: bool
+    image_tag: typing.Optional[str]
+
+
 class ArgoWorkflows(Base):
     enabled: bool
     overrides: typing.Optional[typing.Dict]
+    nebari_workflow_controller: typing.Optional[NebariWorkflowController]
 
 
 # ============== kbatch =============
 
 
 class KBatch(Base):
     enabled: bool
```

### Comparing `nebari-2023.5.1rc1/nebari/upgrade.py` & `nebari-2023.7.1rc1/src/_nebari/upgrade.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import json
 import logging
-import pathlib
 import re
 import secrets
 import string
 from abc import ABC
+from pathlib import Path
 
 import rich
 from pydantic.error_wrappers import ValidationError
 from rich.prompt import Prompt
 
 from .schema import is_version_accepted, verify
 from .utils import backup_config_file, load_yaml, yaml
 from .version import __version__, rounded_ver_parse
 
 logger = logging.getLogger(__name__)
 
+NEBARI_WORKFLOW_CONTROLLER_DOCS = (
+    "https://www.nebari.dev/docs/how-tos/using-argo/#jupyterflow-override-beta"
+)
+ARGO_JUPYTER_SCHEDULER_REPO = "https://github.com/nebari-dev/argo-jupyter-scheduler"
+
 
 def do_upgrade(config_filename, attempt_fixes=False):
     config = load_yaml(config_filename)
     if config.get("qhub_version"):
         rich.print(
             f"Your config file [purple]{config_filename}[/purple] uses the deprecated qhub_version key.  Please change qhub_version to nebari_version and re-run the upgrade command."
         )
@@ -30,40 +35,43 @@
         rich.print(
             f"Your config file [purple]{config_filename}[/purple] appears to be already up-to-date for Nebari version [green]{__version__}[/green]"
         )
         return
     except (ValidationError, ValueError) as e:
         if is_version_accepted(config.get("nebari_version", "")):
             # There is an unrelated validation problem
-            print(
-                f"Your config file {config_filename} appears to be already up-to-date for Nebari version {__version__} but there is another validation error.\n"
+            rich.print(
+                f"Your config file [purple]{config_filename}[/purple] appears to be already up-to-date for Nebari version [green]{__version__}[/green] but there is another validation error.\n"
             )
             raise e
 
     start_version = config.get("nebari_version", "")
+    print("start_version: ", start_version)
 
     UpgradeStep.upgrade(
         config, start_version, __version__, config_filename, attempt_fixes
     )
+    print(config.get("nebari_version"))
+    print(config.get("default_images"))
 
     # Backup old file
     backup_config_file(config_filename, f".{start_version or 'old'}")
 
     with config_filename.open("wt") as f:
         yaml.dump(config, f)
 
-    print(
-        f"Saving new config file {config_filename} ready for Nebari version {__version__}"
+    rich.print(
+        f"Saving new config file [purple]{config_filename}[/purple] ready for Nebari version [green]{__version__}[/green]"
     )
 
     ci_cd = config.get("ci_cd", {}).get("type", "")
     if ci_cd in ("github-actions", "gitlab-ci"):
-        print(
-            f"\nSince you are using ci_cd {ci_cd} you also need to re-render the workflows and re-commit the files to your Git repo:\n"
-            f"   nebari render -c {config_filename}\n"
+        rich.print(
+            f"\nSince you are using ci_cd [green]{ci_cd}[/green] you also need to re-render the workflows and re-commit the files to your Git repo:\n"
+            f"   nebari render -c [purple]{config_filename}[/purple]\n"
         )
 
 
 class UpgradeStep(ABC):
     _steps = {}
 
     version = ""  # Each subclass must have a version - these should be full release versions (not dev/prerelease)
@@ -85,14 +93,15 @@
     ):
         """
         Runs through all required upgrade steps (i.e. relevant subclasses of UpgradeStep).
         Calls UpgradeStep.upgrade_step for each.
         """
         starting_ver = rounded_ver_parse(start_version or "0.0.0")
         finish_ver = rounded_ver_parse(finish_version)
+        print("finish_ver: ", finish_ver)
 
         if finish_ver < starting_ver:
             raise ValueError(
                 f"Your nebari-config.yaml already belongs to a later version ({start_version}) than the installed version of Nebari ({finish_version}).\n"
                 "You should upgrade the installed nebari package (e.g. pip install --upgrade nebari) to work with your deployment."
             )
 
@@ -102,14 +111,16 @@
                 for v in cls._steps.keys()
                 if rounded_ver_parse(v) > starting_ver
                 and rounded_ver_parse(v) <= finish_ver
             ],
             key=rounded_ver_parse,
         )
 
+        print("step_versions: ", step_versions)
+
         current_start_version = start_version
         for stepcls in [cls._steps[str(v)] for v in step_versions]:
             step = stepcls()
             config = step.upgrade_step(
                 config,
                 current_start_version,
                 config_filename,
@@ -140,70 +151,115 @@
         It should normally be left as-is for all upgrades. Use _version_specific_upgrade below
         for any actions that are only required for the particular upgrade you are creating.
         """
         finish_version = self.get_version()
         __rounded_finish_version__ = ".".join(
             [str(c) for c in rounded_ver_parse(finish_version)]
         )
-
-        print(
-            f"\n---> Starting upgrade from {start_version or 'old version'} to {finish_version}\n"
+        rich.print(
+            f"\n---> Starting upgrade from [green]{start_version or 'old version'}[/green] to [green]{finish_version}[/green]\n"
         )
 
         # Set the new version
         if start_version == "":
             assert "nebari_version" not in config
         assert self.version != start_version
 
         if self.requires_nebari_version_field():
-            print(f"Setting nebari_version to {self.version}")
+            rich.print(f"Setting nebari_version to [green]{self.version}[/green]")
             config["nebari_version"] = self.version
 
-        # Update images
-        start_version_regex = start_version.replace(".", "\\.")
-        if start_version == "":
-            print("Looking for any previous image version")
-            start_version_regex = "0\\.[0-3]\\.[0-9]{1,2}"
-        docker_image_regex = re.compile(
-            f"^([A-Za-z0-9_-]+/[A-Za-z0-9_-]+):v{start_version_regex}$"
-        )
+        def contains_image_and_tag(s: str) -> bool:
+            # match on `quay.io/nebari/nebari-<...>:YYYY.MM.XX``
+            pattern = r"^quay\.io\/nebari\/nebari-(jupyterhub|jupyterlab|dask-worker):\d{4}\.\d+\.\d+$"
+            return bool(re.match(pattern, s))
+
+        def replace_image_tag_legacy(image, start_version, new_version):
+            start_version_regex = start_version.replace(".", "\\.")
+            if not start_version:
+                start_version_regex = "0\\.[0-3]\\.[0-9]{1,2}"
 
-        def _new_docker_image(
-            v,
-        ):
-            m = docker_image_regex.match(v)
+            docker_image_regex = re.compile(
+                f"^([A-Za-z0-9_-]+/[A-Za-z0-9_-]+):v{start_version_regex}$"
+            )
+
+            m = docker_image_regex.match(image)
             if m:
-                return ":".join([m.groups()[0], f"v{__rounded_finish_version__}"])
+                return ":".join([m.groups()[0], f"v{new_version}"])
             return None
 
+        def replace_image_tag(s: str, new_version: str, config_path: str) -> str:
+            legacy_replacement = replace_image_tag_legacy(s, start_version, new_version)
+            if legacy_replacement:
+                return legacy_replacement
+
+            if not contains_image_and_tag(s):
+                return s
+            image_name, current_tag = s.split(":")
+            if current_tag == new_version:
+                return s
+            loc = f"{config_path}: {image_name}"
+            response = Prompt.ask(
+                f"\nDo you want to replace current tag [green]{current_tag}[/green] with [green]{new_version}[/green] for:\n[purple]{loc}[/purple]? [Y/n] ",
+                default="Y",
+            )
+            if response.lower() in ["y", "yes", ""]:
+                return s.replace(current_tag, new_version)
+            else:
+                return s
+
+        def set_nested_item(config: dict, config_path: list, value: str):
+            config_path = config_path.split(".")
+            for k in config_path[:-1]:
+                try:
+                    k = int(k)
+                except ValueError:
+                    pass
+                config = config[k]
+            try:
+                config_path[-1] = int(config_path[-1])
+            except ValueError:
+                pass
+            config[config_path[-1]] = value
+
+        def update_image_tag(config, config_path, current_image, new_version):
+            new_image = replace_image_tag(current_image, new_version, config_path)
+            if new_image != current_image:
+                set_nested_item(config, config_path, new_image)
+
+            return config
+
+        # update default_images
         for k, v in config.get("default_images", {}).items():
-            newimage = _new_docker_image(v)
-            if newimage:
-                print(f"In default_images: {k}: upgrading {v} to {newimage}")
-                config["default_images"][k] = newimage
+            config_path = f"default_images.{k}"
+            config = update_image_tag(
+                config, config_path, v, __rounded_finish_version__
+            )
 
+        # update profiles.jupyterlab images
         for i, v in enumerate(config.get("profiles", {}).get("jupyterlab", [])):
-            oldimage = v.get("kubespawner_override", {}).get("image", "")
-            newimage = _new_docker_image(oldimage)
-            if newimage:
-                print(
-                    f"In profiles: jupyterlab: [{i}]: upgrading {oldimage} to {newimage}"
+            current_image = v.get("kubespawner_override", {}).get("image", None)
+            if current_image:
+                config = update_image_tag(
+                    config,
+                    f"profiles.jupyterlab.{i}.kubespawner_override.image",
+                    current_image,
+                    __rounded_finish_version__,
                 )
-                config["profiles"]["jupyterlab"][i]["kubespawner_override"][
-                    "image"
-                ] = newimage
 
+        # update profiles.dask_worker images
         for k, v in config.get("profiles", {}).get("dask_worker", {}).items():
-            oldimage = v.get("image", "")
-            newimage = _new_docker_image(oldimage)
-            if newimage:
-                print(
-                    f"In profiles: dask_worker: {k}: upgrading {oldimage} to {newimage}"
+            current_image = v.get("kubespawner_override", {}).get("image", None)
+            if current_image:
+                config = update_image_tag(
+                    config,
+                    f"profiles.dask_worker.{k}.kubespawner_override.image",
+                    current_image,
+                    __rounded_finish_version__,
                 )
-                config["profiles"]["dask_worker"][k]["image"] = newimage
 
         # Run any version-specific tasks
         return self._version_specific_upgrade(
             config, start_version, config_filename, *args, **kwargs
         )
 
     def _version_specific_upgrade(
@@ -222,24 +278,26 @@
         self, config, start_version, config_filename, *args, **kwargs
     ):
         """
         This version of Nebari requires a conda_store image for the first time.
         """
         if config.get("default_images", {}).get("conda_store", None) is None:
             newimage = "quansight/conda-store-server:v0.3.3"
-            print(f"Adding default_images: conda_store image as {newimage}")
+            rich.print(
+                f"Adding default_images: conda_store image as [green]{newimage}[/green]"
+            )
             config["default_images"]["conda_store"] = newimage
         return config
 
 
 class Upgrade_0_4_0(UpgradeStep):
     version = "0.4.0"
 
     def _version_specific_upgrade(
-        self, config, start_version, config_filename: pathlib.Path, *args, **kwargs
+        self, config, start_version, config_filename: Path, *args, **kwargs
     ):
         """
         Upgrade to Keycloak.
         """
         security = config.get("security", {})
         users = security.get("users", {})
         groups = security.get("groups", {})
@@ -255,16 +313,16 @@
                 "requirements within Keycloak."
             )
             if not kwargs.get("attempt_fixes", False):
                 raise ValueError(
                     f"{customauth_warning}\n\nRun `nebari upgrade --attempt-fixes` to switch to basic Keycloak authentication instead."
                 )
             else:
-                print(f"\nWARNING: {customauth_warning}")
-                print(
+                rich.print(f"\nWARNING: {customauth_warning}")
+                rich.print(
                     "\nSwitching to basic Keycloak authentication instead since you specified --attempt-fixes."
                 )
                 config["security"]["authentication"] = {"type": "password"}
 
         # Create a group/user import file for Keycloak
 
         realm_import_filename = config_filename.parent / "nebari-users-import.json"
@@ -293,16 +351,16 @@
         ]
 
         backup_config_file(realm_import_filename)
 
         with realm_import_filename.open("wt") as f:
             json.dump(realm, f, indent=2)
 
-        print(
-            f"\nSaving user/group import file {realm_import_filename}.\n\n"
+        rich.print(
+            f"\nSaving user/group import file [purple]{realm_import_filename}[/purple].\n\n"
             "ACTION REQUIRED: You must import this file into the Keycloak admin webpage after you redeploy Nebari.\n"
             "Visit the URL path /auth/ and login as 'root'. Under Manage, click Import and select this file.\n\n"
             "Non-admin users will default to analyst group membership after the upgrade (no dask access), "
             "so you may wish to promote some users into the developer group.\n"
         )
 
         if "users" in security:
@@ -311,15 +369,15 @@
             if "users" in security["groups"]:
                 # Ensure the users default group is added to Keycloak
                 security["shared_users_group"] = True
             del security["groups"]
 
         if "terraform_modules" in config:
             del config["terraform_modules"]
-            print(
+            rich.print(
                 "Removing terraform_modules field from config as it is no longer used.\n"
             )
 
         # Remove conda_store image from default_images
         if "conda_store" in config["default_images"]:
             del config["default_images"]["conda_store"]
 
@@ -329,16 +387,16 @@
 
         # Create root password
         default_password = "".join(
             secrets.choice(string.ascii_letters + string.digits) for i in range(16)
         )
         security.setdefault("keycloak", {})["initial_root_password"] = default_password
 
-        print(
-            f"Generated default random password={default_password} for Keycloak root user (Please change at /auth/ URL path).\n"
+        rich.print(
+            f"Generated default random password=[green]{default_password}[/green] for Keycloak root user (Please change at /auth/ URL path).\n"
         )
 
         # project was never needed in Azure - it remained as PLACEHOLDER in earlier nebari inits!
         if "azure" in config:
             if "project" in config["azure"]:
                 del config["azure"]["project"]
 
@@ -360,61 +418,93 @@
         return config
 
 
 class Upgrade_0_4_1(UpgradeStep):
     version = "0.4.1"
 
     def _version_specific_upgrade(
-        self, config, start_version, config_filename: pathlib.Path, *args, **kwargs
+        self, config, start_version, config_filename: Path, *args, **kwargs
     ):
         """
         Upgrade jupyterlab profiles.
         """
-        print("\nUpgrading jupyterlab profiles in order to specify access type:\n")
+        rich.print("\nUpgrading jupyterlab profiles in order to specify access type:\n")
 
         profiles_jupyterlab = config.get("profiles", {}).get("jupyterlab", [])
         for profile in profiles_jupyterlab:
             name = profile.get("display_name", "")
 
             if "groups" in profile or "users" in profile:
                 profile["access"] = "yaml"
             else:
                 profile["access"] = "all"
 
-            print(
-                f"Setting access type of JupyterLab profile {name} to {profile['access']}"
+            rich.print(
+                f"Setting access type of JupyterLab profile [green]{name}[/green] to [green]{profile['access']}[/green]"
             )
         return config
 
 
 class Upgrade_2023_4_2(UpgradeStep):
     version = "2023.4.2"
 
     def _version_specific_upgrade(
-        self, config, start_version, config_filename: pathlib.Path, *args, **kwargs
+        self, config, start_version, config_filename: Path, *args, **kwargs
     ):
         """
         Prompt users to delete Argo CRDs
         """
 
         kubectl_delete_argo_crds_cmd = "kubectl delete crds clusterworkflowtemplates.argoproj.io cronworkflows.argoproj.io workfloweventbindings.argoproj.io workflows.argoproj.io workflowtasksets.argoproj.io workflowtemplates.argoproj.io"
 
+        kubectl_delete_argo_sa_cmd = (
+            f"kubectl delete sa -n {config['namespace']} argo-admin argo-dev argo-view"
+        )
+
         rich.print(
-            f"\n\n[bold cyan]Note:[/] Upgrading requires a one-time manual deletion of the Argo Workflows Custom Resource Definitions (CRDs). \n\n[red bold]Warning:  [link=https://{config['domain']}/argo/workflows]Workflows[/link] and [link=https://{config['domain']}/argo/workflows]CronWorkflows[/link] created before deleting the CRDs will be erased when the CRDs are deleted and will not be restored.[/red bold] \n\nThe updated CRDs will be installed during the next [cyan bold]nebari deploy[/cyan bold] step. Argo Workflows will not function after deleting the CRDs until the updated CRDs are installed in the next nebari deploy. You must delete the Argo CRDs before upgrading to {self.version} or deploy step will fail.  Please delete them before proceeding by generating a kubeconfig (see [link=https://www.nebari.dev/docs/how-tos/debug-nebari/#generating-the-kubeconfig]docs[/link]), installing kubectl (see [link=https://www.nebari.dev/docs/how-tos/debug-nebari#installing-kubectl]docs[/link]), and running the following command:\n\n\t[cyan bold]{kubectl_delete_argo_crds_cmd} [/cyan bold]\n"
+            f"\n\n[bold cyan]Note:[/] Upgrading requires a one-time manual deletion of the Argo Workflows Custom Resource Definitions (CRDs) and service accounts. \n\n[red bold]Warning:  [link=https://{config['domain']}/argo/workflows]Workflows[/link] and [link=https://{config['domain']}/argo/workflows]CronWorkflows[/link] created before deleting the CRDs will be erased when the CRDs are deleted and will not be restored.[/red bold] \n\nThe updated CRDs will be installed during the next [cyan bold]nebari deploy[/cyan bold] step. Argo Workflows will not function after deleting the CRDs until the updated CRDs and service accounts are installed in the next nebari deploy. You must delete the Argo Workflows CRDs and service accounts before upgrading to {self.version} (or later) or the deploy step will fail.  Please delete them before proceeding by generating a kubeconfig (see [link=https://www.nebari.dev/docs/how-tos/debug-nebari/#generating-the-kubeconfig]docs[/link]), installing kubectl (see [link=https://www.nebari.dev/docs/how-tos/debug-nebari#installing-kubectl]docs[/link]), and running the following two commands:\n\n\t[cyan bold]{kubectl_delete_argo_crds_cmd} [/cyan bold]\n\n\t[cyan bold]{kubectl_delete_argo_sa_cmd} [/cyan bold]"
             ""
         )
 
-        continue_ = Prompt.ask("Have you deleted the Argo CRDs? [y/N]", default="N")
+        continue_ = Prompt.ask(
+            "Have you deleted the Argo Workflows CRDs and service accounts? [y/N] ",
+            default="N",
+        )
         if not continue_ == "y":
-            print(f"You must delete the Argo CRDs before upgrading to {self.version}")
+            rich.print(
+                f"You must delete the Argo Workflows CRDs and service accounts before upgrading to [green]{self.version}[/green] (or later)."
+            )
             exit()
 
         return config
 
 
+class Upgrade_2023_5_2(UpgradeStep):
+    version = "2023.5.2"
+
+    def _version_specific_upgrade(
+        self, config, start_version, config_filename: Path, *args, **kwargs
+    ):
+        argo = config.get("argo_workflows", {})
+        if argo.get("enabled"):
+            response = Prompt.ask(
+                f"\nDo you want to enable the [green][link={NEBARI_WORKFLOW_CONTROLLER_DOCS}]Nebari Workflow Controller[/link][/green], required for [green][link={ARGO_JUPYTER_SCHEDULER_REPO}]Argo-Jupyter-Scheduler[/link][green]? [Y/n] ",
+                default="Y",
+            )
+            if response.lower() in ["y", "yes", ""]:
+                argo["nebari_workflow_controller"] = {"enabled": True}
+
+        rich.print("\n ⚠️ Deprecation Warnings ⚠️")
+        rich.print(
+            f"-> [green]{self.version}[/green] is the last Nebari version that supports CDS Dashboards"
+        )
+
+        return config
+
+
 __rounded_version__ = ".".join([str(c) for c in rounded_ver_parse(__version__)])
 
 # Manually-added upgrade steps must go above this line
 if not UpgradeStep.has_step(__rounded_version__):
     # Always have a way to upgrade to the latest full version number, even if no customizations
     # Don't let dev/prerelease versions cloud things
     class UpgradeLatest(UpgradeStep):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nebari-2023.5.1rc1/nebari/utils.py` & `nebari-2023.7.1rc1/src/_nebari/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 import contextlib
 import functools
 import os
-import pathlib
 import re
 import signal
 import subprocess
 import sys
 import threading
 import time
+from pathlib import Path
 from typing import Dict, List
 
 from ruamel.yaml import YAML
 
-from nebari.constants import DEFAULT_NEBARI_DASK_VERSION, DEFAULT_NEBARI_IMAGE_TAG
-from nebari.provider.cloud import (
+from _nebari.constants import DEFAULT_NEBARI_DASK_VERSION, DEFAULT_NEBARI_IMAGE_TAG
+from _nebari.provider.cloud import (
     amazon_web_services,
     azure_cloud,
     digital_ocean,
     google_cloud,
 )
 
 # environment variable overrides
 NEBARI_K8S_VERSION = os.getenv("NEBARI_K8S_VERSION", None)
 NEBARI_GH_BRANCH = os.getenv("NEBARI_GH_BRANCH", None)
 NEBARI_IMAGE_TAG = os.getenv("NEBARI_IMAGE_TAG", None)
 NEBARI_DASK_VERSION = os.getenv("NEBARI_DASK_VERSION", None)
 
-DO_ENV_DOCS = (
-    "https://docs.qhub.dev/en/stable/source/installation/setup.html#digital-ocean"
-)
-AWS_ENV_DOCS = "https://docs.qhub.dev/en/stable/source/installation/setup.html#amazon-web-services-aws"
-GCP_ENV_DOCS = "https://docs.qhub.dev/en/stable/source/installation/setup.html#google-cloud-platform"
-AZURE_ENV_DOCS = (
-    "https://docs.qhub.dev/en/stable/source/installation/setup.html#microsoft-azure"
-)
+DO_ENV_DOCS = "https://www.nebari.dev/docs/how-tos/nebari-do"
+AWS_ENV_DOCS = "https://www.nebari.dev/docs/how-tos/nebari-aws"
+GCP_ENV_DOCS = "https://www.nebari.dev/docs/how-tos/nebari-gcp"
+AZURE_ENV_DOCS = "https://www.nebari.dev/docs/how-tos/nebari-azure"
 
 CONDA_FORGE_CHANNEL_DATA_URL = "https://conda.anaconda.org/conda-forge/channeldata.json"
 
 # Regex for suitable project names
 namestr_regex = r"^[A-Za-z][A-Za-z\-_]*[A-Za-z]$"
 
 # Create a ruamel object with our favored config, for universal use
@@ -51,15 +47,15 @@
     start_time = time.time()
     yield
     logger.info(f"{prefix} took {time.time() - start_time:.3f} [s]")
 
 
 @contextlib.contextmanager
 def change_directory(directory):
-    current_directory = os.getcwd()
+    current_directory = Path.cwd()
     os.chdir(directory)
     yield
     os.chdir(current_directory)
 
 
 def run_subprocess_cmd(processargs, **kwargs):
     """Runs subprocess command with realtime stdout logging with optional line prefix."""
@@ -175,35 +171,35 @@
             )
     elif config["provider"] in ["local", "existing"]:
         pass
     else:
         raise ValueError("Cloud Provider configuration not supported")
 
 
-def load_yaml(config_filename: pathlib.Path):
+def load_yaml(config_filename: Path):
     """
     Return yaml dict containing config loaded from config_filename.
     """
-    with config_filename.open() as f:
+    with open(config_filename) as f:
         config = yaml.load(f.read())
 
     return config
 
 
-def backup_config_file(filename: pathlib.Path, extrasuffix: str = ""):
+def backup_config_file(filename: Path, extrasuffix: str = ""):
     if not filename.exists():
         return
 
     # Backup old file
-    backup_filename = pathlib.Path(f"{filename}{extrasuffix}.backup")
+    backup_filename = Path(f"{filename}{extrasuffix}.backup")
 
     if backup_filename.exists():
         i = 1
         while True:
-            next_backup_filename = pathlib.Path(f"{backup_filename}~{i}")
+            next_backup_filename = Path(f"{backup_filename}~{i}")
             if not next_backup_filename.exists():
                 backup_filename = next_backup_filename
                 break
             i = i + 1
 
     filename.rename(backup_filename)
     print(f"Backing up {filename} as {backup_filename}")
@@ -393,7 +389,19 @@
 def set_nebari_dask_version() -> str:
     """Set version of `nebari-dask` meta package."""
 
     if NEBARI_DASK_VERSION:
         return NEBARI_DASK_VERSION
 
     return DEFAULT_NEBARI_DASK_VERSION
+
+
+def is_relative_to(self: Path, other: Path, /) -> bool:
+    """Compatibility function to bring ``Path.is_relative_to`` to Python 3.8"""
+    if sys.version_info[:2] >= (3, 9):
+        return self.is_relative_to(other)
+
+    try:
+        self.relative_to(other)
+        return True
+    except ValueError:
+        return False
```

### Comparing `nebari-2023.5.1rc1/nebari/version.py` & `nebari-2023.7.1rc1/src/_nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/cli/dev.py` & `nebari-2023.7.1rc1/src/_nebari/cli/dev.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from pathlib import Path
 
 import typer
 
-from nebari.keycloak import keycloak_rest_api_call
+from _nebari.keycloak import keycloak_rest_api_call
 
 app_dev = typer.Typer(
     add_completion=False,
     no_args_is_help=True,
     rich_markup_mode="rich",
     context_settings={"help_option_names": ["-h", "--help"]},
 )
```

### Comparing `nebari-2023.5.1rc1/nebari/cli/init.py` & `nebari-2023.7.1rc1/src/_nebari/cli/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import re
 from pathlib import Path
 
 import questionary
 import rich
 import typer
 
-from nebari.initialize import render_config
-from nebari.schema import (
+from _nebari.initialize import render_config
+from _nebari.schema import (
     AuthenticationEnum,
     CiEnum,
     GitRepoEnum,
     InitInputs,
     ProviderEnum,
     TerraformStateEnum,
     project_name_convention,
 )
-from nebari.utils import NEBARI_DASK_VERSION, NEBARI_IMAGE_TAG, yaml
+from _nebari.utils import NEBARI_DASK_VERSION, NEBARI_IMAGE_TAG, yaml
 
 MISSING_CREDS_TEMPLATE = "Unable to locate your {provider} credentials, refer to this guide on how to generate them:\n\n[green]\t{link_to_docs}[/green]\n\n"
 LINKS_TO_DOCS_TEMPLATE = (
     "For more details, refer to the Nebari docs:\n\n\t[green]{link_to_docs}[/green]\n\n"
 )
 
 # links to external docs
```

### Comparing `nebari-2023.5.1rc1/nebari/cli/keycloak.py` & `nebari-2023.7.1rc1/src/_nebari/cli/keycloak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from pathlib import Path
 from typing import Tuple
 
 import typer
 
-from nebari.keycloak import do_keycloak, export_keycloak_users
+from _nebari.keycloak import do_keycloak, export_keycloak_users
 
 app_keycloak = typer.Typer(
     add_completion=False,
     no_args_is_help=True,
     rich_markup_mode="rich",
     context_settings={"help_option_names": ["-h", "--help"]},
 )
```

### Comparing `nebari-2023.5.1rc1/nebari/cli/main.py` & `nebari-2023.7.1rc1/src/_nebari/cli/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,54 +6,81 @@
 from click import Context
 from kubernetes import client
 from kubernetes import config as kube_config
 from rich import print
 from ruamel import yaml
 from typer.core import TyperGroup
 
-from nebari.cli.dev import app_dev
-from nebari.cli.init import (
+from _nebari.cli.dev import app_dev
+from _nebari.cli.init import (
     check_auth_provider_creds,
     check_cloud_provider_creds,
     check_project_name,
     check_ssl_cert_email,
     enum_to_list,
     guided_init_wizard,
     handle_init,
 )
-from nebari.cli.keycloak import app_keycloak
-from nebari.cost import infracost_report
-from nebari.deploy import deploy_configuration
-from nebari.destroy import destroy_configuration
-from nebari.render import render_template
-from nebari.schema import (
+from _nebari.cli.keycloak import app_keycloak
+from _nebari.deploy import deploy_configuration
+from _nebari.destroy import destroy_configuration
+from _nebari.render import render_template
+from _nebari.schema import (
     AuthenticationEnum,
     CiEnum,
     GitRepoEnum,
     InitInputs,
     ProviderEnum,
     TerraformStateEnum,
     verify,
 )
-from nebari.upgrade import do_upgrade
-from nebari.utils import load_yaml
-from nebari.version import __version__
+from _nebari.upgrade import do_upgrade
+from _nebari.utils import load_yaml
+from _nebari.version import __version__
 
 SECOND_COMMAND_GROUP_NAME = "Additional Commands"
 GUIDED_INIT_MSG = (
     "[bold green]START HERE[/bold green] - this will guide you step-by-step "
     "to generate your [purple]nebari-config.yaml[/purple]. "
     "It is an [i]alternative[/i] to passing the options listed below."
 )
 KEYCLOAK_COMMAND_MSG = (
     "Interact with the Nebari Keycloak identity and access management tool."
 )
 DEV_COMMAND_MSG = "Development tools and advanced features."
 
 
+def path_callback(value: str) -> Path:
+    return Path(value).expanduser().resolve()
+
+
+def config_path_callback(value: str) -> Path:
+    value = path_callback(value)
+    if not value.is_file():
+        raise ValueError(f"Passed configuration path {value} does not exist!")
+    return value
+
+
+CONFIG_PATH_OPTION: Path = typer.Option(
+    ...,
+    "--config",
+    "-c",
+    help="nebari configuration yaml file path, please pass in as -c/--config flag",
+    callback=config_path_callback,
+)
+
+OUTPUT_PATH_OPTION: Path = typer.Option(
+    Path.cwd(),
+    "-o",
+    "--output",
+    help="output directory",
+    callback=path_callback,
+)
+
+
 class OrderCommands(TyperGroup):
     def list_commands(self, ctx: Context):
         """Return list of commands in the order appear."""
         return list(self.commands)
 
 
 app = typer.Typer(
@@ -97,14 +124,16 @@
 def init(
     cloud_provider: str = typer.Argument(
         "local",
         help=f"options: {enum_to_list(ProviderEnum)}",
         callback=check_cloud_provider_creds,
         is_eager=True,
     ),
+    # Although this unused below, the functionality is contained in the callback. Thus,
+    # this attribute cannot be removed.
     guided_init: bool = typer.Option(
         False,
         help=GUIDED_INIT_MSG,
         callback=guided_init_wizard,
         is_eager=True,
     ),
     project_name: str = typer.Option(
@@ -188,95 +217,57 @@
     inputs.disable_prompt = disable_prompt
 
     handle_init(inputs)
 
 
 @app.command(rich_help_panel=SECOND_COMMAND_GROUP_NAME)
 def validate(
-    config: str = typer.Option(
-        ...,
-        "--config",
-        "-c",
-        help="nebari configuration yaml file path, please pass in as -c/--config flag",
-    ),
+    config_path=CONFIG_PATH_OPTION,
     enable_commenting: bool = typer.Option(
         False, "--enable-commenting", help="Toggle PR commenting on GitHub Actions"
     ),
 ):
     """
     Validate the values in the [purple]nebari-config.yaml[/purple] file are acceptable.
     """
-    config_filename = Path(config)
-    if not config_filename.is_file():
-        raise ValueError(
-            f"Passed in configuration filename={config_filename} must exist."
-        )
-
-    config = load_yaml(config_filename)
+    config = load_yaml(config_path)
 
     if enable_commenting:
         # for PR's only
         # comment_on_pr(config)
         pass
     else:
         verify(config)
         print("[bold purple]Successfully validated configuration.[/bold purple]")
 
 
 @app.command(rich_help_panel=SECOND_COMMAND_GROUP_NAME)
 def render(
-    output: str = typer.Option(
-        "./",
-        "-o",
-        "--output",
-        help="output directory",
-    ),
-    config: str = typer.Option(
-        ...,
-        "-c",
-        "--config",
-        help="nebari configuration yaml file path",
-    ),
+    output_path=OUTPUT_PATH_OPTION,
+    config_path=CONFIG_PATH_OPTION,
     dry_run: bool = typer.Option(
         False,
         "--dry-run",
         help="simulate rendering files without actually writing or updating any files",
     ),
 ):
     """
     Dynamically render the Terraform scripts and other files from your [purple]nebari-config.yaml[/purple] file.
     """
-    config_filename = Path(config)
-
-    if not config_filename.is_file():
-        raise ValueError(
-            f"passed in configuration filename={config_filename} must exist"
-        )
-
-    config_yaml = load_yaml(config_filename)
+    config = load_yaml(config_path)
 
-    verify(config_yaml)
+    verify(config)
 
-    render_template(output, config, force=True, dry_run=dry_run)
+    render_template(output_path, config_path, dry_run=dry_run)
 
 
 @app.command()
 def deploy(
-    config: str = typer.Option(
-        ...,
-        "--config",
-        "-c",
-        help="nebari configuration yaml file path",
-    ),
-    output: str = typer.Option(
-        "./",
-        "-o",
-        "--output",
-        help="output directory",
-    ),
+    config_path=CONFIG_PATH_OPTION,
+    output_path=OUTPUT_PATH_OPTION,
     dns_provider: str = typer.Option(
         False,
         "--dns-provider",
         help="dns provider to use for registering domain name mapping",
     ),
     dns_auto_provision: bool = typer.Option(
         False,
@@ -303,49 +294,35 @@
         "--skip-remote-state-provision",
         help="Skip terraform state deployment which is often required in CI once the terraform remote state bootstrapping phase is complete",
     ),
 ):
     """
     Deploy the Nebari cluster from your [purple]nebari-config.yaml[/purple] file.
     """
-    config_filename = Path(config)
-
-    if not config_filename.is_file():
-        raise ValueError(
-            f"passed in configuration filename={config_filename} must exist"
-        )
+    config = load_yaml(config_path)
 
-    config_yaml = load_yaml(config_filename)
-
-    verify(config_yaml)
+    verify(config)
 
     if not disable_render:
-        render_template(output, config, force=True)
+        render_template(output_path, config_path)
 
     deploy_configuration(
-        config_yaml,
+        config,
         dns_provider=dns_provider,
         dns_auto_provision=dns_auto_provision,
         disable_prompt=disable_prompt,
         disable_checks=disable_checks,
         skip_remote_state_provision=skip_remote_state_provision,
     )
 
 
 @app.command()
 def destroy(
-    config: str = typer.Option(
-        ..., "-c", "--config", help="nebari configuration file path"
-    ),
-    output: str = typer.Option(
-        "./",
-        "-o",
-        "--output",
-        help="output directory",
-    ),
+    config_path=CONFIG_PATH_OPTION,
+    output_path=OUTPUT_PATH_OPTION,
     disable_render: bool = typer.Option(
         False,
         "--disable-render",
         help="Disable auto-rendering before destroy",
     ),
     disable_prompt: bool = typer.Option(
         False,
@@ -353,142 +330,67 @@
         help="Destroy entire Nebari cluster without confirmation request. Suggested for CI use.",
     ),
 ):
     """
     Destroy the Nebari cluster from your [purple]nebari-config.yaml[/purple] file.
     """
 
-    def _run_destroy(config=config, disable_render=disable_render):
-        config_filename = Path(config)
-        if not config_filename.is_file():
-            raise ValueError(
-                f"passed in configuration filename={config_filename} must exist"
-            )
+    def _run_destroy(config_path=config_path, disable_render=disable_render):
+        config = load_yaml(config_path)
 
-        config_yaml = load_yaml(config_filename)
-
-        verify(config_yaml)
+        verify(config)
 
         if not disable_render:
-            render_template(output, config, force=True)
+            render_template(output_path, config_path)
 
-        destroy_configuration(config_yaml)
+        destroy_configuration(config)
 
     if disable_prompt:
         _run_destroy()
     elif typer.confirm("Are you sure you want to destroy your Nebari cluster?"):
         _run_destroy()
     else:
         raise typer.Abort()
 
 
 @app.command(rich_help_panel=SECOND_COMMAND_GROUP_NAME)
-def cost(
-    path: str = typer.Option(
-        None,
-        "-p",
-        "--path",
-        help="Pass the path of your stages directory generated after rendering Nebari configurations before deployment",
-    ),
-    dashboard: bool = typer.Option(
-        True,
-        "-d",
-        "--dashboard",
-        help="Enable the cost dashboard",
-    ),
-    file: str = typer.Option(
-        None,
-        "-f",
-        "--file",
-        help="Specify the path of the file to store the cost report",
-    ),
-    currency: str = typer.Option(
-        "USD",
-        "-c",
-        "--currency",
-        help="Specify the currency code to use in the cost report",
-    ),
-    compare: bool = typer.Option(
-        False,
-        "-cc",
-        "--compare",
-        help="Compare the cost report to a previously generated report",
-    ),
-):
-    """
-    Estimate the cost of deploying Nebari based on your [purple]nebari-config.yaml[/purple]. [italic]Experimental.[/italic].
-
-    [italic]This is still only experimental using Infracost under the hood.
-    The estimated value is a base cost and does not include usage costs.[/italic]
-    """
-    infracost_report(
-        path=path,
-        dashboard=True,
-        file=file,
-        currency_code=currency,
-        compare=False,
-    )
-
-
-@app.command(rich_help_panel=SECOND_COMMAND_GROUP_NAME)
 def upgrade(
-    config: str = typer.Option(
-        ...,
-        "-c",
-        "--config",
-        help="nebari configuration file path",
-    ),
+    config_path=CONFIG_PATH_OPTION,
     attempt_fixes: bool = typer.Option(
         False,
         "--attempt-fixes",
         help="Attempt to fix the config for any incompatibilities between your old and new Nebari versions.",
     ),
 ):
     """
-    Upgrade your [purple]nebari-config.yaml[/purple] from pre-0.4.0 to 0.4.0.
+    Upgrade your [purple]nebari-config.yaml[/purple].
+
+    Upgrade your [purple]nebari-config.yaml[/purple] after an nebari upgrade. If necessary, prompts users to perform manual upgrade steps required for the deploy process.
 
-    Due to several breaking changes that came with the 0.4.0 release, this utility is available to help
-    update your [purple]nebari-config.yaml[/purple] to comply with the introduced changes.
     See the project [green]RELEASE.md[/green] for details.
     """
-    config_filename = Path(config)
-    if not config_filename.is_file():
-        raise ValueError(
-            f"passed in configuration filename={config_filename} must exist"
-        )
-
-    do_upgrade(config_filename, attempt_fixes=attempt_fixes)
+    do_upgrade(config_path, attempt_fixes=attempt_fixes)
 
 
 @app.command(rich_help_panel=SECOND_COMMAND_GROUP_NAME)
 def support(
-    config_filename: str = typer.Option(
-        ...,
-        "-c",
-        "--config",
-        help="nebari configuration file path",
-    ),
-    output: str = typer.Option(
-        "./nebari-support-logs.zip",
-        "-o",
-        "--output",
-        help="output filename",
-    ),
+    config_path=CONFIG_PATH_OPTION,
+    output_path=OUTPUT_PATH_OPTION,
 ):
     """
     Support tool to write all Kubernetes logs locally and compress them into a zip file.
 
     The Nebari team recommends k9s to manage and inspect the state of the cluster.
     However, this command occasionally helpful for debugging purposes should the logs need to be shared.
     """
     kube_config.load_kube_config()
 
     v1 = client.CoreV1Api()
 
-    namespace = get_config_namespace(config=config_filename)
+    namespace = get_config_namespace(config_path)
 
     pods = v1.list_namespaced_pod(namespace=namespace)
 
     for pod in pods.items:
         Path(f"./log/{namespace}").mkdir(parents=True, exist_ok=True)
         path = Path(f"./log/{namespace}/{pod.metadata.name}.txt")
         with path.open(mode="wt") as file:
@@ -519,28 +421,22 @@
                         )
                     )
 
             except client.exceptions.ApiException as e:
                 file.write("%s not available" % pod.metadata.name)
                 raise e
 
-    with ZipFile(output, "w") as zip:
+    with ZipFile(output_path, "w") as zip:
         for file in list(Path(f"./log/{namespace}").glob("*.txt")):
             print(file)
             zip.write(file)
 
 
-def get_config_namespace(config):
-    config_filename = Path(config)
-    if not config_filename.is_file():
-        raise ValueError(
-            f"passed in configuration filename={config_filename} must exist"
-        )
-
-    with config_filename.open() as f:
+def get_config_namespace(config_path):
+    with open(config_path) as f:
         config = yaml.safe_load(f.read())
 
     return config["namespace"]
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/git.py` & `nebari-2023.7.1rc1/src/_nebari/provider/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import configparser
 import os
 import subprocess
+from pathlib import Path
 
-from nebari.utils import change_directory
+from _nebari.utils import change_directory
 
 
 def is_git_repo(path=None):
-    path = path or os.getcwd()
+    path = path or Path.cwd()
     return ".git" in os.listdir(path)
 
 
 def initialize_git(path=None):
-    path = path or os.getcwd()
+    path = path or Path.cwd()
     with change_directory(path):
         subprocess.check_output(["git", "init"])
         # Ensure initial branch is called main
         subprocess.check_output(["git", "checkout", "-b", "main"])
 
 
 def add_git_remote(remote_path, path=None, remote_name="origin"):
-    path = path or os.getcwd()
+    path = path or Path.cwd()
 
     c = configparser.ConfigParser()
-    with open(os.path.join(path, ".git/config")) as f:
+    with open(path / ".git/config") as f:
         c.read_file(f)
     if f'remote "{remote_name}"' in c:
         if c[f'remote "{remote_name}"']["url"] == remote_path:
             return  # no action needed
         else:
             raise ValueError(
                 f"git add remote would change existing remote name={remote_name}"
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/terraform.py` & `nebari-2023.7.1rc1/src/_nebari/provider/terraform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import contextlib
 import io
 import json
 import logging
-import os
 import platform
 import re
 import subprocess
 import sys
 import tempfile
 import urllib.request
 import zipfile
+from pathlib import Path
 from typing import Any, Dict, List
 
-from nebari import constants
-from nebari.utils import deep_merge, run_subprocess_cmd, timer
+from _nebari import constants
+from _nebari.utils import deep_merge, run_subprocess_cmd, timer
 
 logger = logging.getLogger(__name__)
 
 
 class TerraformException(Exception):
     pass
 
@@ -94,27 +94,27 @@
         "i386": "386",
         "armv7l": "arm",
         "aarch64": "arm64",
         "arm64": "arm64",
     }
 
     download_url = f"https://releases.hashicorp.com/terraform/{version}/terraform_{version}_{os_mapping[sys.platform]}_{architecture_mapping[platform.machine()]}.zip"
-    filename_directory = os.path.join(tempfile.gettempdir(), "terraform", version)
-    filename_path = os.path.join(filename_directory, "terraform")
+    filename_directory = Path(tempfile.gettempdir()) / "terraform" / version
+    filename_path = filename_directory / "terraform"
 
-    if not os.path.isfile(filename_path):
+    if not filename_path.is_file():
         logger.info(
             f"downloading and extracting terraform binary from url={download_url} to path={filename_path}"
         )
         with urllib.request.urlopen(download_url) as f:
             bytes_io = io.BytesIO(f.read())
         download_file = zipfile.ZipFile(bytes_io)
         download_file.extract("terraform", filename_directory)
 
-    os.chmod(filename_path, 0o555)
+    filename_path.chmod(0o555)
     return filename_path
 
 
 def run_terraform_subprocess(processargs, **kwargs):
     terraform_path = download_terraform_binary()
     logger.info(f" terraform at {terraform_path}")
     if run_subprocess_cmd([terraform_path] + processargs, **kwargs):
@@ -212,20 +212,20 @@
 
     with timer(logger, "terraform destroy"):
         run_terraform_subprocess(command, cwd=directory, prefix="terraform")
 
 
 def rm_local_state(directory=None):
     logger.info(f"rm local state file terraform.tfstate directory={directory}")
-    tfstate_path = "terraform.tfstate"
+    tfstate_path = Path("terraform.tfstate")
     if directory:
-        tfstate_path = os.path.join(directory, tfstate_path)
+        tfstate_path = directory / tfstate_path
 
-    if os.path.isfile(tfstate_path):
-        os.remove(tfstate_path)
+    if tfstate_path.is_file():
+        tfstate_path.unlink()
 
 
 # ========== Terraform JSON ============
 @contextlib.contextmanager
 def tf_context(filename):
     try:
         tf_clear()
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/cicd/github.py` & `nebari-2023.7.1rc1/src/_nebari/provider/cicd/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 from typing import Dict, List, Optional, Union
 
 import requests
 from nacl import encoding, public
 from pydantic import BaseModel, Field
 
-from nebari.constants import LATEST_SUPPORTED_PYTHON_VERSION
-from nebari.provider.cicd.common import pip_install_nebari
+from _nebari.constants import LATEST_SUPPORTED_PYTHON_VERSION
+from _nebari.provider.cicd.common import pip_install_nebari
 
 GITHUB_BASE_URL = "https://api.github.com/"
 
 
 def github_request(url, method="GET", json=None, authenticate=True):
     auth = None
     if authenticate:
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/cicd/gitlab.py` & `nebari-2023.7.1rc1/src/_nebari/provider/cicd/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field
 
-from nebari.constants import LATEST_SUPPORTED_PYTHON_VERSION
-from nebari.provider.cicd.common import pip_install_nebari
+from _nebari.constants import LATEST_SUPPORTED_PYTHON_VERSION
+from _nebari.provider.cicd.common import pip_install_nebari
 
 
 class GLCI_extras(BaseModel):
     # to allow for dynamic key names
     __root__: Union[str, float, int]
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/cicd/linter.py` & `nebari-2023.7.1rc1/src/_nebari/provider/cicd/linter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
-import pathlib
 import textwrap
+from pathlib import Path
 
 import requests
 
-from nebari.schema import verify
+from _nebari.schema import verify
 
 
 def nebari_validate(config):
     # Gather the output of `nebari validate`.
     print("Validate: info: validating Nebari configuration in nebari-config.yaml")
 
     def parse_validation(message):
@@ -28,15 +28,15 @@
         validate_comment = parse_validation(e)
         validate_comment_wrapper = f"\n```\n{validate_comment}\n``` "
         return False, validate_comment_wrapper, 1
 
 
 def generate_lint_message(config):
     # prep for linting
-    pr_config = pathlib.Path("nebari-config.yaml")
+    pr_config = Path("nebari-config.yaml")
     # lint/validate nebari-config.yaml
     all_pass, messages, validate_code = nebari_validate(config)
 
     pass_lint = textwrap.dedent(
         """
             This is an automatic response from the Nebari linter.
             I just wanted to let you know that I linted your `nebari-config.yaml` in your PR and I didn't find any
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/cloud/amazon_web_services.py` & `nebari-2023.7.1rc1/src/_nebari/provider/cloud/amazon_web_services.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import json
 import os
 import subprocess
 
 import boto3
 
-from nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
+from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
 
 
 @functools.lru_cache()
 def regions():
     output = subprocess.check_output(["aws", "ec2", "describe-regions"])
     data = json.loads(output.decode("utf-8"))
     return {_["RegionName"]: _["RegionName"] for _ in data["Regions"]}
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/cloud/azure_cloud.py` & `nebari-2023.7.1rc1/src/_nebari/provider/cloud/azure_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import logging
 import os
 
 from azure.identity import DefaultAzureCredential
 from azure.mgmt.containerservice import ContainerServiceClient
 
-from nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
+from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
 
 logger = logging.getLogger("azure")
 logger.setLevel(logging.ERROR)
 
 
 @functools.lru_cache()
 def initiate_container_service_client():
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/cloud/digital_ocean.py` & `nebari-2023.7.1rc1/src/_nebari/provider/cloud/digital_ocean.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import os
 
 import requests
 
-from nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
+from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
 
 
 def digital_ocean_request(url, method="GET", json=None):
     BASE_DIGITALOCEAN_URL = "https://api.digitalocean.com/v2/"
 
     for name in {"DIGITALOCEAN_TOKEN"}:
         if name not in os.environ:
@@ -37,14 +37,13 @@
     return _kubernetes_options()["options"]["sizes"]
 
 
 def regions():
     return _kubernetes_options()["options"]["regions"]
 
 
-# keep `region` parameter
-def kubernetes_versions(region=None):
+def kubernetes_versions(region):
     """Return list of available kubernetes supported by cloud provider. Sorted from oldest to latest."""
     supported_kubernetes_versions = sorted(
         [_["slug"] for _ in _kubernetes_options()["options"]["versions"]]
     )
     return filter_by_highest_supported_k8s_version(supported_kubernetes_versions)
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/cloud/google_cloud.py` & `nebari-2023.7.1rc1/src/_nebari/provider/cloud/google_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import json
 import subprocess
 
-from nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
+from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
 
 
 @functools.lru_cache()
 def projects():
     output = subprocess.check_output(["gcloud", "projects", "list", "--format=json"])
     data = json.loads(output.decode("utf-8"))
     return {_["name"]: _["projectId"] for _ in data}
```

### Comparing `nebari-2023.5.1rc1/nebari/provider/dns/cloudflare.py` & `nebari-2023.7.1rc1/src/_nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/provider/oauth/auth0.py` & `nebari-2023.7.1rc1/src/_nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/stages/checks.py` & `nebari-2023.7.1rc1/src/_nebari/stages/checks.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/stages/input_vars.py` & `nebari-2023.7.1rc1/src/_nebari/stages/input_vars.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
-import os
 import tempfile
+from pathlib import Path
 from urllib.parse import urlencode
 
-from nebari.constants import (
+from _nebari.constants import (
     DEFAULT_CONDA_STORE_IMAGE_TAG,
     DEFAULT_GKE_RELEASE_CHANNEL,
+    DEFAULT_NEBARI_WORKFLOW_CONTROLLER_IMAGE_TAG,
     DEFAULT_TRAEFIK_IMAGE_TAG,
 )
 
 
 def stage_01_terraform_state(stage_outputs, config):
     if config["provider"] == "do":
         return {
@@ -39,30 +40,30 @@
     else:
         return {}
 
 
 def stage_02_infrastructure(stage_outputs, config):
     if config["provider"] == "local":
         return {
-            "kubeconfig_filename": os.path.join(
-                tempfile.gettempdir(), "NEBARI_KUBECONFIG"
+            "kubeconfig_filename": str(
+                Path(tempfile.gettempdir()) / "NEBARI_KUBECONFIG"
             ),
             "kube_context": config["local"].get("kube_context"),
         }
     elif config["provider"] == "existing":
         return {"kube_context": config["existing"].get("kube_context")}
     elif config["provider"] == "do":
         return {
             "name": config["project_name"],
             "environment": config["namespace"],
             "region": config["digital_ocean"]["region"],
             "kubernetes_version": config["digital_ocean"]["kubernetes_version"],
             "node_groups": config["digital_ocean"]["node_groups"],
-            "kubeconfig_filename": os.path.join(
-                tempfile.gettempdir(), "NEBARI_KUBECONFIG"
+            "kubeconfig_filename": str(
+                Path(tempfile.gettempdir()) / "NEBARI_KUBECONFIG"
             ),
             **config.get("do", {}).get("terraform_overrides", {}),
         }
     elif config["provider"] == "gcp":
         return {
             "name": config["project_name"],
             "environment": config["namespace"],
@@ -81,28 +82,28 @@
                     "guest_accelerators": value["guest_accelerators"]
                     if "guest_accelerators" in value
                     else [],
                     **value,
                 }
                 for key, value in config["google_cloud_platform"]["node_groups"].items()
             ],
-            "kubeconfig_filename": os.path.join(
-                tempfile.gettempdir(), "NEBARI_KUBECONFIG"
+            "kubeconfig_filename": str(
+                Path(tempfile.gettempdir()) / "NEBARI_KUBECONFIG"
             ),
             **config.get("gcp", {}).get("terraform_overrides", {}),
         }
     elif config["provider"] == "azure":
         return {
             "name": config["project_name"],
             "environment": config["namespace"],
             "region": config["azure"]["region"],
             "kubernetes_version": config["azure"]["kubernetes_version"],
             "node_groups": config["azure"]["node_groups"],
-            "kubeconfig_filename": os.path.join(
-                tempfile.gettempdir(), "NEBARI_KUBECONFIG"
+            "kubeconfig_filename": str(
+                Path(tempfile.gettempdir()) / "NEBARI_KUBECONFIG"
             ),
             "resource_group_name": f'{config["project_name"]}-{config["namespace"]}',
             "node_resource_group_name": f'{config["project_name"]}-{config["namespace"]}-node-resource-group',
             **config.get("azure", {}).get("terraform_overrides", {}),
         }
     elif config["provider"] == "aws":
         return {
@@ -118,18 +119,18 @@
                     "max_size": value["max_nodes"],
                     "gpu": value.get("gpu", False),
                     "instance_type": value["instance"],
                     "single_subnet": value.get("single_subnet", False),
                 }
                 for key, value in config["amazon_web_services"]["node_groups"].items()
             ],
-            "kubeconfig_filename": os.path.join(
-                tempfile.gettempdir(), "NEBARI_KUBECONFIG"
+            "kubeconfig_filename": str(
+                Path(tempfile.gettempdir()) / "NEBARI_KUBECONFIG"
             ),
-            **config.get("aws", {}).get("terraform_overrides", {}),
+            **config.get("amazon_web_services", {}).get("terraform_overrides", {}),
         }
     else:
         return {}
 
 
 def stage_03_kubernetes_initialize(stage_outputs, config):
     if config["provider"] == "gcp":
@@ -295,14 +296,20 @@
             },
             "dask-gateway": {
                 "primary_namespace": "",
                 "role_bindings": {
                     "*/*": ["viewer"],
                 },
             },
+            "argo-workflows-jupyter-scheduler": {
+                "primary_namespace": "",
+                "role_bindings": {
+                    "*/*": ["viewer"],
+                },
+            },
         },
         "conda-store-default-namespace": config.get("conda_store", {}).get(
             "default_namespace", "nebari-git"
         ),
         "conda-store-extra-settings": config.get("conda_store", {}).get(
             "extra_settings", {}
         ),
@@ -345,14 +352,26 @@
         # monitoring
         "monitoring-enabled": config["monitoring"]["enabled"],
         # argo-worfklows
         "argo-workflows-enabled": config["argo_workflows"]["enabled"],
         "argo-workflows-overrides": [
             json.dumps(config.get("argo_workflows", {}).get("overrides", {}))
         ],
+        "nebari-workflow-controller": config["argo_workflows"]
+        .get("nebari_workflow_controller", {})
+        .get("enabled", True),
+        "keycloak-read-only-user-credentials": stage_outputs[
+            "stages/06-kubernetes-keycloak-configuration"
+        ]["keycloak-read-only-user-credentials"]["value"],
+        "workflow-controller-image-tag": config.get("argo_workflows", {})
+        .get("nebari_workflow_controller", {})
+        .get(
+            "image_tag",
+            DEFAULT_NEBARI_WORKFLOW_CONTROLLER_IMAGE_TAG,
+        ),
         # kbatch
         "kbatch-enabled": config["kbatch"]["enabled"],
         # prefect
         "prefect-enabled": config.get("prefect", {}).get("enabled", False),
         "prefect-token": config.get("prefect", {}).get("token", ""),
         "prefect-image": config.get("prefect", {}).get("image", ""),
         "prefect-overrides": config.get("prefect", {}).get("overrides", {}),
```

### Comparing `nebari-2023.5.1rc1/nebari/stages/state_imports.py` & `nebari-2023.7.1rc1/src/_nebari/stages/state_imports.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/stages/tf_objects.py` & `nebari-2023.7.1rc1/src/_nebari/stages/tf_objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from pathlib import Path
 from typing import Dict
 
-from nebari.provider.terraform import (
+from _nebari.provider.terraform import (
     Data,
     Provider,
     TerraformBackend,
     tf_render_objects,
 )
-from nebari.utils import deep_merge
+from _nebari.utils import deep_merge
 
 
 def NebariAWSProvider(nebari_config: Dict):
     return Provider("aws", region=nebari_config["amazon_web_services"]["region"])
 
 
 def NebariGCPProvider(nebari_config: Dict):
@@ -137,132 +138,162 @@
     else:
         raise NotImplementedError("state not implemented")
 
 
 def stage_01_terraform_state(config):
     if config["provider"] == "gcp":
         return {
-            "stages/01-terraform-state/gcp/_nebari.tf.json": tf_render_objects(
+            Path("stages")
+            / "01-terraform-state"
+            / "gcp"
+            / "_nebari.tf.json": tf_render_objects(
                 [
                     NebariGCPProvider(config),
                 ]
             )
         }
     elif config["provider"] == "aws":
         return {
-            "stages/01-terraform-state/aws/_nebari.tf.json": tf_render_objects(
+            Path("stages")
+            / "01-terraform-state"
+            / "aws"
+            / "_nebari.tf.json": tf_render_objects(
                 [
                     NebariAWSProvider(config),
                 ]
             )
         }
     else:
         return {}
 
 
 def stage_02_infrastructure(config):
     if config["provider"] == "gcp":
         return {
-            "stages/02-infrastructure/gcp/_nebari.tf.json": tf_render_objects(
+            Path("stages")
+            / "02-infrastructure"
+            / "gcp"
+            / "_nebari.tf.json": tf_render_objects(
                 [
                     NebariGCPProvider(config),
                     NebariTerraformState("02-infrastructure", config),
                 ]
             )
         }
     elif config["provider"] == "do":
         return {
-            "stages/02-infrastructure/do/_nebari.tf.json": tf_render_objects(
+            Path("stages")
+            / "02-infrastructure"
+            / "do"
+            / "_nebari.tf.json": tf_render_objects(
                 [
                     NebariTerraformState("02-infrastructure", config),
                 ]
             )
         }
     elif config["provider"] == "azure":
         return {
-            "stages/02-infrastructure/azure/_nebari.tf.json": tf_render_objects(
+            Path("stages")
+            / "02-infrastructure"
+            / "azure"
+            / "_nebari.tf.json": tf_render_objects(
                 [
                     NebariTerraformState("02-infrastructure", config),
                 ]
             ),
         }
     elif config["provider"] == "aws":
         return {
-            "stages/02-infrastructure/aws/_nebari.tf.json": tf_render_objects(
+            Path("stages")
+            / "02-infrastructure"
+            / "aws"
+            / "_nebari.tf.json": tf_render_objects(
                 [
                     NebariAWSProvider(config),
                     NebariTerraformState("02-infrastructure", config),
                 ]
             )
         }
     else:
         return {}
 
 
 def stage_03_kubernetes_initialize(config):
     return {
-        "stages/03-kubernetes-initialize/_nebari.tf.json": tf_render_objects(
+        Path("stages")
+        / "03-kubernetes-initialize"
+        / "_nebari.tf.json": tf_render_objects(
             [
                 NebariTerraformState("03-kubernetes-initialize", config),
                 NebariKubernetesProvider(config),
                 NebariHelmProvider(config),
             ]
         ),
     }
 
 
 def stage_04_kubernetes_ingress(config):
     return {
-        "stages/04-kubernetes-ingress/_nebari.tf.json": tf_render_objects(
+        Path("stages")
+        / "04-kubernetes-ingress"
+        / "_nebari.tf.json": tf_render_objects(
             [
                 NebariTerraformState("04-kubernetes-ingress", config),
                 NebariKubernetesProvider(config),
                 NebariHelmProvider(config),
             ]
         ),
     }
 
 
 def stage_05_kubernetes_keycloak(config):
     return {
-        "stages/05-kubernetes-keycloak/_nebari.tf.json": tf_render_objects(
+        Path("stages")
+        / "05-kubernetes-keycloak"
+        / "_nebari.tf.json": tf_render_objects(
             [
                 NebariTerraformState("05-kubernetes-keycloak", config),
                 NebariKubernetesProvider(config),
                 NebariHelmProvider(config),
             ]
         ),
     }
 
 
 def stage_06_kubernetes_keycloak_configuration(config):
     return {
-        "stages/06-kubernetes-keycloak-configuration/_nebari.tf.json": tf_render_objects(
+        Path("stages")
+        / "06-kubernetes-keycloak-configuration"
+        / "_nebari.tf.json": tf_render_objects(
             [
                 NebariTerraformState("06-kubernetes-keycloak-configuration", config),
             ]
         ),
     }
 
 
 def stage_07_kubernetes_services(config):
     return {
-        "stages/07-kubernetes-services/_nebari.tf.json": tf_render_objects(
+        Path("stages")
+        / "07-kubernetes-services"
+        / "_nebari.tf.json": tf_render_objects(
             [
                 NebariTerraformState("07-kubernetes-services", config),
                 NebariKubernetesProvider(config),
                 NebariHelmProvider(config),
             ]
         ),
     }
 
 
 def stage_08_nebari_tf_extensions(config):
     return {
-        "stages/08-nebari-tf-extensions/_nebari.tf.json": tf_render_objects(
+        Path("stages")
+        / "08-nebari-tf-extensions"
+        / "_nebari.tf.json": tf_render_objects(
             [
                 NebariTerraformState("08-nebari-tf-extensions", config),
                 NebariKubernetesProvider(config),
                 NebariHelmProvider(config),
             ]
         ),
     }
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,76 @@
 variable "name" {
-  description = "Prefix name to assign to Nebari resources"
+  description = "Prefix name for EKS cluster"
   type        = string
 }
 
-variable "environment" {
-  description = "Environment to create Kubernetes resources"
-  type        = string
+variable "tags" {
+  description = "Additional tags for EKS cluster"
+  type        = map(string)
+  default     = {}
+}
+
+variable "cluster_subnets" {
+  description = "AWS VPC subnets to use for EKS cluster"
+  type        = list(string)
 }
 
 variable "region" {
   description = "AWS region for EKS cluster"
   type        = string
 }
 
+variable "partition" {
+  description = "AWS partition for EKS cluster"
+  type        = string
+}
+
 variable "kubernetes_version" {
   description = "AWS kubernetes version for EKS cluster"
   type        = string
 }
 
+variable "cluster_security_groups" {
+  description = "AWS security groups to use for EKS cluster"
+  type        = list(string)
+}
+
+variable "cluster_additional_policies" {
+  description = "Additional policies to add to cluster"
+  type        = list(string)
+  default     = []
+}
+
+variable "node_group_additional_policies" {
+  description = "Additional policies to add to each node group"
+  type        = list(string)
+  default     = []
+}
+
 variable "node_groups" {
-  description = "AWS node groups"
+  description = "Node groups to add to EKS Cluster"
   type = list(object({
     name          = string
     instance_type = string
     gpu           = bool
     min_size      = number
     desired_size  = number
     max_size      = number
     single_subnet = bool
   }))
 }
 
-variable "availability_zones" {
-  description = "AWS availability zones within AWS region"
-  type        = list(string)
-  default     = []
+variable "node_group_instance_type" {
+  description = "AWS instance types to use for kubernetes nodes"
+  type        = string
+  default     = "m5.large"
 }
 
-variable "vpc_cidr_block" {
-  description = "VPC cidr block for infastructure"
-  type        = string
-  default     = "10.10.0.0/16"
+variable "endpoint_private_access" {
+  type    = bool
+  default = false
 }
 
-variable "kubeconfig_filename" {
-  description = "Kubernetes kubeconfig written to filesystem"
-  type        = string
-  default     = null
+variable "public_access_cidrs" {
+  type    = list(string)
+  default = ["0.0.0.0/0"]
 }
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
   name     = var.name
   role_arn = aws_iam_role.cluster.arn
   version  = var.kubernetes_version
 
   vpc_config {
     security_group_ids = var.cluster_security_groups
     subnet_ids         = var.cluster_subnets
+
+    endpoint_private_access = var.endpoint_private_access
+    public_access_cidrs     = var.public_access_cidrs
   }
 
   depends_on = [
     aws_iam_role_policy_attachment.cluster-policy,
   ]
 
   tags = merge({ Name = var.name }, var.tags)
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,78 @@
 variable "name" {
-  description = "Prefix name for EKS cluster"
+  description = "Prefix name form conda-store server kubernetes resource"
   type        = string
 }
 
-variable "tags" {
-  description = "Additional tags for EKS cluster"
-  type        = map(string)
+variable "namespace" {
+  description = "Namespace to deploy conda-store server"
+  type        = string
+}
+
+variable "nfs_capacity" {
+  description = "Capacity of conda-store filesystem"
+  type        = string
+  default     = "10Gi"
+}
+
+variable "minio_capacity" {
+  description = "Capacity of conda-store object storage"
+  type        = string
+  default     = "10Gi"
+}
+
+variable "environments" {
+  description = "conda environments for conda-store to build"
+  type        = map(any)
   default     = {}
 }
 
-variable "cluster_subnets" {
-  description = "AWS VPC subnets to use for EKS cluster"
-  type        = list(string)
+variable "node-group" {
+  description = "Node key value pair for bound general resources"
+  type = object({
+    key   = string
+    value = string
+  })
 }
 
-variable "region" {
-  description = "AWS region for EKS cluster"
+variable "conda-store-image" {
+  description = "Conda-Store image"
   type        = string
+  default     = "quansight/conda-store-server"
 }
 
-variable "kubernetes_version" {
-  description = "AWS kubernetes version for EKS cluster"
+variable "conda-store-image-tag" {
+  description = "Version of conda-store to use"
   type        = string
 }
 
-variable "cluster_security_groups" {
-  description = "AWS security groups to use for EKS cluster"
-  type        = list(string)
+variable "external-url" {
+  description = "External url that jupyterhub cluster is accessible"
+  type        = string
 }
 
-variable "cluster_additional_policies" {
-  description = "Additional policies to add to cluster"
-  type        = list(string)
-  default     = []
+variable "realm_id" {
+  description = "Keycloak realm to use for deploying openid client"
+  type        = string
 }
 
-variable "node_group_additional_policies" {
-  description = "Additional policies to add to each node group"
-  type        = list(string)
-  default     = []
+variable "extra-settings" {
+  description = "Additional traitlets settings to apply before extra-config traitlets code is run"
+  type        = map(any)
+  default     = {}
 }
 
-variable "node_groups" {
-  description = "Node groups to add to EKS Cluster"
-  type = list(object({
-    name          = string
-    instance_type = string
-    gpu           = bool
-    min_size      = number
-    desired_size  = number
-    max_size      = number
-    single_subnet = bool
-  }))
+variable "extra-config" {
+  description = "Additional traitlets configuration code to be ran"
+  type        = string
+  default     = ""
 }
 
-variable "node_group_instance_type" {
-  description = "AWS instance types to use for kubernetes nodes"
+variable "default-namespace-name" {
+  description = "Name of the default conda-store namespace"
   type        = string
-  default     = "m5.large"
+}
+
+variable "services" {
+  description = "Map of services tokens and scopes for conda-store"
+  type        = map(any)
 }
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/metallb.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             "${var.node-group.key}" = var.node-group.value
           }
         }
       }
     })
   ], var.overrides)
 
-  set {
+  set_sensitive {
     name  = "nebari_bot_password"
     value = var.nebari-bot-password
   }
 
   set {
     name  = "initial_root_password"
     value = var.initial-root-password
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf`

 * *Files 26% similar despite different names*

```diff
@@ -43,14 +43,42 @@
   realm_id = keycloak_realm.main.id
   group_ids = [
     for g in var.default_groups :
     keycloak_group.groups[g].id
   ]
 }
 
+data "keycloak_realm" "master" {
+  realm = "master"
+}
+
+resource "random_password" "keycloak-view-only-user-password" {
+  length  = 32
+  special = false
+}
+
+resource "keycloak_user" "read-only-user" {
+  realm_id = data.keycloak_realm.master.id
+  username = "read-only-user"
+  initial_password {
+    value     = random_password.keycloak-view-only-user-password.result
+    temporary = false
+  }
+}
+
+resource "keycloak_user_roles" "user_roles" {
+  realm_id = data.keycloak_realm.master.id
+  user_id  = keycloak_user.read-only-user.id
+
+  role_ids = [
+    data.keycloak_role.view-users.id,
+  ]
+  exhaustive = true
+}
+
 # needed for keycloak monitoring to function
 resource "keycloak_realm_events" "realm_events" {
   realm_id = keycloak_realm.main.id
 
   events_enabled = true
 
   admin_events_enabled         = true
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,29 @@
 
 data "keycloak_role" "manage-users" {
   realm_id  = keycloak_realm.main.id
   client_id = data.keycloak_openid_client.realm_management.id
   name      = "manage-users"
 }
 
+data "keycloak_openid_client" "nebari-realm" {
+  depends_on = [
+    keycloak_realm.main,
+  ]
+  realm_id  = data.keycloak_realm.master.id
+  client_id = "${var.realm}-realm"
+}
+
+data "keycloak_role" "view-users" {
+  realm_id  = data.keycloak_realm.master.id
+  client_id = data.keycloak_openid_client.nebari-realm.id
+  name      = "view-users"
+}
+
+
 data "keycloak_role" "query-users" {
   realm_id  = keycloak_realm.main.id
   client_id = data.keycloak_openid_client.realm_management.id
   name      = "query-users"
 }
 
 data "keycloak_role" "query-groups" {
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/clearml.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/clearml.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/conda-store.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/conda-store.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/dask_gateway.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/dask_gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/jupyterhub.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub.tf`

 * *Files 7% similar despite different names*

```diff
@@ -94,20 +94,21 @@
 
   overrides = var.jupyterhub-overrides
 
   home-pvc = module.jupyterhub-nfs-mount.persistent_volume_claim.name
 
   shared-pvc = module.jupyterhub-nfs-mount.persistent_volume_claim.name
 
-  conda-store-pvc                = module.conda-store-nfs-mount.persistent_volume_claim.name
-  conda-store-mount              = "/home/conda"
-  conda-store-environments       = var.conda-store-environments
-  default-conda-store-namespace  = var.conda-store-default-namespace
-  conda-store-cdsdashboard-token = module.kubernetes-conda-store-server.service-tokens.cdsdashboards
-  conda-store-service-name       = module.kubernetes-conda-store-server.service_name
+  conda-store-pvc                                    = module.conda-store-nfs-mount.persistent_volume_claim.name
+  conda-store-mount                                  = "/home/conda"
+  conda-store-environments                           = var.conda-store-environments
+  default-conda-store-namespace                      = var.conda-store-default-namespace
+  conda-store-cdsdashboard-token                     = module.kubernetes-conda-store-server.service-tokens.cdsdashboards
+  conda-store-argo-workflows-jupyter-scheduler-token = module.kubernetes-conda-store-server.service-tokens.argo-workflows-jupyter-scheduler
+  conda-store-service-name                           = module.kubernetes-conda-store-server.service_name
 
   extra-mounts = {
     "/etc/dask" = {
       name      = "dask-etc"
       namespace = var.environment
       kind      = "configmap"
     },
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/kbatch.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/kbatch.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/prefect.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/prefect.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 variable "namespace" {
-  description = "deploy argo server on this namespace"
+  description = "deploy monitoring services on this namespace"
   type        = string
   default     = "dev"
 }
 
-variable "argo-workflows-namespace" {
-  description = "deploy argo workflows on this namespace"
+
+variable "external-url" {
+  description = "External url that jupyterhub cluster is accessible"
   type        = string
-  default     = "dev"
+}
+
+
+variable "realm_id" {
+  description = "Keycloak realm for creating oauth client"
+  type        = string
+}
+
+
+variable "dashboards" {
+  description = "Enabled grafana dashboards"
+  type        = set(string)
+  default = [
+    "Main",
+  ]
+}
+
+variable "jupyterhub_api_token" {
+  type      = string
+  default   = ""
+  sensitive = true
 }
 
 variable "node-group" {
   description = "Node key value pair for bound resources"
   type = object({
     key   = string
     value = string
   })
 }
 
-variable "external-url" {
-  description = "External url where jupyterhub cluster is accessible"
-  type        = string
-}
-
 
 variable "overrides" {
-  description = "Argo Workflows helm chart overrides"
+  description = "Grafana helm chart overrides"
   type        = list(string)
   default     = []
 }
-
-variable "realm_id" {
-  description = "Keycloak realm to use for deploying openid client"
-  type        = string
-}
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,72 @@
-variable "name" {
-  description = "Prefix name form conda-store server kubernetes resource"
+variable "namespace" {
+  description = "Namespace to deploy into"
   type        = string
 }
 
-variable "namespace" {
-  description = "Namespace to deploy conda-store server"
+variable "name" {
+  description = "Name of extension"
   type        = string
 }
 
-variable "nfs_capacity" {
-  description = "Capacity of conda-store filesystem"
+variable "external-url" {
+  description = "URL of the Nebari"
   type        = string
-  default     = "10Gi"
 }
 
-variable "minio_capacity" {
-  description = "Capacity of conda-store object storage"
+variable "image" {
+  description = "Docker image for extension"
   type        = string
-  default     = "10Gi"
 }
 
-variable "environments" {
-  description = "conda environments for conda-store to build"
-  type        = map(any)
-  default     = {}
+variable "urlslug" {
+  description = "Slug for URL"
+  type        = string
 }
 
-variable "node-group" {
-  description = "Node key value pair for bound general resources"
-  type = object({
-    key   = string
-    value = string
-  })
+variable "private" {
+  description = "Protect behind login page"
+  type        = bool
+  default     = true
 }
 
-variable "conda-store-image" {
-  description = "Conda-Store image"
-  type        = string
-  default     = "quansight/conda-store-server"
+variable "oauth2client" {
+  description = "Create a Keycloak client and include env vars"
+  type        = bool
+  default     = false
 }
 
-variable "conda-store-image-tag" {
-  description = "Version of conda-store to use"
-  type        = string
+variable "keycloakadmin" {
+  description = "Include env vars for a keycloak admin user to make Keycloak Admin API calls"
+  type        = bool
+  default     = false
 }
 
-variable "external-url" {
-  description = "External url that jupyterhub cluster is accessible"
-  type        = string
+variable "jwt" {
+  description = "Create secret and cookie name for JWT, set as env vars"
+  type        = bool
+  default     = false
 }
 
-variable "realm_id" {
-  description = "Keycloak realm to use for deploying openid client"
-  type        = string
+variable "nebariconfigyaml" {
+  description = "Mount nebari-config.yaml from configmap"
+  type        = bool
+  default     = false
 }
 
-variable "extra-settings" {
-  description = "Additional traitlets settings to apply before extra-config traitlets code is run"
-  type        = map(any)
-  default     = {}
+variable "envs" {
+  description = "List of env var objects"
+  type        = list(map(any))
+  default     = []
 }
 
-variable "extra-config" {
-  description = "Additional traitlets configuration code to be ran"
+variable "nebari-realm-id" {
+  description = "Keycloak nebari realm id"
   type        = string
   default     = ""
 }
 
-variable "default-namespace-name" {
-  description = "Name of the default conda-store namespace"
+variable "keycloak_nebari_bot_password" {
+  description = "Keycloak client password"
   type        = string
-}
-
-variable "services" {
-  description = "Map of services tokens and scopes for conda-store"
-  type        = map(any)
+  default     = ""
 }
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
-import os
 import tempfile
+from pathlib import Path
 
 import requests
 from conda_store_server import api, orm, schema
 from conda_store_server.server.auth import GenericOAuthAuthentication
 from conda_store_server.server.dependencies import get_conda_store
 from conda_store_server.storage import S3Storage
 
@@ -124,15 +124,15 @@
             f"{username}/*": {"admin"},
             f"{default_namespace}/*": {"viewer"},
             "global/*": roles,
         }
 
         for group in user_data.get("groups", []):
             # Use only the base name of Keycloak groups
-            group_name = os.path.basename(group)
+            group_name = Path(group).name
             namespaces.add(group_name)
             role_bindings[f"{group_name}/*"] = roles
 
         conda_store = get_conda_store(request)
         for namespace in namespaces:
             _namespace = api.get_namespace(conda_store.db, name=namespace)
             if _namespace is None:
@@ -165,12 +165,12 @@
 conda_store_settings = config["extra-settings"]
 for classname, attributes in conda_store_settings.items():
     for attribute, value in attributes.items():
         setattr(getattr(c, classname), attribute, value)
 
 # run arbitrary python code
 # compiling makes debugging easier: https://stackoverflow.com/a/437857
-extra_config_filename = os.path.join(tempfile.gettempdir(), "extra-config.py")
+extra_config_filename = Path(tempfile.gettempdir()) / "extra-config.py"
 extra_config = config.get("extra-config", "")
 with open(extra_config_filename, "w") as f:
     f.write(extra_config)
 exec(compile(source=extra_config, filename=extra_config_filename, mode="exec"))
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 import json
-import os
+from pathlib import Path
 
 import urllib3
 from aiohttp import web
 from dask_gateway_server.auth import JupyterHubAuthenticator
 from dask_gateway_server.options import Mapping, Options, Select
 
 
@@ -73,15 +73,15 @@
             and "dask_gateway_admin" not in data["roles"]
         ):
             raise web.HTTPInternalServerError(
                 reason="Permission failure user does not have required dask_gateway roles"
             )
 
         user.admin = "dask_gateway_admin" in data["roles"]
-        user.groups = [os.path.basename(group) for group in data["groups"]]
+        user.groups = [Path(group).name for group in data["groups"]]
         return user
 
 
 c.DaskGateway.authenticator_class = NebariAuthentication
 c.JupyterHubAuthenticator.jupyterhub_api_url = config["jupyterhub_api_url"]
 c.JupyterHubAuthenticator.jupyterhub_api_token = config["jupyterhub_api_token"]
 
@@ -139,15 +139,15 @@
         "scheduler_extra_pod_config": {"nodeSelector": scheduler_node_group},
         "worker_extra_pod_config": {"nodeSelector": worker_node_group},
     }
 
 
 def base_conda_store_mounts(namespace, name):
     conda_store_pvc_name = config["conda-store-pvc"]
-    conda_store_mount = config["conda-store-mount"]
+    conda_store_mount = Path(config["conda-store-mount"])
 
     return {
         "scheduler_extra_pod_config": {
             "volumes": [
                 {
                     "name": "conda-store",
                     "persistentVolumeClaim": {
@@ -155,15 +155,15 @@
                     },
                 }
             ]
         },
         "scheduler_extra_container_config": {
             "volumeMounts": [
                 {
-                    "mountPath": os.path.join(conda_store_mount, namespace),
+                    "mountPath": str(conda_store_mount / namespace),
                     "name": "conda-store",
                     "subPath": namespace,
                 }
             ]
         },
         "worker_extra_pod_config": {
             "volumes": [
@@ -174,26 +174,24 @@
                     },
                 }
             ]
         },
         "worker_extra_container_config": {
             "volumeMounts": [
                 {
-                    "mountPath": os.path.join(conda_store_mount, namespace),
+                    "mountPath": str(conda_store_mount / namespace),
                     "name": "conda-store",
                     "subPath": namespace,
                 }
             ]
         },
         "worker_cmd": "/opt/conda-run-worker",
         "scheduler_cmd": "/opt/conda-run-scheduler",
         "environment": {
-            "CONDA_ENVIRONMENT": os.path.join(
-                conda_store_mount, namespace, "envs", name
-            ),
+            "CONDA_ENVIRONMENT": str(conda_store_mount / namespace / "envs" / name),
         },
     }
 
 
 def base_username_mount(username, uid=1000, gid=100):
     return {
         "scheduler_extra_pod_config": {"volumes": [{"name": "home", "emptyDir": {}}]},
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 locals {
-  jupyter-notebook-config-py-template = templatefile("${path.module}/files/jupyter/jupyter_notebook_config.py.tpl", {
+  jupyter-notebook-config-py-template = templatefile("${path.module}/files/jupyter/jupyter_server_config.py.tpl", {
     terminal_cull_inactive_timeout      = var.idle-culler-settings.terminal_cull_inactive_timeout
     terminal_cull_interval              = var.idle-culler-settings.terminal_cull_interval
     kernel_cull_idle_timeout            = var.idle-culler-settings.kernel_cull_idle_timeout
     kernel_cull_interval                = var.idle-culler-settings.kernel_cull_interval
     kernel_cull_connected               = var.idle-culler-settings.kernel_cull_connected ? "True" : "False" # for Python compatible boolean values
     kernel_cull_busy                    = var.idle-culler-settings.kernel_cull_busy ? "True" : "False"      # for Python compatible boolean values
     server_shutdown_no_activity_timeout = var.idle-culler-settings.server_shutdown_no_activity_timeout
     }
   )
 }
 
 
-resource "local_file" "jupyter_notebook_config_py" {
+resource "local_file" "jupyter_server_config_py" {
   content  = local.jupyter-notebook-config-py-template
-  filename = "${path.module}/files/jupyter/jupyter_notebook_config.py"
+  filename = "${path.module}/files/jupyter/jupyter_server_config.py"
 }
 
 
 resource "kubernetes_config_map" "etc-ipython" {
   metadata {
     name      = "etc-ipython"
     namespace = var.namespace
@@ -29,24 +29,24 @@
     filename => file("${path.module}/files/ipython/${filename}")
   }
 }
 
 
 resource "kubernetes_config_map" "etc-jupyter" {
   depends_on = [
-    local_file.jupyter_notebook_config_py
+    local_file.jupyter_server_config_py
   ]
 
   metadata {
     name      = "etc-jupyter"
     namespace = var.namespace
   }
 
   data = {
-    "jupyter_notebook_config.py" : local_file.jupyter_notebook_config_py.content
+    "jupyter_server_config.py" : local_file.jupyter_server_config_py.content
   }
 }
 
 
 resource "kubernetes_config_map" "etc-skel" {
   metadata {
     name      = "etc-skel"
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,27 @@
   version    = "1.2.0"
 
   values = concat([
     file("${path.module}/values.yaml"),
     jsonencode({
       # custom values can be accessed via z2jh.get_config('custom.<path>')
       custom = {
+        namespace                     = var.namespace
+        external-url                  = var.external-url
         theme                         = var.theme
         profiles                      = var.profiles
         cdsdashboards                 = var.cdsdashboards
         home-pvc                      = var.home-pvc
         shared-pvc                    = var.shared-pvc
         conda-store-pvc               = var.conda-store-pvc
         conda-store-mount             = var.conda-store-mount
         default-conda-store-namespace = var.default-conda-store-namespace
         conda-store-service-name      = var.conda-store-service-name
         conda-store-cdsdashboards     = var.conda-store-cdsdashboard-token
+        conda-store-jupyter-scheduler = var.conda-store-argo-workflows-jupyter-scheduler-token
         skel-mount = {
           name      = kubernetes_config_map.etc-skel.metadata.0.name
           namespace = kubernetes_config_map.etc-skel.metadata.0.namespace
         }
         extra-mounts = merge(
           var.extra-mounts,
           {
@@ -205,7 +208,22 @@
   }
   callback-url-paths = [
     "https://${var.external-url}/hub/oauth_callback",
     var.jupyterhub-logout-redirect-url
   ]
   jupyterlab_profiles_mapper = true
 }
+
+
+resource "kubernetes_secret" "argo-workflows-conda-store-token" {
+  metadata {
+    name      = "argo-workflows-conda-store-token"
+    namespace = var.namespace
+  }
+
+  data = {
+    "conda-store-api-token"    = var.conda-store-argo-workflows-jupyter-scheduler-token
+    "conda-store-service-name" = var.conda-store-service-name
+  }
+
+  type = "Opaque"
+}
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,19 @@
 
 variable "conda-store-cdsdashboard-token" {
   description = "Token for cdsdashboards to use conda-store"
   type        = string
   default     = ""
 }
 
+variable "conda-store-argo-workflows-jupyter-scheduler-token" {
+  description = "Token for argo-workflows-jupyter-schedule to use conda-store"
+  type        = string
+}
+
 variable "jupyterhub-logout-redirect-url" {
   description = "Next redirect destination following a Keycloak logout"
   type        = string
   default     = ""
 }
 
 variable "jupyterhub-hub-extraEnv" {
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl`

 * *Files 22% similar despite different names*

```diff
@@ -32,7 +32,14 @@
 # Shut down the server after N seconds with no kernels or terminals
 # running and no activity.
 c.NotebookApp.shutdown_no_activity_timeout = ${server_shutdown_no_activity_timeout} * 60
 
 ###############################################################################
 # JupyterHub idle culler total timeout corresponds (approximately) to:
 # max(cull_idle_timeout, cull_inactive_timeout) + shutdown_no_activity_timeout
+
+from argo_jupyter_scheduler.executor import ArgoExecutor
+from argo_jupyter_scheduler.scheduler import ArgoScheduler
+
+c.Scheduler.execution_manager_class=ArgoExecutor
+c.SchedulerApp.scheduler_class=ArgoScheduler
+c.SchedulerApp.scheduler_class.use_conda_store_env=True
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import functools
 import json
-import os
+from pathlib import Path
 
 import z2jh
 from tornado import gen
 
 
 def base_profile_home_mounts(username):
     """Configure the home directory mount for user.
@@ -55,15 +55,19 @@
     init_containers = [
         {
             "name": "initialize-home-mount",
             "image": "busybox:1.31",
             "command": ["sh", "-c", command],
             "securityContext": {"runAsUser": 0},
             "volumeMounts": [
-                {"mountPath": "/mnt", "name": "home"},
+                {
+                    "mountPath": f"/mnt/{pvc_home_mount_path.format(username=username)}",
+                    "name": "home",
+                    "subPath": pvc_home_mount_path.format(username=username),
+                },
                 {"mountPath": "/etc/skel", "name": "skel"},
             ],
         }
     ]
     return {
         "extra_pod_config": extra_pod_config,
         "extra_container_config": extra_container_config,
@@ -114,17 +118,19 @@
         {
             "name": "initialize-shared-mounts",
             "image": "busybox:1.31",
             "command": ["sh", "-c", command],
             "securityContext": {"runAsUser": 0},
             "volumeMounts": [
                 {
-                    "mountPath": "/mnt",
+                    "mountPath": f"/mnt/{pvc_shared_mount_path.format(group=group)}",
                     "name": "shared" if home_pvc_name != shared_pvc_name else "home",
+                    "subPath": pvc_shared_mount_path.format(group=group),
                 }
+                for group in groups
             ],
         }
     ]
     return {
         "extra_pod_config": extra_pod_config,
         "extra_container_config": extra_container_config,
         "init_containers": init_containers,
@@ -136,15 +142,15 @@
     user.
 
     Ensure that {shared}/{group} directory exists and user has
     permissions to read/write/execute.
 
     """
     conda_store_pvc_name = z2jh.get_config("custom.conda-store-pvc")
-    conda_store_mount = z2jh.get_config("custom.conda-store-mount")
+    conda_store_mount = Path(z2jh.get_config("custom.conda-store-mount"))
     default_namespace = z2jh.get_config("custom.default-conda-store-namespace")
 
     extra_pod_config = {
         "volumes": [
             {
                 "name": "conda-store",
                 "persistentVolumeClaim": {
@@ -154,15 +160,15 @@
         ]
     }
 
     conda_store_namespaces = [username, default_namespace, "global"] + groups
     extra_container_config = {
         "volumeMounts": [
             {
-                "mountPath": os.path.join(conda_store_mount, namespace),
+                "mountPath": str(conda_store_mount / namespace),
                 "name": "conda-store",
                 "subPath": namespace,
             }
             for namespace in conda_store_namespaces
         ]
     }
 
@@ -177,17 +183,19 @@
         {
             "name": "initialize-conda-store-mounts",
             "image": "busybox:1.31",
             "command": ["sh", "-c", command],
             "securityContext": {"runAsUser": 0},
             "volumeMounts": [
                 {
-                    "mountPath": "/mnt",
+                    "mountPath": f"/mnt/{namespace}",
                     "name": "conda-store",
+                    "subPath": namespace,
                 }
+                for namespace in conda_store_namespaces
             ],
         }
     ]
     return {
         "extra_pod_config": extra_pod_config,
         "extra_container_config": extra_container_config,
         "init_containers": init_containers,
@@ -299,14 +307,72 @@
         "gid": gid,
         "fs_gid": gid,
         "notebook_dir": f"/home/{username}",
         "extra_container_config": extra_container_config,
     }
 
 
+def profile_argo_token(groups):
+    # TODO: create a more robust check user's Argo-Workflow role
+
+    domain = z2jh.get_config("custom.external-url")
+    namespace = z2jh.get_config("custom.namespace")
+
+    ADMIN = "admin"
+    DEVELOPER = "developer"
+    ANALYST = "analyst"
+
+    base = "argo-"
+    argo_sa = None
+
+    if ANALYST in groups:
+        argo_sa = base + "view"
+    if DEVELOPER in groups:
+        argo_sa = base + "developer"
+    if ADMIN in groups:
+        argo_sa = base + "admin"
+    if not argo_sa:
+        return {}
+
+    return {
+        "ARGO_BASE_HREF": "/argo",
+        "ARGO_SERVER": f"{domain}:443",
+        "ARGO_NAMESPACE": namespace,
+        "ARGO_TOKEN": {
+            "valueFrom": {
+                "secretKeyRef": {
+                    "name": f"{argo_sa}.service-account-token",
+                    "key": "token",
+                }
+            }
+        },
+    }
+
+
+def profile_conda_store_viewer_token():
+    return {
+        "CONDA_STORE_TOKEN": {
+            "valueFrom": {
+                "secretKeyRef": {
+                    "name": "argo-workflows-conda-store-token",
+                    "key": "conda-store-api-token",
+                }
+            }
+        },
+        "CONDA_STORE_SERVICE": {
+            "valueFrom": {
+                "secretKeyRef": {
+                    "name": "argo-workflows-conda-store-token",
+                    "key": "conda-store-service-name",
+                }
+            }
+        },
+    }
+
+
 def render_profile(profile, username, groups, keycloak_profilenames):
     """Render each profile for user.
 
     If profile is not available for given username, groups returns
     None. Otherwise profile is transformed into kubespawner profile.
 
     {
@@ -354,15 +420,20 @@
     # This is mainly to ensure JUPYTERHUB_ANYONE/GROUP is passed through from the spawner
     # to control dashboard access.
     envvars_fixed = {**(profile["kubespawner_override"].get("environment", {}))}
 
     def preserve_envvars(spawner):
         # This adds in JUPYTERHUB_ANYONE/GROUP rather than overwrite all env vars,
         # if set in the spawner for a dashboard to control access.
-        return {**envvars_fixed, **spawner.environment}
+        return {
+            **envvars_fixed,
+            **spawner.environment,
+            **profile_argo_token(groups),
+            **profile_conda_store_viewer_token(),
+        }
 
     profile["kubespawner_override"]["environment"] = preserve_envvars
 
     return profile
 
 
 @gen.coroutine
@@ -374,15 +445,15 @@
     auth_state = yield spawner.user.get_auth_state()
     spawner.log.error(str(auth_state))
 
     username = auth_state["oauth_user"]["preferred_username"]
     # only return the lowest level group name
     # e.g. /projects/myproj -> myproj
     # and /developers -> developers
-    groups = [os.path.basename(_) for _ in auth_state["oauth_user"]["groups"]]
+    groups = [Path(group).name for group in auth_state["oauth_user"]["groups"]]
     spawner.log.error(f"user info: {username} {groups}")
 
     keycloak_profilenames = auth_state["oauth_user"].get("jupyterlab_profiles", [])
 
     # fetch available profiles and render additional attributes
     profile_list = z2jh.get_config("custom.profiles")
     return list(
@@ -392,14 +463,18 @@
                 render_profile(p, username, groups, keycloak_profilenames)
                 for p in profile_list
             ],
         )
     )
 
 
+c.KubeSpawner.args = ["--debug"]
+c.KubeSpawner.environment = {
+    "JUPYTERHUB_SINGLEUSER_APP": "jupyter_server.serverapp.ServerApp",
+}
 c.KubeSpawner.profile_list = render_profiles
 
 
 # Utils
 def deep_merge(d1, d2):
     """Deep merge two dictionaries.
     >>> value_1 = {
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 variable "namespace" {
-  description = "deploy monitoring services on this namespace"
+  description = "deploy argo server on this namespace"
   type        = string
   default     = "dev"
 }
 
-
-variable "external-url" {
-  description = "External url that jupyterhub cluster is accessible"
-  type        = string
-}
-
-
-variable "realm_id" {
-  description = "Keycloak realm for creating oauth client"
+variable "argo-workflows-namespace" {
+  description = "deploy argo workflows on this namespace"
   type        = string
-}
-
-
-variable "dashboards" {
-  description = "Enabled grafana dashboards"
-  type        = set(string)
-  default = [
-    "Main",
-  ]
-}
-
-variable "jupyterhub_api_token" {
-  type      = string
-  default   = ""
-  sensitive = true
+  default     = "dev"
 }
 
 variable "node-group" {
   description = "Node key value pair for bound resources"
   type = object({
     key   = string
     value = string
   })
 }
 
+variable "external-url" {
+  description = "External url where jupyterhub cluster is accessible"
+  type        = string
+}
+
 
 variable "overrides" {
-  description = "Grafana helm chart overrides"
+  description = "Argo Workflows helm chart overrides"
   type        = list(string)
   default     = []
 }
+
+variable "realm_id" {
+  description = "Keycloak realm to use for deploying openid client"
+  type        = string
+}
+
+variable "keycloak-read-only-user-credentials" {
+  sensitive   = true
+  description = "Keycloak password for nebari-bot"
+  type        = map(string)
+  default     = {}
+}
+
+variable "workflow-controller-image-tag" {
+  description = "Image tag for nebari-workflow-controller"
+  type        = string
+}
+
+variable "nebari-workflow-controller" {
+  description = "Nebari Workflow Controller enabled"
+  type        = bool
+}
```

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf` & `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/scripts/aws-force-destroy.py` & `nebari-2023.7.1rc1/scripts/aws-force-destroy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import argparse
 import logging
-import pathlib
 import time
+from pathlib import Path
 
-from nebari.utils import check_cloud_credentials, load_yaml, timer
+from _nebari.utils import check_cloud_credentials, load_yaml, timer
 
 logging.basicConfig(level=logging.INFO)
 
 
 def main():
     parser = argparse.ArgumentParser(description="Force Destroy AWS environment.")
     parser.add_argument("-c", "--config", help="nebari configuration", required=True)
     args = parser.parse_args()
 
     handle_force_destroy(args)
 
 
 def handle_force_destroy(args):
-    config_filename = pathlib.Path(args.config)
+    config_filename = Path(args.config)
     if not config_filename.is_file():
         raise ValueError(
             f"passed in configuration filename={config_filename} must exist"
         )
 
     config = load_yaml(config_filename)
```

### Comparing `nebari-2023.5.1rc1/scripts/aws-force-destroy.sh` & `nebari-2023.7.1rc1/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/scripts/keycloak-export.py` & `nebari-2023.7.1rc1/scripts/keycloak-export.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import argparse
 import json
 import logging
-import pathlib
 import sys
+from pathlib import Path
 
-from nebari.keycloak import get_keycloak_admin_from_config
+from _nebari.keycloak import get_keycloak_admin_from_config
 
 logging.basicConfig(level=logging.INFO)
 
 
 def main():
     parser = argparse.ArgumentParser(description="Export users and groups from Nebari.")
     parser.add_argument("-c", "--config", help="nebari configuration", required=True)
     args = parser.parse_args()
 
     handle_keycloak_export(args)
 
 
 def handle_keycloak_export(args):
-    config_filename = pathlib.Path(args.config)
+    config_filename = Path(args.config)
     if not config_filename.is_file():
         raise ValueError(
             f"passed in configuration filename={config_filename} must exist"
         )
 
     keycloak_admin = get_keycloak_admin_from_config(config_filename)
```

### Comparing `nebari-2023.5.1rc1/tests/conftest.py` & `nebari-2023.7.1rc1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 from unittest.mock import Mock
 
 import pytest
 
-from nebari.initialize import render_config
+from _nebari.initialize import render_config
 
 INIT_INPUTS = [
     # project, namespace, domain, cloud_provider, ci_provider, auth_provider
     ("pytestdo", "dev", "do.nebari.dev", "do", "github-actions", "github"),
     ("pytestaws", "dev", "aws.nebari.dev", "aws", "github-actions", "github"),
     ("pytestgcp", "dev", "gcp.nebari.dev", "gcp", "github-actions", "github"),
     ("pytestazure", "dev", "azure.nebari.dev", "azure", "github-actions", "github"),
@@ -55,30 +55,30 @@
         m.return_value = k8s_versions
         if grab_latest_version:
             m.return_value = k8s_versions[-1]
         return m
 
     if cloud_provider == "aws":
         monkeypatch.setattr(
-            "nebari.utils.amazon_web_services.kubernetes_versions",
+            "_nebari.utils.amazon_web_services.kubernetes_versions",
             _mock_kubernetes_versions(),
         )
     elif cloud_provider == "azure":
         monkeypatch.setattr(
-            "nebari.utils.azure_cloud.kubernetes_versions",
+            "_nebari.utils.azure_cloud.kubernetes_versions",
             _mock_kubernetes_versions(),
         )
     elif cloud_provider == "do":
         monkeypatch.setattr(
-            "nebari.utils.digital_ocean.kubernetes_versions",
+            "_nebari.utils.digital_ocean.kubernetes_versions",
             _mock_kubernetes_versions(),
         )
     elif cloud_provider == "gcp":
         monkeypatch.setattr(
-            "nebari.utils.google_cloud.kubernetes_versions",
+            "_nebari.utils.google_cloud.kubernetes_versions",
             _mock_kubernetes_versions(),
         )
 
     output_directory = tmp_path / f"{cloud_provider}_output_dir"
     output_directory.mkdir()
     nebari_config_loc = output_directory / NEBARI_CONFIG_FN
```

### Comparing `nebari-2023.5.1rc1/tests/test_cli.py` & `nebari-2023.7.1rc1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 
 import pytest
 
-from nebari.schema import InitInputs
-from nebari.utils import load_yaml
+from _nebari.schema import InitInputs
+from _nebari.utils import load_yaml
 
 PROJECT_NAME = "clitest"
 DOMAIN_NAME = "clitest.dev"
 
 
 @pytest.mark.parametrize(
     "namespace, auth_provider, ci_provider, ssl_cert_email",
```

### Comparing `nebari-2023.5.1rc1/tests/test_commons.py` & `nebari-2023.7.1rc1/tests/test_commons.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
+from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
 
 
 def test_filter_by_highest_supported_k8s_version():
     version_to_filter = "99.99"
 
     k8s_versions = [
         "1.21.7",
```

### Comparing `nebari-2023.5.1rc1/tests/test_dependencies.py` & `nebari-2023.7.1rc1/tests/test_dependencies.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             check=True,
         )
 
         # get the directory the meta.yaml is in
         meta_loc = tmp_path / "nebari"
         # try to run conda build to build package from meta.yaml
         subprocess.run(
-            ["conda", "build", meta_loc],
+            ["conda", "build", "--channel=conda-forge", meta_loc],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             check=True,
         )
     except subprocess.CalledProcessError as e:
         print(e.stderr.decode("utf-8"))
         raise e
```

### Comparing `nebari-2023.5.1rc1/tests/test_init.py` & `nebari-2023.7.1rc1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests/test_render.py` & `nebari-2023.7.1rc1/tests/test_render.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 import pytest
 from ruamel.yaml import YAML
 
-from nebari.render import render_template, set_env_vars_in_config
+from _nebari.render import render_template, set_env_vars_in_config
 
 from .conftest import PRESERVED_DIR, render_config_partial
 
 
 @pytest.fixture
 def write_nebari_config_to_file(setup_fixture):
     nebari_config_loc, render_config_inputs = setup_fixture
@@ -31,15 +31,15 @@
         kubernetes_version=None,
     )
 
     # write to nebari_config.yaml
     yaml = YAML(typ="unsafe", pure=True)
     yaml.dump(config, nebari_config_loc)
 
-    render_template(str(nebari_config_loc.parent), nebari_config_loc, force=True)
+    render_template(nebari_config_loc.parent, nebari_config_loc)
 
     yield setup_fixture
 
 
 def test_get_secret_config_entries(monkeypatch):
     sec1 = "secret1"
     sec2 = "nestedsecret1"
```

### Comparing `nebari-2023.5.1rc1/tests/test_schema.py` & `nebari-2023.7.1rc1/tests/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import nebari.schema
+import _nebari.schema
 
 from .conftest import render_config_partial
 
 
 def test_schema(setup_fixture):
     (nebari_config_loc, render_config_inputs) = setup_fixture
     (
@@ -20,8 +20,8 @@
         nebari_domain=domain,
         cloud_provider=cloud_provider,
         ci_provider=ci_provider,
         auth_provider=auth_provider,
         kubernetes_version=None,
     )
 
-    nebari.schema.verify(config)
+    _nebari.schema.verify(config)
```

### Comparing `nebari-2023.5.1rc1/tests/test_upgrade.py` & `nebari-2023.7.1rc1/tests/test_upgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 import pytest
 
-from nebari.upgrade import do_upgrade, load_yaml, verify
-from nebari.version import __version__, rounded_ver_parse
+from _nebari.upgrade import do_upgrade, load_yaml, verify
+from _nebari.version import __version__, rounded_ver_parse
 
 
 @pytest.fixture
 def qhub_users_import_json():
     return (
         (
             Path(__file__).parent
```

### Comparing `nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests/scripts/minikube-loadbalancer-ip.py` & `nebari-2023.7.1rc1/tests/scripts/minikube-loadbalancer-ip.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 import json
-import os
 import subprocess
 import sys
+from pathlib import Path
 
 minikube_cmd = ["minikube", "ssh", "--", "ip", "-j", "a"]
 minikube_output = subprocess.check_output(minikube_cmd, encoding="utf-8")[:-1]
 
 address = None
 for interface in json.loads(minikube_output):
     if interface["ifname"] == "eth0":
         address = interface["addr_info"][0]["local"].split(".")
         break
 else:
     print("minikube interface eth0 not found")
     sys.exit(1)
 
-filename = os.path.expanduser("~/.minikube/profiles/minikube/config.json")
+filename = Path.home() / ".minikube" / "profiles" / "minikube" / "config.json"
 with open(filename) as f:
     data = json.load(f)
 
 start_address, end_address = ".".join(address[0:3] + ["100"]), ".".join(
     address[0:3] + ["150"]
 )
 print("Setting start=%s end=%s" % (start_address, end_address))
```

### Comparing `nebari-2023.5.1rc1/tests/vale/styles/vocab.txt` & `nebari-2023.7.1rc1/tests/vale/styles/vocab.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_deployment/test_dask_gateway.py` & `nebari-2023.7.1rc1/tests_deployment/test_dask_gateway.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2023.7.1rc1/tests_deployment/test_jupyterhub_ssh.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_deployment/utils.py` & `nebari-2023.7.1rc1/tests_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2023.7.1rc1/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_e2e/package-lock.json` & `nebari-2023.7.1rc1/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_e2e/cypress/integration/main.js` & `nebari-2023.7.1rc1/tests_e2e/cypress/integration/main.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2023.7.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_e2e/cypress/plugins/index.js` & `nebari-2023.7.1rc1/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/tests_e2e/cypress/support/index.js` & `nebari-2023.7.1rc1/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/.gitignore` & `nebari-2023.7.1rc1/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # docs
 .nox
 _build
+.env
 
 # setuptools scm
-nebari/_version.py
+src/_nebari/_version.py
 
 # ignore terraform state
 .terraform
 terraform.tfstate
 terraform.tfstate.backup
 .terraform.tfstate.lock.info
 
+# tests
+videos/
+
 # python
 __pycache__
 build/
 *.egg
 *.egg-info/
 dist/
 env/
@@ -41,9 +45,10 @@
 # this should cover imported modules while not gitignoring our new direct 'modules' folder.
 
 # ignore nebari files
 nebari-config.yaml
 
 .vscode/
 .pytest_cache
-
+.ipynb_checkpoints
+.DS_Store
 /.ruff_cache
```

### Comparing `nebari-2023.5.1rc1/LICENSE` & `nebari-2023.7.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.5.1rc1/README.md` & `nebari-2023.7.1rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 ---
 
 | Information | Links |
 | :---------- | :-----|
 |   Project   | [![License](https://img.shields.io/badge/License-BSD%203--Clause-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Nebari documentation](https://img.shields.io/badge/%F0%9F%93%96%20Read-the%20docs-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://www.nebari.dev/docs/welcome) [![PyPI](https://img.shields.io/pypi/v/nebari)](https://badge.fury.io/py/nebari) [![conda version](https://img.shields.io/conda/vn/conda-forge/nebari)]((https://anaconda.org/conda-forge/nebari))  |
 |  Community  | [![GH discussions](https://img.shields.io/badge/%F0%9F%92%AC%20-Participate%20in%20discussions-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://github.com/nebari-dev/nebari/discussions) [![Open an issue](https://img.shields.io/badge/%F0%9F%93%9D%20Open-an%20issue-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://github.com/nebari-dev/nebari/issues/new/choose) [![Community guidelines](https://img.shields.io/badge/🤝%20Community-guidelines-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://www.nebari.dev/docs/community/) |
-|     CI      | [![Kubernetes Tests](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml) [![Tests](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml) |
+|     CI      | [![Kubernetes Tests](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml) [![Tests](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml) [![Test Nebari Provider](https://github.com/nebari-dev/nebari/actions/workflows/test-provider.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/test-provider.yaml) |
 
 ## Table of contents
 
 - [Table of contents](#table-of-contents)
-- [QHub HPC](#qhub-hpc)
 - [Nebari](#nebari)
   - [Cloud Providers ☁️](#cloud-providers-️)
 - [Installation 💻](#installation-)
   - [Pre-requisites](#pre-requisites)
   - [Install Nebari](#install-nebari)
 - [Usage 🚀](#usage-)
+- [Nebari HPC](#nebari-hpc)
 - [Contributing to Nebari 👩🏻‍💻](#contributing-to-nebari-)
   - [Installing the Development version of Nebari ⚙️](#installing-the-development-version-of-nebari-️)
   - [Questions? 🤔](#questions-)
 - [Code of Conduct 📖](#code-of-conduct-)
 - [Ongoing Support](#ongoing-support)
 - [License](#license)
 
@@ -43,21 +43,15 @@
 [Dask Gateway](https://docs.dask.org/ "Parallel computing in Python").
 
 Nebari is an open source data platform that enables users to build and maintain cost-effective and scalable compute platforms
 on [HPC](#nebari-hpc) or [Kubernetes](#nebari) with minimal DevOps overhead.
 
 **This repository details the [Nebari](https://nebari.dev/ "Official Nebari docs") (Kubernetes) version.**
 
-Not sure what to choose? Check out our [Setup Initialization](docs/source/installation/setup.md) page.
-
-## QHub HPC
-
-The HPC version of Nebari is based on [OpenHPC](https://openhpc.community/).
-
-> NOTE: The tool is currently under development. Curious? Check out the [Nebari HPC](https://github.com/Quansight/qhub-hpc) repository.
+Not sure what to choose? Check out our documentation on [choosing a deployment platform](https://www.nebari.dev/docs/get-started/deploy)
 
 ## Nebari
 
 The Kubernetes version of Nebari uses [Terraform](https://www.terraform.io/), [Helm](https://helm.sh/), and
 [GitHub Actions](https://docs.github.com/en/free-pro-team@latest/actions).
 
 - Terraform handles the build, change, and versioning of the infrastructure.
@@ -134,14 +128,19 @@
 For details on obtaining those variables, check the [Nebari Get started documentation][docs-get-started].
 
 Once all the necessary credentials are gathered and set as [UNIX environment variables](https://linuxize.com/post/how-to-set-and-list-environment-variables-in-linux/), Nebari can be
 deployed in minutes.
 
 For detailed step-by-step instructions on how to deploy Nebari, check the [Nebari documentation][docs-deploy].
 
+## Nebari HPC
+
+An HPC version of Nebari is currently not available. There is one under development for Nebaris precursor QHub.
+Curious? Check out the [QHub HPC](https://github.com/Quansight/qhub-hpc) repository.
+
 ## Contributing to Nebari 👩🏻‍💻
 
 Thinking about contributing? Check out our [Contribution Guidelines](CONTRIBUTING.md) to get started.
 
 ### Installing the Development version of Nebari ⚙️
 
 To install the latest developer version (unstable) use:
```

### Comparing `nebari-2023.5.1rc1/pyproject.toml` & `nebari-2023.7.1rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 ### Build ###
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-include = ["nebari"]
+packages = [
+    "src/_nebari",
+    "src/nebari",
+]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
-version-file = "nebari/_version.py"
+version-file = "src/_nebari/_version.py"
 local_scheme = "node-and-timestamp"
 
 
 ### Project ###
 [project]
 name = "nebari"
 dynamic = ["version"]
@@ -69,38 +72,45 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==22.3.0",
     "dask-gateway",
     "diagrams",
+    "python-dotenv",
     "escapism",
     "flake8==3.8.4",
     "importlib-metadata<5.0",
     "jhub-client",
     "paramiko",
     "pre-commit",
     "pytest",
     "pytest-timeout",
+    "pytest-playwright",
     "grayskull",
     "build",
+    "jinja2",
 ]
 
 [project.urls]
 Documentation = "https://www.nebari.dev/docs"
 Source = "https://github.com/nebari-dev/nebari"
 
 [project.scripts]
-nebari = "nebari.cli.main:app"
+nebari = "_nebari.cli.main:app"
 
 [tool.ruff]
+select = [
+    "E",
+    "F",
+    "PTH",
+]
 ignore = [
     "E501", # Line too long
     "F821", # Undefined name
+    "PTH123", # open() should be replaced by Path.open()
 ]
 extend-exclude = [
-    "nebari/template",
-    "docs/source/conf.py",
-    "docs",
+    "src/_nebari/template",
     "home",
     "__pycache__"
 ]
```

### Comparing `nebari-2023.5.1rc1/PKG-INFO` & `nebari-2023.7.1rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari
-Version: 2023.5.1rc1
+Version: 2023.7.1rc1
 Summary: A Jupyter and Dask-powered open source data science platform.
 Project-URL: Documentation, https://www.nebari.dev/docs
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
@@ -42,18 +42,21 @@
 Requires-Dist: dask-gateway; extra == 'dev'
 Requires-Dist: diagrams; extra == 'dev'
 Requires-Dist: escapism; extra == 'dev'
 Requires-Dist: flake8==3.8.4; extra == 'dev'
 Requires-Dist: grayskull; extra == 'dev'
 Requires-Dist: importlib-metadata<5.0; extra == 'dev'
 Requires-Dist: jhub-client; extra == 'dev'
+Requires-Dist: jinja2; extra == 'dev'
 Requires-Dist: paramiko; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-playwright; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
+Requires-Dist: python-dotenv; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <p align="center">
 <picture>
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/nebari-dev/nebari-design/main/logo-mark/horizontal/Nebari-Logo-Horizontal-Lockup.svg">
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/nebari-dev/nebari-design/main/logo-mark/horizontal/Nebari-Logo-Horizontal-Lockup-White-text.svg">
   <img alt="Nebari logo mark - text will be black in light color mode and white in dark color mode." src="https://raw.githubusercontent.com/nebari-dev/nebari-design/main/logo-mark/horizontal/Nebari-Logo-Horizontal-Lockup-White-text.svg" width="50%"/>
@@ -64,26 +67,26 @@
 
 ---
 
 | Information | Links |
 | :---------- | :-----|
 |   Project   | [![License](https://img.shields.io/badge/License-BSD%203--Clause-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Nebari documentation](https://img.shields.io/badge/%F0%9F%93%96%20Read-the%20docs-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://www.nebari.dev/docs/welcome) [![PyPI](https://img.shields.io/pypi/v/nebari)](https://badge.fury.io/py/nebari) [![conda version](https://img.shields.io/conda/vn/conda-forge/nebari)]((https://anaconda.org/conda-forge/nebari))  |
 |  Community  | [![GH discussions](https://img.shields.io/badge/%F0%9F%92%AC%20-Participate%20in%20discussions-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://github.com/nebari-dev/nebari/discussions) [![Open an issue](https://img.shields.io/badge/%F0%9F%93%9D%20Open-an%20issue-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://github.com/nebari-dev/nebari/issues/new/choose) [![Community guidelines](https://img.shields.io/badge/🤝%20Community-guidelines-gray.svg?colorA=2D2A56&colorB=5936D9&style=flat.svg)](https://www.nebari.dev/docs/community/) |
-|     CI      | [![Kubernetes Tests](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml) [![Tests](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml) |
+|     CI      | [![Kubernetes Tests](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/kubernetes_test.yaml) [![Tests](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/test.yaml) [![Test Nebari Provider](https://github.com/nebari-dev/nebari/actions/workflows/test-provider.yaml/badge.svg)](https://github.com/nebari-dev/nebari/actions/workflows/test-provider.yaml) |
 
 ## Table of contents
 
 - [Table of contents](#table-of-contents)
-- [QHub HPC](#qhub-hpc)
 - [Nebari](#nebari)
   - [Cloud Providers ☁️](#cloud-providers-️)
 - [Installation 💻](#installation-)
   - [Pre-requisites](#pre-requisites)
   - [Install Nebari](#install-nebari)
 - [Usage 🚀](#usage-)
+- [Nebari HPC](#nebari-hpc)
 - [Contributing to Nebari 👩🏻‍💻](#contributing-to-nebari-)
   - [Installing the Development version of Nebari ⚙️](#installing-the-development-version-of-nebari-️)
   - [Questions? 🤔](#questions-)
 - [Code of Conduct 📖](#code-of-conduct-)
 - [Ongoing Support](#ongoing-support)
 - [License](#license)
 
@@ -97,21 +100,15 @@
 [Dask Gateway](https://docs.dask.org/ "Parallel computing in Python").
 
 Nebari is an open source data platform that enables users to build and maintain cost-effective and scalable compute platforms
 on [HPC](#nebari-hpc) or [Kubernetes](#nebari) with minimal DevOps overhead.
 
 **This repository details the [Nebari](https://nebari.dev/ "Official Nebari docs") (Kubernetes) version.**
 
-Not sure what to choose? Check out our [Setup Initialization](docs/source/installation/setup.md) page.
-
-## QHub HPC
-
-The HPC version of Nebari is based on [OpenHPC](https://openhpc.community/).
-
-> NOTE: The tool is currently under development. Curious? Check out the [Nebari HPC](https://github.com/Quansight/qhub-hpc) repository.
+Not sure what to choose? Check out our documentation on [choosing a deployment platform](https://www.nebari.dev/docs/get-started/deploy)
 
 ## Nebari
 
 The Kubernetes version of Nebari uses [Terraform](https://www.terraform.io/), [Helm](https://helm.sh/), and
 [GitHub Actions](https://docs.github.com/en/free-pro-team@latest/actions).
 
 - Terraform handles the build, change, and versioning of the infrastructure.
@@ -188,14 +185,19 @@
 For details on obtaining those variables, check the [Nebari Get started documentation][docs-get-started].
 
 Once all the necessary credentials are gathered and set as [UNIX environment variables](https://linuxize.com/post/how-to-set-and-list-environment-variables-in-linux/), Nebari can be
 deployed in minutes.
 
 For detailed step-by-step instructions on how to deploy Nebari, check the [Nebari documentation][docs-deploy].
 
+## Nebari HPC
+
+An HPC version of Nebari is currently not available. There is one under development for Nebaris precursor QHub.
+Curious? Check out the [QHub HPC](https://github.com/Quansight/qhub-hpc) repository.
+
 ## Contributing to Nebari 👩🏻‍💻
 
 Thinking about contributing? Check out our [Contribution Guidelines](CONTRIBUTING.md) to get started.
 
 ### Installing the Development version of Nebari ⚙️
 
 To install the latest developer version (unstable) use:
```

