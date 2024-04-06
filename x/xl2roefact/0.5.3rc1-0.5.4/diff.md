# Comparing `tmp/xl2roefact-0.5.3rc1.tar.gz` & `tmp/xl2roefact-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2roefact-0.5.3rc1.tar", last modified: Sun Mar 31 02:53:37 2024, max compression
+gzip compressed data, was "xl2roefact-0.5.4.tar", last modified: Sat Apr  6 17:45:42 2024, max compression
```

## Comparing `xl2roefact-0.5.3rc1.tar` & `xl2roefact-0.5.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0    35149 2024-03-31 02:53:04.647600 xl2roefact-0.5.3rc1/LICENSE
--rw-r--r--   0        0        0    14216 2024-03-31 02:53:04.647600 xl2roefact-0.5.3rc1/README.md
--rw-r--r--   0        0        0     3302 2024-03-31 02:53:37.011192 xl2roefact-0.5.3rc1/pyproject.toml
--rw-r--r--   0        0        0        1 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/tests/.gitkeep
--rw-r--r--   0        0        0    20711 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/tests/Fact_Petrom_11017969.json
--rw-r--r--   0        0        0   268862 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/tests/Fact_Petrom_11017969.xlsx
--rw-r--r--   0        0        0    15740 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/tests/Fact_Petrom_11017969.xml
--rw-r--r--   0        0        0     1052 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/tests/_test_results.txt
--rw-r--r--   0        0        0    23248 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/tests/fact_RENF1004.json
--rw-r--r--   0        0        0    16332 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/tests/fact_RENF1004.xlsx
--rw-r--r--   0        0        0      567 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/__init__.py
--rw-r--r--   0        0        0      626 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/__main__.py
--rw-r--r--   0        0        0     1477 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/__version__.py
--rw-r--r--   0        0        0     6788 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/app_cli.py
--rw-r--r--   0        0        0      727 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/chkisld.py
--rw-r--r--   0        0        0      584 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/chkxml.py
--rw-r--r--   0        0        0    10079 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/config_settings.py
--rw-r--r--   0        0        0     1808 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/data/README_app_config_rules.md
--rw-r--r--   0        0        0        1 2024-03-31 02:53:05.027595 xl2roefact-0.5.3rc1/xl2roefact/data/__init__.py
--rw-r--r--   0        0        0     6867 2024-03-31 02:53:05.031595 xl2roefact-0.5.3rc1/xl2roefact/data/app_settings.yml
--rw-r--r--   0        0        0      941 2024-03-31 02:53:05.031595 xl2roefact-0.5.3rc1/xl2roefact/data/owner_data.json
--rw-r--r--   0        0        0      600 2024-03-31 02:53:05.031595 xl2roefact-0.5.3rc1/xl2roefact/ldxml.py
--rw-r--r--   0        0        0     9024 2024-03-31 02:53:05.031595 xl2roefact-0.5.3rc1/xl2roefact/libutils.py
--rw-r--r--   0        0        0    65290 2024-03-31 02:53:05.031595 xl2roefact-0.5.3rc1/xl2roefact/rdinv.py
--rw-r--r--   0        0        0      612 2024-03-31 02:53:05.031595 xl2roefact-0.5.3rc1/xl2roefact/wrxml.py
--rw-r--r--   0        0        0    56765 1970-01-01 00:00:00.000000 xl2roefact-0.5.3rc1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-06 17:45:09.666372 xl2roefact-0.5.4/LICENSE
+-rw-r--r--   0        0        0    18286 2024-04-06 17:45:09.666372 xl2roefact-0.5.4/README.md
+-rw-r--r--   0        0        0     3284 2024-04-06 17:45:42.462232 xl2roefact-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/.gitkeep
+-rw-r--r--   0        0        0    18903 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/Fact_Petrom_11017969.json
+-rw-r--r--   0        0        0   268862 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xlsx
+-rw-r--r--   0        0        0    15740 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xml
+-rw-r--r--   0        0        0      986 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/_test_results.txt
+-rw-r--r--   0        0        0    20914 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/fact_RENF1004.json
+-rw-r--r--   0        0        0    16332 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/fact_RENF1004.xlsx
+-rw-r--r--   0        0        0      567 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/__main__.py
+-rw-r--r--   0        0        0     1492 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/__version__.py
+-rw-r--r--   0        0        0     7875 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/app_cli.py
+-rw-r--r--   0        0        0      727 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/chkisld.py
+-rw-r--r--   0        0        0      584 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/chkxml.py
+-rw-r--r--   0        0        0     8246 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/config_settings.py
+-rw-r--r--   0        0        0     1808 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/data/README_app_config_rules.md
+-rw-r--r--   0        0        0        1 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/data/__init__.py
+-rw-r--r--   0        0        0     6867 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/data/app_settings.yml
+-rw-r--r--   0        0        0      600 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/ldxml.py
+-rw-r--r--   0        0        0    10480 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/libutils.py
+-rw-r--r--   0        0        0    69307 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/rdinv.py
+-rw-r--r--   0        0        0      612 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/wrxml.py
+-rw-r--r--   0        0        0    60832 1970-01-01 00:00:00.000000 xl2roefact-0.5.4/PKG-INFO
```

### Comparing `xl2roefact-0.5.3rc1/LICENSE` & `xl2roefact-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/README.md` & `xl2roefact-0.5.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # xl2roefact
 
 ![Static Badge](https://img.shields.io/badge/version-{{ xl2roefact_version }}-blue)
 
 Legaturi externe utile:
 
-* [**Site dedicat**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
-* [Pachet pe *PyPi*](https://pypi.org/project/xl2roefact/)
-* [Surse pe *GitHub*](https://github.com/petre-renware/api_to_roefact/)
+* [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
+* [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
+* [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
 * [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
 * [Referinta *API*](./doc/810.05a-xl2roefact_DLD_specs.md)
 
 
 
 ## Facilitati
 
@@ -24,43 +24,34 @@
 ![Static Badge](https://img.shields.io/badge/format_JSON-YES-orange)
 ![Static Badge](https://img.shields.io/badge/format_XML-YES-orange)
 ![Static Badge](https://img.shields.io/badge/format_PDF-YES-orange)
 ![Static Badge](https://img.shields.io/badge/format_RO_eFact-YES-red)
 
 
 
-
-
-
-
 Aceasta componenta este "totul despre crearea de facturi electronice" din formatul Excel office (xlsx). Aplicatia poate genera factura in format JSON, XML, PDF si o poate incarca in sistemul *RO E-Fact*[^ld_roefact].
 
 Aceasta componenta ofera urmatoarele facilitati (acestea fiind obiectivele fundamentale ale componentei):
 
 * **transformarea facturilor din Excel in formatul `XML`** cerut de catre sistemul ANAF RO E-Fact pentru incarcare
-
- * **incarcarea acestora** in sistemul ANAF RO E-Fact[^ld_roefact]
-
-*  **transformarea facturilor din Excel intr-un format `JSON`**  intermediar, independent de platforma si care permite integrarea acestora cu alte sisteme (standard *REST*)
-
+* **incarcarea acestora** in sistemul ANAF RO E-Fact[^ld_roefact]
+* **transformarea facturilor din Excel intr-un format `JSON`**  intermediar, independent de platforma si care permite integrarea acestora cu alte sisteme (standard *REST*)
 * **generarea facturii in format PDF** pentru transmiterea acesteia catre client, semnarea electronica, tiparirea si arhivarea acesteia in format fizic (in general manipularea facturii in format *"human readable"*)
 
 Componenta ofera doua instrumente pentru realizarea si indeplinirea acestor obiective:
 
 * `xl2roefact` o **aplicatie de tip linie de comanda** (disponibila pentru sistemele de operare Windows, Linux si MacOS)
-
-* `xl2roefact PyPi` o **blioteca standard Python** utilizabila pentru dezvoltari proprii in scopul extinderii altor sisteme existente (*custom development*)
+* `xl2roefact PyPi` **blioteca standard Python** utilizabila pentru dezvoltari proprii in scopul extinderii altor sisteme existente (*custom development*)
 
 
 
 
 
 
 ## Instalarea aplicatiei xl2roefact
-
 Instalarea aplicatiei *xl2roefact* este disponibila in urmatoarele variante:
 
 * pentru **Windows**:
     * **`MSI`** pachet instalare pentru *Windows*
     * **`EXE`** executabil *Windows in format "portabil" (un singur fisier)*
 
 * pentru **Linux**:
@@ -82,34 +73,32 @@
 * numele pachetelor includ versiunea de aplicatie utilizata si sistemul de operare pentru care sunt disponibile
 * pentru echivalent utilizare  *portabila pentru Linux* se poate instala biblioteca Python dupa care devine utilizabil scriptul Python "ca orice alta comanda Linux"
 
 
 
 
 
-## Configurarea aplicatiei xl2roefact
 
+## Configurarea aplicatiei xl2roefact
 Parametrii de configurare aplicatiei se gasesc in fisierul *`config_settings.py`*. Acestia sunt sub elaborati in limbaj Python prin utilizarea conventiilor de constante conform recomandarilor PEP (numele capitatlizat) si sunt acompaniti de linii de explicatii privind aplicabilitatea lor.
 
 <!--#TODO: prev paragraph to replace new config method by using `app_settings.yml` in current directory -->
 
 Configurare aplicatiei se poate face interactiv si din aplicatie. Pentru a obtine help referitor la detaliile comenzi se va folosi
-```bash
+```shell
 xl2roefact settings --help
 ```
 
 Configurarile existente si regulile recomandate in configurarea aplicatiei se afiseaza folosind comanda:
-```bash
+```shell
 xl2roefact settings --rules
 ```
 
 
 ### Configurarea din fisier extern
-<!--  --Sablon fisier configurare a aplicatiei xl2roefact -->
-
 Configurarea aplicatuiei se poate face si prin intermediul unui fisier extern numit "*sablon de configurare*" (*en: configuration template*). Sablonul permite configurarea aplicatiei prin modificarea fragmentelor de text care trebuiesc cautate in fisierul Excel pentru identificarea diverselor informatii aferente facturii.
 
 Sablonul este in format [YAML](https://yaml.org/) iar informatiile ce trebuiesc descrise sunt explicate individual in comentarii insotitoare.
 De asemenea este util a fi citite si recomandarile date in pagina de descriere a aplicatiei.
 
 Pentru a beneficia de cobfigurarile facute de dumneavoastra trebuie sa creati un fisier **`app_settings.yml`** in directorul curent din care lansati aplicatia, fisier ce contine noile configurari dorite.
 **Numele fisierelui este obligatoriu a fi respectat.**
@@ -124,40 +113,89 @@
     In conditiile folosirii kitului MSI pentru o instalare locala a aplicatiei (cu utilizari multiple si repetate) si in situatia in care se doreste schimbarea configurarii implicite a aplicatiei se vor urma acesti pasi:
     
     * in directorul de instalare a aplicatiei se va crea daca nu exita directorul `data/`
     * in acest director se va crea un fisier `app_settings.yml` cu configurarea globala dorita
     
     Aceasta configurare inlocuieste configurarea implicita si se va aplica global in utilizarea aplicatiei. In continuare configurarile existente in directorul curent *suprascriu configurarea globala* (se aplica cu precedenta).
 
+>[Aici puteti gasiti pentru descarcare un model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact).
+
 
 
->[Aici puteti gasiti pentru descarcare un model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact).
 
 
 
+## Utilizare nomenclator de furnizori
+Aplicatia *xl2roefact* permite utilizarea datelor pentru furnizori din fisiere externe (in locul informatiilor din fisierele Excel) lucru ce poate fi folositor in urmatoarele situatii:
 
+* cind utilizatorul aplicatiei o face in scopuri personale si multe facturi emise il au *pe el ca furnizor*. Aceast lucru permite ca informatia din Excel referitoare la furnizor sa fie sumara sau sa lipseasca, factura finala format `PDF` fiind generata cu aplicatia
+* cind utilizatorul aplicatiei o foloseste pentru a emite facturi pentru alte firme si astfel este mai comod sa foloseasca fisiere cu datele acestor firme decit sa introduca informatia in fiecare factura
+* cind se doreste ca datele furnizorului sa fie preluate dintr-un sistem extern ce le poate exporta ca si fisisre
 
-## Comenzile aplicatiei
 
+### Reguli generale de utilizare
+Aceasta sectiune descrie regulile generale ce trebuiesc avute in vedere pentru o completa si corecta utilizare a facilitatii "Nomenclator furnizori":
+
+* Nomenclatorul de furnizori se va completa intr-unul sau mai multe fisere de date (de tip text, vezi mai jos formatul exact).
+* Un fisier acomodeaza un singur furnizor. Pentru mai multi furnizori se vor folosi fisiere diferite.
+* Numele fisierului (fara extensie) trebuie sa coincida cu o cheie alternativa a furnizorului respectiv. Prin cheie alternativa se intelege acea cheie care este unica si poate asigura regasirea furnizorului prin folosirea ei. Ca si exemple din practicile curente ar fi cimpul numit uzual `code` sau `code_name` existent in mai toate sistemele de business. Acesta are avantajul unicitatii si a unei reprezentari "umane" (*en: human readable*). Desigur un cimp de tip cheie primara / ID este ideal dar de obicei acesta este tehnic iar valoarea sa nu ofera prea multe indicatii.
+* Formatul fisierului este  [YAML](https://yaml.org/) standard, fara folosirea de modele de date complexe, aatfel incit o eventuala conversie `JSON` <--> `YAML` sa poata fi realizata manual in ambele sensuri si fara necessitatea unor cunostinte avansate ci la nivel de redefinire a numelor cheilor.
+
+
+###  Locatia nomenclatorului
+Fisierele cu datele furnizorilor pot sta in urmatoarele locatii:
+
+* *directorul curent* este locatia cu prioritatea maxima si in caz de "duplicate" ale unui fisier, cel de aici va fi luat in considerare
+* *directorul `data/`* din locatia unde este instalata aplicatia
+
+Recomandari si practici uzuale:
+
+* In situatiile in care sistemul este instalat pe un computer ce se foloseste frecvent cu aplicatia *xl2roefact* si exista un set de furnizori frecvent folositi se recomanda folosirea directorului `data/` pentru stocarea fisierelor nomenclator astfel incit sa poata fi refolosite usor.
+* In situatia folosirii a "multe" fisiere date furnizori se recomanda crearea unui director dedicat in locatia utilizata (vezi mai sus) si acesta sa fie referit in numle fisierului.
+
+
+### Utilizarea nomenclatorului
+Pentru a folosi cu aplicatia un fisier tip nomenclator furnizor se va utiliza optiunea:
+```shell
+xl2roefact xl2json -o fisier_furnizor
+```
+unde `fisier_furnizor` este numele fisierului ce contine datele unui furnizor. Locatia acestui fisier este relativa la [locatia considerata pentru folosire](#locatia-nomenclatorului)
+
+
+### Sablon pentru nomenclator de furnizori
+Sablonul este proiectat pentru utilizarea in facturile emise si contine numai informatiile necesare in acest scop.<br>
+Astfel cimpurile existente trebuiesc pastrate, adica nu vor fi sterse.
+
+Vor fi *respectate si completate* corespunzator cimpurile specificate ca *obligatoriii (en: mandatory* in comentariile aferente fiecarui cimp.<br>
+Pentru acele cimpuri pentru care informatia este necunoscuta sau considerata irelevanta se va completa cu `null`.
+
+Se vor putea adauga orice alte cimpuri suplimentare cu conditia sa fie respectat formatul fisierului (`YAML`). acestea nu vor fi folosite de catre aplicatie, ci pur si simplu ignorate.
+
+>[Aici puteti gasiti un model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor).
+
+
+
+
+
+
+## Comenzile aplicatiei
 Interfata aplicatie este realizata utilizind conventiile si practicile uzuale pentru aplicatii tip linie de comanda consola. Pentru informatii privind comenzile se poate folosi optiunea de **help**, dispobilia atit la nivelul general:
-```bash
+```shell
 xl2roefact --help
 ```
 cit si la nivel detaliat pentru fiecare comanda
-```bash
+```shell
 xl2roefact [COMMAND] --help
 ```
 
 
 **Lista comenzilor:**
 
 * **about** - Afiseaza informatii despre aceatsa aplicatie (copyright, scop, etc)
-
 * **settings** _ Afiseaza parametrii de configurare a aplicatiei. [Vezi sectiunea de configurare a aplicatiei](#configurarea-aplicatiei-xl2roefact)
-
 * **xl2json** - Transforma fisierul (fisierele) Excel in forma JSON pentru utilizare ulterioara ca forma de date standardizat pentru schimbul de informatii cu alte sisteme electronice
 
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
@@ -169,15 +207,14 @@
     :depth: 2
 
 
 
 
 
 ## Practici si regului referitoare la continutul facturilor din Excel
-
 Acest capitol se refera la modul in care este "tratat" continutul fisierului Excel cu factura, mai exact la modalitatea in care informatia facturii este cautata, identificata si gasita in scopul de a fi salvata in oricare din formatele de "factura electronica / E-Fact".
 
 Utilizarea sablonului de factura Excel ce este livrat impreuna cu aplicatia **ESTE O VARIANTA DE LUCRU RECOMANDATA**, dar nu obligatorie. Chiar si in cazul utilizarii acestuia, prin modificarea "structurii" acestuia, informatia poate ajunge *nerecognoscibila / neidentificabila* total sau partial daca nu sunt urmate regulile expuse.
 
 >In general trebuie facuta diferenta intre datele facturii si modul in care aceasta va fi tiparita (va aparea la tiparire / previzualizare).
 >
 >Mai exact **continutul informational** al facturii nu trebuie nici confundat si nici mixat cu **formatul de afisare al acesteia** (layout). Pentru acesta din urma se recomanda a fi folosite cu precadere *regulile de formatare* din Excel si nu cele stocare a datelor. Un exemplu este un numar zecimal oarecare unde:
@@ -278,14 +315,17 @@
 
 
 ## Descarcare (download) aplicatie xl2roefact CLI
 
 * [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
 * [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
 * [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
+* [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
+
+
 
 
 
 
 ## Date identificare
 
 * part number (p/n): `0000-0095-xl2roefact`
```

### Comparing `xl2roefact-0.5.3rc1/pyproject.toml` & `xl2roefact-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
     "Topic :: Office/Business :: Financial",
 ]
-version = "0.5.3rc1"
+version = "0.5.4"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://invoicetoroefact.renware.eu"
 PDF-Documentation = "https://invoicetoroefact.renware.eu/pdfs/print_page.html/print_page.pdf"
@@ -88,15 +88,15 @@
 [tool.pdm.scripts.build_msi]
 shell = "python setup.py bdist_msi"
 
 [tool.pdm.scripts.build_sexe]
 cmd = [
     "pyinstaller",
     "--distpath=dist_sexe/",
-    "--name=xl2roefact_to_update_name",
+    "--name=xl2roefact",
     "--log-level=WARN",
     "--onefile",
     "--noconfirm",
     "xl2roefact_copy_for_sexe.py",
 ]
 
 [tool.pdm.scripts.post_build_sexe]
```

### Comparing `xl2roefact-0.5.3rc1/tests/Fact_Petrom_11017969.xlsx` & `xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/tests/Fact_Petrom_11017969.xml` & `xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/tests/fact_RENF1004.xlsx` & `xl2roefact-0.5.4/tests/fact_RENF1004.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/__init__.py` & `xl2roefact-0.5.4/xl2roefact/__init__.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/__main__.py` & `xl2roefact-0.5.4/xl2roefact/__main__.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/app_cli.py` & `xl2roefact-0.5.4/xl2roefact/app_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! /usr/bin/env python
+#! /usr/bin/env python
 """app_cli: the command line application for all xl2roefact functionalities.
 
 Identification:
 
 * copyright: (c) 2023 RENWare Software Systems
 * author: Petre Iordanescu (petre.iordanescu@gmail.com)
 """
@@ -18,16 +18,16 @@
 from typing_extensions import Annotated
 from pathlib import Path
 from typing import Optional
 from datetime import datetime
 from rich import print
 from rich.pretty import pprint
 from rich.markdown import Markdown
-
 # xl2roefact specific libraries
+from xl2roefact.libutils import hier_get_data_file
 import xl2roefact.config_settings as configs  # configuration elements to use with `settings` command
 from xl2roefact.rdinv import rdinv  # status #TODO: wip...
 from xl2roefact.wrxml import wrxml  # status #FIXME: not yet started
 from xl2roefact.chkxml import chkxml  # status #FIXME: not yet started
 from xl2roefact.ldxml import ldxml  # status #FIXME: not yet started
 from xl2roefact.chkisld import chkisld  # status #FIXME: not yet started
 
@@ -38,15 +38,15 @@
 app_cli = typer.Typer(name="xl2roefact")
 
 
 
 
 @app_cli.command()
 def about():
-    """provide a short application description.
+    """Provide a short application description.
     """
     version_string = normalized_version()
     print(Markdown(app_logo))
     print(f"xl2roefact {version_string} application by RENware Software Systems (c) 2023, 2024")
     # about details
     print("[yellow]extract & convert Excel invoice files to JSON, XML and upload info to [cyan]RO ANAF e-Fact[/] system")
     print("Support: [yellow]www.renware.eu, petre.iordanescu@gmail.com[/]")
@@ -62,17 +62,18 @@
         bool,
         typer.Option(
             "--rules", "-r",
             help="show settings recommended update rules"
         ),
     ] = False
 ):
-    """display application configuration parameters and settings that are subject to be changed by user.
+    """Display application configuration parameters and settings that are subject to be changed by user.
 
     Args:
+    
         `rules`: show recommended rules to follow when change application configurable settings (available in both RO & EN languages). Defaults to `False`.
     """
 
     if rules:  # show configuration rules from module docstring
         from xl2roefact.config_settings import rules_content
         print(rules_content)  # content is already rendered
         print()  # print a blank line for readability
@@ -103,75 +104,98 @@
             dir_okay=True,
             writable=True,
             readable=True,
             resolve_path=True,
             help="directory to be used to look for Excel files (if default directory does not exists will consider current directory instead)."
         ),
     ] = "invoice_files/",
+    owner_datafile: Annotated[
+        Path,
+        typer.Option(
+            "--owner-datafile", "-o",
+            exists=False,
+            file_okay=False,
+            dir_okay=False,
+            writable=False,
+            readable=True,
+            resolve_path=False,
+            help="File to read invoice supplier (owner) data instead Excel."
+        ),
+    ] = None,
     verbose: Annotated[
         bool,
         typer.Option(
             "--verbose", "-v",
             help="show detailed processing messages"
         ),
     ] = False
 ):
-    """extract data from an Excel file (save data to JSON format file with the same name as original file but `.json` extension).
+    """Extract data from an Excel file (save data to JSON format file with the same name as original file but `.json` extension).
 
     Args:
+    
         `file_name`: files to process (wildcards allowed).
         `files_directory`: directory to be used to look for Excel files. Defaults to `invoice_files/`. NOTE: if default directory does not exists will consider current directory instead
+        `owner_datafile`: File to read invoice supplier (owner) data instead Excel.
         `verbose`: show detailed processing messages". Defaults to `False`.
     """
     print(f"*** Application [red]xl2roefact[/] launched at {datetime.now()}")
-
     # process files as requested in command line (NOTE: if default directory does not exists will consider current directory instead)
     tmp_files_to_process = Path(files_directory)
     if not (tmp_files_to_process.exists() and tmp_files_to_process.is_dir()):
         tmp_files_to_process = Path(".").absolute()
-        print(f"[dark_orange]WARNING note:[/] Default directory not found. Will consider current directory instead: [cyan]{tmp_files_to_process}[/].")
+        print(f"[dark_orange]WARNING note:[/] Default directory not found. Will consider current directory: [cyan]{tmp_files_to_process}[/].")
     print(f"[yellow]INFO note:[/] files to process: [cyan]{Path(tmp_files_to_process, file_name)}[/]")
     list_of_files_to_process = list(tmp_files_to_process.glob(file_name))  # `glob()` will unify in a list with specified files as pattern
     if verbose:
         print(f"[yellow]DEBUG note:[/] list object with files to process: [green]{list_of_files_to_process}[/]")
     for a_file in list_of_files_to_process:
         if verbose:
             print(f"[yellow]DEBUG note:[/] to process now: [green]{a_file}[/]")
         #
         invoice_to_process = Path("./", a_file)  # current file name to process, starting from current directory (the `files_directory` is already contained in)
-        invoice_datadict = rdinv(file_to_process=invoice_to_process, debug_info=verbose)
+        if owner_datafile is not None:  # prep are to call `rdinv()` module with parameter to read supplier data from external file instead Excel
+            full_path_owner_datafile = hier_get_data_file(owner_datafile)
+            if full_path_owner_datafile:
+                invoice_datadict = rdinv(file_to_process=invoice_to_process, debug_info=verbose, owner_datafile=full_path_owner_datafile)
+            else:
+                print(f"[red]ERROR: Owner data file ([cyan]{owner_datafile}[/]) is not valid or does not exists. Process terminated.[/].")
+                return  # just exit...
+        else:
+            invoice_datadict = rdinv(file_to_process=invoice_to_process, debug_info=verbose)
         if not invoice_datadict:
             print(f"[yellow]INFO note:[/] last step returned an error and process could be incomplete. Please review previous messages.")
         #
         if verbose:
             print(f"[yellow]DEBUG note:[/] `xl2roefact` module, content of resulted `invoice` data dictionary:")
             pprint(invoice_datadict)
             print()
 
 
 
+
 @app_cli.callback(invoke_without_command=True)
 def called_when_no_command(
     ctx: typer.Context,
     version: Annotated[
         bool,
         typer.Option(
-            "--version",
+            "--version", "-V",
             help="show application version"
         ),
     ] = False
 ):
-    """function called when no command is invoked and to provide only application version (for external users to test it!).
+    """Application global information (command agnostic).
     """
     if (ctx.invoked_subcommand is None) and not version:
         print("[red]No command. Please use --help to get help.[/]")
         sys.exit(0)
     version_string = normalized_version()
     if version:
-            print(f"xl2roefact {version_string}")
+        print(f"xl2roefact {version_string}")
 
 
 
 
 def main():
     app_cli()
```

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/chkisld.py` & `xl2roefact-0.5.4/xl2roefact/chkisld.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/chkxml.py` & `xl2roefact-0.5.4/xl2roefact/chkxml.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/config_settings.py` & `xl2roefact-0.5.4/xl2roefact/config_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Configuration and setting parameters.
 
-Regulile recomandate se gasessc in documentul (recommended rules are in document) [`doc/README_app_config_rules.md`](../doc/README_app_config_rules.md)
+Regulile recomandate se gasessc in documentul (recommended rules are in document `xl2roefact/data/README_app_config_rules.md`)
 
-    Public objects:
+Public objects:
 
-        `rules_content`: contains the rules text (rendered)
+* `rules_content`: contains the rules text (rendered)
+
+Info:
 
 * copyright: (c) 2023 RENWare Software Systems
 * author: Petre Iordanescu (petre.iordanescu@gmail.com)
 """
 
 from pathlib import Path
 import os
 import sys
 from rich.markdown import Markdown
 import yaml
 from pprint import pprint
+from .libutils import hier_get_data_file
 
 """---------------------------------------------------------------------------------------------------------------------------
 # NOTE: urmatorii parametri sunt utilizati pentru a obtine valori implicite (default) atunci cind nu sunt gasite anumite date / informatii.
 #   Uzual ei sunt folositi de comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
 ---------------------------------------------------------------------------------------------------------------------------"""
 
 # --- coeficientul TVA implicit
@@ -42,14 +45,15 @@
 DEFAULT_CURRENCY: str = "RON"
 
 # --- tara implicita
 # aceste constante sunt utilizate ca si tara implicita pentru "parterii" facturilor in condtiile in care tarile "parterilor" nu sunt gasite
 # in mod explicit pe factura (in zona de adresa). Prin sintagma "partener" pe factura sa intelege oricare din cele doua parti implicate in
 # procesul de facturare, si anume: FURNIZORUL si CLIENTUL
 DEFAULT_CUSTOMER_COUNTRY: str = "RO"
+# ...and the corresponding one for supplier
 DEFAULT_SUPPLIER_COUNTRY: str = "RO"
 
 
 """---------------------------------------------------------------------------------------------------------------------------
 # NOTE: "pattern-uri" (sabloane) de identificare si regasire a datelor folositi de
 #   comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
 ---------------------------------------------------------------------------------------------------------------------------"""
@@ -174,77 +178,25 @@
 # pattern utilizat pentru regasirea numelui legal al furnizorului
 # NOTE se presupune a fi la inceputul zonei cu datele furnizorului, deci se ca cauta dupa acelasi pattern
 PATTERN_FOR_SUPPLIER_LEGAL_NAME = PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
 
 
 
 
+# ------- NOTE: the following code runs unconditionally at module import
 
-
-
-
-
-
-# ----------------------------------------------------------
-# here start the code section where external data is get
-
-# settings to differently treat single EXE vs other application types
-frozen_sexe = getattr(sys, 'frozen', False)
-if frozen_sexe:
-    app_dir = sys._MEIPASS
-else:
-    app_dir = os.path.dirname(os.path.abspath(__file__))
-crt_dir = Path.cwd()
-
-# get & render rules text from markdown file. Available ONLY for applications non standalone-EXE
-if not frozen_sexe:
-    rules_file = Path(
-        app_dir,
-        "data/README_app_config_rules.md"
-    )
-    rules_content = Markdown(rules_file.read_text())
-else:
-    rules_content = Markdown(
-        "***WARNING NOTE: **Rules cannot be displayed for standalone exe application**. Please visit the application site: *`http://invoicetoroefact.renware.eu`*."
-    )
-
-# read app_settings.yml. Use below order to apply
-'''Specs: order to search and load for `app_config.yml`. Rule: First found win:
-    * (1) crt directory (with `cwd`) with `Path(Path.cwd(), "data/app_settings.yml")`
-    * (2) package / application directory and file with `Path(os.path.dirname(__file__), "data/app_settings.yml")`
-    * (3) settings from `config_settings.py`
-'''
-# order method (1) - method apply for all application types
-config_file = Path(
-    crt_dir,
-    "app_settings.yml"
-)
-ok_to_use = config_file.exists() and config_file.is_file()
-python_object = None  # suppose no info found
-if ok_to_use:
-    yaml_in = config_file.read_text()
+# section to read settings from external data file
+file_to_use = hier_get_data_file("app_settings.yml")
+python_object = None  # suppose no settings loaded
+if file_to_use:
+    yaml_in = file_to_use.read_text()
     python_object = yaml.safe_load(yaml_in)
-    print("***INFO: Application settings loaded from current directory (local settings).")
-
-# order method (2) - method apply ONLY for applications non standalone-EXE
-if not frozen_sexe:
-    if python_object is None:  # exec only if previous method did not read something
-        config_file = Path(
-            app_dir,
-            "data/app_settings.yml"
-        )
-        ok_to_use = config_file.exists() and config_file.is_file()
-        python_object = None  # suppose no info found
-        if ok_to_use:
-            yaml_in = config_file.read_text()
-            python_object = yaml.safe_load(yaml_in)
-            print("***INFO: Application settings loaded from installation directory (global settings).")
-
-# assign `python_object` to locals() environment
-if python_object is not None:  # exec only if previous method has been read something
+    print("***INFO: Application settings loaded from file.")
+# assign `python_object` to locals() environment...
+if python_object is not None:  # ...only if previous method has read something
     locals().update(python_object)
-else:  # if none of previous methods applied then will remain the content hard-coded in this module
+else:  # if nothing or wrong read from previous method, settings applied will remain to values hard-coded in this module
     print("***INFO: Application settings loaded from application code (default settings).")
```

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/data/README_app_config_rules.md` & `xl2roefact-0.5.4/xl2roefact/data/README_app_config_rules.md`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/data/app_settings.yml` & `xl2roefact-0.5.4/xl2roefact/data/app_settings.yml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/ldxml.py` & `xl2roefact-0.5.4/xl2roefact/ldxml.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/libutils.py` & `xl2roefact-0.5.4/xl2roefact/libutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,49 +7,98 @@
 * author: Petre Iordanescu (petre.iordanescu@gmail.com)
 
 Components:
 
 * `complete_sexe_file() -> bool`: Rename and move resulted exe file (called from `build_sexe` script)
 * `dict_sum_by_key(dict, str) -> float`: Sum a dictionary for a given key at all depth levels
 * `find_str_in_list(list, list) -> int`: Search more strings (ie, a list) in list of strings
+* `hier_get_data_file(file_name: str) -> Path`: Get `Path(file_name)` from hierarchy of locations
 * `invoice_taxes_summary(list[dict]) -> dict`: Calculates invoice taxes summary as required by ROefact requirements
 * `isnumber(str) -> bool`: Test a string if it could be used as number (int or float)
 
 """
 
 import sys
+import os
 from rich import print
 from fractions import Fraction
 import copy
 from xl2roefact.__version__ import normalized_version
 from pathlib import Path
 import shutil
 
 
 
 
+# NOTE: rdy, unit test PASS @240401
+def hier_get_data_file(
+    file_name: str
+) -> Path | None:
+    """Get `Path(file_name)` from hierarchy of locations: (1) current directory, (2) package `data/` directory, (3) `None` is file does not exists in 1 or 2 locations.
+    
+    Args:
+    
+        `file_name`: the name of the file to be returned as full path
+    
+    Return:
+    
+        `Path`: path of file if was found in (1) or (2) locations or `None` if not found
+    """
+    # settings to differently treat single EXE vs other application types
+    frozen_sexe = getattr(sys, 'frozen', False)
+    if frozen_sexe:
+        app_dir = sys._MEIPASS
+    else:
+        app_dir = os.path.dirname(os.path.abspath(__file__))
+    crt_dir = Path.cwd()
+    # first search in current directory
+    file_to_find = Path(
+        crt_dir, file_name
+    )
+    ok_to_use = file_to_find.exists() and file_to_find.is_file()
+    if ok_to_use:
+        return file_to_find
+    # second search in application directory
+    file_to_find = Path(
+        app_dir, "data/", file_name
+    )
+    ok_to_use = file_to_find.exists() and file_to_find.is_file()
+    if ok_to_use:
+        return file_to_find
+    # if both searches failed will return None
+    return None
+
+
+
+
+
 # NOTE: rdy, unit test PASS @240309
 def complete_sexe_file(
     drop_source: bool = True
 ) -> bool:
     """Rename and move resulted exe file. This function is dedicated only to development phase, so various objects are hard coded.
 
-    * Specs: file to process `.../dist_sexe/xl2roefact_to_update_name.exe` --> `.../dist/xl2roefact-version-win64.exe
-    * NOTE: all function code suppose that current directory is root of `xl2roefact`, ie where is located `pyproject.toml` of package
+    Specs:
+
+    * `file to process `.../dist_sexe/xl2roefact_to_update_name.exe` --> `.../dist/xl2roefact-version-win64.exe
+    * Note 1: all function code suppose that current directory is root of `xl2roefact`, ie where is located `pyproject.toml` of package
 
     Args:
+    
         `drop_source`: indicate to delete source file after copying, ie make a "move" operation, otherwise make a copy keeping the source file. Default behaviour is to delete source.
+    
     Return:
+    
         `bool`: True if file was found, renamed and moved with no error
     """
     process_stat = False
     # get canonical version string
     canonical_version = str(normalized_version())
     # construct a Path() type for source
-    source_file = Path("./dist_sexe/xl2roefact_to_update_name.exe")
+    source_file = Path("./dist_sexe/xl2roefact.exe")
     # construct a Path() type for for destination
     dest_file = Path(f"./dist/xl2roefact-{canonical_version}-win64.exe")
     # mv source file to dest using new name. If destination exists is replaced
     tstdst = bool(dest_file.is_file() and dest_file.exists())
     tstsrc = bool(source_file.is_file() and source_file.exists())
     if not tstsrc:  # we have no work object. exit with False
         return False
@@ -69,17 +118,19 @@
 # NOTE: ready, unit test PASS @240305
 def invoice_taxes_summary(
     invoice_lines: list[dict]
 ) -> list:
     """Calculates invoice taxes summary as required by ROefact requirements.
 
     Args:
+    
         `invoice_lines`: section with item lines from 'big' invoice dictionary
 
     Return:
+    
         `list`: usable for "cac_TaxSubtotal" key
     """
     copyof_invoice_lines = copy.deepcopy(invoice_lines)[0]  # make a copy and keep only real-effective list (first item of)
     tmp_InvoiceLine_dict = dict()
     tmpCompondedVAT_list = list()  # intended to keep found `VAT_types-Percent` combinations (ie, to do opera SQL-UPSERT like)
     for item_info in copyof_invoice_lines:
         req_item_info = dict()
@@ -123,18 +174,20 @@
 def dict_sum_by_key(
     search_dict: dict | list[dict],
     sum_key: str
 ) -> float:
     """Sum all dictionary (or list off dictionaries) items, at all levels, for a given key.
 
     Args:
+    
         `search_dict`: dictionary to be searched for
         `sum_key`: key to be searched
 
     Return:
+    
         `float`: with required sum
     """
     s = 0
     if isinstance(search_dict, list) or isinstance(search_dict, tuple):
         for local_search_dict in search_dict:
             for k in local_search_dict:
                 if isinstance(local_search_dict[k], dict):
@@ -157,17 +210,19 @@
 
 
 # NOTE: ready, test PASS @231123
 def isnumber(a_string: str) -> bool:
     """test if a string is valid as any kind of number.
 
     Args:
+    
         `a_string`: input string.
 
     Return:
+    
         `True`: if input string is valid as any kind of number, orherwise `False`.
     """
     try:
         float(a_string)
         return True
     except ValueError:
         try:
@@ -179,18 +234,20 @@
 
 
 # NOTE: ready, test PASS @231123
 def find_str_in_list(list_of_str_to_find: list, list_to_search: list) -> int:
     """find a substring from `list_of_str_to_find` in elements of `list_to_search`.
 
     Args:
+    
         `list_of_str_to_find`: list of strings to search for.
         `list_to_search`: liste where to search for substrings.
 
     Return:
+    
         `index`: the index of list item which contains `str_to_find` (first found) or `None` if not found.
     """
     __found = False
     for __crt_str_to_search_for in list_of_str_to_find:
         __tmp_list = [
             x.find(str(__crt_str_to_search_for))
             for i, x in enumerate(
```

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/rdinv.py` & `xl2roefact-0.5.4/xl2roefact/rdinv.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 import os, sys
 from datetime import datetime, timezone, tzinfo
 from rich import print
 import copy
 from rich.pretty import pprint
 from string import ascii_lowercase
 import json
+import yaml
 from typing import Callable, Any
 from functools import partial
+from pathlib import Path
 import pylightxl as xl
 import openpyxl as opnxl
 
 # local modules (part of package), application misc/general utilities
 from .libutils import isnumber
 from .libutils import find_str_in_list
 from .libutils import dict_sum_by_key
 from .libutils import invoice_taxes_summary
+from .libutils import hier_get_data_file
 from . import config_settings  # application configuration parameters
 
 __all__ = ["rdinv"]  # limit what symbols to be available when import all/full module as `from xl2roefact.rdinv import *`
 
 # local constants. Change them with caution only for a functional objective
 SYS_FILLED_EMPTY_CELL = "_sys_keep_cell"
 
@@ -68,31 +71,36 @@
 PATTERN_FOR_SUPPLIER_LEGAL_NAME = config_settings.PATTERN_FOR_SUPPLIER_LEGAL_NAME
 
 
 def rdinv(
     file_to_process: str,
     invoice_worksheet_name: str = None,
     *,
-    debug_info: bool = False
+    debug_info: bool = False,
+    owner_datafile: Path = None
 ) -> dict:
     """read Excel file for invoice data.
 
-    Produce a dictionary structure + JSON file with all data regarding read invoice: canonical KV data, meta data, map to convert to XML and original Excel data.
+    Produce a dictionary structure + JSON file with all data regarding read invoice: canonical KV data, meta data, map to convert to XML and original Excel data.
+
+    Args:
 
-    Args:
         `file_to_process`: the invoice file (exact file with path).
         `invoice_worksheet_name`: the worksheet containing invoice, optional, defaults to first found worksheet.
         `debug_info`: key only, show debugging information, default `False`.
+        `owner_datafile`: specify a file to read supplier data from, default `None` meaning to read supplier data from Excel file
 
     Return:
-        `dict`: the invoice extracted information from Excel file as `dict(Invoice: dict, meta_info: dict, excel_original_data: dict)`
+    
+        `dict`: the invoice extracted information from Excel file as `dict(Invoice: dict, meta_info: dict, excel_original_data: dict)`
+
+    Notes:
 
-    NOTE ref important variables:
-        * `db: pylightxl object`: EXCEL object with invoice (as a whole)
-        * `ws: pylightxl object`: WORKSHEET object with invoice
+    * `db: pylightxl object`: EXCEL object with invoice (as a whole)
+    * `ws: pylightxl object`: WORKSHEET object with invoice
     """
     # use as global only for those constants that could be changed by this function
     global DEFAULT_VAT_PERCENT
     global DEFAULT_UNKNOWN_ITEM_NAME
     global DEFAULT_UNKNOWN_UOM
     global DEFAULT_CURRENCY
     global DEFAULT_SUPPLIER_COUNTRY
@@ -136,15 +144,15 @@
         )  # here you still need to construct `_found_cell_for_invoice_items_area_marker = (row, col, val)` as it is used in prev code (before `231220piu_a` change)
     else:
         print(f"[red]***FATAL ERROR - Cannot find a relevant cell where invoice items table start (basically containing string \" crt\"). File processing terminated[/]")
         return False
     keyword_for_items_table_marker = _found_cell_for_invoice_items_area_marker[2]
 
     # detect all cells that should be filled with SYS_FILLED_EMPTY_CELL (these are cells id merged groups where first cell in merged group is relevant (diff from empty))
-    detected_cells_which_will_be_fake_filled = _get_merged_cells_tobe_changed(
+    detected_cells_which_will_be_fake_filled = get_merged_cells_tobe_changed(
         file_to_scan=file_to_process,
         invoice_worksheet_name=invoice_worksheet_name,
         keep_cells_of_items_ssd_marker=_found_cell_for_invoice_items_area_marker)  # this call specify to keep unchanged that cells with some description
     for _cell_index in detected_cells_which_will_be_fake_filled:  # scan all detectected cell and change them
         _cell_row = _cell_index[0]
         _cell_col = _cell_index[1]
         ws.update_index(row = _cell_row, col = _cell_col, val = SYS_FILLED_EMPTY_CELL)
@@ -228,31 +236,38 @@
     _ = get_partner_data(
         partner_type="CUSTOMER",
         wks=ws,
         param_invoice_header_area=invoice_header_area
     )
     #
     # get and solve `invoice_header_area` for all SUPPLIER data
-    _ = get_partner_data(
-        partner_type="SUPPLIER",
-        wks=ws,
-        param_invoice_header_area=invoice_header_area
-    )
+    if owner_datafile is None:  # get supplier data from Excel file
+        _ = get_partner_data(
+            partner_type="SUPPLIER",
+            wks=ws,
+            param_invoice_header_area=invoice_header_area
+        )
+    else:  # get supplier data from `owner-data-file`
+        _ = get_partner_data(
+            partner_type="OWNER",
+            wks=ws,
+            param_invoice_header_area=invoice_header_area,
+            supplier_datafile=owner_datafile
+        )
     #
-    # TODO: ... mai sunt ai cele "pre-stabilite" in versiunea curenta, gen `cbc:InvoiceTypeCode = 380`
-
+    # TODO: ... mai sunt ai cele "pre-stabilite" in versiunea curenta, gen `cbc:InvoiceTypeCode = 380`. SEE ALSO line 331
 
     """#NOTE: section to ( Excel data )--->( JSON ) format preparation and finishing
         this is required to be after header determination (because CURRENCY could be known here and will impact config param `DEFAULT_CURRENCY`)
     """
     # transform `invoice_items_area` in "canonical JSON kv pairs format" (NOTE this step is done only for invoice_items_area and is required because this section is "table with more rows", ie, not a simple key-val)
     invoice_items_as_kv_pairs = mk_kv_invoice_items_area(invoice_items_area_xl_format=invoice_items_area)
 
     # preserve processed Excel file meta information: start address, size.
-    meta_info = _build_meta_info_key(
+    meta_info = build_meta_info_key(
         excel_file_to_process=file_to_process,
         invoice_worksheet_name=invoice_worksheet_name,
         ws_size=tuple(ws.size),
         keyword_for_items_table_marker=keyword_for_items_table_marker,
         found_cell=tuple(_found_cell_for_invoice_items_area_marker))
 
     # build final structure to be returned (`invoice`) - MAIN OBJECTIVE of this function
@@ -312,15 +327,15 @@
                 "cbc_TaxInclusiveAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"] + tmp_reusable_items["LineVatAmount"], 2),
                 "cbc_PayableAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"] + tmp_reusable_items["LineVatAmount"], 2),
             },
             "cac_TaxTotal": {
                 "cbc_TaxAmount": round(sum([i["cbc_TaxAmount"] if i["cbc_TaxAmount"] is not None else 0 for i in tmp_cac_TaxSummary]), 2),
                 "cac_TaxSubtotal": copy.deepcopy(tmp_cac_TaxSummary),
             },
-            # TODO: ... chk for remained structure values and check XLM-JSON map
+            # TODO: ... chk for remained structure values and check XLM-JSON map. SEE ALSO line 254
         },
         "meta_info": copy.deepcopy(meta_info),
         "excel_original_data": dict(
             invoice_items_area = copy.deepcopy(invoice_items_area),  # NOTE ready, test PASS @ 231205 by [piu]
             invoice_header_area = copy.deepcopy(invoice_header_area),  # NOTE ready, test PASS @ 2440326 by [piu]
             invoice_footer_area = copy.deepcopy(invoice_footer_area)  #TODO wip... TBD-(cac_TaxTotal) / RDY-(cac_LegalMonetaryTotal
         ),
@@ -358,27 +373,30 @@
     area_to_scan: list[list[int]] = None,
     targeted_type: Callable = str,
     down_search_try: bool = True
 ) -> dict:
     """get "one key Excel values", like invoice number or invoice issue date.
 
     Args:
+    
         `pattern_to_search_for`: for example for inv number, will pass the `PATTERN_FOR_INVOICE_NUMBER_LABEL`.
         `worksheet`: the worksheet containing invoice (as object of `pyxllight` library).
         `area_to_scan`: area of cells to be searched, default whole worksheet.
         `targeted_type`: what type expect (will try to convert to, if cannot will return str), default `str`.
         `down_search_try`: establish if DOWN search method is tried, default `True`.
 
     Return:
+    
         `None` if not found OR `dictionary` containing:
             * `"value": int | float | str` - the value found covenrted to requested `targeted_type` if possible or `str` otherwise; if "out of space" then returns `None`
             * `"location": (row, col)` - adrees of cell where found value
 
     Notes:
-        * normal scan order is 1.RIGHT, 2.DOWN (if allowed), 3.IN-LABEL only in given area and pattern.
+    
+    * normal scan order is 1.RIGHT, 2.DOWN (if allowed), 3.IN-LABEL only in given area and pattern.
     """
     def __check_value(val: Any) -> bool:
         """ return `True` if a `val` is different of None or empty string or SYS_FILLED_EMPTY_CELL, otherwise return `False`
         """
         if val is None:
             return False
         if isinstance(val, str) and val.strip() == "":
@@ -458,21 +476,24 @@
 
 
 # NOTE: ready, test PASS @ 231126 by [piu]
 def mk_kv_invoice_items_area(invoice_items_area_xl_format) -> dict:
     """transform `invoice_items_area` in "canonical JSON format" (as kv pairs).
 
     Args:
+    
         `invoice_items_area_xl_format`: invoice items area in Excel format (ie, DataFrame with row, col, data).
 
     Return:
+    
         `invoice_items_area_xl_format`: dictionary with invoice items in Excel format (ie, rows, columns).
 
     Notes:
-        * for ROefact XML model (& plan) see `invoice_files/__model_test_factura_generat_anaf.xml`.
+    
+    * for ROefact XML model (& plan) see `invoice_files/__model_test_factura_generat_anaf.xml`.
     """
     _invoice_items_data_key = copy.deepcopy(invoice_items_area_xl_format["data"])
     _invoice_items_cols_key = copy.deepcopy(invoice_items_area_xl_format["keycols"])
     _invoice_items_rows_key = copy.deepcopy(invoice_items_area_xl_format["keyrows"])
 
     _invoice_items_area_json_format = list()
     for _i, _line in enumerate (_invoice_items_rows_key):
@@ -569,26 +590,29 @@
     worksheet,
     invoice_items_area_marker,
     wks_name
 ) -> dict:
     """get invoice for `invoice_items_area`, process it and return its Excel format.
 
     Process steps & notes:
-        * find invoice items subtable.
-        * clean invoice items subtable.
-        * extract relevenat data.
-        * NOTE: all Excel cell addresses are in `(row, col)` format (ie, Not Excel format like "A:26, C:42, ...")
+    
+    * find invoice items subtable.
+    * clean invoice items subtable.
+    * extract relevenat data.
+    * NOTE: all Excel cell addresses are in `(row, col)` format (ie, Not Excel format like "A:26, C:42, ...")
 
     Args:
+    
         `worksheet`: the worksheet containing invoice (as object of `pyxllight` library).
         `invoice_items_area_marker`: string with exact marker of invoice items table.
             NOTE: this is the UPPER-LEFT corner and is determined before calling this procedure.
         `wks_name`: the wroksheet name (string) of the `worksheet` object.
 
     Return:
+    
         `invoice_items_area`: dictionary with invoice items in Excel format (ie, rows, columns).
     """
     # obtain table with invoice items ==> `invoice_items_area`
     invoice_items_area = worksheet.ssd(keycols = invoice_items_area_marker, keyrows = invoice_items_area_marker)
     if (invoice_items_area is None or ((isinstance(invoice_items_area, list)) and len(invoice_items_area) < 1)):  # there was not detected any area candidate to "invoice items / lines", so will exit rasing error
         print(f"[red]***FATAL ERROR - Cannot find any candidate to for invoice ITEMS. Worksheet - \"{wks_name}\" in Module [red] RDINV (code-name: `rdinv`). File processing terminated[/]")
         return False
@@ -658,35 +682,38 @@
 
 
 
 
 
 
 # NOTE: ready, test PASS @ 231111 by [piu]
-def _get_merged_cells_tobe_changed(
+def get_merged_cells_tobe_changed(
     file_to_scan,
     invoice_worksheet_name,
     keep_cells_of_items_ssd_marker = None
 ) -> list:
     """scan Excel file to detect all merged ranges.
 
     Args:
+    
         `file_to_scan`: the excel file to be scanned.
         `invoice_worksheet_name`: the worksheet to be scanned.
         `keep_cells_of_items_ssd_marker`: tuple with cells that will be marked IN ANY CASE to be preserved:
             * use case: to keep all potential invoice items ssd rows.
             * format: `tuple(row, col, val)` where row & col are relevant here
             * default: `None`
 
     Return:
+    
         `cells_to_be_changed`: list with cells that need to be chaged in format `(row,col)`.
 
     Notes:
-        * function is intended to be used ONLY internal in this module.
-        * use `openpyxl` library to do its job.
+    
+    * function is intended to be used ONLY internal in this module.
+    * use `openpyxl` library to do its job.
     """
     all_detected_ranges = []
     # open Excel file & worksheet
     workbook_opnxl= opnxl.load_workbook(file_to_scan)
     worksheet_opnxl = workbook_opnxl[invoice_worksheet_name]
     all_detected_ranges = worksheet_opnxl.merged_cells.ranges  # get all merged ranges
     _cells_to_be_changed = list()  # will retaing cells that should be marked with SYS_FILLED_EMPTY_CELL
@@ -731,36 +758,39 @@
 
 
 
 
 
 
 # NOTE: ready, test PASS @ 231127 by [piu]
-def _build_meta_info_key(
+def build_meta_info_key(
     excel_file_to_process: str,
     invoice_worksheet_name: str,
     ws_size: list,
     keyword_for_items_table_marker: str,
     found_cell: list
 ) -> dict:
     """build meta_info key to preserve processed Excel file meta information: start address, size.
 
     Notes:
-        1: all cell addresses are in format (row, col) and are absolute (ie, valid for whole Excel file) #TODO subject of documentation update.
-        2: this function is designed to be used internally by current module (using outside it is not guaranteed for information 'quality').
+    
+    * (1.) all cell addresses are in format (row, col) and are absolute (ie, valid for whole Excel file).
+    * (2.) this function is designed to be used internally by current module (using outside it is not guaranteed for information 'quality').
 
     Args:
+    
         `excel_file_to_process`: name of file to process as would appear in `meta_info` key.
         `invoice_worksheet_name`: the worksheet name as would appear in `meta_info` key.
         `ws_size`: worksheet size as would appear in `meta_info` key (index 0 max rows, index 1 max columns).
         `keyword_for_items_table_marker`: the content of cell used as start of invoice items subtable as would appear in `meta_info`.
         `found_cell`: position of cell used as start of invoice items subtable as would appear in `meta_info` key (index 0 row, index 1 column).
 
-    Return:
-        `meta_info` dictionary built with meta information to be incorpoarted in final invoice dict
+    Returns:
+    
+        `meta_info`: dictionary built with meta information to be incorpoarted in final invoice dict
     """
     _tmp_meta_info = dict()
 
     _tmp_meta_info["file"] = os.path.basename(excel_file_to_process)
     _tmp_meta_info["file_CRC"] = "...file CRC (uniquely identify the invoice file used)"  #TODO to be done... #NOTE this calculation should be done as last step after final XLSX file writing
     _tmp_meta_info["last_processing_time"] = datetime.now(timezone.utc).isoformat()  # set to ISO 8601 format
     _tmp_meta_info["invoice_worksheet"] = invoice_worksheet_name
@@ -826,31 +856,39 @@
     return copy.deepcopy(_tmp_meta_info)
 
 
 
 
 
 
-# NOTE: ready, test PASS @ 240325 by [piu]
+# NOTE: ready, test PASS @ 240404 by [piu]
 def get_partner_data(
-    partner_type: str,  # IN
+    partner_type: str,
     *,
-    wks,  # INOUT
-    param_invoice_header_area: dict  # INOUT
+    wks,
+    param_invoice_header_area: dict,
+    supplier_datafile: Path = None
 ) -> None:
     """Get invoice partener data from Excel.
 
-    For developers note: function works by generating side effects and must be located in `rdinv.py`
+    Notes:
+    
+    * *for developers*: function works by generating side effects and must be located in `rdinv.py`
+    * *side effects*: this function works by directly modifying `param_invoice_header_area` sent parameter
+    * *supplier_datafile exception*: if file is not found or cannot be read, this function will force complete application termination (`sys.exit`)
 
     Args:
+    
         `partner_type`: one of "CUSTOMER", "SUPPLIER" or "OWNER" to specify for what kind of parner get data. The value "OWNER" is designed to get data from an outside database / file (master data)
         `wks`: current work-on `pylightxl Worksheet` object
-        `param_invoice_header_area`: outside `param_invoice_header_area` as used and needed in `rdinv()`. This function will write back in this variable
+        `param_invoice_header_area`: _mode IN-OUT_, outside `param_invoice_header_area` as used and needed in `rdinv()`. This function will write back in this variable
+        `supplier_datafile`: for `partner_type = "CUSTOMER"` here is expected the file where to get supplier data
 
     Return:
+    
         `None`: all data is produced directly in parameters as side effect
     """
     # set variables constant-like suspected to be changed as global
     global DEFAULT_CUSTOMER_COUNTRY
     global DEFAULT_SUPPLIER_COUNTRY
     # normalize partner_type for easier usage and more flexibility to developers misusing
     partner_type = partner_type.upper().strip()
@@ -863,17 +901,75 @@
     elif partner_type =="SUPPLIER":
         # NOTE: pls be patient. Here will raise errs because used EXPECTED constant names. Check `config_settings.py` and adjust accordingly
         UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER = PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
         UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME = PATTERN_FOR_SUPPLIER_LEGAL_NAME
         UNIF_DEFAULT_PARTNER_COUNTRY = DEFAULT_SUPPLIER_COUNTRY
         unif_partner_area_key = "supplier_area"
     elif partner_type == "OWNER":  # subject to load SUPPLIER data from external data source
-        ...  # TODO: get OWNER EXTERNAL DATA feature code here
-    else:
-        # accept only known operations
+        unif_partner_area_key = "supplier_area"
+        # safe read data from `supplier_datafile` file only if it exists
+        file_ok = supplier_datafile.exists() and supplier_datafile.is_file()
+        if file_ok:
+            yaml_in = supplier_datafile.read_text()
+            suppl_data_read = yaml.safe_load(yaml_in)
+        else:
+            print(f"[red]ERROR: Owner / Supplier data file ([cyan]{supplier_datafile}[/]) cannot be read. Process terminated.[/].")
+            sys.exit()
+        supplier_datafile_name = str(supplier_datafile)
+        # save info about area to search as external file and its name
+        param_invoice_header_area[unif_partner_area_key] = {
+            "area_info": {
+               "value": supplier_datafile_name,
+                "location": "external file",
+            }
+        }
+        # CUI
+        param_invoice_header_area[unif_partner_area_key]["CUI"] = {
+            "value": suppl_data_read["PartyLegalEntity"]["CompanyID"],
+            "location": "external file (PartyLegalEntity -> CompanyID)",
+            "label_value": None,
+            "label_location": None
+        }
+        # RegName
+        param_invoice_header_area[unif_partner_area_key]["RegistrationName"] = {
+            "value": suppl_data_read["PartyLegalEntity"]["RegistrationName"],
+            "location": "external file (PartyLegalEntity -> CompanyID)",
+            "label_value": None,
+            "label_location": None
+        }
+        # PostalAddress
+        param_invoice_header_area[unif_partner_area_key]["PostalAddress"] = {
+            "cbc_StreetName": suppl_data_read["PostalAddress"]["StreetName"],
+            "cbc_CityName": suppl_data_read["PostalAddress"]["CityName"],
+            "cbc_PostalZone": suppl_data_read["PostalAddress"]["PostalZone"],
+            "cac_Country": { "cbc_IdentificationCode": suppl_data_read["PostalAddress"]["CountryCode"] },
+        }
+        # Bank, Tax & Contact
+        param_invoice_header_area[unif_partner_area_key]["reg_com"] = {
+            "value": suppl_data_read["PartyTaxScheme"]["CompanyID"],
+            "location": "external file (PartyLegalEntity -> CompanyID)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["phone"] = {
+            "value": suppl_data_read["Contact"]["Telephone"],
+            "location": "external file (Contact -> Telephone)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["email"] = {
+            "value": suppl_data_read["Contact"]["ElectronicMail"],
+            "location": "external file (Contact -> ElectronicMail)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["bank"] = {
+            "value": suppl_data_read["Contact"]["Bank"],
+            "location": "external file (Contact -> Bank)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["IBAN"] = {
+            "value": suppl_data_read["Contact"]["IBAN"],
+            "location": "external file (Contact -> IBAN)"
+        }
+        return
+    else:  # accept only known operations
         raise Exception("partner_type parameter not recognized value")
     #
     # find invoice partner ==> one of (cac:AccountingCustomerParty , cac:AccountingSupplierParty)
     invoice_partner_info = get_excel_data_at_label(
         pattern_to_search_for=UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER,  # NOTE: constant adjusted in refactoring process
         worksheet=wks,
         area_to_scan=(param_invoice_header_area["start_cell"], param_invoice_header_area["end_cell"]),
@@ -1006,15 +1102,14 @@
     _tmp_email = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_EMAIL)
     # store "full" variables in `partner_area...` for excel original values
     param_invoice_header_area[unif_partner_area_key]["reg_com"] = _tmp_reg_com
     param_invoice_header_area[unif_partner_area_key]["bank"] = _tmp_bank
     param_invoice_header_area[unif_partner_area_key]["IBAN"] = _tmp_IBAN
     param_invoice_header_area[unif_partner_area_key]["phone"] = _tmp_phone
     param_invoice_header_area[unif_partner_area_key]["email"] = _tmp_email
-
     return
```

### Comparing `xl2roefact-0.5.3rc1/xl2roefact/wrxml.py` & `xl2roefact-0.5.4/xl2roefact/wrxml.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.3rc1/PKG-INFO` & `xl2roefact-0.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2roefact
-Version: 0.5.3rc1
+Version: 0.5.4
 Summary: Excel invoices data retrieve, export & upload to RO E-Fact system
 Author-Email: Petre Iordanescu <petre.iordanescu@gmail.com>, RENware Software Systems <renware.systems@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -729,17 +729,17 @@
 
 # xl2roefact
 
 ![Static Badge](https://img.shields.io/badge/version-{{ xl2roefact_version }}-blue)
 
 Legaturi externe utile:
 
-* [**Site dedicat**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
-* [Pachet pe *PyPi*](https://pypi.org/project/xl2roefact/)
-* [Surse pe *GitHub*](https://github.com/petre-renware/api_to_roefact/)
+* [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
+* [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
+* [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
 * [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
 * [Referinta *API*](./doc/810.05a-xl2roefact_DLD_specs.md)
 
 
 
 ## Facilitati
 
@@ -751,43 +751,34 @@
 ![Static Badge](https://img.shields.io/badge/format_JSON-YES-orange)
 ![Static Badge](https://img.shields.io/badge/format_XML-YES-orange)
 ![Static Badge](https://img.shields.io/badge/format_PDF-YES-orange)
 ![Static Badge](https://img.shields.io/badge/format_RO_eFact-YES-red)
 
 
 
-
-
-
-
 Aceasta componenta este "totul despre crearea de facturi electronice" din formatul Excel office (xlsx). Aplicatia poate genera factura in format JSON, XML, PDF si o poate incarca in sistemul *RO E-Fact*[^ld_roefact].
 
 Aceasta componenta ofera urmatoarele facilitati (acestea fiind obiectivele fundamentale ale componentei):
 
 * **transformarea facturilor din Excel in formatul `XML`** cerut de catre sistemul ANAF RO E-Fact pentru incarcare
-
- * **incarcarea acestora** in sistemul ANAF RO E-Fact[^ld_roefact]
-
-*  **transformarea facturilor din Excel intr-un format `JSON`**  intermediar, independent de platforma si care permite integrarea acestora cu alte sisteme (standard *REST*)
-
+* **incarcarea acestora** in sistemul ANAF RO E-Fact[^ld_roefact]
+* **transformarea facturilor din Excel intr-un format `JSON`**  intermediar, independent de platforma si care permite integrarea acestora cu alte sisteme (standard *REST*)
 * **generarea facturii in format PDF** pentru transmiterea acesteia catre client, semnarea electronica, tiparirea si arhivarea acesteia in format fizic (in general manipularea facturii in format *"human readable"*)
 
 Componenta ofera doua instrumente pentru realizarea si indeplinirea acestor obiective:
 
 * `xl2roefact` o **aplicatie de tip linie de comanda** (disponibila pentru sistemele de operare Windows, Linux si MacOS)
-
-* `xl2roefact PyPi` o **blioteca standard Python** utilizabila pentru dezvoltari proprii in scopul extinderii altor sisteme existente (*custom development*)
+* `xl2roefact PyPi` **blioteca standard Python** utilizabila pentru dezvoltari proprii in scopul extinderii altor sisteme existente (*custom development*)
 
 
 
 
 
 
 ## Instalarea aplicatiei xl2roefact
-
 Instalarea aplicatiei *xl2roefact* este disponibila in urmatoarele variante:
 
 * pentru **Windows**:
     * **`MSI`** pachet instalare pentru *Windows*
     * **`EXE`** executabil *Windows in format "portabil" (un singur fisier)*
 
 * pentru **Linux**:
@@ -809,34 +800,32 @@
 * numele pachetelor includ versiunea de aplicatie utilizata si sistemul de operare pentru care sunt disponibile
 * pentru echivalent utilizare  *portabila pentru Linux* se poate instala biblioteca Python dupa care devine utilizabil scriptul Python "ca orice alta comanda Linux"
 
 
 
 
 
-## Configurarea aplicatiei xl2roefact
 
+## Configurarea aplicatiei xl2roefact
 Parametrii de configurare aplicatiei se gasesc in fisierul *`config_settings.py`*. Acestia sunt sub elaborati in limbaj Python prin utilizarea conventiilor de constante conform recomandarilor PEP (numele capitatlizat) si sunt acompaniti de linii de explicatii privind aplicabilitatea lor.
 
 <!--#TODO: prev paragraph to replace new config method by using `app_settings.yml` in current directory -->
 
 Configurare aplicatiei se poate face interactiv si din aplicatie. Pentru a obtine help referitor la detaliile comenzi se va folosi
-```bash
+```shell
 xl2roefact settings --help
 ```
 
 Configurarile existente si regulile recomandate in configurarea aplicatiei se afiseaza folosind comanda:
-```bash
+```shell
 xl2roefact settings --rules
 ```
 
 
 ### Configurarea din fisier extern
-<!--  --Sablon fisier configurare a aplicatiei xl2roefact -->
-
 Configurarea aplicatuiei se poate face si prin intermediul unui fisier extern numit "*sablon de configurare*" (*en: configuration template*). Sablonul permite configurarea aplicatiei prin modificarea fragmentelor de text care trebuiesc cautate in fisierul Excel pentru identificarea diverselor informatii aferente facturii.
 
 Sablonul este in format [YAML](https://yaml.org/) iar informatiile ce trebuiesc descrise sunt explicate individual in comentarii insotitoare.
 De asemenea este util a fi citite si recomandarile date in pagina de descriere a aplicatiei.
 
 Pentru a beneficia de cobfigurarile facute de dumneavoastra trebuie sa creati un fisier **`app_settings.yml`** in directorul curent din care lansati aplicatia, fisier ce contine noile configurari dorite.
 **Numele fisierelui este obligatoriu a fi respectat.**
@@ -851,40 +840,89 @@
     In conditiile folosirii kitului MSI pentru o instalare locala a aplicatiei (cu utilizari multiple si repetate) si in situatia in care se doreste schimbarea configurarii implicite a aplicatiei se vor urma acesti pasi:
     
     * in directorul de instalare a aplicatiei se va crea daca nu exita directorul `data/`
     * in acest director se va crea un fisier `app_settings.yml` cu configurarea globala dorita
     
     Aceasta configurare inlocuieste configurarea implicita si se va aplica global in utilizarea aplicatiei. In continuare configurarile existente in directorul curent *suprascriu configurarea globala* (se aplica cu precedenta).
 
+>[Aici puteti gasiti pentru descarcare un model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact).
+
 
 
->[Aici puteti gasiti pentru descarcare un model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact).
 
 
 
+## Utilizare nomenclator de furnizori
+Aplicatia *xl2roefact* permite utilizarea datelor pentru furnizori din fisiere externe (in locul informatiilor din fisierele Excel) lucru ce poate fi folositor in urmatoarele situatii:
 
+* cind utilizatorul aplicatiei o face in scopuri personale si multe facturi emise il au *pe el ca furnizor*. Aceast lucru permite ca informatia din Excel referitoare la furnizor sa fie sumara sau sa lipseasca, factura finala format `PDF` fiind generata cu aplicatia
+* cind utilizatorul aplicatiei o foloseste pentru a emite facturi pentru alte firme si astfel este mai comod sa foloseasca fisiere cu datele acestor firme decit sa introduca informatia in fiecare factura
+* cind se doreste ca datele furnizorului sa fie preluate dintr-un sistem extern ce le poate exporta ca si fisisre
 
-## Comenzile aplicatiei
 
+### Reguli generale de utilizare
+Aceasta sectiune descrie regulile generale ce trebuiesc avute in vedere pentru o completa si corecta utilizare a facilitatii "Nomenclator furnizori":
+
+* Nomenclatorul de furnizori se va completa intr-unul sau mai multe fisere de date (de tip text, vezi mai jos formatul exact).
+* Un fisier acomodeaza un singur furnizor. Pentru mai multi furnizori se vor folosi fisiere diferite.
+* Numele fisierului (fara extensie) trebuie sa coincida cu o cheie alternativa a furnizorului respectiv. Prin cheie alternativa se intelege acea cheie care este unica si poate asigura regasirea furnizorului prin folosirea ei. Ca si exemple din practicile curente ar fi cimpul numit uzual `code` sau `code_name` existent in mai toate sistemele de business. Acesta are avantajul unicitatii si a unei reprezentari "umane" (*en: human readable*). Desigur un cimp de tip cheie primara / ID este ideal dar de obicei acesta este tehnic iar valoarea sa nu ofera prea multe indicatii.
+* Formatul fisierului este  [YAML](https://yaml.org/) standard, fara folosirea de modele de date complexe, aatfel incit o eventuala conversie `JSON` <--> `YAML` sa poata fi realizata manual in ambele sensuri si fara necessitatea unor cunostinte avansate ci la nivel de redefinire a numelor cheilor.
+
+
+###  Locatia nomenclatorului
+Fisierele cu datele furnizorilor pot sta in urmatoarele locatii:
+
+* *directorul curent* este locatia cu prioritatea maxima si in caz de "duplicate" ale unui fisier, cel de aici va fi luat in considerare
+* *directorul `data/`* din locatia unde este instalata aplicatia
+
+Recomandari si practici uzuale:
+
+* In situatiile in care sistemul este instalat pe un computer ce se foloseste frecvent cu aplicatia *xl2roefact* si exista un set de furnizori frecvent folositi se recomanda folosirea directorului `data/` pentru stocarea fisierelor nomenclator astfel incit sa poata fi refolosite usor.
+* In situatia folosirii a "multe" fisiere date furnizori se recomanda crearea unui director dedicat in locatia utilizata (vezi mai sus) si acesta sa fie referit in numle fisierului.
+
+
+### Utilizarea nomenclatorului
+Pentru a folosi cu aplicatia un fisier tip nomenclator furnizor se va utiliza optiunea:
+```shell
+xl2roefact xl2json -o fisier_furnizor
+```
+unde `fisier_furnizor` este numele fisierului ce contine datele unui furnizor. Locatia acestui fisier este relativa la [locatia considerata pentru folosire](#locatia-nomenclatorului)
+
+
+### Sablon pentru nomenclator de furnizori
+Sablonul este proiectat pentru utilizarea in facturile emise si contine numai informatiile necesare in acest scop.<br>
+Astfel cimpurile existente trebuiesc pastrate, adica nu vor fi sterse.
+
+Vor fi *respectate si completate* corespunzator cimpurile specificate ca *obligatoriii (en: mandatory* in comentariile aferente fiecarui cimp.<br>
+Pentru acele cimpuri pentru care informatia este necunoscuta sau considerata irelevanta se va completa cu `null`.
+
+Se vor putea adauga orice alte cimpuri suplimentare cu conditia sa fie respectat formatul fisierului (`YAML`). acestea nu vor fi folosite de catre aplicatie, ci pur si simplu ignorate.
+
+>[Aici puteti gasiti un model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor).
+
+
+
+
+
+
+## Comenzile aplicatiei
 Interfata aplicatie este realizata utilizind conventiile si practicile uzuale pentru aplicatii tip linie de comanda consola. Pentru informatii privind comenzile se poate folosi optiunea de **help**, dispobilia atit la nivelul general:
-```bash
+```shell
 xl2roefact --help
 ```
 cit si la nivel detaliat pentru fiecare comanda
-```bash
+```shell
 xl2roefact [COMMAND] --help
 ```
 
 
 **Lista comenzilor:**
 
 * **about** - Afiseaza informatii despre aceatsa aplicatie (copyright, scop, etc)
-
 * **settings** _ Afiseaza parametrii de configurare a aplicatiei. [Vezi sectiunea de configurare a aplicatiei](#configurarea-aplicatiei-xl2roefact)
-
 * **xl2json** - Transforma fisierul (fisierele) Excel in forma JSON pentru utilizare ulterioara ca forma de date standardizat pentru schimbul de informatii cu alte sisteme electronice
 
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
@@ -896,15 +934,14 @@
     :depth: 2
 
 
 
 
 
 ## Practici si regului referitoare la continutul facturilor din Excel
-
 Acest capitol se refera la modul in care este "tratat" continutul fisierului Excel cu factura, mai exact la modalitatea in care informatia facturii este cautata, identificata si gasita in scopul de a fi salvata in oricare din formatele de "factura electronica / E-Fact".
 
 Utilizarea sablonului de factura Excel ce este livrat impreuna cu aplicatia **ESTE O VARIANTA DE LUCRU RECOMANDATA**, dar nu obligatorie. Chiar si in cazul utilizarii acestuia, prin modificarea "structurii" acestuia, informatia poate ajunge *nerecognoscibila / neidentificabila* total sau partial daca nu sunt urmate regulile expuse.
 
 >In general trebuie facuta diferenta intre datele facturii si modul in care aceasta va fi tiparita (va aparea la tiparire / previzualizare).
 >
 >Mai exact **continutul informational** al facturii nu trebuie nici confundat si nici mixat cu **formatul de afisare al acesteia** (layout). Pentru acesta din urma se recomanda a fi folosite cu precadere *regulile de formatare* din Excel si nu cele stocare a datelor. Un exemplu este un numar zecimal oarecare unde:
@@ -1005,14 +1042,17 @@
 
 
 ## Descarcare (download) aplicatie xl2roefact CLI
 
 * [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
 * [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
 * [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
+* [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
+
+
 
 
 
 
 ## Date identificare
 
 * part number (p/n): `0000-0095-xl2roefact`
```

