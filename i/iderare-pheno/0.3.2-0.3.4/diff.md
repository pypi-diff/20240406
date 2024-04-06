# Comparing `tmp/iderare-pheno-0.3.2.tar.gz` & `tmp/iderare-pheno-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.3.2.tar", last modified: Sat Apr  6 18:15:20 2024, max compression
+gzip compressed data, was "iderare-pheno-0.3.4.tar", last modified: Sat Apr  6 18:34:39 2024, max compression
```

## Comparing `iderare-pheno-0.3.2.tar` & `iderare-pheno-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:15:20.126692 iderare-pheno-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-06 18:15:20.126692 iderare-pheno-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:15:20.122692 iderare-pheno-0.3.2/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/iderare_pheno/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/simrec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:15:20.122692 iderare-pheno-0.3.2/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:15:20.126692 iderare-pheno-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:34:39.097136 iderare-pheno-0.3.4/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/iderare_pheno/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/simrec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/setup.cfg
```

### Comparing `iderare-pheno-0.3.2/LICENSE` & `iderare-pheno-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.2/PKG-INFO` & `iderare-pheno-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.2
-Author-email: Ivan William Harsono <contact@ivanwilliammd.org>
+Version: 0.3.4
+Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -30,19 +30,20 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Repository, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://iderare-pheno.readthedocs.io/
 Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.2 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.4 Author-email: Ivan
 William Harsono
-ivanwilliammd.org> License: BSD 3-Clause License Copyright (c) 2024, Ivan
-William Harsono Redistribution and use in source and binary forms, with or
-without modification, are permitted provided that the following conditions are
-met: 1. Redistributions of source code must retain the above copyright notice,
-this list of conditions and the following disclaimer. 2. Redistributions in
-binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials
-provided with the distribution. 3. Neither the name of the copyright holder nor
-the names of its contributors may be used to endorse or promote products
-derived from this software without specific prior written permission. THIS
-SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-
-URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
-Repository, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
-Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/
-CHANGELOG.md Classifier: Intended Audience :: Science/Research Classifier:
-Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Programming Language :: Python :: 3 Classifier:
-Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: pandas Requires-Dist: numpy Requires-Dist: matplotlib Requires-Dist:
-scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn Requires-Dist: pyyaml
-Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist:
-mypy<1.10,>=1.0; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
-"dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
-isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
-== "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
-extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
-extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
-extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
-Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-Dist:
-sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist: packaging;
-extra == "dev" # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/) IDeRare
-or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is simple and
-ready to use variant discovery pipeline to discover rare disease variants from
-exome sequencing data.
+gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
+Harsono Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met: 1.
+Redistributions of source code must retain the above copyright notice, this
+list of conditions and the following disclaimer. 2. Redistributions in binary
+form must reproduce the above copyright notice, this list of conditions and the
+following disclaimer in the documentation and/or other materials provided with
+the distribution. 3. Neither the name of the copyright holder nor the names of
+its contributors may be used to endorse or promote products derived from this
+software without specific prior written permission. THIS SOFTWARE IS PROVIDED
+BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED
+WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
+EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: Homepage, https://
+github.com/ivanwilliammd/iderare-pheno Project-URL: Repository, https://
+github.com/ivanwilliammd/iderare-pheno Project-URL: Changelog, https://
+github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md Project-URL:
+Documentation, https://iderare-pheno.readthedocs.io/ Classifier: Intended
+Audience :: Science/Research Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License Classifier: Programming
+Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Medical
+Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist:
+matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn
+Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist:
+black<25.0,>=23.0; extra == "dev" Requires-Dist: black[jupyter]; extra == "dev"
+Requires-Dist: isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra
+== "dev" Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-
+cov; extra == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist:
+build; extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist:
+wheel; extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
+Requires-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-
+parser<2.1,>=1.0; extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra
+== "dev" Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-
+Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist:
+packaging; extra == "dev" # [IDeRare-Pheno](https://iderare-
+pheno.readthedocs.io/) IDeRare or "Indonesia Exome Rare Disease Variant
+Discovery Pipeline" is simple and ready to use variant discovery pipeline to
+discover rare disease variants from exome sequencing data.
              _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
 ## Quick links - [Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI
 Package](https://pypi.org/project/iderare-pheno/) - [License](https://
 github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) - Interactive Webapps
 Implementation of at [Streamlit](https://bioinformatics-
 ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
 script is recommended if you would like to do conversion, linkage analysis,
```

### Comparing `iderare-pheno-0.3.2/README.md` & `iderare-pheno-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.2/iderare_pheno/converter.py` & `iderare-pheno-0.3.4/iderare_pheno/converter.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.2/iderare_pheno/simrec.py` & `iderare-pheno-0.3.4/iderare_pheno/simrec.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.2/iderare_pheno/utils.py` & `iderare-pheno-0.3.4/iderare_pheno/utils.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.2/iderare_pheno.egg-info/PKG-INFO` & `iderare-pheno-0.3.4/iderare_pheno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.2
-Author-email: Ivan William Harsono <contact@ivanwilliammd.org>
+Version: 0.3.4
+Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -30,19 +30,20 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Repository, https://github.com/ivanwilliammd/iderare-pheno
 Project-URL: Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://iderare-pheno.readthedocs.io/
 Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.2 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.4 Author-email: Ivan
 William Harsono
-ivanwilliammd.org> License: BSD 3-Clause License Copyright (c) 2024, Ivan
-William Harsono Redistribution and use in source and binary forms, with or
-without modification, are permitted provided that the following conditions are
-met: 1. Redistributions of source code must retain the above copyright notice,
-this list of conditions and the following disclaimer. 2. Redistributions in
-binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials
-provided with the distribution. 3. Neither the name of the copyright holder nor
-the names of its contributors may be used to endorse or promote products
-derived from this software without specific prior written permission. THIS
-SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-
-URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
-Repository, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
-Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/
-CHANGELOG.md Classifier: Intended Audience :: Science/Research Classifier:
-Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Programming Language :: Python :: 3 Classifier:
-Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: pandas Requires-Dist: numpy Requires-Dist: matplotlib Requires-Dist:
-scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn Requires-Dist: pyyaml
-Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist:
-mypy<1.10,>=1.0; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
-"dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
-isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
-== "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
-extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
-extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
-extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
-Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-Dist:
-sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist: packaging;
-extra == "dev" # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/) IDeRare
-or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is simple and
-ready to use variant discovery pipeline to discover rare disease variants from
-exome sequencing data.
+gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
+Harsono Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met: 1.
+Redistributions of source code must retain the above copyright notice, this
+list of conditions and the following disclaimer. 2. Redistributions in binary
+form must reproduce the above copyright notice, this list of conditions and the
+following disclaimer in the documentation and/or other materials provided with
+the distribution. 3. Neither the name of the copyright holder nor the names of
+its contributors may be used to endorse or promote products derived from this
+software without specific prior written permission. THIS SOFTWARE IS PROVIDED
+BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED
+WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
+EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: Homepage, https://
+github.com/ivanwilliammd/iderare-pheno Project-URL: Repository, https://
+github.com/ivanwilliammd/iderare-pheno Project-URL: Changelog, https://
+github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md Project-URL:
+Documentation, https://iderare-pheno.readthedocs.io/ Classifier: Intended
+Audience :: Science/Research Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License Classifier: Programming
+Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Medical
+Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist:
+matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn
+Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist:
+black<25.0,>=23.0; extra == "dev" Requires-Dist: black[jupyter]; extra == "dev"
+Requires-Dist: isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra
+== "dev" Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-
+cov; extra == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist:
+build; extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist:
+wheel; extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
+Requires-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-
+parser<2.1,>=1.0; extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra
+== "dev" Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-
+Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist:
+packaging; extra == "dev" # [IDeRare-Pheno](https://iderare-
+pheno.readthedocs.io/) IDeRare or "Indonesia Exome Rare Disease Variant
+Discovery Pipeline" is simple and ready to use variant discovery pipeline to
+discover rare disease variants from exome sequencing data.
              _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
 ## Quick links - [Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI
 Package](https://pypi.org/project/iderare-pheno/) - [License](https://
 github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) - Interactive Webapps
 Implementation of at [Streamlit](https://bioinformatics-
 ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
 script is recommended if you would like to do conversion, linkage analysis,
```

### Comparing `iderare-pheno-0.3.2/pyproject.toml` & `iderare-pheno-0.3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 [project]
 # See https://setuptools.pypa.io/en/latest/userguide/quickstart.html for more project configuration options.
 name = "iderare-pheno"
 dynamic = ["version"]
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: Apache Software License",
+    "Development Status :: 4 - Beta",
+    "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Scientific/Engineering :: Medical Science Apps.",
 ]
 authors = [
-    {name = "Ivan William Harsono", email = "contact@ivanwilliammd.org"}
+    {name = "Ivan William Harsono", email = "ivanwilliam.md@gmail.com"}
 ]
 requires-python = ">=3.8"
 dependencies = [
   "pandas",
   "numpy",
   "matplotlib",
   "scipy",
@@ -29,15 +29,15 @@
 ]
 license = {file = "LICENSE"}
 
 [project.urls]
 Homepage = "https://github.com/ivanwilliammd/iderare-pheno"
 Repository = "https://github.com/ivanwilliammd/iderare-pheno"
 Changelog = "https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md"
-# Documentation = "https://iderare-pheno.readthedocs.io/"
+Documentation = "https://iderare-pheno.readthedocs.io/"
 
 [project.optional-dependencies]
 dev = [
     "ruff",
     "mypy>=1.0,<1.10",
     "black>=23.0,<25.0",
     "black[jupyter]",
@@ -68,15 +68,15 @@
     "scripts*"
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
-iderare_pheno = ["py.typed"]
+iderare_pheno = ["phenotype/*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "iderare_pheno.version.VERSION"}
 
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
```

