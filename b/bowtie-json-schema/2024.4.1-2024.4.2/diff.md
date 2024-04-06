# Comparing `tmp/bowtie_json_schema-2024.4.1.tar.gz` & `tmp/bowtie_json_schema-2024.4.2.tar.gz`

## Comparing `bowtie_json_schema-2024.4.1.tar` & `bowtie_json_schema-2024.4.2.tar`

### file list

```diff
@@ -1,236 +1,236 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.prettierrc.json
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/action.yml
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/noxfile.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/test-requirements.in
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/test-requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.devcontainer/Containerfile
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/__main__.py
--rw-r--r--   0        0        0    43985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_cli.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_containers.py
--rw-r--r--   0        0        0    21220 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_core.py
--rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_report.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/exceptions.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/py.typed
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/Makefile
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/cli.rst
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/github-actions.rst
--rw-r--r--   0        0        0    36245 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/requirements.in
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/index.html
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/package.json
--rw-r--r--   0        0        0   152698 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/conftest.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_github.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_implementation.py
--rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_integration.py
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_report.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/hatch_build.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.prettierrc.json
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/action.yml
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/noxfile.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/test-requirements.in
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/test-requirements.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.devcontainer/Containerfile
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/__main__.py
+-rw-r--r--   0        0        0    44741 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/_cli.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/_commands.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/_containers.py
+-rw-r--r--   0        0        0    21220 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/_core.py
+-rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/_report.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/py.typed
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/Makefile
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/cli.rst
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/github-actions.rst
+-rw-r--r--   0        0        0    36245 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/index.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/requirements.in
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/index.html
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/package.json
+-rw-r--r--   0        0        0   152698 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_cli.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_github.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_implementation.py
+-rw-r--r--   0        0        0    64093 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_integration.py
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_report.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/hatch_build.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.2/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.4.1/.gitpod.yml` & `bowtie_json_schema-2024.4.2/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/.pre-commit-config.yaml` & `bowtie_json_schema-2024.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/CONTRIBUTING.rst` & `bowtie_json_schema-2024.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/action.yml` & `bowtie_json_schema-2024.4.2/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/noxfile.py` & `bowtie_json_schema-2024.4.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/requirements.txt` & `bowtie_json_schema-2024.4.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/test-requirements.txt` & `bowtie_json_schema-2024.4.2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.4.2/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.4.2/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/_cli.py` & `bowtie_json_schema-2024.4.2/bowtie/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         Awaitable,
         Mapping,
         Sequence,
         Set,
     )
     from typing import Any, TextIO
 
+    from click.decorators import FC
     from referencing.jsonschema import Schema, SchemaRegistry, SchemaResource
 
     from bowtie._commands import AnyTestResult, ImplementationId
     from bowtie._core import DialectRunner, ImplementationInfo, MakeValidator
 
 # Windows fallbacks...
 _EX_CONFIG = getattr(os, "EX_CONFIG", 1)
@@ -754,48 +755,44 @@
         ctx: click.Context | None,
     ) -> CaseTransform:
         return lambda cases: (
             case for case in cases if fnmatch(case.description, f"*{value}*")
         )
 
 
+def _set_dialect(ctx: click.Context, _, value: _Dialect):
+    """
+    Set the dialect according to a possibly present :kw:`$schema` keyword.
+    """
+    if value:
+        return value
+    schema = ctx.params.get("schema")
+    dialect_from_schema: str | None = (  # type: ignore[reportUnknownVariableType]
+        schema.get("$schema")  # type: ignore[reportUnknownMemberType]
+        if isinstance(schema, dict)
+        else None
+    )
+    return (
+        Dialect.from_str(dialect_from_schema)  # type: ignore[reportUnknownArgumentType]
+        if dialect_from_schema
+        else max(Dialect.known())
+    )
+
+
 def _set_schema(dialect: Dialect) -> CaseTransform:
     """
     Explicitly set a dialect on schemas passing through by setting ``$schema``.
     """
     return lambda cases: (c.with_explicit_dialect(dialect) for c in cases)
 
 
 def _do_nothing(*args: Any, **kwargs: Any) -> CaseTransform:
     return lambda cases: cases
 
 
-# Both are these are needed because parsing is order dependent :/
-def _disallow_fail_fast(
-    ctx: click.Context,
-    _,
-    value: int | None,
-) -> int | None:
-    if ctx.params.get("fail_fast"):
-        if value is None:
-            return 1
-        raise click.UsageError(
-            "don't provide both --fail-fast and --max-fail / --max-error",
-        )
-    return value
-
-
-def _disallow_max_fail(ctx: click.Context, _, value: int | None) -> int | None:
-    if value and ctx.params.get("max_fail", 1) != 1:
-        raise click.UsageError(
-            "don't provide both --fail-fast and --max-fail / --max-error",
-        )
-    return value
-
-
 IMPLEMENTATION = click.option(
     "--implementation",
     "-i",
     "image_names",
     type=_Image(),
     required=True,
     multiple=True,
@@ -803,15 +800,15 @@
     help="A container image which implements the bowtie IO protocol.",
 )
 DIALECT = click.option(
     "--dialect",
     "-D",
     "dialect",
     type=_Dialect(),
-    default=max(Dialect.known()),
+    callback=_set_dialect,
     show_default=True,
     metavar="URI_OR_NAME",
     help=(
         "A URI or shortname identifying the dialect of each test. Possible "
         f"shortnames include: {', '.join(sorted(Dialect.by_alias()))}."
     ),
 )
@@ -819,36 +816,14 @@
     "--filter",
     "-k",
     default="",
     type=_Filter(),
     metavar="GLOB",
     help="Only run cases whose description match the given glob pattern.",
 )
-FAIL_FAST = click.option(
-    "-x",
-    "--fail-fast",
-    callback=_disallow_max_fail,
-    is_flag=True,
-    default=False,
-    help="Fail immediately after the first error or disagreement.",
-)
-MAX_FAIL = click.option(
-    "--max-fail",
-    metavar="COUNT",
-    type=click.IntRange(min=1),
-    callback=_disallow_fail_fast,
-    help="Fail immediately if x tests fail in total across implementations",
-)
-MAX_ERROR = click.option(
-    "--max-error",
-    metavar="COUNT",
-    type=click.IntRange(min=1),
-    callback=_disallow_fail_fast,
-    help="Fail immediately if x errors occur in total across implementations",
-)
 SET_SCHEMA = click.option(
     "--set-schema",
     "-S",
     "maybe_set_schema",
     # I have no idea why Click makes this so hard, but no combination of:
     #     type, default, is_flag, flag_value, nargs, ...
     # makes this work without doing it manually with callback.
@@ -891,21 +866,71 @@
         "specification. Generally, this option protects against broken Bowtie "
         "implementations and can be left at its default (of off) unless "
         "you are developing a new implementation container."
     ),
 )
 
 
+def fail_fast(fn: FC) -> FC:
+    conflict = "don't provide both --fail-fast and --max-fail / --max-error"
+
+    # Both are these are needed because parsing is order dependent :/
+    def disallow_fail_fast(
+        ctx: click.Context,
+        _,
+        value: int | None,
+    ) -> int | None:
+        if ctx.params.get("fail_fast"):
+            if value is None:
+                return 1
+            raise click.UsageError(conflict)
+        return value
+
+    def disallow_max_fail(
+        ctx: click.Context,
+        _,
+        value: int | None,
+    ) -> int | None:
+        if value and ctx.params.get("max_fail", 1) != 1:
+            raise click.UsageError(conflict)
+        return value
+
+    N = "COUNT"
+    msg = f"Stop running once {N} tests {{}} in total across implementations."
+    return click.option(
+        "-x",
+        "--fail-fast",
+        callback=disallow_max_fail,
+        is_flag=True,
+        default=False,
+        help="Stop running immediately after the first failure or error.",
+    )(
+        click.option(
+            "--max-fail",
+            metavar=N,
+            type=click.IntRange(min=1),
+            callback=disallow_fail_fast,
+            help=msg.format("fail"),
+        )(
+            click.option(
+                "--max-error",
+                metavar=N,
+                type=click.IntRange(min=1),
+                callback=disallow_fail_fast,
+                help=msg.format("error"),
+            )(fn),
+        ),
+    )
+
+
 @subcommand
 @IMPLEMENTATION
 @DIALECT
 @FILTER
-@FAIL_FAST
-@MAX_FAIL
-@MAX_ERROR
+@fail_fast
 @SET_SCHEMA
 @TIMEOUT
 @VALIDATE
 @click.argument(
     "input",
     default="-",
     type=click.File(mode="rb"),
@@ -945,32 +970,36 @@
     default="any",
     type=click.Choice(["valid", "invalid", "any"], case_sensitive=False),
     help=(
         "Expect the given input to be considered valid or invalid, "
         "or else (with 'any') to allow either result."
     ),
 )
-@click.argument("schema", type=click.File(mode="rb"))
+@click.argument(
+    "schema",
+    type=click.File(mode="rb"),
+    callback=lambda _, __, value: json.load(value),  # type: ignore[reportUnknownLambdaType]
+)
 @click.argument("instances", nargs=-1, type=click.File(mode="rb"))
 def validate(
-    schema: TextIO,
+    schema: Any,
     instances: Iterable[TextIO],
     expect: str,
     description: str,
     **kwargs: Any,
 ):
     """
     Validate instances across any implementation.
     """
     if not instances:
         return _EX_NOINPUT
 
     case = TestCase(
         description=description,
-        schema=json.load(schema),
+        schema=schema,
         tests=[
             Test(
                 description="",
                 instance=json.load(instance),
                 valid=dict(valid=True, invalid=False, any=None)[expect],
             )
             for instance in instances
@@ -1222,17 +1251,15 @@
 
     return exit_code
 
 
 @subcommand
 @IMPLEMENTATION
 @FILTER
-@FAIL_FAST
-@MAX_FAIL
-@MAX_ERROR
+@fail_fast
 @SET_SCHEMA
 @TIMEOUT
 @VALIDATE
 @click.argument("input", type=_suite.ClickParam())
 def suite(
     input: tuple[Iterable[TestCase], Dialect, dict[str, Any]],
     filter: CaseTransform,
@@ -1324,24 +1351,21 @@
         )
 
         count = 0
         should_stop = False
         unsucessful = Unsuccessful()
         for count, case in enumerate(maybe_set_schema(dialect)(cases), 1):
             seq_case = SeqCase(seq=count, case=case)
-            case_reporter = reporter.case_started(seq_case)
-
-            if not seq_case.matches_dialect(dialect):
-                case_reporter.mismatched_dialect(expected=dialect)
+            got_result = reporter.case_started(seq_case, dialect)
 
             responses = [seq_case.run(runner=runner) for runner in runners]
 
             for each in asyncio.as_completed(responses):
                 result = await each
-                case_reporter.got_result(result=result)
+                got_result(result=result)
                 unsucessful += result.unsuccessful()
                 if (
                     max_fail
                     and unsucessful.failed >= max_fail
                     or (max_error and unsucessful.errored >= max_error)
                 ):
                     should_stop = True
```

### Comparing `bowtie_json_schema-2024.4.1/bowtie/_commands.py` & `bowtie_json_schema-2024.4.2/bowtie/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,18 @@
         return runner.validate(run, expected=expected)
 
     def serializable(self):
         return dict(seq=self.seq, case=self.case.serializable())
 
     def matches_dialect(self, dialect: _Dialect):
         try:
-            schema = self.case.schema["$schema"]
+            uri = URL.parse(self.case.schema["$schema"])
         except (TypeError, LookupError):
             return True
-        return URL.parse(schema) == dialect.uri
+        return uri == dialect.uri
 
 
 @frozen
 class Started:
     implementation: dict[str, Any]
     version: int = field(
         validator=lambda _, __, got: exceptions.VersionMismatch.check(got),
```

### Comparing `bowtie_json_schema-2024.4.1/bowtie/_containers.py` & `bowtie_json_schema-2024.4.2/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/_core.py` & `bowtie_json_schema-2024.4.2/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/_report.py` & `bowtie_json_schema-2024.4.2/bowtie/_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,38 +86,33 @@
     def ready(self, run_metadata: RunMetadata):
         self._log.debug("Will speak", dialect=run_metadata.dialect)
         self._write(**run_metadata.serializable())
 
     def finished(self, did_fail_fast: bool):
         self._write(did_fail_fast=did_fail_fast)
 
-    def case_started(self, seq_case: SeqCase):
+    def case_started(self, seq_case: SeqCase, dialect: Dialect):
         self._write(**seq_case.serializable())
         log = self._log.bind(
             case=seq_case.case.description,
             schema=seq_case.case.schema,
         )
-        return CaseReporter(write=self._write, log=log)
 
+        if not seq_case.matches_dialect(dialect):
+            log.warning(
+                "$schema keyword does not seem to match the expected dialect",
+                expected=dialect,
+            )
+
+        def got_result(result: SeqResult):
+            bound = log.bind(logger_name=result.implementation)
+            serialized = result.log_and_be_serialized(log=bound)
+            self._write(**serialized)
 
-@frozen
-class CaseReporter:
-    _write: Callable[..., Any] = field(alias="write")
-    _log: structlog.stdlib.BoundLogger = field(alias="log")
-
-    def mismatched_dialect(self, expected: Dialect):
-        self._log.warn(
-            "$schema keyword does not appear to match "
-            f"a {expected.pretty_name} schema.",
-        )
-
-    def got_result(self, result: SeqResult):
-        log = self._log.bind(logger_name=result.implementation)
-        serialized = result.log_and_be_serialized(log=log)
-        self._write(**serialized)
+        return got_result
 
 
 @frozen
 class RunMetadata:
     dialect: Dialect
     implementations: Sequence[ImplementationInfo] = field(
         repr=lambda value: f"({len(value)} implementations)",
```

### Comparing `bowtie_json_schema-2024.4.1/bowtie/_suite.py` & `bowtie_json_schema-2024.4.2/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/exceptions.py` & `bowtie_json_schema-2024.4.2/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/hypothesis.py` & `bowtie_json_schema-2024.4.2/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.4.2/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/data/dialects.json` & `bowtie_json_schema-2024.4.2/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/Makefile` & `bowtie_json_schema-2024.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/cli.rst` & `bowtie_json_schema-2024.4.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/conf.py` & `bowtie_json_schema-2024.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/contributing.rst` & `bowtie_json_schema-2024.4.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/github-actions.rst` & `bowtie_json_schema-2024.4.2/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/implementers.rst` & `bowtie_json_schema-2024.4.2/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/index.rst` & `bowtie_json_schema-2024.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/motd.txt` & `bowtie_json_schema-2024.4.2/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/requirements.txt` & `bowtie_json_schema-2024.4.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/docs/_static/logo.svg` & `bowtie_json_schema-2024.4.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/package.json` & `bowtie_json_schema-2024.4.2/frontend/package.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.4.2/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/tsconfig.json` & `bowtie_json_schema-2024.4.2/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/public/favicon.svg` & `bowtie_json_schema-2024.4.2/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/index.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.4.2/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.4.2/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.4.2/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.4.2/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.4.2/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.4.2/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.4.2/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.4.2/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.4.2/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.4.2/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.4.2/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.4.2/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.4.2/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.4.2/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.4.2/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.4.2/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.4.2/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.4.2/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.4.2/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.4.2/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.4.2/implementations/java-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.4.2/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.4.2/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.4.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.4.2/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.4.2/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.4.2/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.4.2/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files 2% similar despite different names*

```diff
@@ -77,9 +77,8 @@
     ) : TestResult()
 }
 
 @Serializable
 class ErrorContext(
     val message: String? = null,
     val traceback: String? = null,
-    val stderr: String? = null,
 )
```

### Comparing `bowtie_json_schema-2024.4.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.4.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.2/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.4.2/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.4.2/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.4.2/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.4.2/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.4.2/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.4.2/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.4.2/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.4.2/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.4.2/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.4.2/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -384,17 +384,17 @@
 name = "gimli"
 version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
 
 [[package]]
 name = "h2"
-version = "0.3.24"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
```

### Comparing `bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.4.2/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.4.2/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.4.2/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.4.2/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.4.2/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.4.2/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/test_cli.py` & `bowtie_json_schema-2024.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/test_github.py` & `bowtie_json_schema-2024.4.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/test_hypothesis.py` & `bowtie_json_schema-2024.4.2/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/test_integration.py` & `bowtie_json_schema-2024.4.2/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2020,24 +2020,26 @@
 @pytest.mark.asyncio
 async def test_validate_mismatched_dialect(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text(
         '{"$schema": "https://json-schema.org/draft/2020-12/schema"}',
     )
     tmp_path.joinpath("instance.json").write_text("12")
 
-    _, stderr = await bowtie(
+    stdout, stderr = await bowtie(
         "validate",
         "-D",
         "7",
         "-i",
         envsonschema,
         tmp_path / "schema.json",
         tmp_path / "instance.json",
     )
+    dialect = _json.loads(stdout.split("\n")[0])["dialect"]
 
+    assert dialect == "http://json-schema.org/draft-07/schema#"
     assert "$schema keyword does not" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_run_mismatched_dialect(envsonschema, tmp_path):
     async with run("-i", envsonschema, "-D", "2019") as send:
         results, stderr = await send(
@@ -2047,14 +2049,32 @@
         )
 
     assert results == [{tag("envsonschema"): TestResult.INVALID}], stderr
     assert "$schema keyword does not" in stderr, stderr
 
 
 @pytest.mark.asyncio
+async def test_run_mismatched_dialect_total_junk(envsonschema, tmp_path):
+    """
+    A $schema keyword that isn't even a string just gets ignored.
+
+    At this point we're likely testing completely broken schemas.
+    """
+    async with run("-i", envsonschema, "-D", "2019") as send:
+        results, stderr = await send(
+            """
+            {"description": "BOOM", "schema": {"$schema": 37}, "tests": [{"description": "a test", "instance": {}}] }
+            """,  # noqa: E501
+        )
+
+    assert results == [{tag("envsonschema"): TestResult.INVALID}], stderr
+    assert stderr == ""
+
+
+@pytest.mark.asyncio
 async def test_validate_boolean_schema(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text("false")
     tmp_path.joinpath("instance.json").write_text("12")
 
     _, stderr = await bowtie(
         "validate",
         "-i",
@@ -2073,7 +2093,45 @@
             """
             {"description": "wrong dialect", "schema": false, "tests": [{"description": "a test", "instance": {}}] }
             """,  # noqa: E501
         )
 
     assert results == [{tag("envsonschema"): TestResult.INVALID}], stderr
     assert stderr == "", stderr
+
+
+@pytest.mark.asyncio
+async def test_validate_set_dialect_from_schema(envsonschema, tmp_path):
+    tmp_path.joinpath("schema.json").write_text(
+        '{"$schema": "https://json-schema.org/draft/2019-09/schema"}',
+    )
+    tmp_path.joinpath("instance.json").write_text("12")
+
+    stdout, stderr = await bowtie(
+        "validate",
+        "-i",
+        envsonschema,
+        tmp_path / "schema.json",
+        tmp_path / "instance.json",
+    )
+    report = Report.from_serialized(stdout.splitlines())
+    assert report.metadata.dialect == Dialect.by_short_name()["draft2019-09"]
+
+
+@pytest.mark.asyncio
+async def test_validate_specify_dialect(envsonschema, tmp_path):
+    tmp_path.joinpath("schema.json").write_text(
+        "{}",
+    )
+    tmp_path.joinpath("instance.json").write_text("12")
+
+    stdout, stderr = await bowtie(
+        "validate",
+        "-i",
+        envsonschema,
+        "-D",
+        "2019",
+        tmp_path / "schema.json",
+        tmp_path / "instance.json",
+    )
+    report = Report.from_serialized(stdout.splitlines())
+    assert report.metadata.dialect == Dialect.by_short_name()["draft2019-09"]
```

### Comparing `bowtie_json_schema-2024.4.1/tests/test_report.py` & `bowtie_json_schema-2024.4.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/test_schemas.py` & `bowtie_json_schema-2024.4.2/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.4.2/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/.gitignore` & `bowtie_json_schema-2024.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/LICENSE` & `bowtie_json_schema-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/README.rst` & `bowtie_json_schema-2024.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/hatch_build.py` & `bowtie_json_schema-2024.4.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/pyproject.toml` & `bowtie_json_schema-2024.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.1/PKG-INFO` & `bowtie_json_schema-2024.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```

