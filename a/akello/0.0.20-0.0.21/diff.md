# Comparing `tmp/akello-0.0.20.tar.gz` & `tmp/akello-0.0.21.tar.gz`

## Comparing `akello-0.0.20.tar` & `akello-0.0.21.tar`

### file list

```diff
@@ -1,120 +1,136 @@
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 akello-0.0.20/.dockerignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.20/Dockerfile
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 akello-0.0.20/Dockerfile.aws.lambda
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/__init__.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 akello-0.0.20/management.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/module_name.md
--rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.20/openapi.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.20/openapi.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.20/publish_test_pypi.sh
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 akello-0.0.20/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/.gitignore
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/api-server.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/modules.xml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/vcs.xml
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/workspace.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 akello-0.0.20/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 akello-0.0.20/akello/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 akello-0.0.20/akello/app_configs.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 akello-0.0.20/akello/main.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.20/akello/secrets.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.20/akello/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/__init__.py
--rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/registry.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/reports.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 akello-0.0.20/akello/api/app/v1/endpoints/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/provider.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/__init__.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/auth_settings.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 akello-0.0.20/akello/auth/aws_cognito/aws_cognito.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/__init__.py
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/models.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/connector/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/connector/dynamodb.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 akello-0.0.20/akello/db/connector/s3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/decorators/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 akello-0.0.20/akello/decorators/akello_plan_tier.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 akello-0.0.20/akello/decorators/mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/__init__.py
--rw-r--r--   0        0        0  4322416 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/fhir.schema.json
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/hl7/README.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/hl7/__init__.py
--rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.20/akello/fhir/hl7/fhir_v6_models.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/__init__.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/FHIR/phq9_fhir.json
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/FHIR/phq9_response.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/R4/__init__.py
--rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/R4/gad7.R4.json
--rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/R4/phq9.R4.json
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/FHIR_weights.template
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/api_weights.template
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_GAD-7.yaml
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_HEADS-ED.yaml
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_PHQ-9.yaml
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/measurements/survey_PMQ.yaml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/questionnaires/gad7.json
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.20/akello/screeners/questionnaires/phq9.json
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/__init__.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/akello_apps.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/registry.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/reports.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/screeners.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/stripe_payment.py
--rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/user.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_decorators.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_registry_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_reports_service.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_screeners_service.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 akello-0.0.20/akello/services/tests/test_user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/akello/utils/email.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.20/commands/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/commands/__init__.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/__init__.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/patient.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/registry.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/treatment_log.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 akello-0.0.20/commands/mock/user.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 akello-0.0.20/docs/Makefile
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.fhir.rst
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.fhir.v1.endpoints.rst
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.fhir.v1.rst
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.api.rst
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.auth.aws_cognito.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.auth.rst
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.db.connector.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.db.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.decorators.rst
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.fhir.hl7.rst
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.fhir.rst
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.rst
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.screeners.R4.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.screeners.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.services.rst
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.services.tests.rst
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 akello-0.0.20/docs/akello.utils.rst
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 akello-0.0.20/docs/conf.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 akello-0.0.20/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 akello-0.0.20/docs/make.bat
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 akello-0.0.20/docs/modules.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/README.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/generate_data.sh
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/load_fhir_data.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 akello-0.0.20/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 akello-0.0.20/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.20/LICENSE
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 akello-0.0.20/README.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 akello-0.0.20/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 akello-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 akello-0.0.21/.dockerignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.21/Dockerfile
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 akello-0.0.21/Dockerfile.aws.lambda
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/__init__.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 akello-0.0.21/management.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/module_name.md
+-rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.21/openapi.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.21/openapi.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.21/publish_test_pypi.sh
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 akello-0.0.21/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/.gitignore
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/api-server.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/modules.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/vcs.xml
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/workspace.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 akello-0.0.21/akello/app_configs.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 akello-0.0.21/akello/main.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.21/akello/secrets.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.21/akello/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/__init__.py
+-rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/registry.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/reports.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/provider.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/__init__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/auth_settings.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/aws_cognito.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.template.api.env
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.template.env
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/akello.py
+-rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/dev-build-single.sh
+-rwxr-xr-x   0        0        0     2581 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/dev-setup-local.sh
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/docker-compose.yml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.cognito/config.json
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.cognito/db/clients.json
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.cognito/db/local_4yfGDg3h.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/analytics.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/local.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/setup.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/__init__.py
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/models.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/connector/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/connector/dynamodb.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/connector/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/decorators/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 akello-0.0.21/akello/decorators/akello_plan_tier.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 akello-0.0.21/akello/decorators/mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/__init__.py
+-rw-r--r--   0        0        0  4322416 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/fhir.schema.json
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/hl7/README.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/hl7/__init__.py
+-rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/hl7/fhir_v6_models.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/__init__.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/FHIR/phq9_fhir.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/FHIR/phq9_response.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/R4/__init__.py
+-rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/R4/gad7.R4.json
+-rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/R4/phq9.R4.json
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/FHIR_weights.template
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/api_weights.template
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_GAD-7.yaml
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_HEADS-ED.yaml
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_PHQ-9.yaml
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_PMQ.yaml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/questionnaires/gad7.json
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/questionnaires/phq9.json
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/__init__.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/akello_apps.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/registry.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/reports.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/screeners.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/stripe_payment.py
+-rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/user.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_decorators.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_registry_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_reports_service.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_screeners_service.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/utils/email.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.21/commands/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/commands/__init__.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/__init__.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/patient.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/registry.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/treatment_log.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/user.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 akello-0.0.21/docs/Makefile
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.fhir.rst
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.fhir.v1.endpoints.rst
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.fhir.v1.rst
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.rst
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.auth.aws_cognito.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.auth.rst
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.db.connector.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.db.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.decorators.rst
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.fhir.hl7.rst
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.fhir.rst
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.screeners.R4.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.screeners.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.services.rst
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.services.tests.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.utils.rst
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 akello-0.0.21/docs/conf.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 akello-0.0.21/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 akello-0.0.21/docs/make.bat
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 akello-0.0.21/docs/modules.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/README.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/generate_data.sh
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/load_fhir_data.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 akello-0.0.21/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.21/LICENSE
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 akello-0.0.21/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 akello-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 akello-0.0.21/PKG-INFO
```

### Comparing `akello-0.0.20/.dockerignore` & `akello-0.0.21/.dockerignore`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/management.py` & `akello-0.0.21/management.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/openapi.json` & `akello-0.0.21/openapi.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/requirements.txt` & `akello-0.0.21/requirements.txt`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/.idea/api-server.iml` & `akello-0.0.21/.idea/api-server.iml`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/.idea/workspace.xml` & `akello-0.0.21/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/app_configs.yaml` & `akello-0.0.21/akello/app_configs.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/main.py` & `akello-0.0.21/akello/main.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/secrets.py` & `akello-0.0.21/akello/secrets.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/api/app/v1/endpoints/registry.py` & `akello-0.0.21/akello/api/app/v1/endpoints/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/api/app/v1/endpoints/reports.py` & `akello-0.0.21/akello/api/app/v1/endpoints/reports.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/api/app/v1/endpoints/user.py` & `akello-0.0.21/akello/api/app/v1/endpoints/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 from fastapi import APIRouter, Request, Depends, UploadFile
 from akello.auth.provider import auth_token_check
 from akello.auth.aws_cognito.auth_settings import CognitoTokenCustom
 from akello.db.types import UserInvite
 from akello.services.user import UserService
 from akello.services.registry import RegistryService
-from akello.services.reports import ReportsService  
-from akello.db.connector.s3 import S3StorageLocal
-from datetime import datetime, timedelta
+from akello.db.connector.s3 import S3Storage
 import logging
 
 logger = logging.getLogger('mangum')
 router = APIRouter()
 
 
 @router.post("/profile_photo")
-async def update_profile_photo(file: UploadFile, auth: CognitoTokenCustom = Depends(auth_token_check)):    
-    file_path = await S3StorageLocal().set_item(file.filename, file)      
+async def update_profile_photo(file: UploadFile, auth: CognitoTokenCustom = Depends(auth_token_check)):
+    file_path = await S3Storage().set_item(file.filename, file)
     return file_path
 
 
 @router.get("")
-async def get_user(request: Request, auth: CognitoTokenCustom = Depends(auth_token_check)):            
+async def get_user(request: Request, auth: CognitoTokenCustom = Depends(auth_token_check)):
     UserService.save_user_session(auth.cognito_id, request.headers['user-agent'], request.client.host)
     logger.info('calling get_user: email:%s' % auth.username)
-    user = UserService.get_user(auth.cognito_id)    
+    user = UserService.get_user(auth.cognito_id)
     if not user:
         logger.info('registering a new User for the first time - %s ' % auth.username)
         UserService.create_user(auth.cognito_id, auth.username, auth.given_name, auth.family_name, None)
         #raise Exception('User not found')
     else:
         UserService.set_user_active(auth.cognito_id)
-    
-    # TODO: WE SHOULD ONLY DO THIS ONCE ON LOGIN    
-            
+
+    # TODO: WE SHOULD ONLY DO THIS ONCE ON LOGIN
+
     invites = UserInvite.get_invites(auth.username)
     print('invites: %s ' % auth.username)
     print('invites')
-    print(invites)    
+    print(invites)
     for invite in invites:
         logger.info('adding user - %s to registry %s ' % (auth.username, invite['registry_id']))
         UserService.create_registry_user(
             registry_id=invite['registry_id'],
             first_name='Vijay',  #TODO: Remove hardcoded value
             last_name='Selvaraj', #TODO: Remove hardcoded value
             email=invite['email'],
             user_id=auth.cognito_id,
             role=invite['role'],
             is_admin=False
         )
         UserService.create_user_registry(auth.cognito_id, invite['registry_id'])
         RegistryService.update_stats(invite['registry_id'])
-        
+
     return user
 
 
 @router.get("/sessions")
 async def get_user_sessions(auth: CognitoTokenCustom = Depends(auth_token_check)):
     return UserService.get_user_sessions(auth.cognito_id)
```

### Comparing `akello-0.0.20/akello/auth/aws_cognito/README.md` & `akello-0.0.21/akello/auth/aws_cognito/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/auth/aws_cognito/auth_settings.py` & `akello-0.0.21/akello/auth/aws_cognito/auth_settings.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/auth/aws_cognito/aws_cognito.py` & `akello-0.0.21/akello/auth/aws_cognito/aws_cognito.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/db/models.py` & `akello-0.0.21/akello/db/models.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/db/types.py` & `akello-0.0.21/akello/db/types.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/db/connector/dynamodb.py` & `akello-0.0.21/akello/db/connector/dynamodb.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/decorators/akello_plan_tier.py` & `akello-0.0.21/akello/decorators/akello_plan_tier.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/decorators/mixin.py` & `akello-0.0.21/akello/decorators/mixin.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/fhir/fhir.schema.json` & `akello-0.0.21/akello/fhir/fhir.schema.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/fhir/hl7/README.md` & `akello-0.0.21/akello/fhir/hl7/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/fhir/hl7/fhir_v6_models.py` & `akello-0.0.21/akello/fhir/hl7/fhir_v6_models.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/FHIR/phq9_fhir.json` & `akello-0.0.21/akello/screeners/FHIR/phq9_fhir.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/FHIR/phq9_response.json` & `akello-0.0.21/akello/screeners/FHIR/phq9_response.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/R4/gad7.R4.json` & `akello-0.0.21/akello/screeners/R4/gad7.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/R4/phq9.R4.json` & `akello-0.0.21/akello/screeners/R4/phq9.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/measurements/FHIR_weights.template` & `akello-0.0.21/akello/screeners/measurements/FHIR_weights.template`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/measurements/survey_GAD-7.yaml` & `akello-0.0.21/akello/screeners/measurements/survey_GAD-7.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/measurements/survey_HEADS-ED.yaml` & `akello-0.0.21/akello/screeners/measurements/survey_HEADS-ED.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/measurements/survey_PHQ-9.yaml` & `akello-0.0.21/akello/screeners/measurements/survey_PHQ-9.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/measurements/survey_PMQ.yaml` & `akello-0.0.21/akello/screeners/measurements/survey_PMQ.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/questionnaires/gad7.json` & `akello-0.0.21/akello/screeners/questionnaires/gad7.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/screeners/questionnaires/phq9.json` & `akello-0.0.21/akello/screeners/questionnaires/phq9.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/akello_apps.py` & `akello-0.0.21/akello/services/akello_apps.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/registry.py` & `akello-0.0.21/akello/services/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/reports.py` & `akello-0.0.21/akello/services/reports.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/screeners.py` & `akello-0.0.21/akello/services/screeners.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/stripe_payment.py` & `akello-0.0.21/akello/services/stripe_payment.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/user.py` & `akello-0.0.21/akello/services/user.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/tests/__init__.py` & `akello-0.0.21/akello/services/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/tests/test_registry_service.py` & `akello-0.0.21/akello/services/tests/test_registry_service.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/akello/services/tests/test_user_service.py` & `akello-0.0.21/akello/services/tests/test_user_service.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/commands/mock_registry.py` & `akello-0.0.21/commands/mock_registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/commands/mock/patient.py` & `akello-0.0.21/commands/mock/patient.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/commands/mock/registry.py` & `akello-0.0.21/commands/mock/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/commands/mock/treatment_log.py` & `akello-0.0.21/commands/mock/treatment_log.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/Makefile` & `akello-0.0.21/docs/Makefile`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/akello.auth.aws_cognito.rst` & `akello-0.0.21/docs/akello.auth.aws_cognito.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/akello.db.connector.rst` & `akello-0.0.21/docs/akello.db.connector.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/akello.db.rst` & `akello-0.0.21/docs/akello.db.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/akello.rst` & `akello-0.0.21/docs/akello.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/akello.services.rst` & `akello-0.0.21/docs/akello.services.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/akello.services.tests.rst` & `akello-0.0.21/docs/akello.services.tests.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/conf.py` & `akello-0.0.21/docs/conf.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/index.rst` & `akello-0.0.21/docs/index.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/docs/make.bat` & `akello-0.0.21/docs/make.bat`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/synthetic_data/load_fhir_data.py` & `akello-0.0.21/synthetic_data/load_fhir_data.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json` & `akello-0.0.21/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/.gitignore` & `akello-0.0.21/.gitignore`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/LICENSE` & `akello-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `akello-0.0.20/pyproject.toml` & `akello-0.0.21/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "akello"
-version = "0.0.20"
+version = "0.0.21"
 authors = [
   { name="Vijay Selvaraj", email="vijay@akellohealth.com" },
 ]
 description = "FastAPI server akello.io"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -29,13 +29,17 @@
     'mangum',
     'aws_lambda_powertools',
     'stripe',
     'sendgrid',
     'aiofiles',
     'python-multipart',
     'flatten_json',
-    'jsonschema'
+    'jsonschema',
+    'click'
 ]
 
 [project.urls]
 Homepage = "https://akello.io"
-Issues = "https://github.com/akello-io/akello/issues"
+Issues = "https://github.com/akello-io/akello/issues"
+
+[project.scripts]
+akello = "akello.cli.akello:cli()"
```

### Comparing `akello-0.0.20/PKG-INFO` & `akello-0.0.21/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: akello
-Version: 0.0.20
+Version: 0.0.21
 Summary: FastAPI server akello.io
 Project-URL: Homepage, https://akello.io
 Project-URL: Issues, https://github.com/akello-io/akello/issues
 Author-email: Vijay Selvaraj <vijay@akellohealth.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: aiofiles
 Requires-Dist: aws-lambda-powertools
 Requires-Dist: boto3
+Requires-Dist: click
 Requires-Dist: fastapi
 Requires-Dist: fastapi-cognito
 Requires-Dist: flatten-json
 Requires-Dist: jsonschema
 Requires-Dist: mangum
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
```

