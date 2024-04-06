# Comparing `tmp/scores-0.4.tar.gz` & `tmp/scores-0.5.tar.gz`

## Comparing `scores-0.4.tar` & `scores-0.5.tar`

### file list

```diff
@@ -1,191 +1,115 @@
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 scores-0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 scores-0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scores-0.4/InternalBacklog.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.4/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.4/mkdocs.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scores-0.4/pylintrc
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.4/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.4/setup.cfg
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 scores-0.4/.github/workflows/draft-pdf.yml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 scores-0.4/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.buildinfo
--rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/SECURITY.html
--rw-r--r--   0        0        0    86305 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/api.html
--rw-r--r--   0        0        0    32597 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/contributing.html
--rw-r--r--   0        0        0    20238 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/data.html
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/genindex.html
--rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/index.html
--rw-r--r--   0        0        0    22966 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/installation.html
--rw-r--r--   0        0        0    17471 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/maintainer.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/objects.inv
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/py-modindex.html
--rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/quickstart.html
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/search.html
--rw-r--r--   0        0        0    24485 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/searchindex.js
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/summary_table_of_scores.html
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/SECURITY.doctree
--rw-r--r--   0        0        0   743940 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/api.doctree
--rw-r--r--   0        0        0    38837 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/contributing.doctree
--rw-r--r--   0        0        0    14890 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/data.doctree
--rw-r--r--   0        0        0   546425 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/environment.pickle
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/index.doctree
--rw-r--r--   0        0        0    16953 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/installation.doctree
--rw-r--r--   0        0        0    14678 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/maintainer.doctree
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/quickstart.doctree
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/.doctrees/summary_table_of_scores.doctree
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/SECURITY.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/api.md
--rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/contributing.md
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/data.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/index.md
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/installation.md
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/maintainer.md
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/quickstart.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_sources/summary_table_of_scores.md
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/doctools.js
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/plus.png
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/pygments.css
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/sbt-webpack-macros.html
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/webpack-macros.html
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/images/logo_binder.svg
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/images/logo_colab.png
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/images/logo_deepnote.svg
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/images/logo_jupyterhub.svg
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ar/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/bg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/bn/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ca/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/cs/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/da/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/de/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/el/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/eo/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/es/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/et/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/fi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/fr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/hr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/id/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/it/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/iw/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ja/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ko/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/lt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/lv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ml/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/mr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ms/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/nl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/no/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/pl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/pt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ro/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ru/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ta/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/te/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/tg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/th/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/tl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/tr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/uk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ur/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/vi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   335757 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0        0        0   176654 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/styles/bootstrap.css
--rw-r--r--   0        0        0    63341 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/styles/sphinx-book-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/LICENSE.txt
--rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/css/all.min.css
--rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 scores-0.4/htmldocs/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scores-0.4/src/scores/__init__.py
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 scores-0.4/src/scores/continuous.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 scores-0.4/src/scores/functions.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 scores-0.4/src/scores/sample_data.py
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 scores-0.4/src/scores/utils.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 scores-0.4/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     9503 2020-02-02 00:00:00.000000 scores-0.4/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scores-0.4/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 scores-0.4/src/scores/probability/checks.py
--rw-r--r--   0        0        0    32236 2020-02-02 00:00:00.000000 scores-0.4/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0    15518 2020-02-02 00:00:00.000000 scores-0.4/src/scores/probability/functions.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 scores-0.4/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scores-0.4/src/scores/stats/tests/__init__.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 scores-0.4/src/scores/stats/tests/acovf.py
--rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 scores-0.4/src/scores/stats/tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 scores-0.4/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.4/LICENSE
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 scores-0.4/README.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 scores-0.4/pyproject.toml
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 scores-0.4/PKG-INFO
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 scores-0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.5/environment.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.5/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.5/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.5/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.5/setup.cfg
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 scores-0.5/.github/pull_request_template.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scores-0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 scores-0.5/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 scores-0.5/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.5/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.5/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scores-0.5/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9___init___py.html
+-rw-r--r--   0        0        0   308776 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_cdf_test_data_py.html
+-rw-r--r--   0        0        0   231586 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_crps_test_data_py.html
+-rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_functions_test_data_py.html
+-rw-r--r--   0        0        0    53771 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_roc_test_data_py.html
+-rw-r--r--   0        0        0    45169 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_test_brier_py.html
+-rw-r--r--   0        0        0   157787 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_test_crps_py.html
+-rw-r--r--   0        0        0    65192 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_test_functions_py.html
+-rw-r--r--   0        0        0    50904 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_196c199763c487c9_test_roc_py.html
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_3421a23d4325477f___init___py.html
+-rw-r--r--   0        0        0   114225 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_3421a23d4325477f_flip_flop_impl_py.html
+-rw-r--r--   0        0        0   176515 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_3421a23d4325477f_isoreg_impl_py.html
+-rw-r--r--   0        0        0   176359 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_3421a23d4325477f_isoreg_py.html
+-rw-r--r--   0        0        0    79751 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_3421a23d4325477f_murphy_impl_py.html
+-rw-r--r--   0        0        0    27743 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_3421a23d4325477f_quantile_loss_impl_py.html
+-rw-r--r--   0        0        0    51058 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_3421a23d4325477f_standard_impl_py.html
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_77f509327f4cfccd___init___py.html
+-rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_77f509327f4cfccd_brier_impl_py.html
+-rw-r--r--   0        0        0    18057 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_77f509327f4cfccd_checks_py.html
+-rw-r--r--   0        0        0   212629 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_77f509327f4cfccd_crps_impl_py.html
+-rw-r--r--   0        0        0   105511 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_77f509327f4cfccd_functions_py.html
+-rw-r--r--   0        0        0    38214 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_77f509327f4cfccd_roc_impl_py.html
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_9e03d4585d4ce690___init___py.html
+-rw-r--r--   0        0        0    42739 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_9e03d4585d4ce690_binary_impl_py.html
+-rw-r--r--   0        0        0    63835 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_9e03d4585d4ce690_multicategorical_impl_py.html
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    55964 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_assertions_py.html
+-rw-r--r--   0        0        0    26257 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_test_functions_py.html
+-rw-r--r--   0        0        0   283274 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_test_processing_data_py.html
+-rw-r--r--   0        0        0   161406 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_test_processing_py.html
+-rw-r--r--   0        0        0    18456 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_test_sample_data_py.html
+-rw-r--r--   0        0        0   192800 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_test_utils_py.html
+-rw-r--r--   0        0        0    56187 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_test_weights_py.html
+-rw-r--r--   0        0        0    17230 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a44f0ac069e85531_utils_test_data_py.html
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a837850aa7022bcf___init___py.html
+-rw-r--r--   0        0        0    42497 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a837850aa7022bcf_test_acovf_py.html
+-rw-r--r--   0        0        0   118857 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_a837850aa7022bcf_test_diebold_mariano_py.html
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_b5d7082d1482d9f1___init___py.html
+-rw-r--r--   0        0        0   193979 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_b5d7082d1482d9f1_multicategorical_test_data_py.html
+-rw-r--r--   0        0        0    65796 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_b5d7082d1482d9f1_test_binary_py.html
+-rw-r--r--   0        0        0   114760 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_b5d7082d1482d9f1_test_multicategorical_py.html
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_c9c9b489b8fbf792___init___py.html
+-rw-r--r--   0        0        0    33973 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_c9c9b489b8fbf792_acovf_py.html
+-rw-r--r--   0        0        0   106642 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_c9c9b489b8fbf792_diebold_mariano_impl_py.html
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_e9e7c70ce9e31b19___init___py.html
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58___init___py.html
+-rw-r--r--   0        0        0   127244 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_flip_flop_test_data_py.html
+-rw-r--r--   0        0        0    91063 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_isoreg_test_data_py.html
+-rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_quantile_loss_test_data_py.html
+-rw-r--r--   0        0        0   126014 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_test_flip_flop_py.html
+-rw-r--r--   0        0        0   119047 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_test_isoreg_py.html
+-rw-r--r--   0        0        0   182217 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_test_murphy_py.html
+-rw-r--r--   0        0        0    44829 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_test_quantile_loss_py.html
+-rw-r--r--   0        0        0   204069 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fa972d61f811bd58_test_standard_py.html
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fe94c6366a0da9bc___init___py.html
+-rw-r--r--   0        0        0    21762 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fe94c6366a0da9bc_functions_py.html
+-rw-r--r--   0        0        0    95641 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fe94c6366a0da9bc_processing_py.html
+-rw-r--r--   0        0        0    43505 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fe94c6366a0da9bc_sample_data_py.html
+-rw-r--r--   0        0        0    10098 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fe94c6366a0da9bc_typing_py.html
+-rw-r--r--   0        0        0    95582 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/d_fe94c6366a0da9bc_utils_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0    26225 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0    13704 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 scores-0.5/htmlcov/style.css
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scores-0.5/src/scores/__init__.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scores-0.5/src/scores/functions.py
+-rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 scores-0.5/src/scores/processing.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 scores-0.5/src/scores/sample_data.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 scores-0.5/src/scores/typing.py
+-rw-r--r--   0        0        0    14729 2020-02-02 00:00:00.000000 scores-0.5/src/scores/utils.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 scores-0.5/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 scores-0.5/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 scores-0.5/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 scores-0.5/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 scores-0.5/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    28478 2020-02-02 00:00:00.000000 scores-0.5/src/scores/continuous/isoreg_impl.py
+-rw-r--r--   0        0        0    12424 2020-02-02 00:00:00.000000 scores-0.5/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 scores-0.5/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0     9974 2020-02-02 00:00:00.000000 scores-0.5/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.5/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 scores-0.5/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.5/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.5/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 scores-0.5/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.5/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    36685 2020-02-02 00:00:00.000000 scores-0.5/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0    16016 2020-02-02 00:00:00.000000 scores-0.5/src/scores/probability/functions.py
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 scores-0.5/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.5/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.5/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.5/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 scores-0.5/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 scores-0.5/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.5/LICENSE
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 scores-0.5/README.md
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.5/pyproject.toml
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 scores-0.5/PKG-INFO
```

### Comparing `scores-0.4/.pre-commit-config.yaml` & `scores-0.5/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ---
 repos:
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
     - id: black
+      name: black
+      entry: black --check
 # use local version of package with core deps to avoid import-errors from virtual env
 - repo: local
   hooks:
     - id: pylint
       name: pylint
       entry: pylint --reports=n
       language: system
```

### Comparing `scores-0.4/CODE_OF_CONDUCT.md` & `scores-0.5/CODE_OF_CONDUCT.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 posting via an official social media account, or acting as an appointed
 representative at an online or offline event.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be
 reported to the community leaders responsible for enforcement at
-jive@bom.gov.au.
+scores@bom.gov.au.
 
 All complaints will be reviewed and investigated promptly and fairly.
 
 All community leaders are obligated to respect the privacy and security of the
 reporter of any incident.
 
 ## Enforcement Guidelines
```

### Comparing `scores-0.4/readthedocs.yaml` & `scores-0.5/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.4/src/scores/sample_data.py` & `scores-0.5/src/scores/sample_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         num_lons = 720  # pragma: no cover - used in notebooks and tested manually
         periods = 240  # pragma: no cover - used in notebooks and tested manually
 
     lat = np.linspace(-90, 90, num_lats)
     lon = np.linspace(0, 360, num_lons)
     time_series = pd.date_range(
         start="2022-11-20T01:00:00.000000000",
-        freq="1H",
+        freq="h",
         periods=periods,
     )
 
     np.random.seed(42)
     data = 10 * np.random.rand(len(lat), len(lon), len(time_series))
     obs = xr.DataArray(coords={"lat": lat, "lon": lon, "time": time_series}, data=data)
```

### Comparing `scores-0.4/src/scores/categorical/multicategorical_impl.py` & `scores-0.5/src/scores/categorical/multicategorical_impl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
 This module contains methods which may be used for scoring multicategorical forecasts
 """
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 import xarray as xr
 
-from scores.utils import check_dims, dims_complement, gather_dimensions
 from scores.functions import apply_weights
+from scores.typing import FlexibleDimensionTypes
+from scores.utils import check_dims, gather_dimensions
 
 
-def firm(
+def firm(  # pylint: disable=too-many-arguments
     fcst: xr.DataArray,
     obs: xr.DataArray,
     risk_parameter: float,
     categorical_thresholds: Sequence[float],
     threshold_weights: Sequence[Union[float, xr.DataArray]],
     discount_distance: Optional[float] = 0,
-    reduce_dims: Optional[Sequence[str]] = None,
-    preserve_dims: Optional[Sequence[str]] = None,
-    weights: Optional[xr.DataArray]=None
+    reduce_dims: FlexibleDimensionTypes = None,
+    preserve_dims: FlexibleDimensionTypes = None,
+    weights: Optional[xr.DataArray] = None,
+    threshold_assignment: Optional[str] = "lower",
 ) -> xr.Dataset:
     """
     Calculates the FIxed Risk Multicategorical (FIRM) score including the
     underforecast and overforecast penalties.
 
     `categorical_thresholds` and `threshold_weights` must be the same length.
 
@@ -59,14 +62,17 @@
             shape/dimensionality as the forecast, and the errors will be
             the FIRM score at each point (i.e. single-value comparison
             against observed), and the forecast and observed dimensions
             must match precisely. Only one of `reduce_dims` and `preserve_dims` can be
             supplied. The default behaviour if neither are supplied is to reduce all dims.
         weights: Optionally provide an array for weighted averaging (e.g. by area, by latitude,
             by population, custom)
+        threshold_assignment: Specifies whether the intervals defining the categories are
+            left or right closed. That is whether the decision threshold is included in
+            the upper (left closed) or lower (right closed) category. Defaults to "lower".
 
     Returns:
         An xarray Dataset with data vars:
 
         * firm_score: A score for a single category for each coord based on
           the FIRM framework.
         * overforecast_penalty: Penalty for False Alarms.
@@ -93,53 +99,43 @@
 
     References:
         Taggart, R., Loveday, N. and Griffiths, D., 2022. A scoring framework for tiered
         warnings and multicategorical forecasts based on fixed risk measures. Quarterly
         Journal of the Royal Meteorological Society, 148(744), pp.1389-1406.
     """
     _check_firm_inputs(
-        obs,
-        risk_parameter,
-        categorical_thresholds,
-        threshold_weights,
-        discount_distance,
+        obs, risk_parameter, categorical_thresholds, threshold_weights, discount_distance, threshold_assignment
     )
     total_score = []
     for categorical_threshold, weight in zip(categorical_thresholds, threshold_weights):
         score = weight * _single_category_score(
-            fcst, obs, risk_parameter, categorical_threshold, discount_distance
+            fcst, obs, risk_parameter, categorical_threshold, discount_distance, threshold_assignment
         )
         total_score.append(score)
     summed_score = sum(total_score)
     reduce_dims = gather_dimensions(
-        fcst.dims, obs.dims, reduce_dims, preserve_dims
-    )
+        fcst.dims, obs.dims, reduce_dims=reduce_dims, preserve_dims=preserve_dims
+    )  # type: ignore[assignment]
     summed_score = apply_weights(summed_score, weights)
     score = summed_score.mean(dim=reduce_dims)
 
     return score
 
 
 def _check_firm_inputs(
-    obs,
-    risk_parameter,
-    categorical_thresholds,
-    threshold_weights,
-    discount_distance,
+    obs, risk_parameter, categorical_thresholds, threshold_weights, discount_distance, threshold_assignment
 ):
     """
     Checks that the FIRM inputs are suitable
     """
     if len(categorical_thresholds) < 1:
         raise ValueError("`categorical_thresholds` must have at least one threshold")
 
     if not len(categorical_thresholds) == len(threshold_weights):
-        raise ValueError(
-            "The length of `categorical_thresholds` and `weights` must be equal"
-        )
+        raise ValueError("The length of `categorical_thresholds` and `weights` must be equal")
     if risk_parameter <= 0 or risk_parameter >= 1:
         raise ValueError("0 < `risk_parameter` < 1 must be satisfied")
 
     for count, weight in enumerate(threshold_weights):
         if isinstance(weight, xr.DataArray):
             check_dims(weight, obs.dims, "subset")
             if np.any(weight <= 0):
@@ -147,25 +143,29 @@
                     f"""
                     No values <= 0 are allowed in `weights`. At least one
                     negative value was found in index {count} of `weights`
                     """
                 )
         elif weight <= 0:
             raise ValueError("All values in `weights` must be > 0")
-    if discount_distance is not None:
-        if discount_distance < 0:
-            raise ValueError("`discount_distance` must be >= 0")
+
+    if discount_distance < 0:
+        raise ValueError("`discount_distance` must be >= 0")
+
+    if threshold_assignment not in ["upper", "lower"]:
+        raise ValueError(""" `threshold_assignment` must be either \"upper\" or \"lower\" """)
 
 
 def _single_category_score(
     fcst: xr.DataArray,
     obs: xr.DataArray,
     risk_parameter: float,
     categorical_threshold: float,
-    discount_distance: float,
+    discount_distance: Optional[float] = None,
+    threshold_assignment: Optional[str] = "lower",
 ) -> xr.Dataset:
     """
     Calculates the score for a single category for the `firm` metric at each
     coord. Under-forecast and over-forecast penalties are also calculated
 
     Args:
         fcst: An array of real-valued forecasts.
@@ -176,30 +176,39 @@
         categorical_threshold: Category threshold (theta) to delineate the
             category.
         discount_distance: A discounting distance parameter which must
             be >= 0 such that the cost of misses and false alarms are
             discounted whenever the observation is within distance
             `discount_distance` of the forecast category. A value of 0
             will not a apply any discounting.
+        threshold_assignment: Specifies whether the intervals defining the categories are
+            left or right closed. That is whether the decision threshold is included in
+            the upper (left closed) or lower (right closed) category. Defaults to "lower".
 
     Returns:
         An xarray Dataset with data vars:
 
             * firm_score: a score for a single category for each coord
               based on the FIRM framework. All dimensions are preserved.
             * overforecast_penalty: Penalty for False Alarms.
             * underforecast_penalty: Penalty for Misses.
     """
     # pylint: disable=unbalanced-tuple-unpacking
     fcst, obs = xr.align(fcst, obs)
 
-    # False Alarms
-    condition1 = (obs <= categorical_threshold) & (categorical_threshold < fcst)
-    # Misses
-    condition2 = (fcst <= categorical_threshold) & (categorical_threshold < obs)
+    if threshold_assignment == "lower":
+        # False Alarms
+        condition1 = (obs <= categorical_threshold) & (categorical_threshold < fcst)
+        # Misses
+        condition2 = (fcst <= categorical_threshold) & (categorical_threshold < obs)
+    else:
+        # False Alarms
+        condition1 = (obs < categorical_threshold) & (categorical_threshold <= fcst)
+        # Misses
+        condition2 = (fcst < categorical_threshold) & (categorical_threshold <= obs)
 
     # Bring back NaNs
     condition1 = condition1.where(~np.isnan(fcst))
     condition1 = condition1.where(~np.isnan(obs))
     condition2 = condition2.where(~np.isnan(fcst))
     condition2 = condition2.where(~np.isnan(obs))
```

### Comparing `scores-0.4/src/scores/probability/checks.py` & `scores-0.5/src/scores/probability/checks.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     Args:
         cdf (xr.DataArray): array of CDF values
 
     Returns:
         (bool): `True` if `cdf` values are all between 0 and 1 whenever values are not NaN,
             or if all values are NaN; and `False` otherwise.
     """
-    return cdf.count() == 0 or ((cdf.min() >= 0) & (cdf.max() <= 1))
+    flag = cdf.count() == 0 or ((cdf.min() >= 0) & (cdf.max() <= 1))
+    return flag  # type: ignore  # mypy thinks flag could be a DataArray
 
 
 def check_nan_decreasing_inputs(cdf, threshold_dim, tolerance):
     """Checks inputs to `nan_decreasing_cdfs` and `_decreasing_cdfs`."""
 
     if threshold_dim not in cdf.dims:
         raise ValueError(f"'{threshold_dim}' is not a dimension of `cdf`")
```

### Comparing `scores-0.4/src/scores/probability/crps_impl.py` & `scores-0.5/src/scores/probability/crps_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module supports the implementation of the CRPS scoring function, drawing from additional functions.
-The primary method, `crps_cdf` is imported into the probability module to be part of the probability API
+The two primary methods, `crps_cdf` and `crps_for_ensemble` are imported into 
+the probability module to be part of the probability API.
 """
-
-from typing import Iterable, Literal, Optional
+from collections.abc import Iterable
+from typing import Literal, Optional, Sequence
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 import scores.utils
 from scores.probability.checks import coords_increasing
@@ -152,15 +153,15 @@
     threshold_weight_fill_method: Literal["linear", "step", "forward", "backward"] = "forward",
     integration_method: Literal["exact", "trapz"] = "exact",
     reduce_dims: Optional[Iterable[str]] = None,
     preserve_dims: Optional[Iterable[str]] = None,
     weights=None,
     include_components=False,
 ):
-    """Calculates CRPS CDF probabilistic metric.
+    """Calculates the CRPS probabilistic metric given CDF input.
 
     Calculates the continuous ranked probability score (CRPS), or the mean CRPS over
     specified dimensions, given forecasts in the form of predictive cumulative
     distribution functions (CDFs). Can also calculate threshold-weighted versions of the
     CRPS by supplying a `threshold_weight`.
 
     Predictive CDFs here are described by an indexed set of values rather than by
@@ -245,15 +246,16 @@
             "linear" is probably the best choice. If it is an increasing step function,
             "forward" may be best.
         integration_method (str): one of "exact" or "trapz".
         preserve_dims (Tuple[str]): dimensions to preserve in the output. All other dimensions are collapsed
             by taking the mean.
         reduce_dims (Tuple[str]): dimensions to reduce in the output by taking the mean. All other dimensions are
             preserved.
-        weights: Not yet implemented. Allow weighted averaging (e.g. by area, by latitude, by population, custom)
+        weights: Optionally provide an array for weighted averaging (e.g. by area, by latitude,
+            by population, custom)
         include_components (bool): if True, include the under and over forecast components of
             the score in the returned dataset.
 
     Returns:
         xr.Dataset: The following are the produced Dataset variables:
             - "total" the total CRPS.
             - "underforecast_penalty": the under-forecast penalty contribution of the CRPS.
@@ -275,15 +277,16 @@
         ValueError: if `fcst[threshold_dim]` has less than 2 values.
         ValueError: if coordinates in `fcst[threshold_dim]` are not increasing.
         ValueError: if `threshold_weight` is not `None` and coordinates in
             `threshold_weight[threshold_dim]` are not increasing.
         ValueError: if `threshold_weight` has negative values.
 
     See also:
-        `scores.probability.crps_cdf_brier_decomposition`
+        - `scores.probability.crps_cdf_brier_decomposition`
+        - `scores.probability.crps_for_ensemble`
 
     References:
         - Matheson, J. E., and R. L. Winkler, 1976: Scoring rules for continuous probability distributions.
             Manage. Sci.,22, 1087–1095.
         - Gneiting, T., & Ranjan, R. (2011). Comparing Density Forecasts Using Threshold- and
             Quantile-Weighted Scoring Rules.
             Journal of Business & Economic Statistics, 29(3), 411–422. http://www.jstor.org/stable/23243806
@@ -338,15 +341,15 @@
             threshold_weight,
             threshold_dim,
             include_components=include_components,
         )
 
     weighted = scores.functions.apply_weights(result, weights)
 
-    dims.remove(threshold_dim)
+    dims.remove(threshold_dim)  # type: ignore
 
     result = weighted.mean(dim=dims)
 
     return result
 
 
 def crps_cdf_exact(
@@ -495,15 +498,15 @@
         threshold_dim,
         None,
         additional_thresholds,
         fcst_fill_method,
         "forward",
     )
 
-    dims.remove(threshold_dim)
+    dims.remove(threshold_dim)  # type: ignore
 
     # brier score for each forecast case
     bscore = (fcst - obs) ** 2
     not_nan = ~np.isnan(bscore)
 
     # `obs` here is the empirical CDF of the observation
     # when `obs == 1` the observation was lower than the threshold considered
@@ -730,7 +733,102 @@
         precision=steppoint_precision,
     )
 
     if not weight_upper:
         weight = 1 - weight
 
     return weight
+
+
+def crps_for_ensemble(
+    fcst: xr.DataArray,
+    obs: xr.DataArray,
+    ensemble_member_dim: str,
+    method: Literal["ecdf", "fair"] = "ecdf",
+    reduce_dims: Optional[Sequence[str]] = None,
+    preserve_dims: Optional[Sequence[str]] = None,
+    weights: xr.DataArray = None,
+) -> xr.DataArray:
+    """Calculates the CRPS probabilistic metric given ensemble input.
+
+    Calculates the continuous ranked probability score (CRPS) given an ensemble of forecasts.
+    An ensemble of forecasts can also be thought of as a random sample from the predictive
+    distribution.
+
+    Given an observation y, and ensemble member values {x_i} (for 1 <= i <= M), the CRPS is
+    calculated by the formula
+        CRPS({x_i}, y) = (1 / M) * sum(|x_i - y|) - (1 / 2 * K) * sum(|x_i - x_j|),
+    where the first sum is iterated over 1 <= i <= M and the second sum is iterated over
+    1 <= i <= M and 1 <= j <= M.
+
+    The value of the constant K in this formula depends on the method.
+        - If `method="ecdf"` then K = M ** 2. In this case the CRPS value returned is
+            the exact CRPS value for the emprical cumulation distribution function
+            constructed using the ensemble values.
+        - If `method="fair"` then K = M * (M - 1). In this case the CRPS value returned
+            is the approximated CRPS where the ensemble values can be interpreted as a
+            random sample from the underlying predictive distribution. This interpretation
+            stems from the formula CRPS(F, Y) = E|X - Y| - E|X - X'|/2, where X and X'
+            are independent samples of the predictive distribution F, Y is the observation
+            (possibly unknown) and E denotes the expectation. This choice of K gives an
+            unbiased estimate for the second expectation.
+
+    Args:
+        fcst: Forecast data. Must have a dimension `ensemble_member_dim`.
+        obs: Observation data.
+        ensemble_member_dim: the dimension that specifies the ensemble member or the sample
+            from the predictive distribution.
+        method: Either "ecdf" or "fair".
+        reduce_dims: Dimensions to reduce. Can be "all" to reduce all dimensions.
+        preserve_dims: Dimensions to preserve. Can be "all" to preserve all dimensions.
+        weights: Weights for calculating a weighted mean of individual scores.
+
+    Returns:
+        xarray object of (weighted mean) CRPS values.
+
+    Raises:
+        ValueError: when method is not one of "ecdf" or "fair".
+
+    See also:
+        `scores.probability.crps_cdf`
+
+    References:
+        - C. Ferro (2014), "Fair scores for ensemble forecasts", Q J R Meteorol Soc
+            140(683):1917-1923.
+        - T. Gneiting T and A. Raftery (2007), "Strictly proper scoring rules, prediction,
+            and estimation", J Am Stat Assoc, 102(477):359-37.
+        - M. Zamo and P. Naveau (2018), "Estimation of the Continuous Ranked Probability
+            Score with Limited Information and Applications to Ensemble Weather Forecasts",
+            Math Geosci 50:209-234, https://doi.org/10.1007/s11004-017-9709-7
+    """
+    if method not in ["ecdf", "fair"]:
+        raise ValueError("`method` must be one of 'ecdf' or 'fair'")
+
+    dims_for_mean = scores.utils.gather_dimensions2(
+        fcst,
+        obs,
+        weights=weights,
+        reduce_dims=reduce_dims,
+        preserve_dims=preserve_dims,
+        special_fcst_dims=ensemble_member_dim,
+    )
+
+    ensemble_member_dim1 = scores.utils.tmp_coord_name(fcst)
+
+    # calculate forecast spread contribution
+    fcst_copy = fcst.rename({ensemble_member_dim: ensemble_member_dim1})
+
+    fcst_spread_term = np.abs(fcst - fcst_copy).sum([ensemble_member_dim, ensemble_member_dim1])
+    ens_count = fcst.count(ensemble_member_dim)
+    if method == "ecdf":
+        fcst_spread_term = fcst_spread_term / (2 * ens_count**2)
+    if method == "fair":
+        fcst_spread_term = fcst_spread_term / (2 * ens_count * (ens_count - 1))
+
+    # calculate final CRPS for each forecast case
+    fcst_obs_term = np.abs(fcst - obs).mean(ensemble_member_dim)
+    result = fcst_obs_term - fcst_spread_term
+
+    # apply weights and take means across specified dims
+    result = scores.functions.apply_weights(result, weights).mean(dim=dims_for_mean)
+
+    return result
```

### Comparing `scores-0.4/src/scores/probability/functions.py` & `scores-0.5/src/scores/probability/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """
 This module contains a variety of functions which modify data in various ways to process data structures
 to support probablistic verification.
 """
-
-from typing import Iterable, Literal, Optional
+from collections.abc import Iterable
+from typing import Literal, Optional
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from scores.probability.checks import (
     cdf_values_within_bounds,
     check_nan_decreasing_inputs,
 )
+from scores.typing import XarrayLike
 
 
 def round_values(array: xr.DataArray, rounding_precision: float, final_round_decpl: int = 7) -> xr.DataArray:
     """Round data array to specified precision.
 
+    Rounding is done differently to `xarray.DataArray.round` or `numpy.round` where
+    the number of decimal places is specified in those cases. Instead, here the rounding
+    precision is specified as a float. The value is rounded to the nearest value that is
+    divisible by `rounding_precision`.
+
+    For example, 3.73 rounded to precision 0.2 is 3.8, and 37.3 rounded to precision 20
+    is 40.
+
     Assumes that rounding_precision >=0, with 0 indicating no rounding to be performed.
-    For example, 3.73 rounded to precision 0.2 is 3.8.
     If rounding_precision > 0, a final round to `final_round_decpl` decimal places is performed
     to remove artefacts of python rounding process.
 
     Args:
         array (xr.DataArray): array of data to be rounded
         rounding_precision (float): rounding precision
         final_round_decpl (int): final round to specified number of decimal
@@ -41,15 +49,15 @@
     if rounding_precision > 0:
         array = (array / rounding_precision).round() * rounding_precision
         array = array.round(decimals=final_round_decpl)
 
     return array
 
 
-def propagate_nan(cdf: xr.DataArray, threshold_dim: str) -> xr.DataArray:
+def propagate_nan(cdf: XarrayLike, threshold_dim: str) -> XarrayLike:
     """Propagates the NaN values from a "cdf" variable along the `threshold_dim`.
 
     Args:
         cdf (xr.DataArray): CDF values, so that P(X <= threshold) = cdf_value for
             each threshold in the `threshold_dim` dimension.
         threshold_dim (str): name of the threshold dimension in `cdf`.
 
@@ -58,15 +66,15 @@
 
     Raises:
         ValueError: If `threshold_dim` is not a dimension of `cdf`.
     """
     if threshold_dim not in cdf.dims:
         raise ValueError(f"'{threshold_dim}' is not a dimension of `cdf`")
 
-    where_nan = np.isnan(cdf).any(dim=threshold_dim)
+    where_nan = xr.DataArray(np.isnan(cdf)).any(dim=threshold_dim)
     result = cdf.where(~where_nan, np.nan)
     return result
 
 
 def observed_cdf(
     obs: xr.DataArray,
     threshold_dim: str,
@@ -95,21 +103,23 @@
         ValueError: if `precision < 0`.
         ValueError: if all observations are NaN and no non-NaN `threshold_values`
             are not supplied.
     """
     if precision < 0:
         raise ValueError("`precision` must be nonnegative.")
 
-    if np.isnan(obs).all() and (threshold_values is None or np.isnan(threshold_values).all()):
+    threshold_values_as_array = np.array(threshold_values)
+
+    if np.isnan(obs).all() and (threshold_values is None or np.isnan(threshold_values_as_array).all()):
         raise ValueError("must include non-NaN observations in thresholds or supply threshold values")
 
     if precision > 0:
         obs = round_values(obs, precision)
 
-    thresholds = threshold_values if threshold_values is not None else []
+    thresholds = threshold_values_as_array if threshold_values is not None else []
 
     if include_obs_in_thresholds:
         thresholds = np.concatenate((obs.values.flatten(), thresholds))
 
     # remove any NaN
     thresholds = [x for x in thresholds if not np.isnan(x)]
```

### Comparing `scores-0.4/src/scores/stats/tests/acovf.py` & `scores-0.5/src/scores/stats/statistical_tests/acovf.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
 OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
 DAMAGE.
 """
 
 import numpy as np
 
+# pylint: skip-file
+
 __all__ = ["acovf"]
 
 
 def _next_regular(target):
     """
     Find the next regular number greater than or equal to target.
     Regular numbers are composites of the prime factors 2, 3, and 5.
```

### Comparing `scores-0.4/src/scores/stats/tests/diebold_mariano_impl.py` & `scores-0.5/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from typing import Literal
 
 import numpy as np
 import scipy as sp
 import xarray as xr
 from scipy.optimize import least_squares
 
+from scores.stats.statistical_tests.acovf import acovf
 from scores.utils import dims_complement
 
 
-def diebold_mariano(
+def diebold_mariano(  # pylint: disable=R0914
     da_timeseries: xr.DataArray,
     ts_dim: str,
     h_coord: str,
     method: Literal["HG", "HLN"] = "HG",
     confidence_level: float = 0.95,
     statistic_distribution: Literal["normal", "t"] = "normal",
 ) -> xr.Dataset:
@@ -51,14 +52,17 @@
     Confidence intervals and "confidence_gt_0" statistics are calculated using the
     test statistic, which is assumed to have either the standard normal distribution
     or Student's t distribution with n - 1 degrees of freedom (where n is the length of
     the timeseries). The distribution used is specified by `statistic_distribution`. See
     Harvey, Leybourne and Newbold (1997) for why the t distribution may be preferred,
     especially for shorter timeseries.
 
+    If `da_timeseries` is a chunked array, data will be brought into memory during
+    this calculation due to the autocovariance implementation.
+
     Args:
         da_timeseries: a 2 dimensional array containing the timeseries.
         ts_dim: name of the dimension which identifies each timeseries in the array.
         h_coord: name of the coordinate specifying, for each timeseries, that the
             timeseries is an h-step ahead forecast. `h_coord` coordinates must be
             indexed by the dimension `ts_dim`.
         method: method for calculating the test statistic, one of "HG" or "HLN".
@@ -174,22 +178,22 @@
         pvals = sp.stats.norm.cdf(test_stats)
         ci_quantile = sp.stats.norm.ppf(1 - (1 - confidence_level) / 2)
     else:
         pvals = sp.stats.t.cdf(test_stats, da_timeseries_len.values - 1)
         ci_quantile = sp.stats.t.ppf(1 - (1 - confidence_level) / 2, da_timeseries_len.values - 1)
 
     result = xr.Dataset(
-        data_vars=dict(
-            mean=([ts_dim], ts_mean),
-            dm_test_stat=([ts_dim], test_stats),
-            timeseries_len=([ts_dim], da_timeseries_len.values),
-            confidence_gt_0=([ts_dim], pvals),
-            ci_upper=([ts_dim], ts_mean * (1 + ci_quantile / test_stats)),
-            ci_lower=([ts_dim], ts_mean * (1 - ci_quantile / test_stats)),
-        ),
+        data_vars={
+            "mean": ([ts_dim], ts_mean),
+            "dm_test_stat": ([ts_dim], test_stats),
+            "timeseries_len": ([ts_dim], da_timeseries_len.values),
+            "confidence_gt_0": ([ts_dim], pvals),
+            "ci_upper": ([ts_dim], ts_mean * (1 + ci_quantile / test_stats)),
+            "ci_lower": ([ts_dim], ts_mean * (1 - ci_quantile / test_stats)),
+        },
         coords={ts_dim: da_timeseries[ts_dim].values},
     )
 
     return result
 
 
 def _dm_test_statistic(diffs: np.ndarray, h: int, method: Literal["HG", "HLN"] = "HG") -> float:
@@ -262,15 +266,15 @@
     if len(nonzero_diffs) == 0:
         test_stat = np.nan
     elif method == "HLN":
         test_stat = _hln_method_stat(diffs, h)
     else:  # method == 'HG'
         test_stat = _hg_method_stat(diffs, h)
 
-    return test_stat
+    return test_stat  # type: ignore
 
 
 def _hg_func(pars: list, lag: np.ndarray, acv: np.ndarray) -> np.ndarray:
     """
     Function whose values are to be minimised as part of the HG method for estimating
     the spectral density at 0.
 
@@ -285,15 +289,15 @@
     Returns:
         Difference between modelled and empirical autocoveriances.
 
     References:
         Hering and Genton, 'Comparing spatial predictions',
         Technometrics 53 no. 4 (2011), 414-425.
     """
-    return (pars[0] ** 2) * np.exp(-3 * lag / pars[1]) - acv
+    return (pars[0] ** 2) * np.exp(-3 * lag / pars[1]) - acv  # ignore: type
 
 
 def _hg_method_stat(diffs: np.ndarray, h: int) -> float:
     """
     Calculates the modified Diebold-Mariano test statistic using the "HG" method.
     Assumes that h < len(diffs).
 
@@ -301,15 +305,14 @@
         diffs: a single (1D array) timeseries of score differences with NaNs removed.
         h: integer indicating that forecasts are h-step ahead, assumed to be positive
             and less than the length of the timeseries with NaNs removed.
 
     Returns:
         Diebold-Mariano test statistic using the HG method.
     """
-    from scores.stats.tests.acovf import acovf
 
     n = len(diffs)
 
     # use an exponential model for autocovariances of `diffs`
     max_lag = int(max(np.floor((n - 1) / 2), h))
     sample_autocvs = acovf(diffs)[0:max_lag]
     sample_lags = np.arange(max_lag)
@@ -317,15 +320,15 @@
 
     # use the model autocovariances to estimate spectral density at 0
     all_lags = np.arange(n)
     model_autocovs = (model_params[0] ** 2) * np.exp(-3 * all_lags / model_params[1])
     density_estimate = model_autocovs[0] + 2 * np.sum(model_autocovs[1:])
     test_stat = np.mean(diffs) / np.sqrt(density_estimate / n)
 
-    return test_stat
+    return test_stat  # type: ignore
 
 
 def _hln_method_stat(diffs: np.ndarray, h: int) -> float:
     """
     Given a timeseries of score differences for h-step ahead forecasts, as a 1D numpy
     array without NaNs, returns the modified Diebold-Mariano test statistic of
     Harvey et al (1997).
@@ -346,15 +349,15 @@
     # Harvey (1997) Equation (3)
     test_stat = diffs_bar / _dm_v_hat(diffs, diffs_bar, n, h) ** 0.5
 
     # Harvey (1997) Equation (9)
     correction_factor = (n + 1 - 2 * h + h * (h - 1) / n) / n
     test_stat = (correction_factor**0.5) * test_stat
 
-    return test_stat
+    return test_stat  # type: ignore
 
 
 def _dm_gamma_hat_k(diffs: np.ndarray, diffs_bar: float, n: int, k: int) -> float:
     """
     Computes the quantity (n - k) * gamma_hat_star_k of Equation (5) in
     Harvey et al (1997).
 
@@ -365,15 +368,15 @@
         k: integer between 1 and n-1 (inclusive), where n = len(diffs)
 
     Returns:
         The quantity (n - k) * gamma_hat_star_k.
     """
     prod = (diffs[k:n] - diffs_bar) * (diffs[0 : n - k] - diffs_bar)
 
-    return np.sum(prod)
+    return np.sum(prod)  # type: ignore
 
 
 def _dm_v_hat(diffs: np.ndarray, diffs_bar: float, n: int, h: int) -> float:
     """
     Computes the the quantity V_hat(d_bar) of Equation (5) in Harvey et al (1997).
 
     Args:
@@ -390,8 +393,8 @@
         summands[k] = _dm_gamma_hat_k(diffs, diffs_bar, n, k + 1)
 
     result = (_dm_gamma_hat_k(diffs, diffs_bar, n, 0) + 2 * np.sum(summands)) / n**2
 
     if result <= 0:
         result = np.nan
 
-    return result
+    return result  # type: ignore
```

### Comparing `scores-0.4/LICENSE` & `scores-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.4/README.md` & `scores-0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # About the Scores Project
 
 One-line intro: xarray based verification (accuracy) scoring that can scale with Dask if needed. Pandas supported where possible.
 Why use it: trusted implementations, novel metrics, performance, one-stop-shop.
 
-Currently Included Metrics:
-
-| continuous | probability | categorical | statistical tests      |
-| ---------- | ----------- | ----------- | ----------- |
-| MAE, MSE, RMSE | CRPS | FIRM |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
+Currently Included Metrics and Tools:
 
+| continuous                      | probability | categorical      | statistical tests |
+| ----------                      | ----------- | -----------      | ----------------- |
+| MAE, MSE, RMSE, Flip Flop Index, Quantile Score, Isotonic Regression, Pearsons correlation coefficient  | CRPS for CDF, CRPS for ensemble, ROC, Brier score   | FIRM, POD, POFD  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
 
 **Notice -- This repository is currently undergoing initial construction and maintenance. It is not yet recommended for use. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io)
 
-`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of model outputs and predictions. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather. 
+`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of model outputs and predictions. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
 
 `scores` includes novel scores not commonly found elsewhere (e.g. FIRM, FlipFlop Index), complex scores (e.g. CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
 `scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to utilise Dask for scaling and performance.
 
 All of the scores and metrics in this package have undergone a thorough statistical and scientific review. Every score has a companion Jupyter Notebook tutorial demonstrating its use in practice.
 
 All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40, 000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
-The [installation guide](docs/installation.md) contains information on the various ways of installing, using and working with this package. 
+The [installation guide](docs/installation.md) contains information on the various ways of installing, using and working with this package.
 
 Installation of the core mathematical API may be performed with:
 
 ```py
 > pip install scores
 ```
```

### Comparing `scores-0.4/PKG-INFO` & `scores-0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 Metadata-Version: 2.1
 Name: scores
-Version: 0.4
+Version: 0.5
 Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of model outputs and predictions.
 Project-URL: Homepage, http://www.bom.gov.au
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bottleneck
 Requires-Dist: pandas
+Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: scores[dev,tutorial]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
+Requires-Dist: dask; extra == 'dev'
+Requires-Dist: h5netcdf; extra == 'dev'
 Requires-Dist: mypy==1.3.0; extra == 'dev'
+Requires-Dist: nbmake; extra == 'dev'
+Requires-Dist: pandas-stubs; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: pylint==2.17.4; extra == 'dev'
+Requires-Dist: pylint==3.0.1; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-watch; extra == 'dev'
 Provides-Extra: maintainer
 Requires-Dist: build; extra == 'maintainer'
 Requires-Dist: hatch; extra == 'maintainer'
 Requires-Dist: myst-parser; extra == 'maintainer'
 Requires-Dist: sphinx; extra == 'maintainer'
 Requires-Dist: sphinx-book-theme; extra == 'maintainer'
+Requires-Dist: twine; extra == 'maintainer'
 Provides-Extra: tutorial
 Requires-Dist: h5netcdf; extra == 'tutorial'
 Requires-Dist: jupyterlab; extra == 'tutorial'
 Requires-Dist: matplotlib; extra == 'tutorial'
+Requires-Dist: plotly; extra == 'tutorial'
 Requires-Dist: rasterio; extra == 'tutorial'
 Requires-Dist: rioxarray; extra == 'tutorial'
 Description-Content-Type: text/markdown
 
 # About the Scores Project
 
 One-line intro: xarray based verification (accuracy) scoring that can scale with Dask if needed. Pandas supported where possible.
 Why use it: trusted implementations, novel metrics, performance, one-stop-shop.
 
-Currently Included Metrics:
-
-| continuous | probability | categorical | statistical tests      |
-| ---------- | ----------- | ----------- | ----------- |
-| MAE, MSE, RMSE | CRPS | FIRM |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
+Currently Included Metrics and Tools:
 
+| continuous                      | probability | categorical      | statistical tests |
+| ----------                      | ----------- | -----------      | ----------------- |
+| MAE, MSE, RMSE, Flip Flop Index, Quantile Score, Isotonic Regression, Pearsons correlation coefficient  | CRPS for CDF, CRPS for ensemble, ROC, Brier score   | FIRM, POD, POFD  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
 
 **Notice -- This repository is currently undergoing initial construction and maintenance. It is not yet recommended for use. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io)
 
-`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of model outputs and predictions. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather. 
+`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of model outputs and predictions. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
 
 `scores` includes novel scores not commonly found elsewhere (e.g. FIRM, FlipFlop Index), complex scores (e.g. CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
 `scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to utilise Dask for scaling and performance.
 
 All of the scores and metrics in this package have undergone a thorough statistical and scientific review. Every score has a companion Jupyter Notebook tutorial demonstrating its use in practice.
 
 All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40, 000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
-The [installation guide](docs/installation.md) contains information on the various ways of installing, using and working with this package. 
+The [installation guide](docs/installation.md) contains information on the various ways of installing, using and working with this package.
 
 Installation of the core mathematical API may be performed with:
 
 ```py
 > pip install scores
 ```
```

