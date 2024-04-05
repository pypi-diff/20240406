# Comparing `tmp/robotframework-browser-translation-fi-0.4.1.tar.gz` & `tmp/robotframework-browser-translation-fi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-browser-translation-fi-0.4.1.tar", last modified: Wed Apr  3 13:44:09 2024, max compression
+gzip compressed data, was "robotframework-browser-translation-fi-0.4.2.tar", last modified: Fri Apr  5 23:02:59 2024, max compression
```

## Comparing `robotframework-browser-translation-fi-0.4.1.tar` & `robotframework-browser-translation-fi-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:44:09.952541 robotframework-browser-translation-fi-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 13:43:26.000000 robotframework-browser-translation-fi-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-03 13:44:09.952541 robotframework-browser-translation-fi-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-03 13:43:26.000000 robotframework-browser-translation-fi-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-03 13:44:05.000000 robotframework-browser-translation-fi-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:44:09.952541 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-03 13:44:05.000000 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   256796 2024-04-03 13:43:26.000000 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:44:09.952541 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-03 13:44:09.000000 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 13:44:09.000000 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:44:09.000000 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 13:44:09.000000 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:44:09.000000 robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:44:09.952541 robotframework-browser-translation-fi-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 23:02:08.000000 robotframework-browser-translation-fi-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-05 23:02:08.000000 robotframework-browser-translation-fi-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-05 23:02:55.000000 robotframework-browser-translation-fi-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-05 23:02:55.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   256796 2024-04-05 23:02:08.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/setup.cfg
```

### Comparing `robotframework-browser-translation-fi-0.4.1/LICENSE` & `robotframework-browser-translation-fi-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-browser-translation-fi-0.4.1/PKG-INFO` & `robotframework-browser-translation-fi-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-browser-translation-fi
-Version: 0.4.1
+Version: 0.4.2
 Summary: Robot Framework Browser library translation to Finnish languege
 Author-email: Tatu Aalto <aalto.tatu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `robotframework-browser-translation-fi-0.4.1/README.md` & `robotframework-browser-translation-fi-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-browser-translation-fi-0.4.1/pyproject.toml` & `robotframework-browser-translation-fi-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robotframework-browser-translation-fi"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Tatu Aalto", email="aalto.tatu@gmail.com" },
 ]
 license = {file = "LICENSE"}
 description = "Robot Framework Browser library translation to Finnish languege"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -66,17 +66,14 @@
 )/
 '''
 
 [tool.ruff]
 lint.unfixable = []
 exclude = [
   "__pycache__",
-  "generated",
-  "wrapper",
-  "browser.pyi",
 ]
 target-version = "py38"
 lint.select = [
   "E",
   "F",
   "W",
   "C90",
@@ -102,14 +99,15 @@
   "SIM",
   "RUF"
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tasks.py" = ["T201"]
 "utest/*" = ["INP001"]
+"atest/*" = ["INP001"]
 
 [tool.pytest.ini_options]
 testpaths = ["utest"]
 log_format = "%(asctime)s %(levelname)s %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.robotidy]
@@ -117,7 +115,12 @@
 configure = [
     "NormalizeAssignments:equal_sign_type=space_and_equal_sign",
     "NormalizeAssignments:equal_sign_type_variables=space_and_equal_sign",
     "NormalizeNewLines:section_lines=1",
     "RenameTestCases:enabled=True:capitalize_each_word=True",
     "RenameKeywords:enabled=True",
 ]
+
+[tool.mypy]
+exclude = [
+  "utest/*",
+]
```

### Comparing `robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi/__init__.py` & `robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 from typing import TypedDict
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 class Language(TypedDict):
     language: str
     path: str
```

### Comparing `robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi/translation.json` & `robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/translation.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996268656716418%*

 * *Differences: {"'check_checkbox'": "{'name': 'valiste_valintaruutu'}",*

 * * "'get_element_by'": "{'name': 'hae_elementti_avulla'}",*

 * * "'highlight_elements'": "{'name': 'korosta_elementtejä'}",*

 * * "'set_assertion_formatters'": "{'name': 'aseta_väitteen_muotoilijat'}"}*

```diff
@@ -17,15 +17,15 @@
     },
     "cancel_download": {
         "doc": "Peruuttaa aktiivisen latauksen.\n\n        | =Argumentit= | =Kuvaus= |\n        | lataus    | `DownloadInfo` -objekti tai latauksen tunniste, joka peruutetaan. |\n\n        [https://forum.robotframework.org/t//6478|Kommentti >>]\n        ",
         "name": "peruuta_lataus"
     },
     "check_checkbox": {
         "doc": "Tarkistaa valintaruudun tai valitsee valintapainikkeen, jonka l\u00f6yt\u00e4\u00e4 ``selector``-valitsimen avulla.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``selector`` | Valintaruudun valitsin. Katso `Elementtien etsiminen` -osio tarkempien valitsintietojen saamiseksi. |\n        | ``force`` | Aseta Trueksi ohittaaksesi Playwrightin [https://playwright.dev/docs/actionability | Toimintakyvyn tarkistukset]. |\n\n        Avainsana k\u00e4ytt\u00e4\u00e4 tiukkaa tilaa, katso `Elementtien etsiminen` lis\u00e4tietoja tiukasta tilasta.\n\n        Ei tee mit\u00e4\u00e4n, jos elementti on jo tarkistettu/valittu.\n\n        [https://forum.robotframework.org/t//4235|Kommentti >>]\n        ",
-        "name": "valiste valintaruutu"
+        "name": "valiste_valintaruutu"
     },
     "clear_permissions": {
         "doc": "Tyhjent\u00e4\u00e4 kaikki oikeudet nykyisest\u00e4 kontekstista.\n\n        [https://forum.robotframework.org/t//4236|Kommentti >>]\n        ",
         "name": "tyhjenn\u00e4_oikeudet"
     },
     "clear_text": {
         "doc": "Tyhjent\u00e4\u00e4 tekstikent\u00e4n, joka l\u00f6ytyy ``selector``-valitsimen avulla.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``selector`` | Tekstikent\u00e4n valitsin. Katso `Elementtien etsiminen` -osio tarkempien valitsintietojen saamiseksi. |\n\n        Avainsana k\u00e4ytt\u00e4\u00e4 tiukkaa tilaa, katso `Elementtien etsiminen` lis\u00e4tietoja tiukasta tilasta.\n\n        [https://forum.robotframework.org/t//4237|Kommentti >>]\n        ",
@@ -169,15 +169,15 @@
     },
     "get_element": {
         "doc": "Palauttaa viittauksen Playwrightin [https://playwright.dev/docs/api/class-locator|Locator]-objektiin.\n\n        Viittausta voidaan k\u00e4ytt\u00e4\u00e4 my\u00f6hemmiss\u00e4 valitsimissa.\n\n\n        | =Argumentit= | =Kuvaus= |\n        | ``valitsin`` | Valitsin, josta on haettava . Katso `Elementtien etsiminen` -osio lis\u00e4tietoja valitsimista. |\n\n        Avainsana k\u00e4ytt\u00e4\u00e4 tiukkaa tilaa, katso `Elementtien etsiminen` lis\u00e4tietoja tiukasta tilasta.\n\n        Esimerkki:\n        | ${elementti} =    `Hae elementti`    \\#k\u00e4ytt\u00e4j\u00e4tunnuskentt\u00e4\n        | ${valinta_arvo} =    `Hae ominaisuus`    ${elementti} >> vaihtoehtoYksi    arvo    # Valitsin ratkaistaan sivulta.\n        | ${valinta_arvo} =    `Hae ominaisuus`    ${elementti} >> vaihtoehtoKaksi    arvo    # Valitsin ratkaistaan uudelleen sivulta.\n\n        [https://forum.robotframework.org/t//4269|Kommentti >>]\n        ",
         "name": "hae_elementti"
     },
     "get_element_by": {
         "doc": "Mahdollistaa elementtien paikantamisen niiden ominaisuuksien perusteella.\n\n        Valintastrategioita voi olla useita Playwright-strategioita, kuten AltText tai Label.\n        Katso lis\u00e4tietoja [https://playwright.dev/docs/locators|Playwright Locators] -sivulta.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``paikannusstrategia`` | K\u00e4ytett\u00e4v\u00e4 SelectionStrategy. Viittaa Playwrightin ``page.getBy***`` -toimintoihin. Katso https://playwright.dev/docs/locators |\n        | ``teksti`` | Teksti, jonka perusteella elementti paikannetaan. |\n        | ``tarkka`` | M\u00e4\u00e4ritt\u00e4\u00e4k\u00f6 etsitt\u00e4v\u00e4n tarkan osuman: isot ja pienet kirjaimet huomioiden koko merkkijono. Oletusarvo on ep\u00e4tosi. Sit\u00e4 ei huomioida, kun etsit\u00e4\u00e4n s\u00e4\u00e4nn\u00f6llisell\u00e4 lausekkeella. Huomaa, ett\u00e4 tarkka osuma poistaa v\u00e4lily\u00f6nnit. T\u00e4ll\u00e4 ei ole vaikutusta, jos k\u00e4ytet\u00e4\u00e4n RegExpia tai jos TestID:a k\u00e4ytet\u00e4\u00e4n strategiana. |\n        | ``kaikki_elementit`` | Jos tosi, palauttaa kaikki sopivat elementit listana. |\n\n        T\u00e4m\u00e4 avainsana toteuttaa seuraavat Playwright-toiminnot:\n        - [https://playwright.dev/docs/api/class-page#page-get-by-alt-text|page.getByAltText]\n        - [https://playwright.dev/docs/api/class-page#page-get-by-label|page.getByLabel]\n        - [https://playwright.dev/docs/api/class-page#page-get-by-placeholder|page.getByPlaceholder]\n        - [https://playwright.dev/docs/api/class-page#page-get-by-test-id|page.getByTestId]\n        - [https://playwright.dev/docs/api/class-page#page-get-by-text|page.getByText]\n        - [https://playwright.dev/docs/api/class-page#page-get-by-title|page.getByTitle]\n\n        ``page.getByRole`` tukee `Hae elementti roolin mukaan`-avainsanaa.\n\n        Jos elementti on haettava iframe:sta, valitsimen etuliite on m\u00e4\u00e4ritett\u00e4v\u00e4 k\u00e4ytt\u00e4en `Aseta valitsimen etuliite`-avainsanaa, joka sis\u00e4lt\u00e4\u00e4 ``>>>`` lopetuksena.\n\n        [https://forum.robotframework.org/t//5937|Kommentti >>]\n        ",
-        "name": "hae_elementti avulla"
+        "name": "hae_elementti_avulla"
     },
     "get_element_by_role": {
         "doc": "Palauttaa viittauksen Playwrightin [https://playwright.dev/docs/api/class-locator|Locator]-objektiin\n        sopivasta elementist\u00e4 ``rooli`` mukaan tai luettelon viittauksista, jos ``kaikki_elementit`` on asetettu ``Tosi``.\n\n        Mahdollistaa elementtien paikantamisen niiden [https://www.w3.org/TR/wai-aria-1.2/#roles|ARIA-roolin],\n        [https://www.w3.org/TR/wai-aria-1.2/#aria-attributes|ARIA-attribuuttien] ja\n        [https://w3c.github.io/accname/#dfn-accessible-name|saavutettavan nimen] perusteella.\n\n\n        Harkitse seuraavaa DOM-rakennetta.\n\n        | <h3>Rekister\u00f6idy</h3>\n        | <label>\n        |   <input type=\"checkbox\" /> Tilaa\n        | </label>\n        | <br/>\n        | <button>L\u00e4het\u00e4</button>\n\n        Voit paikantaa jokaisen elementin sen implisiittisen roolin perusteella:\n        | ${otsikko}    Hae elementti roolin mukaan    otsikko    nimi=Rekister\u00f6idy\n        | ${valintaruutu}   Hae elementti roolin mukaan    valintaruutu    nimi=Tilaa\n        | ${painike}     Hae elementti roolin mukaan    painike    nimi=/l\u00e4het\u00e4/i\n\n        | =Argumentit= | =Kuvaus= |\n        | ``kaikki_elementit`` | Jos tosi, palauttaa kaikki sopivat elementit listana. |\n        | ``rooli`` | Rooli, josta on haettava. |\n        | ``valittu`` | Attribuutti, joka on yleens\u00e4 asetettu aria-checked tai native <input type=checkbox> -ohjaimilla. |\n        | ``pois_p\u00e4\u00e4lt\u00e4`` | Attribuutti, joka on yleens\u00e4 asetettu aria-disabled tai disabled. |\n        | ``tarkka`` | M\u00e4\u00e4ritt\u00e4\u00e4k\u00f6 nimi t\u00e4sm\u00e4lleen: isot ja pienet kirjaimet huomioiden koko merkkijono. Oletusarvo on ep\u00e4tosi. Sit\u00e4 ei huomioida, kun nimi on s\u00e4\u00e4nn\u00f6llinen lauseke. Huomaa, ett\u00e4 tarkka osuma poistaa v\u00e4lily\u00f6nnit. |\n        | ``laajennettu`` | Attribuutti, joka on yleens\u00e4 asetettu aria-expanded. |\n        | ``sis\u00e4llyt\u00e4_piilotetut`` | Vaihtoehto, joka ohjaa, vastaavatko piilotetut elementit. Oletuksena vain ARIA:n m\u00e4\u00e4rittelem\u00e4tt\u00f6m\u00e4t piilotetut elementit vastaavat roolivalitsintaan. |\n        | ``taso`` | Numeroattribuutti, joka on yleens\u00e4 l\u00e4sn\u00e4 rooleissa otsikko, listaelementti, rivi, puun alkio, oletusarvoina <h1>-<h6> elementeille. |\n        | ``nimi`` | Vaihtoehto vastata saavutettavaan nimeen. Oletuksena vastaaminen on kirjainten koosta riippumaton ja etsii alimerkkijonoa, k\u00e4yt\u00e4 tarkkaa ohjaamaan t\u00e4t\u00e4 k\u00e4ytt\u00e4ytymist\u00e4. |\n        | ``painettu`` | Attribuutti, joka on yleens\u00e4 asetettu aria-pressed. |\n        | ``valittu`` | Attribuutti, joka on yleens\u00e4 asetettu aria-selected. |\n\n        Jos elementti on haettava iframe:sta, valitsimen etuliite on m\u00e4\u00e4ritett\u00e4v\u00e4 k\u00e4ytt\u00e4en `Aseta valitsimen etuliite`-avainsanaa, joka sis\u00e4lt\u00e4\u00e4 ``>>>`` lopetuksena.\n\n        [https://forum.robotframework.org/t//5938|Kommentti >>]\n        ",
         "name": "hae_elementti_roolilla"
     },
     "get_element_count": {
         "doc": "Palauttaa elementtien lukum\u00e4\u00e4r\u00e4n, jotka on l\u00f6ydetty ``valitsin``-parametrilla.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``valitsin`` | Valitsin, jota on laskettava. Katso `Elementtien etsiminen` -osio lis\u00e4tietoja valitsimista. |\n        | ``v\u00e4itt\u00e4m\u00e4_operaattori`` | Katso `V\u00e4itteet` lis\u00e4tietoja varten. Oletusarvo on Ei mit\u00e4\u00e4n. |\n        | ``v\u00e4itt\u00e4m\u00e4_odotettu`` | Odotettu arvo laskennalle |\n        | ``viesti`` | korvaa v\u00e4itteen oletusvirhesanoman. |\n\n        Vaihtoehtoisesti v\u00e4itt\u00e4\u00e4, ett\u00e4 tila vastaa m\u00e4\u00e4ritetty\u00e4 v\u00e4itett\u00e4. Katso\n        `V\u00e4itteet` lis\u00e4tietoja varten v\u00e4itteiden argumenteista. Oletuksena v\u00e4itett\u00e4\n        ei tehd\u00e4.\n\n        Esimerkki:\n        | `Hae elementtien laskum\u00e4\u00e4r\u00e4`    valintaruutu    >    1\n\n        [https://forum.robotframework.org/t//4270|Kommentti >>]\n        ",
@@ -273,15 +273,15 @@
     },
     "handle_future_dialogs": {
         "doc": "K\u00e4sittele seuraava dialogi sivulla ``toiminnolla``.\n\n        Dialogi voi olla mik\u00e4 tahansa varoitus-, ennen-poistumista-, vahvista- tai kysy-dialogi. Dialogin k\u00e4sittely\n        on kutsuttava ennen toimintaa, kuten esimerkiksi napsautusta, joka laukaisee\n        dialogin.\n\n        Jos k\u00e4sittelij\u00e4\u00e4 ei ole asetettu, dialogit hyl\u00e4t\u00e4\u00e4n oletuksena.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``toiminto`` | Miten varoitus k\u00e4sitell\u00e4\u00e4n. Voi olla ``hyv\u00e4ksy`` tai ``hylk\u00e4\u00e4``. |\n        | ``kysy_tieto`` | Arvo, joka sy\u00f6tet\u00e4\u00e4n kyselyyn. K\u00e4ytet\u00e4\u00e4n vain, jos ``toiminto``-argumentti on ``hyv\u00e4ksy``. Oletusarvo on tyhj\u00e4 merkkijono. |\n\n        Esimerkki:\n        | `K\u00e4sittele Tulevat Dialogit`    toiminto=hyv\u00e4ksy\n        | `Napsauta`                    \\#varoitukset\n\n        [https://forum.robotframework.org/t//4293|Kommentoi >>]\n        ",
         "name": "k\u00e4sittele_tulevat_dialogit"
     },
     "highlight_elements": {
         "doc": "Lis\u00e4\u00e4 korostuksen elementteihin, jotka vastaavat ``selector``-valitsinta. Tarjoaa tyylis\u00e4\u00e4d\u00f6n.\n\n        Palauttaa korostettujen elementtien lukum\u00e4\u00e4r\u00e4n. Avainsana ei ep\u00e4onnistu, jos `locator` ei vastaa yht\u00e4k\u00e4\u00e4n elementti\u00e4\n        sivulla. Avainsana ei vierit\u00e4 elementtej\u00e4 n\u00e4kym\u00e4\u00e4n, ja korostettu elementti voi olla n\u00e4kym\u00e4n ulkopuolella. K\u00e4yt\u00e4 `Scroll To Element`-avainsanaa vieritt\u00e4\u00e4ksesi elementti n\u00e4kym\u00e4\u00e4n.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``selector`` | Valitsimet, jotka halutaan korostaa. Katso `Elementtien etsiminen` -osio tarkempien valitsintietojen saamiseksi. |\n        | ``duration`` | M\u00e4\u00e4ritt\u00e4\u00e4 kuinka kauan valitsin pysyy korostettuna. Oletusarvoisesti ``5s`` => 5 sekuntia. |\n        | ``width`` | Asettaa korostuksen reunuksen leveyden. Oletusarvo on 2px. |\n        | ``style`` | Asettaa reunuksen tyylin. Oletusarvo on pisteviiva. |\n        | ``color`` | Asettaa reunuksen v\u00e4rin. Kelvollisia v\u00e4rej\u00e4 ovat esimerkiksi: ``red``, ``blue``, ``yellow``, ``pink``, ``black`` |\n\n        Avainsana ei ep\u00e4onnistu, vaikka valitsin ratkaisisi useisiin elementteihin.\n\n        Esimerkki:\n        | `Korosta elementit`    input#kirjautumispainike    kesto=200ms\n        | ${lukum\u00e4\u00e4r\u00e4} =    `Korosta elementit`    input#kirjautumispainike    kesto=200ms    leveys=4px    tyyli=solid    v\u00e4ri=\\#FF00FF\n        | Pit\u00e4isi olla yht\u00e4 suuri    ${lukum\u00e4\u00e4r\u00e4}    ${5}\n\n        [https://forum.robotframework.org/t//4294|Kommentti >>]\n        ",
-        "name": "korosta elementtej\u00e4"
+        "name": "korosta_elementtej\u00e4"
     },
     "hover": {
         "doc": "Siirt\u00e4\u00e4 virtuaalisen hiiren ja vieritt\u00e4\u00e4 elementtiin, joka l\u00f6ydet\u00e4\u00e4n ``selector``:n perusteella.\n\n        T\u00e4m\u00e4 metodi leijuu elementin yli, joka vastaa ``selector``:ia suorittamalla seuraavat vaiheet:\n        - Etsi elementti, joka vastaa ``selector``:ia. Jos sellaista ei ole,\n          odota kunnes vastaava elementti on liitetty DOM:aan.\n        - Odota toimintakyvyn tarkistuksia vastaavalle elementille, ellei ``pakota``-valintaa ole asetettu.\n          Jos elementti irrotetaan tarkistusten aikana, koko toiminto yritet\u00e4\u00e4n uudelleen.\n        - Vierit\u00e4 elementti n\u00e4kyviin tarvittaessa.\n        - K\u00e4yt\u00e4 `Hiiren Siirto` -toimintoa leijumaan elementin keskustan yli tai m\u00e4\u00e4ritettyyn ``sijaintiin``.\n\n\n        | =Argumentit= | =Kuvaus= |\n        | ``selector`` | Valitsin elementille, jonka yli leijutaan. Katso `Elementtien l\u00f6yt\u00e4minen` -osio tarkemmat tiedot valitsimista. |\n        | ``sijainti_x`` & ``sijainti_y`` | Piste, johon leijutaan suhteessa elementin bounding boxin vasempaan yl\u00e4kulmaan. Jos ei ole m\u00e4\u00e4ritetty, leijutaan elementin n\u00e4kyviss\u00e4 olevaan pisteeseen. Vain positiiviset arvot bounding-boxin sis\u00e4ll\u00e4 ovat sallittuja. |\n        | ``pakota`` | Aseta Tosi arvoksi ohittaaksesi Playwrightin [https://playwright.dev/docs/actionability | Toimintakyky tarkistukset]. |\n        | ``*modifikaattorit`` | Muokkausn\u00e4pp\u00e4imet painettavaksi. Varmistaa, ett\u00e4 vain n\u00e4m\u00e4 muokkausn\u00e4pp\u00e4imet ovat painettuna leijumisen aikana ja palauttaa sitten nykyiset muokkausn\u00e4pp\u00e4imet takaisin. Jos ei ole m\u00e4\u00e4ritetty, k\u00e4ytet\u00e4\u00e4n t\u00e4ll\u00e4 hetkell\u00e4 painettuja muokkausn\u00e4pp\u00e4imi\u00e4. |\n\n        Avainsana k\u00e4ytt\u00e4\u00e4 tiukkaa tilaa, katso `Elementtien l\u00f6yt\u00e4minen` lis\u00e4tietoja tiukasta tilasta.\n\n        Esimerkki:\n        | `Leijuta`    h1\n        | `Leijuta`    h1    10   20    Alt\n\n        [https://forum.robotframework.org/t//4295|Kommentoi >>]\n        ",
         "name": "leijuta"
     },
     "http": {
         "doc": "Suorittaa HTTP-pyynn\u00f6n nykyisess\u00e4 selaimen kontekstissa\n\n        | =Argumentit= | =Kuvaus= |\n        | ``url`` | Pyynt\u00f6-URL-osoite, esim. ``/api/foo``. |\n        | ``method`` | HTTP-menetelm\u00e4 pyynn\u00f6lle. Oletusarvo on GET. |\n        | ``body`` | Pyynt\u00f6tieto. GET-pyynn\u00f6ill\u00e4 ei voi olla tietoa. Jos tieto voidaan tulkita JSON-muotoon, pyynn\u00f6n ``Content-Type``-otsikko asetetaan automaattisesti arvoon ``application/json``. Oletusarvo on Ei mit\u00e4\u00e4n. |\n        | ``headers`` | Lis\u00e4otsikoista koostuva sanakirja. Oletusarvo on Ei mit\u00e4\u00e4n. |\n\n        Vastaus on Python-sanakirja, jossa on seuraavat ominaisuudet:\n          - ``status`` <int> Vastauksen tilakoodi.\n          - ``statusText`` <str> Tilateksti vastaten ``status``-arvoa, esim. OK tai INTERNAL SERVER ERROR. T\u00e4t\u00e4 ei v\u00e4ltt\u00e4m\u00e4tt\u00e4 ole saatavilla kaikille selaimille.\n          - ``body`` <dict> | <str> Vastauksen tieto. Jos tieto voidaan tulkita JSON-objektiksi,\n          se palautetaan Pythonin sanakirjana, muuten se palautetaan merkkijonona.\n          - ``headers`` <dict> Sanakirja, joka sis\u00e4lt\u00e4\u00e4 kaikki vastauksen otsikot.\n          - ``ok`` <bool> Oliko pyynt\u00f6 onnistunut, eli ``status`` on 200-299 -alueella.\n\n        T\u00e4ss\u00e4 on esimerkki Robot Frameworkin sanakirjamuuttujien ja laajennetun muuttujasyntaksin k\u00e4yt\u00f6st\u00e4\n        v\u00e4itt\u00e4mien tekemiseen vastausobjektissa:\n\n        | &{res}=             `HTTP`                       /api/loppupiste\n        | Should Be Equal     ${res.status}              200\n        | Should Be Equal     ${res.body.jokin_kentt\u00e4}     jokin arvo\n\n        [https://forum.robotframework.org/t//4296|Kommentti >>]\n        ",
@@ -413,15 +413,15 @@
     },
     "session_storage_set_item": {
         "doc": "Tallenna tiedot istuntotallennukseen.\n\n| =Argumentit= | =Kuvaus= |\n| ``avain`` | Avain, jonka alle se tulisi tallentaa. |\n| ``arvo`` | Arvo, joka tulisi tallentaa merkkijonona. |\n| ``kehysvalitsin`` | Jos t\u00e4m\u00e4 valitsin osoittaa elementtiin iframe-kehikon sis\u00e4ll\u00e4, k\u00e4ytet\u00e4\u00e4n kyseisen kehyksen SessionStoragea. Esimerkki: ``iframe[name=\"test\"] >>> body`` |\n\nEsimerkki:\n| `Istuntotallennus Aseta Kentt\u00e4`    avain2    arvo2\n\n[https://forum.robotframework.org/t//4326|Kommentti >>]\n        ",
         "name": "istunnon_tallennustila_aseta_tuote"
     },
     "set_assertion_formatters": {
         "doc": "Aseta v\u00e4itteiden muotoilijat avainsanoille.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``formatters`` | Avainsanojen ja muotoilijoiden sanakirja, jossa avain on avainsanan nimi, johon muotoilijat ovat sovellettu. Sanakirjan arvo on luettelo muotoilijoista, jotka ovat k\u00e4yt\u00f6ss\u00e4. M\u00e4\u00e4ritellyn avainsanan muotoilijat korvataan aina. Tyhj\u00e4 luettelo poistaa kaikki muotoilijat avainsanasta. Jos ``formatters`` on tyhj\u00e4 sanakirja, silloin kaikki muotoilijat poistetaan kaikista avainsanoista. |\n        | ``scope`` | M\u00e4\u00e4ritt\u00e4\u00e4 muotoilijan elini\u00e4n, mahdolliset arvot ovat Global, Suite ja Test. |\n\n        Katso `FormatterTypes` -tyypin dokumentaatiota lis\u00e4tietoja varten.\n\n        On mahdollista m\u00e4\u00e4ritt\u00e4\u00e4 omia muotoilijoita lambda-funktioina.\n\n        Esimerkki:\n        | `Aseta v\u00e4itteiden muotoilijat`    {\"Hanki teksti\": [\"strip\", \"normaalitilassa v\u00e4lit\"]}  # T\u00e4m\u00e4 muuttaa kaikki v\u00e4lit yhdeksi v\u00e4lily\u00f6nniksi ja poistaa v\u00e4lily\u00f6nnit merkkijonon alusta ja lopusta.\n        | `Aseta v\u00e4itteiden muotoilijat`    {\"Hanki otsikko\": [\"sovelletaan odotettuun\",\"lambda x: x.replace(' ', '')\"]}  # T\u00e4m\u00e4 poistaa kaikki v\u00e4lit merkkijonosta.\n        ",
-        "name": "aseta v\u00e4itteen muotoilijat"
+        "name": "aseta_v\u00e4itteen_muotoilijat"
     },
     "set_browser_timeout": {
         "doc": "Asettaa suurimman osan sy\u00f6tteist\u00e4 ja getter-avainsanojen k\u00e4ytt\u00e4m\u00e4n aikakatkaisun.\n\n        | =Argumentit= | =Kuvaus= |\n        | ``aikakatkaisu`` | Aikakatkaisu on nykyisen playwright-kontekstin ja uusien kontekstien aikakatkaisu. Tukee Robot Frameworkin [https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format|aikamuotoa]. Palauttaa edellisen aikakatkaisun arvon. |\n        | ``laajuus``   | Laajuus m\u00e4\u00e4rittelee asetuksen voimassaoloajan. K\u00e4ytett\u00e4viss\u00e4 olevat arvot ovat ``Globaali``, ``Kokoelma`` tai ``Testi`` / ``Teht\u00e4v\u00e4``. Katso `Laajuuden asetukset` lis\u00e4tietoja varten. |\n\n        Esimerkki:\n        | ${vanha_aikakatkaisu} =    `Aseta Selaimen Aikakatkaisu`    1m 30 sekuntia\n        | Click     //button\n        | `Aseta Selaimen Aikakatkaisu`    ${vanha_aikakatkaisu}\n\n        [https://forum.robotframework.org/t//4328|Kommentti >>]\n        ",
         "name": "aseta_selaimen_aikakatkaisu"
     },
     "set_default_run_before_unload": {
         "doc": "Aseta oletusarvoinen runBeforeUnload-arvo, kun `Sulje Sivu` kutsutaan ep\u00e4suorasti.\n\n        Sulje Sivu kutsutaan ep\u00e4suorasti, kun\n        [https://marketsquare.github.io/robotframework-browser/Browser.html#Automatic%20page%20and%20context%20closing|sivun sulkeminen automaattisesti]\n        tapahtuu. Oletusarvo on ep\u00e4tosi, ja t\u00e4t\u00e4 avainsanaa voidaan k\u00e4ytt\u00e4\u00e4 arvon muuttamiseen.\n        Palauttaa vanhan runBeforeUnload-arvon.\n\n        [https://forum.robotframework.org/t/6203|Kommentti >>]\n        ",
```

### Comparing `robotframework-browser-translation-fi-0.4.1/robotframework_browser_translation_fi.egg-info/PKG-INFO` & `robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-browser-translation-fi
-Version: 0.4.1
+Version: 0.4.2
 Summary: Robot Framework Browser library translation to Finnish languege
 Author-email: Tatu Aalto <aalto.tatu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

