# Comparing `tmp/sparrow_python-0.1.9.tar.gz` & `tmp/sparrow_python-0.2.0.tar.gz`

## Comparing `sparrow_python-0.1.9.tar` & `sparrow_python-0.2.0.tar`

### file list

```diff
@@ -1,156 +1,159 @@
--rwxr-xr-x   0        0        0      319 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/__init__.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/__main__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/constant.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/core.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/version_ops.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/api/__init__.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/api/common.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/api/fetch.py
--rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/api/static/icon.png
--rw-r--r--   0        0        0  1042008 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/api/static/redoc.standalone.js
--rw-r--r--   0        0        0  1442694 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/api/static/swagger-ui-bundle.js
--rw-r--r--   0        0        0   150947 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/api/static/swagger-ui.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/async_api/__init__.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/async_api/core.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/async_api/example.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/async_api/example2.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/async_api/异步并发执行.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cli/__init__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cli/core.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cli/demo.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cli/downloader.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cli/git.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cli/script.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cli/tree.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/color/__init__.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/color/color.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/color/constant.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cv/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/cv/utils.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/datasets/__init__.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/datasets/fake_data.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/debug/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/decorators/__init__.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/decorators/core.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/distance/__init__.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/distance/distance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/doc/__init__.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/docker/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/docker/nvidia_stat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/espec/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/espec/app.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/espec/date.py
--rw-r--r--   0        0        0    14472 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/espec/especial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/flow/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/flow/executor1/__init__.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/flow/executor1/executor.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/functions/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/functions/bezier.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/functions/core.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/functions/rate_function.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/git/__init__.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/git/monitor.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/inspect/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/inspect/core.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/io/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/io/core.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/io/ops.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/jupyter/__init__.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/jupyter/utils/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/log/__init__.py
--rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/log/core.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/log/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/math/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/math/algebra.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/math/common.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/math/geometry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/math/probability.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/math/sampling/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/models/__init__.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/__init__.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/client.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/config.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/kill_pid.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/mq/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/mq/client.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/multiprocess/mq/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/nlp/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/nlp/ngram.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/nn/__init__.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/nn/activations.py
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/nn/attention.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/nn/losses.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/nn/utils.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/path/__init__.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/path/core.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/performance/__init__.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/performance/_measure_time.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/performance/_record_memory.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/performance/_stat_memory.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/performance/stat.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/performance/torch_cuda_memory.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/progress_bar/__init__.py
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/progress_bar/bar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/__init__.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/build-proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/python/__init__.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/python/coordinate_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/python/coordinate_pb2_grpc.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/python/sparray_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/python/sparray_pb2_grpc.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/python/trainstatus_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/proto/python/trainstatus_pb2_grpc.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/string/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/string/color_string.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/string/ops.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/subtitles/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/table_ops/__init__.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/table_ops/core.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/__init__.py
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/core.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/.dockerignore
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/.gitignore
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/REAMEME.md
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/REAMEME_ZH.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/mainxit.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/pyproject.toml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/pytest.ini
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/start_entrypoint.sh
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/.github/workflows/gh-release.yml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/Examples/debug.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/conf/logging.yaml
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/docker/Dockerfile
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/project_name/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/project_name/__main__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/project_name/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/project_name/api/schemas.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/project_name/api/routes/index.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/template/scaffold/src/tests/conftest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/transform/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/transform/hilbert.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/transform/transform.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/trie/__init__.py
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/trie/trie.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/utils/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/utils/compress.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/utils/core.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/utils/cursor.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/utils/net.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/web/__init__.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/web/share_page.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/sparrow/widgets/__init__.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/LICENSE
--rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/README.md
--rwxr-xr-x   0        0        0     3556 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 sparrow_python-0.1.9/PKG-INFO
+-rwxr-xr-x   0        0        0      319 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/__init__.py
+-rw-r--r--   0        0        0     7611 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/__main__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/constant.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/core.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/version_ops.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/api/__init__.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/api/common.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/api/fetch.py
+-rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/api/static/icon.png
+-rw-r--r--   0        0        0  1042008 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/api/static/redoc.standalone.js
+-rw-r--r--   0        0        0  1442694 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/api/static/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   150947 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/api/static/swagger-ui.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/async_api/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/async_api/core.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/async_api/example.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/async_api/example2.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/async_api/异步并发执行.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cli/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cli/core.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cli/demo.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cli/downloader.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cli/git.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cli/script.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cli/tree.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/color/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/color/color.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/color/constant.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cv/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/cv/utils.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/datasets/__init__.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/datasets/fake_data.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/debug/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/decorators/__init__.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/decorators/core.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/distance/__init__.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/distance/distance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/doc/__init__.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/docker/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/docker/nvidia_stat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/espec/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/espec/app.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/espec/date.py
+-rw-r--r--   0        0        0    14472 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/espec/especial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/extras/__init__.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/extras/packages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/flow/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/flow/executor1/__init__.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/flow/executor1/executor.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/functions/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/functions/bezier.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/functions/core.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/functions/rate_function.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/git/__init__.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/git/monitor.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/inspect/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/inspect/core.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/io/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/io/core.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/io/ops.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/jupyter/__init__.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/jupyter/utils/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/log/__init__.py
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/log/core.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/log/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/math/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/math/algebra.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/math/common.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/math/geometry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/math/probability.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/math/sampling/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/models/__init__.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/__init__.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/client.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/config.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/kill_pid.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/mq/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/mq/client.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/multiprocess/mq/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nlp/__init__.py
+-rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nlp/deduplicate.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nlp/ngram.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nn/__init__.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nn/activations.py
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nn/attention.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nn/losses.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/nn/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/path/__init__.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/path/core.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/performance/__init__.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/performance/_measure_time.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/performance/_record_memory.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/performance/_stat_memory.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/performance/stat.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/performance/torch_cuda_memory.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/progress_bar/__init__.py
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/progress_bar/bar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/__init__.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/build-proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/python/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/python/coordinate_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/python/coordinate_pb2_grpc.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/python/sparray_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/python/sparray_pb2_grpc.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/python/trainstatus_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/proto/python/trainstatus_pb2_grpc.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/string/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/string/color_string.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/string/ops.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/subtitles/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/table_ops/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/table_ops/core.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/__init__.py
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/core.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/.dockerignore
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/.gitignore
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/REAMEME.md
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/REAMEME_ZH.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/mainxit.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/pyproject.toml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/pytest.ini
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/start_entrypoint.sh
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/.github/workflows/gh-release.yml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/Examples/debug.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/conf/logging.yaml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/docker/Dockerfile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/project_name/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/project_name/__main__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/project_name/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/project_name/api/schemas.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/project_name/api/routes/index.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/template/scaffold/src/tests/conftest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/transform/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/transform/hilbert.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/transform/transform.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/trie/__init__.py
+-rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/trie/trie.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/utils/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/utils/compress.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/utils/core.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/utils/cursor.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/utils/net.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/web/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/web/share_page.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/sparrow/widgets/__init__.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/README.md
+-rwxr-xr-x   0        0        0     3620 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 sparrow_python-0.2.0/PKG-INFO
```

### Comparing `sparrow_python-0.1.9/sparrow/__main__.py` & `sparrow_python-0.2.0/sparrow/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,40 @@
 from __future__ import annotations
 
 import os
 import pretty_errors
 import rich
+from typing import Literal
 
 
 class Cli:
     def __init__(self):
         ...
 
+    def deduplicate(self, in_file: str, out_file: str, target_col='data', chunk_size = 200, threshold=None, method:Literal["edit", "rouge", "bleu"]='edit', use_jieba=False):
+        if method == "edit":
+            from .nlp.deduplicate import EditSimilarity
+            simi = EditSimilarity()
+            if threshold is None:
+                threshold = 0.666
+        elif method == "rouge":
+            from .nlp.deduplicate import RougeSimilarity
+            simi = RougeSimilarity(use_jieba=use_jieba)
+            if threshold is None:
+                threshold = 0.5
+        elif method == "bleu":
+            from .nlp.deduplicate import BleuSimilarity
+            simi = BleuSimilarity(use_jieba=use_jieba)
+            if threshold is None:
+                threshold = 0.5
+        else:
+            raise ValueError(f"method should be one of 'edit', 'rouge', 'bleu', but got {method}")
+        simi.load_data(in_file, target_col=target_col)
+        simi.deduplicate(chunk_size=chunk_size, save_to_file=out_file, threshold=threshold)
+
     @staticmethod
     def post(url: str, data: dict, concurrent: int = 10, ):
         import asyncio
         from .api.fetch import run
         asyncio.run(
             run(url=url, data=data, concurrent=concurrent, method="POST")
         )
@@ -29,17 +51,24 @@
 
     @staticmethod
     def timer(dt=0.01):
         from .widgets import timer
         return timer(dt)
 
     @staticmethod
-    def auto_commit(repo_path='.', remote_repo_name: str | None = None):
+    def auto_commit(
+            repo_path='.',
+            remote_repo_name: str | None = None,
+            name="K.Y.Bot", email="beidongjiedeguang@gmail.com",
+            interval=60
+    ):
         from .git.monitor import start_watcher
-        start_watcher(repo_path, remote_repo_name)
+        start_watcher(repo_path=repo_path, remote_repo_name=remote_repo_name,
+                      name=name, email=email,
+                      interval=interval)
 
     @staticmethod
     def install_node(version=16):
         from .cli.script import install_node_with_nvm
         install_node_with_nvm(version=version)
 
     @staticmethod
```

### Comparing `sparrow_python-0.1.9/sparrow/constant.py` & `sparrow_python-0.2.0/sparrow/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/core.py` & `sparrow_python-0.2.0/sparrow/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/version_ops.py` & `sparrow_python-0.2.0/sparrow/version_ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/api/common.py` & `sparrow_python-0.2.0/sparrow/api/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/api/fetch.py` & `sparrow_python-0.2.0/sparrow/api/fetch.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/api/static/icon.png` & `sparrow_python-0.2.0/sparrow/api/static/icon.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/api/static/redoc.standalone.js` & `sparrow_python-0.2.0/sparrow/api/static/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/api/static/swagger-ui-bundle.js` & `sparrow_python-0.2.0/sparrow/api/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/api/static/swagger-ui.css` & `sparrow_python-0.2.0/sparrow/api/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/async_api/core.py` & `sparrow_python-0.2.0/sparrow/async_api/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/async_api/example.py` & `sparrow_python-0.2.0/sparrow/async_api/example.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/async_api/example2.py` & `sparrow_python-0.2.0/sparrow/async_api/example2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/async_api/异步并发执行.py` & `sparrow_python-0.2.0/sparrow/async_api/异步并发执行.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/cli/core.py` & `sparrow_python-0.2.0/sparrow/cli/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/cli/demo.py` & `sparrow_python-0.2.0/sparrow/cli/demo.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/cli/downloader.py` & `sparrow_python-0.2.0/sparrow/cli/downloader.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/cli/git.py` & `sparrow_python-0.2.0/sparrow/cli/git.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/cli/script.py` & `sparrow_python-0.2.0/sparrow/cli/script.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/cli/tree.py` & `sparrow_python-0.2.0/sparrow/cli/tree.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/color/color.py` & `sparrow_python-0.2.0/sparrow/color/color.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/color/constant.py` & `sparrow_python-0.2.0/sparrow/color/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/cv/utils.py` & `sparrow_python-0.2.0/sparrow/cv/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/datasets/fake_data.py` & `sparrow_python-0.2.0/sparrow/datasets/fake_data.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/decorators/core.py` & `sparrow_python-0.2.0/sparrow/decorators/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/distance/distance.py` & `sparrow_python-0.2.0/sparrow/distance/distance.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/docker/__init__.py` & `sparrow_python-0.2.0/sparrow/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/docker/nvidia_stat.py` & `sparrow_python-0.2.0/sparrow/docker/nvidia_stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/espec/date.py` & `sparrow_python-0.2.0/sparrow/espec/date.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/espec/especial.py` & `sparrow_python-0.2.0/sparrow/espec/especial.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/flow/executor1/executor.py` & `sparrow_python-0.2.0/sparrow/flow/executor1/executor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/functions/core.py` & `sparrow_python-0.2.0/sparrow/functions/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/functions/rate_function.py` & `sparrow_python-0.2.0/sparrow/functions/rate_function.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/functions/utils.py` & `sparrow_python-0.2.0/sparrow/functions/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/git/monitor.py` & `sparrow_python-0.2.0/sparrow/git/monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,25 @@
         repo = git.Repo(repo_path)
     except git.InvalidGitRepositoryError:
         repo = git.Repo.init(repo_path)
         print(f"Initialized a new repository at {repo_path}")
     return repo
 
 
-def start_watcher(repo_path='.', remote_repo_name: str | None = None):
+def start_watcher(
+        repo_path='.',
+        remote_repo_name: str | None = None,
+        name="K.Y.Bot", email="beidongjiedeguang@gmail.com",
+        interval=60
+):
     repo = get_repo(repo_path)
 
-    author = git.Actor('K.Y.Bot', 'beidongjiedeguang@gmail.com')
-    branch_name = 'dev'
+    author = git.Actor(name=name, email=email)
+    # use the active branch name
+    branch_name = repo.active_branch.name
 
     # Setup remote
     if 'origin' in [remote.name for remote in repo.remotes]:
         remote = repo.remotes.origin
     else:
         assert remote_repo_name
         remote_url = f'git@guang:KenyonY/{remote_repo_name}.git'
@@ -60,19 +66,20 @@
             repo.create_head(branch_name, commit='HEAD')
 
     repo.heads[branch_name].checkout()
 
     try:
         while True:
             print("Checking for changes...")
-            time.sleep(3 * 60)  # 3 minutes
+            time.sleep(interval)
 
             if repo.is_dirty(untracked_files=True):
                 repo.git.add(A=True)
                 repo.index.commit('Automatic commit', author=author)
+                remote.push(branch_name)
                 print("Committed and pushed changes!")
     except KeyboardInterrupt:
         if repo.is_dirty(untracked_files=True):
             repo.git.add(A=True)
             repo.index.commit('Automatic commit', author=author)
             remote.push(branch_name)
             print("Committed and pushed changes!")
```

### Comparing `sparrow_python-0.1.9/sparrow/inspect/core.py` & `sparrow_python-0.2.0/sparrow/inspect/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/io/__init__.py` & `sparrow_python-0.2.0/sparrow/io/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/io/core.py` & `sparrow_python-0.2.0/sparrow/io/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/io/ops.py` & `sparrow_python-0.2.0/sparrow/io/ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/jupyter/utils/__init__.py` & `sparrow_python-0.2.0/sparrow/jupyter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/log/core.py` & `sparrow_python-0.2.0/sparrow/log/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/log/setup.py` & `sparrow_python-0.2.0/sparrow/log/setup.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/math/common.py` & `sparrow_python-0.2.0/sparrow/math/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/math/geometry.py` & `sparrow_python-0.2.0/sparrow/math/geometry.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/multiprocess/__init__.py` & `sparrow_python-0.2.0/sparrow/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/multiprocess/client.py` & `sparrow_python-0.2.0/sparrow/multiprocess/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/multiprocess/kill_pid.py` & `sparrow_python-0.2.0/sparrow/multiprocess/kill_pid.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/multiprocess/server.py` & `sparrow_python-0.2.0/sparrow/multiprocess/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/multiprocess/mq/client.py` & `sparrow_python-0.2.0/sparrow/multiprocess/mq/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/multiprocess/mq/server.py` & `sparrow_python-0.2.0/sparrow/multiprocess/mq/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/nn/activations.py` & `sparrow_python-0.2.0/sparrow/nn/activations.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/nn/attention.py` & `sparrow_python-0.2.0/sparrow/nn/attention.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/nn/losses.py` & `sparrow_python-0.2.0/sparrow/nn/losses.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/nn/utils.py` & `sparrow_python-0.2.0/sparrow/nn/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/path/core.py` & `sparrow_python-0.2.0/sparrow/path/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/performance/_measure_time.py` & `sparrow_python-0.2.0/sparrow/performance/_measure_time.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/performance/_record_memory.py` & `sparrow_python-0.2.0/sparrow/performance/_record_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/performance/_stat_memory.py` & `sparrow_python-0.2.0/sparrow/performance/_stat_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/performance/stat.py` & `sparrow_python-0.2.0/sparrow/performance/stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/progress_bar/bar.py` & `sparrow_python-0.2.0/sparrow/progress_bar/bar.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/proto/build-proto.py` & `sparrow_python-0.2.0/sparrow/proto/build-proto.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/proto/python/coordinate_pb2.py` & `sparrow_python-0.2.0/sparrow/proto/python/coordinate_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/proto/python/sparray_pb2.py` & `sparrow_python-0.2.0/sparrow/proto/python/sparray_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/proto/python/trainstatus_pb2.py` & `sparrow_python-0.2.0/sparrow/proto/python/trainstatus_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/string/color_string.py` & `sparrow_python-0.2.0/sparrow/string/color_string.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/string/ops.py` & `sparrow_python-0.2.0/sparrow/string/ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/subtitles/__init__.py` & `sparrow_python-0.2.0/sparrow/subtitles/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/table_ops/core.py` & `sparrow_python-0.2.0/sparrow/table_ops/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/core.py` & `sparrow_python-0.2.0/sparrow/template/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/core.py` & `sparrow_python-0.2.0/sparrow/template/scaffold/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/.gitignore` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/.gitignore`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/REAMEME.md` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/REAMEME.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/REAMEME_ZH.md` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/REAMEME_ZH.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/pyproject.toml` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/.github/workflows/gh-release.yml` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/.github/workflows/gh-release.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/.github/workflows/python-publish.yml` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/conf/logging.yaml` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/conf/logging.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/conf/uvicorn.log.yaml` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/conf/uvicorn.log.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/template/scaffold/src/docker/Dockerfile` & `sparrow_python-0.2.0/sparrow/template/scaffold/src/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/transform/transform.py` & `sparrow_python-0.2.0/sparrow/transform/transform.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/trie/trie.py` & `sparrow_python-0.2.0/sparrow/trie/trie.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/utils/compress.py` & `sparrow_python-0.2.0/sparrow/utils/compress.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/utils/core.py` & `sparrow_python-0.2.0/sparrow/utils/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/utils/cursor.py` & `sparrow_python-0.2.0/sparrow/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/utils/net.py` & `sparrow_python-0.2.0/sparrow/utils/net.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/web/share_page.py` & `sparrow_python-0.2.0/sparrow/web/share_page.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/sparrow/widgets/__init__.py` & `sparrow_python-0.2.0/sparrow/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/.gitignore` & `sparrow_python-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/LICENSE` & `sparrow_python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/README.md` & `sparrow_python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.9/pyproject.toml` & `sparrow_python-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,21 @@
 Source = "https://github.com/beidongjiedeguang/sparrow"
 
 [project.optional-dependencies]
 latex = [
     "pix2tex[gui]", # https://github.com/lukas-blecher/LaTeX-OCR/blob/main/setup.py
     "opencv-python-headless<4.3", # 如果已经安装了opencv-python 也可以直接卸载掉headless版本
 ]
+
+nlp = [
+    "levenshtein",
+    "rouge-chinese",
+    "nltk",
+]
+
 cli = [
     "GitPython",
     "twine",
     "asciinema",
     "schedule",
     "docker",
     "paramiko",
```

### Comparing `sparrow_python-0.1.9/PKG-INFO` & `sparrow_python-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sparrow-python
-Version: 0.1.9
+Version: 0.2.0
 Project-URL: homepage, https://github.com/beidongjiedeguang/sparrow
 Project-URL: repository, https://github.com/beidongjiedeguang/sparrow
 Project-URL: documentation, https://github.com/beidongjiedeguang/sparrow#sparrow_tool
 Project-URL: Issues, https://github.com/beidongjiedeguang/sparrow/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/sparrow
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -65,14 +65,18 @@
 Provides-Extra: ml
 Requires-Dist: fastapi>=0.80.0; extra == 'ml'
 Requires-Dist: marisa-trie>=0.7.8; extra == 'ml'
 Requires-Dist: orjson; extra == 'ml'
 Requires-Dist: pysnooper; extra == 'ml'
 Requires-Dist: ray; extra == 'ml'
 Requires-Dist: uvicorn>=0.16.0; extra == 'ml'
+Provides-Extra: nlp
+Requires-Dist: levenshtein; extra == 'nlp'
+Requires-Dist: nltk; extra == 'nlp'
+Requires-Dist: rouge-chinese; extra == 'nlp'
 Provides-Extra: other
 Requires-Dist: aiortc; extra == 'other'
 Requires-Dist: arrayfire; extra == 'other'
 Requires-Dist: awkward; extra == 'other'
 Requires-Dist: cn2an; extra == 'other'
 Requires-Dist: gradio; extra == 'other'
 Requires-Dist: grpcio-reflection~=1.46.3; extra == 'other'
```

