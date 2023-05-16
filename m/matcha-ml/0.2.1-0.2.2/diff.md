# Comparing `tmp/matcha_ml-0.2.1.tar.gz` & `tmp/matcha_ml-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matcha_ml-0.2.1.tar", max compression
+gzip compressed data, was "matcha_ml-0.2.2.tar", max compression
```

## Comparing `matcha_ml-0.2.1.tar` & `matcha_ml-0.2.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0    11357 2023-04-04 14:10:40.520364 matcha_ml-0.2.1/LICENSE
--rw-r--r--   0        0        0     1338 2023-05-09 13:44:21.956337 matcha_ml-0.2.1/README.md
--rw-r--r--   0        0        0     3436 2023-05-09 14:05:13.072604 matcha_ml-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        6 2023-05-09 14:04:42.186493 matcha_ml-0.2.1/src/matcha_ml/VERSION
--rw-r--r--   0        0        0      220 2023-04-04 14:10:40.522843 matcha_ml-0.2.1/src/matcha_ml/__init__.py
--rw-r--r--   0        0        0       70 2023-04-04 14:10:40.523033 matcha_ml-0.2.1/src/matcha_ml/cli/__init__.py
--rw-r--r--   0        0        0     7325 2023-05-09 11:58:51.235252 matcha_ml-0.2.1/src/matcha_ml/cli/_validation.py
--rw-r--r--   0        0        0     4162 2023-05-09 11:58:51.236865 matcha_ml-0.2.1/src/matcha_ml/cli/cli.py
--rw-r--r--   0        0        0     1299 2023-05-09 11:58:51.237110 matcha_ml-0.2.1/src/matcha_ml/cli/destroy.py
--rw-r--r--   0        0        0     2046 2023-05-09 11:58:51.237901 matcha_ml-0.2.1/src/matcha_ml/cli/provision.py
--rw-r--r--   0        0        0      278 2023-04-04 14:10:40.524450 matcha_ml-0.2.1/src/matcha_ml/cli/ui/emojis.py
--rw-r--r--   0        0        0     1173 2023-05-05 09:28:43.777509 matcha_ml-0.2.1/src/matcha_ml/cli/ui/print_messages.py
--rw-r--r--   0        0        0     2549 2023-05-05 09:28:43.777724 matcha_ml-0.2.1/src/matcha_ml/cli/ui/resource_message_builders.py
--rw-r--r--   0        0        0     1249 2023-04-04 14:10:40.524914 matcha_ml-0.2.1/src/matcha_ml/cli/ui/spinner.py
--rw-r--r--   0        0        0     1703 2023-04-04 14:10:40.525043 matcha_ml-0.2.1/src/matcha_ml/cli/ui/status_message_builders.py
--rw-r--r--   0        0        0     1780 2023-05-05 09:28:43.778741 matcha_ml-0.2.1/src/matcha_ml/core/core.py
--rw-r--r--   0        0        0     2535 2023-05-05 09:28:43.779321 matcha_ml-0.2.1/src/matcha_ml/errors.py
--rw-r--r--   0        0        0      882 2023-04-04 14:10:40.525367 matcha_ml-0.2.1/src/matcha_ml/infrastructure/.gitignore
--rw-r--r--   0        0        0     9245 2023-04-06 09:56:48.027234 matcha_ml-0.2.1/src/matcha_ml/infrastructure/.terraform.lock.hcl
--rw-r--r--   0        0        0     4696 2023-05-05 09:28:43.779729 matcha_ml-0.2.1/src/matcha_ml/infrastructure/README.md
--rw-r--r--   0        0        0     2213 2023-05-05 09:28:43.779888 matcha_ml-0.2.1/src/matcha_ml/infrastructure/aks/README.md
--rw-r--r--   0        0        0      439 2023-05-05 09:28:43.780559 matcha_ml-0.2.1/src/matcha_ml/infrastructure/aks/main.tf
--rw-r--r--   0        0        0     1437 2023-05-05 09:28:43.780870 matcha_ml-0.2.1/src/matcha_ml/infrastructure/aks/output.tf
--rw-r--r--   0        0        0      386 2023-05-05 09:28:43.781112 matcha_ml-0.2.1/src/matcha_ml/infrastructure/aks/variables.tf
--rw-r--r--   0        0        0     1605 2023-05-05 09:28:43.781271 matcha_ml-0.2.1/src/matcha_ml/infrastructure/azure_container_registry/README.md
--rw-r--r--   0        0        0      484 2023-05-05 09:28:43.781437 matcha_ml-0.2.1/src/matcha_ml/infrastructure/azure_container_registry/main.tf
--rw-r--r--   0        0        0      327 2023-05-05 09:28:43.781688 matcha_ml-0.2.1/src/matcha_ml/infrastructure/azure_container_registry/output.tf
--rw-r--r--   0        0        0      462 2023-05-05 09:28:43.781873 matcha_ml-0.2.1/src/matcha_ml/infrastructure/azure_container_registry/variables.tf
--rw-r--r--   0        0        0      458 2023-04-06 09:56:48.032139 matcha_ml-0.2.1/src/matcha_ml/infrastructure/configure_kubectl.tf
--rw-r--r--   0        0        0      337 2023-04-06 09:56:48.032648 matcha_ml-0.2.1/src/matcha_ml/infrastructure/helm.tf
--rw-r--r--   0        0        0      947 2023-04-06 09:56:48.032839 matcha_ml-0.2.1/src/matcha_ml/infrastructure/kubernetes.tf
--rw-r--r--   0        0        0     1829 2023-05-05 09:28:43.782518 matcha_ml-0.2.1/src/matcha_ml/infrastructure/main.tf
--rw-r--r--   0        0        0     2208 2023-05-05 09:28:43.782745 matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/README.md
--rw-r--r--   0        0        0      148 2023-05-05 09:28:43.783447 matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/getURI.tf
--rw-r--r--   0        0        0     1139 2023-05-05 09:28:43.783993 matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/main.tf
--rw-r--r--   0        0        0      251 2023-05-05 09:28:43.784519 matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/output.tf
--rw-r--r--   0        0        0      210 2023-04-04 15:05:54.475770 matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/providers.tf
--rw-r--r--   0        0        0      803 2023-05-05 09:28:43.784828 matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/variables.tf
--rw-r--r--   0        0        0       81 2023-05-05 09:28:43.785262 matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/zenml_namespace.tf
--rw-r--r--   0        0        0     1945 2023-05-05 09:28:43.786589 matcha_ml-0.2.1/src/matcha_ml/infrastructure/output.tf
--rw-r--r--   0        0        0       33 2023-04-06 09:56:48.034468 matcha_ml-0.2.1/src/matcha_ml/infrastructure/printf.cmd
--rw-r--r--   0        0        0      782 2023-05-05 09:28:43.786930 matcha_ml-0.2.1/src/matcha_ml/infrastructure/providers.tf
--rw-r--r--   0        0        0      892 2023-05-05 09:28:43.787082 matcha_ml-0.2.1/src/matcha_ml/infrastructure/resource_group/README.md
--rw-r--r--   0        0        0      110 2023-05-05 09:28:43.787427 matcha_ml-0.2.1/src/matcha_ml/infrastructure/resource_group/main.tf
--rw-r--r--   0        0        0      106 2023-05-05 09:28:43.787653 matcha_ml-0.2.1/src/matcha_ml/infrastructure/resource_group/output.tf
--rw-r--r--   0        0        0      224 2023-05-05 09:28:43.787874 matcha_ml-0.2.1/src/matcha_ml/infrastructure/resource_group/variables.tf
--rw-r--r--   0        0        0     3010 2023-05-05 09:28:43.788103 matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/README.md
--rw-r--r--   0        0        0     1730 2023-05-05 09:28:43.788796 matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/istio.tf
--rw-r--r--   0        0        0      993 2023-05-05 09:28:43.788994 matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/main.tf
--rw-r--r--   0        0        0      496 2023-05-05 09:28:43.789695 matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/outputs.tf
--rw-r--r--   0        0        0      925 2023-05-05 09:28:43.790208 matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/permissions.tf
--rw-r--r--   0        0        0      214 2023-04-04 15:05:54.476827 matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/providers.tf
--rw-r--r--   0        0        0      285 2023-05-05 09:28:43.790435 matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/variables.tf
--rw-r--r--   0        0        0     2914 2023-05-05 09:28:43.790638 matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/README.md
--rw-r--r--   0        0        0      866 2023-04-04 14:10:40.528281 matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/main.tf
--rw-r--r--   0        0        0     1779 2023-05-05 09:28:43.790845 matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/output.tf
--rw-r--r--   0        0        0      124 2023-04-04 14:10:40.528517 matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/providers.tf
--rw-r--r--   0        0        0      454 2023-05-05 09:28:43.791041 matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/variables.tf
--rw-r--r--   0        0        0      754 2023-05-05 09:28:43.791258 matcha_ml-0.2.1/src/matcha_ml/infrastructure/variables.tf
--rw-r--r--   0        0        0     6080 2023-05-05 09:28:43.791406 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/README.md
--rw-r--r--   0        0        0      216 2023-05-05 09:28:43.792124 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/getURL.tf
--rw-r--r--   0        0        0      979 2023-04-06 09:56:48.037603 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/ingress.tf
--rw-r--r--   0        0        0     2857 2023-05-05 09:28:43.792357 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/main.tf
--rw-r--r--   0        0        0      704 2023-05-05 09:28:43.792543 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/outputs.tf
--rw-r--r--   0        0        0      292 2023-04-06 09:56:48.038718 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/providers.tf
--rw-r--r--   0        0        0     1943 2023-04-06 09:56:48.039153 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/sql.tf
--rw-r--r--   0        0        0     4701 2023-05-05 09:28:43.792820 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/variables.tf
--rw-r--r--   0        0        0      342 2023-04-06 09:56:48.040666 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/Chart.yaml
--rw-r--r--   0        0        0     1987 2023-04-06 09:56:48.040971 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt
--rw-r--r--   0        0        0     2054 2023-04-06 09:56:48.041139 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl
--rw-r--r--   0        0        0     1565 2023-04-06 09:56:48.041323 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml
--rw-r--r--   0        0        0      910 2023-04-06 09:56:48.041582 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml
--rw-r--r--   0        0        0    10774 2023-04-06 09:56:48.041821 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml
--rw-r--r--   0        0        0     2225 2023-04-06 09:56:48.042001 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml
--rw-r--r--   0        0        0     3584 2023-04-06 09:56:48.042196 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml
--rw-r--r--   0        0        0      367 2023-04-06 09:56:48.042390 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-service.yaml
--rw-r--r--   0        0        0      316 2023-04-06 09:56:48.042628 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      379 2023-04-06 09:56:48.043020 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0    11587 2023-04-06 09:56:48.044021 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml
--rw-r--r--   0        0        0     3453 2023-05-05 09:28:43.792952 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zenml_storage/README.md
--rw-r--r--   0        0        0     1102 2023-04-04 14:10:40.528879 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zenml_storage/main.tf
--rw-r--r--   0        0        0     1926 2023-05-05 09:28:43.793304 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zenml_storage/output.tf
--rw-r--r--   0        0        0      468 2023-05-05 09:28:43.793535 matcha_ml-0.2.1/src/matcha_ml/infrastructure/zenml_storage/variables.tf
--rw-r--r--   0        0        0      103 2023-04-04 14:10:40.529246 matcha_ml-0.2.1/src/matcha_ml/services/__init__.py
--rw-r--r--   0        0        0     7929 2023-05-05 09:28:43.794319 matcha_ml-0.2.1/src/matcha_ml/services/azure_service.py
--rw-r--r--   0        0        0     2652 2023-05-05 09:28:43.794530 matcha_ml-0.2.1/src/matcha_ml/services/matcha_state.py
--rw-r--r--   0        0        0     4934 2023-05-09 09:54:17.783570 matcha_ml-0.2.1/src/matcha_ml/services/terraform_service.py
--rw-r--r--   0        0        0       41 2023-05-05 09:28:43.795524 matcha_ml-0.2.1/src/matcha_ml/templates/__init__.py
--rw-r--r--   0        0        0     7148 2023-05-09 11:58:51.240136 matcha_ml-0.2.1/src/matcha_ml/templates/build_templates/azure_template.py
--rw-r--r--   0        0        0     9647 2023-05-05 09:28:43.796777 matcha_ml-0.2.1/src/matcha_ml/templates/run_template.py
--rw-r--r--   0        0        0     3139 1970-01-01 00:00:00.000000 matcha_ml-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 13:30:52.718239 matcha_ml-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4177 2023-05-16 14:32:14.573403 matcha_ml-0.2.2/README.md
+-rw-r--r--   0        0        0     3465 2023-05-16 14:35:21.950085 matcha_ml-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-05-16 14:35:32.438541 matcha_ml-0.2.2/src/matcha_ml/VERSION
+-rw-r--r--   0        0        0      220 2023-05-16 13:30:52.737917 matcha_ml-0.2.2/src/matcha_ml/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-16 13:30:52.738233 matcha_ml-0.2.2/src/matcha_ml/cli/__init__.py
+-rw-r--r--   0        0        0     7645 2023-05-16 13:30:52.738457 matcha_ml-0.2.2/src/matcha_ml/cli/_validation.py
+-rw-r--r--   0        0        0     3928 2023-05-16 13:30:52.738697 matcha_ml-0.2.2/src/matcha_ml/cli/cli.py
+-rw-r--r--   0        0        0     1298 2023-05-16 13:30:52.738966 matcha_ml-0.2.2/src/matcha_ml/cli/destroy.py
+-rw-r--r--   0        0        0     3571 2023-05-16 13:30:52.739356 matcha_ml-0.2.2/src/matcha_ml/cli/provision.py
+-rw-r--r--   0        0        0      278 2023-05-16 13:30:52.739662 matcha_ml-0.2.2/src/matcha_ml/cli/ui/emojis.py
+-rw-r--r--   0        0        0     1173 2023-05-16 13:30:52.739975 matcha_ml-0.2.2/src/matcha_ml/cli/ui/print_messages.py
+-rw-r--r--   0        0        0     2549 2023-05-16 13:30:52.740225 matcha_ml-0.2.2/src/matcha_ml/cli/ui/resource_message_builders.py
+-rw-r--r--   0        0        0     1249 2023-05-16 13:30:52.740423 matcha_ml-0.2.2/src/matcha_ml/cli/ui/spinner.py
+-rw-r--r--   0        0        0     1703 2023-05-16 13:30:52.740612 matcha_ml-0.2.2/src/matcha_ml/cli/ui/status_message_builders.py
+-rw-r--r--   0        0        0     1780 2023-05-16 13:30:52.740937 matcha_ml-0.2.2/src/matcha_ml/core/core.py
+-rw-r--r--   0        0        0     2535 2023-05-16 13:30:52.741158 matcha_ml-0.2.2/src/matcha_ml/errors.py
+-rw-r--r--   0        0        0      882 2023-05-16 13:30:52.741464 matcha_ml-0.2.2/src/matcha_ml/infrastructure/.gitignore
+-rw-r--r--   0        0        0     9245 2023-05-16 13:30:52.741780 matcha_ml-0.2.2/src/matcha_ml/infrastructure/.terraform.lock.hcl
+-rw-r--r--   0        0        0     4696 2023-05-16 13:30:52.741981 matcha_ml-0.2.2/src/matcha_ml/infrastructure/README.md
+-rw-r--r--   0        0        0     2213 2023-05-16 13:30:52.742246 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/README.md
+-rw-r--r--   0        0        0      439 2023-05-16 13:30:52.742403 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/main.tf
+-rw-r--r--   0        0        0     1437 2023-05-16 13:30:52.742560 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/output.tf
+-rw-r--r--   0        0        0      386 2023-05-16 13:30:52.742727 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/variables.tf
+-rw-r--r--   0        0        0     1605 2023-05-16 13:30:52.743071 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/README.md
+-rw-r--r--   0        0        0      484 2023-05-16 13:30:52.743315 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/main.tf
+-rw-r--r--   0        0        0      327 2023-05-16 13:30:52.743521 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/output.tf
+-rw-r--r--   0        0        0      462 2023-05-16 13:30:52.743734 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/variables.tf
+-rw-r--r--   0        0        0      625 2023-05-16 13:30:52.743945 matcha_ml-0.2.2/src/matcha_ml/infrastructure/configure_kubectl.tf
+-rw-r--r--   0        0        0      337 2023-05-16 13:30:52.744107 matcha_ml-0.2.2/src/matcha_ml/infrastructure/helm.tf
+-rw-r--r--   0        0        0     1107 2023-05-16 13:30:52.744511 matcha_ml-0.2.2/src/matcha_ml/infrastructure/kubernetes.tf
+-rw-r--r--   0        0        0     1912 2023-05-16 13:30:52.744677 matcha_ml-0.2.2/src/matcha_ml/infrastructure/main.tf
+-rw-r--r--   0        0        0     2208 2023-05-16 13:30:52.744957 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/README.md
+-rw-r--r--   0        0        0      308 2023-05-16 13:30:52.745228 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/getURI.tf
+-rw-r--r--   0        0        0     1314 2023-05-16 13:30:52.745733 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/main.tf
+-rw-r--r--   0        0        0      251 2023-05-16 13:30:52.745977 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/output.tf
+-rw-r--r--   0        0        0      383 2023-05-16 13:30:52.746211 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/providers.tf
+-rw-r--r--   0        0        0      803 2023-05-16 13:30:52.746415 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/variables.tf
+-rw-r--r--   0        0        0       81 2023-05-16 13:30:52.746583 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/zenml_namespace.tf
+-rw-r--r--   0        0        0     1945 2023-05-16 13:30:52.746754 matcha_ml-0.2.2/src/matcha_ml/infrastructure/output.tf
+-rw-r--r--   0        0        0       33 2023-05-16 13:30:52.747081 matcha_ml-0.2.2/src/matcha_ml/infrastructure/printf.cmd
+-rw-r--r--   0        0        0      782 2023-05-16 13:30:52.747345 matcha_ml-0.2.2/src/matcha_ml/infrastructure/providers.tf
+-rw-r--r--   0        0        0      892 2023-05-16 13:30:52.747629 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/README.md
+-rw-r--r--   0        0        0      110 2023-05-16 13:30:52.747966 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/main.tf
+-rw-r--r--   0        0        0      106 2023-05-16 13:30:52.748218 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/output.tf
+-rw-r--r--   0        0        0      224 2023-05-16 13:30:52.748422 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/variables.tf
+-rw-r--r--   0        0        0     3010 2023-05-16 13:30:52.748665 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/README.md
+-rw-r--r--   0        0        0     1894 2023-05-16 13:30:52.748903 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/istio.tf
+-rw-r--r--   0        0        0     1158 2023-05-16 13:30:52.749104 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/main.tf
+-rw-r--r--   0        0        0      663 2023-05-16 13:30:52.749379 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/outputs.tf
+-rw-r--r--   0        0        0      925 2023-05-16 13:30:52.749651 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/permissions.tf
+-rw-r--r--   0        0        0      380 2023-05-16 13:30:52.749843 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/providers.tf
+-rw-r--r--   0        0        0      453 2023-05-16 13:30:52.750059 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/variables.tf
+-rw-r--r--   0        0        0     2914 2023-05-16 13:30:52.750412 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/README.md
+-rw-r--r--   0        0        0      866 2023-05-16 13:30:52.750629 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/main.tf
+-rw-r--r--   0        0        0     1779 2023-05-16 13:30:52.750835 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/output.tf
+-rw-r--r--   0        0        0      124 2023-05-16 13:30:52.751031 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/providers.tf
+-rw-r--r--   0        0        0      454 2023-05-16 13:30:52.751271 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/variables.tf
+-rw-r--r--   0        0        0      754 2023-05-16 13:30:52.751482 matcha_ml-0.2.2/src/matcha_ml/infrastructure/variables.tf
+-rw-r--r--   0        0        0     6080 2023-05-16 13:30:52.751745 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/README.md
+-rw-r--r--   0        0        0      216 2023-05-16 13:30:52.751978 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/getURL.tf
+-rw-r--r--   0        0        0      979 2023-05-16 13:30:52.752167 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/ingress.tf
+-rw-r--r--   0        0        0     3026 2023-05-16 13:30:52.752460 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/main.tf
+-rw-r--r--   0        0        0      704 2023-05-16 13:30:52.752657 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/outputs.tf
+-rw-r--r--   0        0        0      292 2023-05-16 13:30:52.752818 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/providers.tf
+-rw-r--r--   0        0        0     1943 2023-05-16 13:30:52.753089 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/sql.tf
+-rw-r--r--   0        0        0     4701 2023-05-16 13:30:52.753426 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/variables.tf
+-rw-r--r--   0        0        0      342 2023-05-16 13:30:52.753742 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/Chart.yaml
+-rw-r--r--   0        0        0     1987 2023-05-16 13:30:52.754025 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt
+-rw-r--r--   0        0        0     2054 2023-05-16 13:30:52.754318 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1565 2023-05-16 13:30:52.754544 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml
+-rw-r--r--   0        0        0      910 2023-05-16 13:30:52.754804 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml
+-rw-r--r--   0        0        0    10774 2023-05-16 13:30:52.755024 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml
+-rw-r--r--   0        0        0     2225 2023-05-16 13:30:52.755283 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml
+-rw-r--r--   0        0        0     3584 2023-05-16 13:30:52.755448 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml
+-rw-r--r--   0        0        0      367 2023-05-16 13:30:52.755599 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-service.yaml
+-rw-r--r--   0        0        0      316 2023-05-16 13:30:52.755785 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      379 2023-05-16 13:30:52.756101 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0    11587 2023-05-16 13:30:52.756349 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml
+-rw-r--r--   0        0        0     3453 2023-05-16 13:30:52.756631 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/README.md
+-rw-r--r--   0        0        0     1102 2023-05-16 13:30:52.756856 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/main.tf
+-rw-r--r--   0        0        0     1926 2023-05-16 13:30:52.757124 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/output.tf
+-rw-r--r--   0        0        0      468 2023-05-16 13:30:52.757274 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/variables.tf
+-rw-r--r--   0        0        0      103 2023-05-16 13:30:52.757540 matcha_ml-0.2.2/src/matcha_ml/services/__init__.py
+-rw-r--r--   0        0        0     7929 2023-05-16 13:30:52.757814 matcha_ml-0.2.2/src/matcha_ml/services/azure_service.py
+-rw-r--r--   0        0        0     2652 2023-05-16 13:30:52.757983 matcha_ml-0.2.2/src/matcha_ml/services/matcha_state.py
+-rw-r--r--   0        0        0     5503 2023-05-16 13:30:52.758191 matcha_ml-0.2.2/src/matcha_ml/services/terraform_service.py
+-rw-r--r--   0        0        0       41 2023-05-16 13:30:52.758697 matcha_ml-0.2.2/src/matcha_ml/templates/__init__.py
+-rw-r--r--   0        0        0     7396 2023-05-16 13:30:52.759121 matcha_ml-0.2.2/src/matcha_ml/templates/build_templates/azure_template.py
+-rw-r--r--   0        0        0    10509 2023-05-16 13:30:52.759483 matcha_ml-0.2.2/src/matcha_ml/templates/run_template.py
+-rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 matcha_ml-0.2.2/PKG-INFO
```

### Comparing `matcha_ml-0.2.1/LICENSE` & `matcha_ml-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/pyproject.toml` & `matcha_ml-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matcha-ml"
-version = "0.2.1"
+version = "0.2.2"
 description = "Matcha: A open source tool for provisioning MLOps environments to the cloud."
 authors = ["FuzzyLabs <info@fuzzylabs.ai>"]
 license = "Apache-2.0"
 homepage = "http://fuzzylabs.github.io/matcha"
 documentation = "http://fuzzylabs.github.io/matcha"
 repository = "https://github.com/fuzzylabs/matcha"
 readme = "README.md"
@@ -57,16 +57,17 @@
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 mypy = "^1.1.1"
 
 [tool.poetry.group.doc.dependencies]
-mkdocs-material = "^9.1.3"
 mkdocs-glightbox = "^0.3.4"
+pymdown-extensions = "10.0"
+mkdocs-material = "^9.1.12"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 show_error_codes = true
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/cli/_validation.py` & `matcha_ml-0.2.2/src/matcha_ml/cli/_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,17 @@
 
     Raises:
         BadParameter: when the region doesn't exist.
 
     Returns:
         str: the region after checks are passed.
     """
+    if not region:
+        return region
+
     try:
         region_validation(region)
     except MatchaInputError as e:
         raise BadParameter(str(e))
 
     return region
 
@@ -175,14 +178,16 @@
     Raises:
         BadParameter: raised when the prefix doesn't pass the rules.
         BadParameter: raised when the prefix already exists.
 
     Returns:
         str: if valid, the prefix is returned.
     """
+    if not prefix:
+        return prefix
 
     def _to_lowercase(prefix: str) -> str:
         """Convert the prefix to lowercase (a requirement of Azure).
 
         Args:
             prefix (str): the prefix passed to the callback.
 
@@ -207,37 +212,43 @@
 
     return prefix
 
 
 def check_current_deployment_exists() -> bool:
     """Checks the current deployment using the .matcha directory current contents if it exists.
 
+    Specifically, it checks whether the resource group exists on Azure.
+
     Returns:
         bool: True if a deployment currently exists, else False.
     """
     if not os.path.isfile(MATCHA_STATE_DIR):
         return False
 
     with open(MATCHA_STATE_DIR) as f:
         data = json.load(f)
 
-    resource_group_name = data["cloud"]["resource-group-name"]
-
-    client = get_azure_client()
-    rg_state = client.resource_group_state(resource_group_name)
-
-    if rg_state is None:
-        return False
-    elif rg_state == ProvisionState.SUCCEEDED:
-        return True
+    # Check if resource-group-name is present in matcha.state file
+    if "prefix" in data:
+        resource_group_name = data["prefix"] + "-resources"
+
+        client = get_azure_client()
+        rg_state = client.resource_group_state(resource_group_name)
+
+        if rg_state is None:
+            return False
+        elif rg_state == ProvisionState.SUCCEEDED:
+            return True
+        else:
+            print_error(
+                f"Error, resource group '{resource_group_name}' is currently in the state '{rg_state.value}' which is currently not handled by matcha. Please check your resources on Azure."
+            )
+            return True
     else:
-        print_error(
-            f"Error, resource group '{resource_group_name}' is currently in the state '{rg_state.value}' which is currently not handled by matcha. Please check your resources on Azure."
-        )
-        return True
+        return False
 
 
 def get_command_validation(argument: str, valid_options: List[str], noun: str) -> None:
     """Checks if an argument exists within a list of valid options, if it is not valid an exception is raised.
 
     Args:
         argument (str): A string to check
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/cli/cli.py` & `matcha_ml-0.2.2/src/matcha_ml/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,30 +24,25 @@
 
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_show_locals=False)
 
 
 @app.command()
 def provision(
     location: str = typer.Option(
-        None,
-        prompt="What region should your resources be provisioned in (e.g., 'ukwest')?",
         callback=region_typer_callback,
+        default="",
         help="The region where your resources will be provisioned, e.g., 'ukwest'",
     ),
     prefix: str = typer.Option(
-        prompt="Your resources need a name (an alphanumerical prefix; 3-11 character limit), what should matcha call them?",
         callback=prefix_typer_callback,
-        default="matcha",
+        default="",
         help="A unique prefix for your resources.",
     ),
     password: str = typer.Option(
-        default=None,
-        prompt="Set a password for your deployment server",
-        confirmation_prompt=True,
-        hide_input=True,
+        default="",
         help="A password for the deployment server",
     ),
     verbose: Optional[bool] = typer.Option(
         False, help="Get more detailed information from matcha provision!"
     ),
 ) -> None:
     """Provision cloud resources with a template."""
@@ -93,15 +88,15 @@
 
     resource_output = build_resource_output(resources=resources, output_format=output)
     print_resource_output(resource_output=resource_output, output_format=output)
 
 
 @app.command()
 def destroy() -> None:
-    """Destroy the provisioned cloud resources."""
+    """Destroy the provisioned cloud resources. It will destroy the resource group even if resources are provisioned inside the group."""
     destroy_resources()
 
 
 def version_callback(value: bool) -> None:
     """Print version for matcha cli.
 
     Args:
@@ -121,14 +116,14 @@
         None, "--version", callback=version_callback, help="Matcha version."
     ),
 ) -> None:
     """CLI base command for matcha.
 
     Run 'matcha <command> --help' for more information on a specific command.
 
-    For more help on how to use matcha, head to https://docs.mlops.wtf
+    For more help on how to use matcha, head to https://fuzzylabs.github.io/matcha/
     """
     pass
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/cli/destroy.py` & `matcha_ml-0.2.2/src/matcha_ml/cli/destroy.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     if not check_current_deployment_exists():
         print_error(
             "Error - you cannot destroy resources that have not been provisioned yet."
         )
         raise typer.Exit()
 
     if template_runner.is_approved(verb="destroy"):
-
         # deprovision the resources
         template_runner.deprovision()
         print_status(build_step_success_status("Destroying resources is complete!"))
     else:
         print_status(
             build_status(
                 "You decided to cancel - your resources will remain active! If you change your mind, then run 'matcha destroy' again."
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/cli/ui/print_messages.py` & `matcha_ml-0.2.2/src/matcha_ml/cli/ui/print_messages.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/cli/ui/resource_message_builders.py` & `matcha_ml-0.2.2/src/matcha_ml/cli/ui/resource_message_builders.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/cli/ui/spinner.py` & `matcha_ml-0.2.2/src/matcha_ml/cli/ui/spinner.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/cli/ui/status_message_builders.py` & `matcha_ml-0.2.2/src/matcha_ml/cli/ui/status_message_builders.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/core/core.py` & `matcha_ml-0.2.2/src/matcha_ml/core/core.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/errors.py` & `matcha_ml-0.2.2/src/matcha_ml/errors.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/.gitignore` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/.gitignore`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/.terraform.lock.hcl` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/aks/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/aks/output.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/azure_container_registry/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/kubernetes.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/kubernetes.tf`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Derived from ZenML's stack recipes; source: https://github.com/zenml-io/mlops-stacks/blob/8eb06596bf836d3a3dd2634fbc7f2b5687421811/aws-minimal/kubernetes.tf
+
 # check if the host OS is Linux or Windows
 data "external" "os" {
   working_dir = path.module
   program     = ["printf", "{\"os\": \"Linux\"}"]
 }
 
 locals {
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/main.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/main.tf`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 provider "azurerm" {
-  features {}
+  features {
+    resource_group {
+      prevent_deletion_if_contains_resources = false
+    }
+  }
 }
 
 module "resource_group" {
   source = "./resource_group"
 
   prefix   = var.prefix
   location = var.location
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/mlflow_module/variables.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/output.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/providers.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/providers.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/resource_group/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/main.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/main.tf`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Derived from ZenML's stack recipes; source: https://github.com/zenml-io/mlops-stacks/blob/8eb06596bf836d3a3dd2634fbc7f2b5687421811/aws-minimal/seldon/seldon.tf
+
 # creating the namespace for the seldon deployment
 resource "kubernetes_namespace" "seldon_ns" {
   metadata {
     name = var.seldon_namespace
   }
 }
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/seldon/permissions.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/permissions.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/main.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/storage/output.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/variables.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/ingress.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/ingress.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/main.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/main.tf`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Derived from ZenML's stack recipes; source: https://github.com/zenml-io/mlops-stacks/blob/8eb06596bf836d3a3dd2634fbc7f2b5687421811/modules/zenml-module/zen_server.tf
+
 # create the ZenServer deployment
 resource "kubernetes_namespace" "zen_server" {
   metadata {
     name = "${var.prefix}-${var.namespace}"
   }
 }
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/outputs.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/sql.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/sql.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/variables.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zenml_storage/README.md` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zenml_storage/main.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/infrastructure/zenml_storage/output.tf` & `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/services/azure_service.py` & `matcha_ml-0.2.2/src/matcha_ml/services/azure_service.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/services/matcha_state.py` & `matcha_ml-0.2.2/src/matcha_ml/services/matcha_state.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.1/src/matcha_ml/services/terraform_service.py` & `matcha_ml-0.2.2/src/matcha_ml/services/terraform_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,29 @@
         try:
             self.terraform_client.cmd(cmd="-help")
         except Exception:
             return False
 
         return True
 
+    def verify_kubectl_config_file(self, config_path: str = ".kube/config") -> None:
+        """Checks if kubeconfig is present at location ~/.kube/config.
+
+        Args:
+            config_path (str): Relative path to location of kubeconfig
+
+        If not, it creates a empty config file.
+        """
+        kubeconfig_path = os.path.join(os.path.expanduser("~"), config_path)
+
+        if not os.path.exists(kubeconfig_path):
+            os.makedirs(os.path.dirname(kubeconfig_path), exist_ok=True)
+            with open(kubeconfig_path, "a"):
+                pass
+
     def check_matcha_directory_integrity(self) -> bool:
         """Checks the integrity of the .matcha directory.
 
         Args:
             directory_path (str): .matcha directory path
 
         Returns:
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/templates/build_templates/azure_template.py` & `matcha_ml-0.2.2/src/matcha_ml/templates/build_templates/azure_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,16 +171,23 @@
                     )
                 )
 
         if verbose:
             print_status(build_substep_success_status("Configuration was copied"))
 
         configuration_destination = os.path.join(destination, "terraform.tfvars.json")
+        state_file_destination = os.path.join(destination, "matcha.state")
+
+        config_dict = dataclasses.asdict(config)
         with open(configuration_destination, "w") as f:
-            json.dump(dataclasses.asdict(config), f)
+            json.dump(config_dict, f)
+
+        _ = config_dict.pop("password", None)
+        with open(state_file_destination, "w") as f:
+            json.dump(config_dict, f)
 
         if verbose:
             print_status(build_substep_success_status("Template variables were added."))
 
     except PermissionError:
         raise MatchaPermissionError(
             f"Error - You do not have permission to write the configuration. Check if you have write permissions for '{destination}'."
```

### Comparing `matcha_ml-0.2.1/src/matcha_ml/templates/run_template.py` & `matcha_ml-0.2.2/src/matcha_ml/templates/run_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,22 @@
             print_error(
                 "The file terraform.tfvars.json was not found in the "
                 f"current directory at {self.tfs.config.var_file}. Please "
                 "verify if it exists."
             )
             raise typer.Exit()
 
+    def _validate_kubeconfig(self, base_path: str = ".kube/config") -> None:
+        """Check if kubeconfig file exists at location '~/.kube/config', if not create empty config file.
+
+        Args:
+            base_path (str): Relative path to location of kubeconfig
+        """
+        self.tfs.verify_kubectl_config_file(base_path)
+
     def _initialize_terraform(self) -> None:
         """Run terraform init to initialize Terraform .
 
         Raises:
             MatchaTerraformError: if 'terraform init' failed.
         """
         if self.tf_state_dir.exists():
@@ -181,16 +189,27 @@
         for output_name, properties in tf_outputs.items():
             resource_type, flavor, resource_name = self._build_resource_output(
                 output_name
             )
             state_outputs[resource_type].setdefault("flavor", flavor)
             state_outputs[resource_type][resource_name] = properties["value"]
 
+        self._update_state_file(state_outputs)
+
+    def _update_state_file(self, state_outputs: Dict[str, Dict[str, str]]) -> None:
+        """Read and update the matcha state file with new provisioned resources.
+
+        Args:
+            state_outputs (Dict[str, Dict[str, str]]): Dictionary containing outputs to be written to state file.
+        """
+        with open(self.state_file) as fp:
+            out_data = json.load(fp)
+        out_data.update(state_outputs)
         with open(self.state_file, "w") as fp:
-            json.dump(state_outputs, fp, indent=4)
+            json.dump(out_data, fp, indent=4)
 
     def _show_terraform_outputs(self) -> None:
         """Print the terraform outputs from state file."""
         self._write_outputs_state()
         print_status(build_status("Here are the endpoints for what's been provisioned"))
         # print terraform output from state file
         with open(self.state_file) as fp:
@@ -249,14 +268,15 @@
         print_status(summary_message)
         return typer.confirm(f"Are you happy for '{verb}' to run?")
 
     def provision(self) -> None:
         """Provision resources required for the deployment."""
         self._check_terraform_installation()
         self._validate_terraform_config()
+        self._validate_kubeconfig(base_path=".kube/config")
         self._initialize_terraform()
         self._apply_terraform()
         self._show_terraform_outputs()
 
     def deprovision(self) -> None:
         """Destroy the provisioned resources."""
         self._check_matcha_directory_exists()
```

