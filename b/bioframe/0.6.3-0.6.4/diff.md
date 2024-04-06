# Comparing `tmp/bioframe-0.6.3.tar.gz` & `tmp/bioframe-0.6.4.tar.gz`

## Comparing `bioframe-0.6.3.tar` & `bioframe-0.6.4.tar`

### file list

```diff
@@ -1,100 +1,99 @@
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 bioframe-0.6.3/.readthedocs.yaml
--rw-r--r--   0        0        0     7981 2020-02-02 00:00:00.000000 bioframe-0.6.3/CHANGES.md
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 bioframe-0.6.3/CITATION.cff
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 bioframe-0.6.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bioframe-0.6.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 bioframe-0.6.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/_version.py
--rw-r--r--   0        0        0    16622 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/extras.py
--rw-r--r--   0        0        0    64677 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/ops.py
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/vis.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/core/__init__.py
--rw-r--r--   0        0        0    24935 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/core/arrops.py
--rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/core/checks.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/core/construction.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/core/specs.py
--rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/core/stringops.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/__init__.py
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/assembly.py
--rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/fileops.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/resources.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/schemas.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/_assemblies.yml
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/ce10.seqinfo.tsv
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/ce11.seqinfo.tsv
--rw-r--r--   0        0        0    70878 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/danRer10.seqinfo.tsv
--rw-r--r--   0        0        0    66339 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/danRer11.seqinfo.tsv
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/dm3.seqinfo.tsv
--rw-r--r--   0        0        0   161973 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/dm6.seqinfo.tsv
--rw-r--r--   0        0        0    30781 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/hg19.cytoband.tsv
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/hg19.seqinfo.tsv
--rw-r--r--   0        0        0    30775 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/hg38.cytoband.tsv
--rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/hg38.seqinfo.tsv
--rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/hs1.cytoband.tsv
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/hs1.seqinfo.tsv
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/mm10.seqinfo.tsv
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/mm39.seqinfo.tsv
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/mm9.seqinfo.tsv
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/sacCer3.seqinfo.tsv
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/io/data/wuhCor1.seqinfo.tsv
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/sandbox/clients.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/sandbox/gtf_io.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 bioframe-0.6.3/bioframe/sandbox/parquet_io.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/Makefile
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-construction.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-extras.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-fileops.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-intervalops.rst
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-lowlevel.md
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-resources.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-validation.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/api-vis.rst
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/conf.py
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/guide-definitions.rst
--rw-r--r--   0        0        0    16241 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/guide-intervalops.md
--rw-r--r--   0        0        0    13704 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/guide-io.ipynb
--rw-r--r--   0        0        0   374027 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/guide-performance.ipynb
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/guide-quickstart.rst
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/guide-recipes.md
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/guide-specifications.rst
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/make.bat
--rw-r--r--   0        0        0    38715 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/times100.bw
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/._bioframe-logo.png
--rw-r--r--   0        0        0    68759 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/bioframe-logo.png
--rw-r--r--   0        0        0    65297 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/bioframe_closest.pdf
--rw-r--r--   0        0        0    21587 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/closest0.png
--rw-r--r--   0        0        0    56069 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/closest1.png
--rw-r--r--   0        0        0    50871 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/closest2.png
--rw-r--r--   0        0        0    44726 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/closest3.png
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/df1.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/df2.png
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/df@.png
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/merge_df1.png
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/overlap_inner_0.png
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/figs/overlap_inner_1.png
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/lowlevel/arrops.rst
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/lowlevel/specs.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/lowlevel/stringops.rst
--rw-r--r--   0        0        0   272664 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb
--rw-r--r--   0        0        0    72730 2020-02-02 00:00:00.000000 bioframe-0.6.3/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_assembly_info.py
--rw-r--r--   0        0        0    14388 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_core_checks.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_core_construction.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_core_specs.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_core_stringops.py
--rw-r--r--   0        0        0     9025 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_extras.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_fileops.py
--rw-r--r--   0        0        0    60568 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_ops.py
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_ops_select.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_resources.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_vis.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_data/test.chrom.sizes
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_data/test.fa
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bioframe-0.6.3/tests/test_data/test.fa.fai
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 bioframe-0.6.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bioframe-0.6.3/LICENSE
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 bioframe-0.6.3/README.md
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 bioframe-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 bioframe-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 bioframe-0.6.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 bioframe-0.6.4/CHANGES.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 bioframe-0.6.4/CITATION.cff
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 bioframe-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bioframe-0.6.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 bioframe-0.6.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/__init__.py
+-rw-r--r--   0        0        0    16583 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/extras.py
+-rw-r--r--   0        0        0    64680 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/ops.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/vis.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/__init__.py
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/arrops.py
+-rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/checks.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/construction.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/specs.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/stringops.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/__init__.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/assembly.py
+-rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/fileops.py
+-rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/resources.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/schemas.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/_assemblies.yml
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/ce10.seqinfo.tsv
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/ce11.seqinfo.tsv
+-rw-r--r--   0        0        0    70878 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/danRer10.seqinfo.tsv
+-rw-r--r--   0        0        0    66339 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/danRer11.seqinfo.tsv
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/dm3.seqinfo.tsv
+-rw-r--r--   0        0        0   161973 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/dm6.seqinfo.tsv
+-rw-r--r--   0        0        0    30781 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg19.cytoband.tsv
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg19.seqinfo.tsv
+-rw-r--r--   0        0        0    30775 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg38.cytoband.tsv
+-rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg38.seqinfo.tsv
+-rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hs1.cytoband.tsv
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hs1.seqinfo.tsv
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/mm10.seqinfo.tsv
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/mm39.seqinfo.tsv
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/mm9.seqinfo.tsv
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/sacCer3.seqinfo.tsv
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/wuhCor1.seqinfo.tsv
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/sandbox/clients.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/sandbox/gtf_io.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/sandbox/parquet_io.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/Makefile
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-construction.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-extras.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-fileops.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-intervalops.rst
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-lowlevel.md
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-resources.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-validation.rst
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-vis.rst
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/conf.py
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-definitions.rst
+-rw-r--r--   0        0        0    16241 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-intervalops.md
+-rw-r--r--   0        0        0    13704 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-io.ipynb
+-rw-r--r--   0        0        0   374027 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-performance.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-quickstart.rst
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-recipes.md
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-specifications.rst
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/make.bat
+-rw-r--r--   0        0        0    38715 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/times100.bw
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/._bioframe-logo.png
+-rw-r--r--   0        0        0    68759 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/bioframe-logo.png
+-rw-r--r--   0        0        0    65297 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/bioframe_closest.pdf
+-rw-r--r--   0        0        0    21587 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest0.png
+-rw-r--r--   0        0        0    56069 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest1.png
+-rw-r--r--   0        0        0    50871 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest2.png
+-rw-r--r--   0        0        0    44726 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest3.png
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/df1.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/df2.png
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/df@.png
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/merge_df1.png
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/overlap_inner_0.png
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/overlap_inner_1.png
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/lowlevel/arrops.rst
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/lowlevel/specs.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/lowlevel/stringops.rst
+-rw-r--r--   0        0        0   272664 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb
+-rw-r--r--   0        0        0    72730 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_assembly_info.py
+-rw-r--r--   0        0        0    14096 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_checks.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_construction.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_specs.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_stringops.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_extras.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_fileops.py
+-rw-r--r--   0        0        0    69553 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_ops.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_ops_select.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_resources.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_vis.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_data/test.chrom.sizes
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_data/test.fa
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_data/test.fa.fai
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 bioframe-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bioframe-0.6.4/LICENSE
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 bioframe-0.6.4/README.md
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 bioframe-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 bioframe-0.6.4/PKG-INFO
```

### Comparing `bioframe-0.6.3/.readthedocs.yaml` & `bioframe-0.6.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/CHANGES.md` & `bioframe-0.6.4/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 # Release notes
 
-## [Upcoming release](https://github.com/open2c/bioframe/compare/v0.6.3...HEAD)
+## [Upcoming release](https://github.com/open2c/bioframe/compare/v0.6.4...HEAD)
+
+## [v0.6.4](https://github.com/open2c/bioframe/compare/v0.6.3...v0.6.4)
+Date 2024-04-06
+
+Maintenance:
+* Migrate from setuptools `pkg_resources` to `importlib.resources` by @nvictus in https://github.com/open2c/bioframe/pull/194
+* Use `importlib.metadata` for versioning by @nvictus in https://github.com/open2c/bioframe/pull/195
+
+Bug fixes:
+* Overlap point segment patch #183 by @smitkadvani in https://github.com/open2c/bioframe/pull/184
+* #167: Replaced np.int with int as the attribute is deprecated by numpy by @harshit148 in https://github.com/open2c/bioframe/pull/192
+
+New Contributors:
+* @harshit148 made a first contribution in https://github.com/open2c/bioframe/pull/192
+
+**Full Changelog**: https://github.com/open2c/bioframe/compare/v0.6.3...v0.6.4
 
 ## [v0.6.3](https://github.com/open2c/bioframe/compare/v0.6.2...v0.6.3)
 Date 2024-03-11
 
 Fixes:
 * Prevent dropout from `closest` in some cases of left intervals with no neighbors by @agalitsyna in https://github.com/open2c/bioframe/pull/185
 * Fix overlap returning float indexes causing failing tests (numpy v1.22.4, pandas v1.5.2)  by @agalitsyna in https://github.com/open2c/bioframe/pull/185
```

### Comparing `bioframe-0.6.3/CITATION.cff` & `bioframe-0.6.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/CONTRIBUTING.md` & `bioframe-0.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/.github/workflows/ci.yml` & `bioframe-0.6.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/.github/workflows/publish.yml` & `bioframe-0.6.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/extras.py` & `bioframe-0.6.4/bioframe/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,27 +301,25 @@
 
     def _each(chrom_group):
         chrom = chrom_group.name
         seq = fasta_records[chrom]
         seq = str(seq[:])
         gc = []
         for _, bin in chrom_group.iterrows():
-            s = seq[bin.start : bin.end]
+            s = seq[bin["start"] : bin["end"]]
             gc.append(seq_gc(s, mapped_only=mapped_only))
         return gc
 
-    out = df.groupby("chrom", sort=False).apply(_each)
+    agg = df.groupby("chrom", sort=False)[["start", "end"]].apply(_each)
+    out_col = pd.Series(data=np.concatenate(agg.values), index=df.index).rename("GC")
 
     if return_input:
-        return pd.concat(
-            [df, pd.Series(data=np.concatenate(out), index=df.index).rename("GC")],
-            axis="columns",
-        )
+        return pd.concat([df, out_col], axis="columns")
     else:
-        return pd.Series(data=np.concatenate(out), index=df.index).rename("GC")
+        return out_col
 
 
 def seq_gc(seq, mapped_only=True):
     """
     Calculate the fraction of GC basepairs for a string of nucleotides.
 
     Parameters
```

### Comparing `bioframe-0.6.3/bioframe/ops.py` & `bioframe-0.6.4/bioframe/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1091,15 +1091,15 @@
                 ).T,
             ]
         )
 
         closest_intidxs.append(closest_idxs_group)
 
     if len(closest_intidxs) == 0:
-        return np.ndarray(shape=(0, 2), dtype=np.int)
+        return np.ndarray(shape=(0, 2), dtype=int)
     closest_intidxs = np.vstack(closest_intidxs)
 
     return closest_intidxs
 
 
 def closest(
     df1,
@@ -1629,16 +1629,16 @@
     if unassigned_intervals.any():
         df_trimmed.loc[unassigned_intervals, [ck, sk, ek]] = pd.NA
         df_trimmed.astype({sk: pd.Int64Dtype(), ek: pd.Int64Dtype()})
 
     lower_vector = df_trimmed[sk + "_view"].values
     upper_vector = df_trimmed[ek + "_view"].values
 
-    df_trimmed[sk].clip(lower=lower_vector, upper=upper_vector, inplace=True)
-    df_trimmed[ek].clip(lower=lower_vector, upper=upper_vector, inplace=True)
+    df_trimmed[sk] = df_trimmed[sk].clip(lower=lower_vector, upper=upper_vector)
+    df_trimmed[ek] = df_trimmed[ek].clip(lower=lower_vector, upper=upper_vector)
 
     if return_view_columns:
         return df_trimmed
     else:
         return df_trimmed[df_columns]
```

### Comparing `bioframe-0.6.3/bioframe/vis.py` & `bioframe-0.6.4/bioframe/vis.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/core/arrops.py` & `bioframe-0.6.4/bioframe/core/arrops.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,31 @@
 
     # Sort overlaps according to the 1st
     if sort:
         overlap_ids = overlap_ids[np.lexsort([overlap_ids[:, 1], overlap_ids[:, 0]])]
 
     return overlap_ids
 
+def _convert_points_to_len1_segments(starts, ends):
+    """
+    Convert points to len1 segments for internal use in overlap().
+    This enables desired overlap behavior for points and preserves
+    behavior for semi-open intervals of len>=1.
+    Parameters
+    ----------
+    starts, ends : numpy.ndarray
+
+    Returns
+    -------
+    pseudo_ends : numpy.ndarray
+    An array of pseudo-ends for overlapping intervals.
+    """
+    pseudo_ends = ends.copy()
+    pseudo_ends[ends == starts] += 1
+    return [starts, pseudo_ends]
 
 def overlap_intervals(starts1, ends1, starts2, ends2, closed=False, sort=False):
     """
     Take two sets of intervals and return the indices of pairs of overlapping intervals.
 
     Parameters
     ----------
@@ -292,16 +309,19 @@
                 "One of the inputs is provided as pandas.Series and its index "
                 "will be ignored.",
                 SyntaxWarning,
             )
 
     starts1 = np.asarray(starts1)
     ends1 = np.asarray(ends1)
+    starts1, ends1 = _convert_points_to_len1_segments(starts1, ends1)
+
     starts2 = np.asarray(starts2)
     ends2 = np.asarray(ends2)
+    starts2, ends2 = _convert_points_to_len1_segments(starts2, ends2)
 
     # Concatenate intervals lists
     n1 = len(starts1)
     n2 = len(starts2)
     ids1 = np.arange(0, n1)
     ids2 = np.arange(0, n2)
```

### Comparing `bioframe-0.6.3/bioframe/core/checks.py` & `bioframe-0.6.4/bioframe/core/checks.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/core/construction.py` & `bioframe-0.6.4/bioframe/core/construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,16 +152,16 @@
             out_df = from_ucsc_string_list(regions, cols=[ck1, sk1, ek1])
         else:
             out_df = from_list(regions, name_col=name_col, cols=[ck1, sk1, ek1])
     else:
         raise ValueError(f"Unknown input format: {type(regions)}")
 
     if fill_null:
+        out_df[sk1] = pd.to_numeric(out_df[sk1]).fillna(0)
         try:
-            out_df[sk1].fillna(0, inplace=True)
             ends = []
             for i in range(len(out_df)):
                 if out_df[ek1].values[i] is None:
                     ends.append(fill_null[out_df[ck1].values[i]])
                 else:
                     ends.append(out_df[ek1].values[i])
             out_df[ek1] = ends
```

### Comparing `bioframe-0.6.3/bioframe/core/specs.py` & `bioframe-0.6.4/bioframe/core/specs.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/core/stringops.py` & `bioframe-0.6.4/bioframe/core/stringops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/assembly.py` & `bioframe-0.6.4/bioframe/io/assembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from dataclasses import dataclass
-from typing import Dict, List, Optional, Tuple, Union
 
-import pkg_resources
+try:
+    from importlib.resources import files as resource_path
+except ImportError:
+    from importlib_resources import files as resource_path
+
+from typing import Dict, List, Optional, Tuple, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 import numpy as np
 import pandas as pd
 import yaml
 
 from bioframe import make_viewframe
 
 __all__ = ["assemblies_available", "assembly_info"]
 
-ASSEMBLY_MANIFEST_PATH = "data/_assemblies.yml"
+ASSEMBLY_METADATA_ROOT = resource_path("bioframe.io") / "data"
 
 
 @dataclass
 class GenomeAssembly:
     """
     A dataclass containing information about sequences in a genome assembly.
     """
@@ -69,16 +73,15 @@
     Returns
     -------
     pandas.DataFrame
         A dataframe with metadata fields for available assemblies, including
         'provider', 'provider_build', 'default_roles', 'default_units',
         and names of seqinfo and cytoband files.
     """
-    path = pkg_resources.resource_filename("bioframe.io", ASSEMBLY_MANIFEST_PATH)
-    with open(path) as f:
+    with open(ASSEMBLY_METADATA_ROOT / "_assemblies.yml") as f:
         assemblies = yaml.safe_load(f)
     return pd.DataFrame.from_records(assemblies)
 
 
 def assembly_info(
     name: str,
     roles: Optional[Union[List, Tuple, Literal["all"]]] = None,
@@ -144,17 +147,16 @@
     elif len(result) > 1:
         raise ValueError(f"Assembly identifer not unique: {result}")
 
     assembly = result.iloc[0].replace([np.nan], [None]).to_dict()
     default_roles = assembly["default_roles"]
     default_units = assembly["default_units"]
     seqinfo_path = assembly["seqinfo"]
-    seqinfo = pd.read_table(
-        pkg_resources.resource_filename("bioframe.io", f"data/{seqinfo_path}")
-    )
+    seqinfo = pd.read_table(ASSEMBLY_METADATA_ROOT / seqinfo_path)
+
     mask = np.ones(len(seqinfo), dtype=bool)
     if roles is None:
         mask &= seqinfo["role"].isin(default_roles)
     elif isinstance(roles, (tuple, list)):
         mask &= seqinfo["role"].isin(roles)
     elif isinstance(roles, str) and roles != "all":
         raise ValueError(f"roles must be a tuple or 'all', not {roles}")
@@ -165,19 +167,15 @@
     elif isinstance(units, str) and units != "all":
         raise ValueError(f"units must be a tuple or 'all', not {units}")
     seqinfo = seqinfo.loc[mask]
 
     cytobands = None
     cytobands_path = assembly["cytobands"]
     if cytobands_path is not None:
-        cytobands = pd.read_table(
-            pkg_resources.resource_filename(
-                "bioframe.io", f"data/{cytobands_path}"
-            )
-        )
+        cytobands = pd.read_table(ASSEMBLY_METADATA_ROOT / cytobands_path)
 
     return GenomeAssembly(
         organism=assembly["organism"],
         provider=assembly["provider"],
         provider_build=assembly["provider_build"],
         release_year=assembly["release_year"],
         seqinfo=seqinfo,
```

### Comparing `bioframe-0.6.3/bioframe/io/fileops.py` & `bioframe-0.6.4/bioframe/io/fileops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/resources.py` & `bioframe-0.6.4/bioframe/io/resources.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/schemas.py` & `bioframe-0.6.4/bioframe/io/schemas.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/_assemblies.yml` & `bioframe-0.6.4/bioframe/io/data/_assemblies.yml`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/danRer10.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/danRer10.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/danRer11.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/danRer11.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/dm3.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/dm3.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/dm6.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/dm6.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/hg19.cytoband.tsv` & `bioframe-0.6.4/bioframe/io/data/hg19.cytoband.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/hg19.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/hg19.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/hg38.cytoband.tsv` & `bioframe-0.6.4/bioframe/io/data/hg38.cytoband.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/hg38.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/hg38.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/hs1.cytoband.tsv` & `bioframe-0.6.4/bioframe/io/data/hs1.cytoband.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/hs1.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/hs1.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/mm10.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/mm10.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/mm39.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/mm39.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/mm9.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/mm9.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/io/data/sacCer3.seqinfo.tsv` & `bioframe-0.6.4/bioframe/io/data/sacCer3.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/sandbox/clients.py` & `bioframe-0.6.4/bioframe/sandbox/clients.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/sandbox/gtf_io.py` & `bioframe-0.6.4/bioframe/sandbox/gtf_io.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/bioframe/sandbox/parquet_io.py` & `bioframe-0.6.4/bioframe/sandbox/parquet_io.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/Makefile` & `bioframe-0.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/api-lowlevel.md` & `bioframe-0.6.4/docs/api-lowlevel.md`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/api-resources.rst` & `bioframe-0.6.4/docs/api-resources.rst`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/conf.py` & `bioframe-0.6.4/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,33 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-import os
-import sys
-
-sys.path.insert(0, os.path.abspath("../"))
-
+# import sys
+from datetime import datetime
+from importlib.metadata import metadata
+from pathlib import Path
 # autodoc_mock_imports = ["numpy", "pandas", "matplotlib", "requests"]
 
 
 # -- Project information -----------------------------------------------------
-
-project = "bioframe"
-copyright = "2020, Open2C"
+# NOTE: If you installed your project in editable mode, this might be stale.
+#       If this is the case, reinstall it to refresh the metadata
+info = metadata("bioframe")
+project_name = info["Name"]
 author = "Open2C"
-
+copyright = f"{datetime.now():%Y}, {author}."
+version = info["Version"]
+urls = dict(pu.split(", ") for pu in info.get_all("Project-URL"))
 
 # The full version, including alpha/beta/rc tags
-def _read(*parts, **kwargs):
-    import os
-
-    filepath = os.path.join(os.path.dirname(__file__), *parts)
-    encoding = kwargs.pop("encoding", "utf-8")
-    with open(filepath, encoding=encoding) as fh:
-        text = fh.read()
-    return text
-
-
-def get_version():
-    import re
-
-    version = re.search(
-        r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-        _read("..", "bioframe", "_version.py"),
-        re.MULTILINE,
-    ).group(1)
-    return version
-
-
-version = get_version()
-# The full version, including alpha/beta/rc tags.
-release = version
+release = info["Version"]
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `bioframe-0.6.3/docs/guide-definitions.rst` & `bioframe-0.6.4/docs/guide-definitions.rst`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/guide-intervalops.md` & `bioframe-0.6.4/docs/guide-intervalops.md`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/guide-io.ipynb` & `bioframe-0.6.4/docs/guide-io.ipynb`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/guide-performance.ipynb` & `bioframe-0.6.4/docs/guide-performance.ipynb`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/guide-quickstart.rst` & `bioframe-0.6.4/docs/guide-quickstart.rst`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/guide-recipes.md` & `bioframe-0.6.4/docs/guide-recipes.md`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/guide-specifications.rst` & `bioframe-0.6.4/docs/guide-specifications.rst`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/index.rst` & `bioframe-0.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/make.bat` & `bioframe-0.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/times100.bw` & `bioframe-0.6.4/docs/times100.bw`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/._bioframe-logo.png` & `bioframe-0.6.4/docs/figs/._bioframe-logo.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/bioframe-logo.png` & `bioframe-0.6.4/docs/figs/bioframe-logo.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/bioframe_closest.pdf` & `bioframe-0.6.4/docs/figs/bioframe_closest.pdf`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/closest0.png` & `bioframe-0.6.4/docs/figs/closest0.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/closest1.png` & `bioframe-0.6.4/docs/figs/closest1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/closest2.png` & `bioframe-0.6.4/docs/figs/closest2.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/closest3.png` & `bioframe-0.6.4/docs/figs/closest3.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/df1.png` & `bioframe-0.6.4/docs/figs/df1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/df2.png` & `bioframe-0.6.4/docs/figs/df2.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/df@.png` & `bioframe-0.6.4/docs/figs/df@.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/merge_df1.png` & `bioframe-0.6.4/docs/figs/merge_df1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/overlap_inner_0.png` & `bioframe-0.6.4/docs/figs/overlap_inner_0.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/figs/overlap_inner_1.png` & `bioframe-0.6.4/docs/figs/overlap_inner_1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb` & `bioframe-0.6.4/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb` & `bioframe-0.6.4/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/tests/test_assembly_info.py` & `bioframe-0.6.4/tests/test_assembly_info.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/tests/test_core_checks.py` & `bioframe-0.6.4/tests/test_core_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,15 @@
             ["chr1", 0, 12, "chr1p"],
             ["chr2", 13, 26, "chr1q"],
             ["chrX", 1, 8, "chrX_0"],
         ],
         columns=["chrom", "start", "end", "funny_view_region"],
     )
     assert is_cataloged(
-        df,
-        view_df,
-        df_view_col="funny_view_region",
-        view_name_col="funny_name"
+        df, view_df, df_view_col="funny_view_region", view_name_col="funny_name"
     )
 
 
 def test_is_contained():
 
     view_df = pd.DataFrame(
         [
@@ -127,16 +124,16 @@
     )
     assert is_contained(
         df,
         view_df,
         cols=["chrom1", "start1", "end1"],
         cols_view=["CHROM", "START", "END"],
         df_view_col="VIEW_REGION",
-        view_name_col="NAME"
-        )
+        view_name_col="NAME",
+    )
 
     with pytest.raises(TypeError):
         # cols and view_cols are not passed as an arguments
         is_contained(df, view_df, raise_errors=True)
 
     # is not contained, because assignments are not inferred
     view_df = pd.DataFrame(
@@ -215,27 +212,24 @@
             ["chr1", -5, 10],
             ["chr1", 11, 12],
             ["chr1", 12, 20],
         ],
         columns=["chrom1", "start1", "end1"],
     )
     chromsizes = pd.DataFrame(
-        [
-            ["chr1", 0, 9, "chr1p"],
-            ["chr1", 11, 20, "chr1q"]
-        ],
+        [["chr1", 0, 9, "chr1p"], ["chr1", 11, 20, "chr1q"]],
         columns=["CHROM", "START", "END", "NAME"],
-        )
+    )
     assert is_covering(
-                        df1,
-                        chromsizes,
-                        cols=["chrom1", "start1", "end1"],
-                        cols_view=["CHROM", "START", "END"],
-                        view_name_col="NAME"
-                    )
+        df1,
+        chromsizes,
+        cols=["chrom1", "start1", "end1"],
+        cols_view=["CHROM", "START", "END"],
+        view_name_col="NAME",
+    )
 
     with pytest.raises(ValueError):
         # cols and view_cols are not passed as an arguments
         is_covering(df1, chromsizes)
 
     #   test is_covering where two intervals from df overlap
     #   two different regions from view
@@ -270,27 +264,24 @@
             ["chr1", 0, 9, "chr1p"],
             ["chr1", 11, 12, "chr1q"],
             ["chr1", 12, 20, "chr1q"],
         ],
         columns=["chrom1", "start1", "end1", "view_region"],
     )
     chromsizes = pd.DataFrame(
-        [
-            ["chr1", 0, 9, "chr1p"],
-            ["chr1", 11, 20, "chr1q"]
-        ],
+        [["chr1", 0, 9, "chr1p"], ["chr1", 11, 20, "chr1q"]],
         columns=["CHROM", "START", "END", "NAME"],
-        )
+    )
     assert is_tiling(
-                        df1,
-                        chromsizes,
-                        cols=["chrom1", "start1", "end1"],
-                        cols_view=["CHROM", "START", "END"],
-                        view_name_col="NAME"
-                    )
+        df1,
+        chromsizes,
+        cols=["chrom1", "start1", "end1"],
+        cols_view=["CHROM", "START", "END"],
+        view_name_col="NAME",
+    )
 
     with pytest.raises(KeyError):
         # cols and view_cols are not passed as an arguments
         is_tiling(df1, chromsizes)
 
     #  not tiling, since (chr1,0,9) is associated with chr1q
     df1 = pd.DataFrame(
@@ -473,15 +464,15 @@
 
     assert is_sorted(
         view_df,
         view_df=view_df,
         view_name_col="FRUIT",
         df_view_col="FRUIT",
         cols=["CHROM", "START", "END"],
-        cols_view=["CHROM", "START", "END"]
+        cols_view=["CHROM", "START", "END"],
     )
 
     with pytest.raises(ValueError):
         # cols and view_cols are not passed as an arguments
         is_sorted(view_df, view_df=view_df)
 
     df = pd.DataFrame(
```

### Comparing `bioframe-0.6.3/tests/test_core_construction.py` & `bioframe-0.6.4/tests/test_core_construction.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/tests/test_core_specs.py` & `bioframe-0.6.4/tests/test_core_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import numpy as np
 import pandas as pd
 import pytest
 
 import bioframe
 from bioframe.core import specs
```

### Comparing `bioframe-0.6.3/tests/test_core_stringops.py` & `bioframe-0.6.4/tests/test_core_stringops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/tests/test_extras.py` & `bioframe-0.6.4/tests/test_extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,15 @@
     result = bioframe.make_chromarms(
         df,
         mids,
         cols_chroms=["chromosome", "lo", "hi"],
         cols_mids=["chromosome", "loc"],
     )
     pd.testing.assert_frame_equal(
-        result,
-        arms.rename(columns={"chrom": "chromosome", "start": "lo", "end": "hi"})
+        result, arms.rename(columns={"chrom": "chromosome", "start": "lo", "end": "hi"})
     )
 
     # test passing 2 columns
     result = bioframe.make_chromarms(
         df,
         mids,
         cols_chroms=["chromosome", "hi"],
@@ -48,17 +47,15 @@
     pd.testing.assert_frame_equal(
         result,
         arms.rename(columns={"chrom": "chromosome"}),
     )
 
     # test for passing Series or dict
     result = bioframe.make_chromarms(
-        pd.Series({"chrX": 8}),
-        mids,
-        cols_mids=["chromosome", "loc"]
+        pd.Series({"chrX": 8}), mids, cols_mids=["chromosome", "loc"]
     )
     pd.testing.assert_frame_equal(arms, result)
 
     result = bioframe.make_chromarms(pd.Series({"chrX": 8}), pd.Series({"chrX": 4}))
     pd.testing.assert_frame_equal(arms, result)
 
     bioframe.make_chromarms({"chrX": 8}, mids, cols_mids=["chromosome", "loc"])
@@ -192,19 +189,19 @@
             mapped_only=False,
         ).values
     ).all()
 
 
 def test_seq_gc():
 
-    assert (0 == bioframe.seq_gc("AT"))
-    assert (np.isnan( bioframe.seq_gc("NNN")))
-    assert (1 == bioframe.seq_gc("NGnC"))
-    assert (0.5 == bioframe.seq_gc("GTCA"))
-    assert (0.25 == bioframe.seq_gc("nnnNgTCa", mapped_only=False))
+    assert 0 == bioframe.seq_gc("AT")
+    assert np.isnan(bioframe.seq_gc("NNN"))
+    assert 1 == bioframe.seq_gc("NGnC")
+    assert 0.5 == bioframe.seq_gc("GTCA")
+    assert 0.25 == bioframe.seq_gc("nnnNgTCa", mapped_only=False)
     with pytest.raises(ValueError):
         bioframe.seq_gc(["A", "T"])
     with pytest.raises(ValueError):
         bioframe.seq_gc(np.array("ATGC"))
 
 
 ### todo: test frac_gene_coverage(bintable, mrna):
```

### Comparing `bioframe-0.6.3/tests/test_fileops.py` & `bioframe-0.6.4/tests/test_fileops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/tests/test_ops.py` & `bioframe-0.6.4/tests/test_ops.py`

 * *Files 12% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         ],
         columns=["chrom", "start", "end"],
     ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
     df_trimmed = pd.DataFrame(
         [
             ["chr1", 0, 12, "chr1p"],
             ["chr1", 0, 12, "chr1p"],
-            [pd.NA, pd.NA, pd.NA, pd.NA],
+            [pd.NA, pd.NA, pd.NA, None],
             ["chrX", 1, 12, "chrX_0"],
         ],
         columns=["chrom", "start", "end", "view_region"],
     ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
     # infer df_view_col with assign_view and ignore NAs
     pd.testing.assert_frame_equal(
         df_trimmed,
@@ -422,14 +422,267 @@
         on=["animal"],
         how="left",
         cols1=("chrom1", "start", "end"),
         cols2=("chrom2", "start2", "end2"),
     )
     assert len(b) == 3
 
+    ### test overlap with point and segment data
+    df_point1 = pd.DataFrame(
+        [["chr1", 1, 1]], columns=["chrom", "start", "end"]
+    ).astype({"chrom": "object", "start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    df_segment12 = pd.DataFrame(
+        [["chr1", 1, 2]], columns=["chrom", "start", "end"]
+    ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    b = bioframe.overlap(
+        df_point1,
+        df_segment12,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 1, "chr1", 1, 2]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    ### test for changed order of input point and segment
+    b = bioframe.overlap(
+        df_segment12,
+        df_point1,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 2, "chr1", 1, 1]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    ### test for overlap with point and segment with right method
+    b = bioframe.overlap(
+        df_point1,
+        df_segment12,
+        on=None,
+        how="right",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 1, "chr1", 1, 2]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    ### test for swapped order of input point and segment
+    b = bioframe.overlap(
+        df_segment12,
+        df_point1,
+        on=None,
+        how="right",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 2, "chr1", 1, 1]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    ### Two adjacent point should not overlap with each other
+    df_point1 = pd.DataFrame(
+        [["chr1", 1, 1]], columns=["chrom", "start", "end"]
+    ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    df_point2 = pd.DataFrame(
+        [["chr1", 2, 2]], columns=["chrom", "start", "end"]
+    ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    b = bioframe.overlap(
+        df_point1,
+        df_point2,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 1, None, pd.NA, pd.NA]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    ### test for changed order of input point
+    b = bioframe.overlap(
+        df_point2,
+        df_point1,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 2, 2, None, pd.NA, pd.NA]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    ### Point adjacent to the end of the segment should not
+    ### overlap with the segment
+    df_segment12 = pd.DataFrame(
+        [["chr1", 1, 2]], columns=["chrom", "start", "end"]
+    ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    df_point2 = pd.DataFrame(
+        [["chr1", 2, 2]], columns=["chrom", "start", "end"]
+    ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    b = bioframe.overlap(
+        df_segment12,
+        df_point2,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 2, None, pd.NA, pd.NA]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    b = bioframe.overlap(
+        df_point2,
+        df_segment12,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 2, 2, None, pd.NA, pd.NA]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    ### Point adjacent to the start of the segment should
+    ### overlap with the segment
+    df_point1 = pd.DataFrame(
+        [["chr1", 1, 1]], columns=["chrom", "start", "end"]
+    ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    df_segment12 = pd.DataFrame(
+        [["chr1", 1, 2]], columns=["chrom", "start", "end"]
+    ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
+
+    b = bioframe.overlap(
+        df_point1,
+        df_segment12,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 1, "chr1", 1, 2]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
+    b = bioframe.overlap(
+        df_segment12,
+        df_point1,
+        on=None,
+        how="left",
+        return_index=False,
+        return_input=True,
+    )
+    df_expected = pd.DataFrame(
+        [["chr1", 1, 2, "chr1", 1, 1]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_"],
+    ).astype(
+        {
+            "start": pd.Int64Dtype(),
+            "end": pd.Int64Dtype(),
+            "start_": pd.Int64Dtype(),
+            "end_": pd.Int64Dtype(),
+        }
+    )
+    pd.testing.assert_frame_equal(df_expected, b)
+
     ### test keep_order and NA handling
     df1 = pd.DataFrame(
         [
             ["chr1", 8, 12, "+"],
             [pd.NA, pd.NA, pd.NA, "-"],
             ["chrX", 1, 8, "+"],
         ],
@@ -442,19 +695,20 @@
     ).astype({"start2": pd.Int64Dtype(), "end2": pd.Int64Dtype()})
 
     assert df1.equals(
         bioframe.overlap(
             df1, df2, how="left", keep_order=True, cols2=["chrom2", "start2", "end2"]
         )[["chrom", "start", "end", "strand"]]
     )
-    assert ~df1.equals(
-        bioframe.overlap(
-            df1, df2, how="left", keep_order=False, cols2=["chrom2", "start2", "end2"]
-        )[["chrom", "start", "end", "strand"]]
-    )
+
+    # keep_order=False is non-deterministic
+    # assert not df1.equals(
+    #     bioframe.overlap(
+    #         df1, df2, how="left", keep_order=False, cols2=["chrom2", "start2", "end2"]
+    #     )[["chrom", "start", "end", "strand"]])
 
     df1 = pd.DataFrame(
         [
             ["chr1", 8, 12, "+", pd.NA],
             [pd.NA, pd.NA, pd.NA, "-", pd.NA],
             ["chrX", 1, 8, pd.NA, pd.NA],
         ],
@@ -1179,21 +1433,19 @@
 
     ### closest(df1, df2, k=1, ignore_upstream=False, ignore_downstream=True,
     ### ignore_overlaps=True) when upstream region is absent ###
 
     df2 = pd.DataFrame(
         [["chr1", 5, 6], ["chr1", 10, 11]], columns=["chrom", "start", "end"]
     )
-
-    d = """chrom  start  end chrom_  start_  end_  distance
-        0    chr1        3      5    NaN        NaN      NaN         NaN
-        """
-    df = pd.read_csv(StringIO(d), sep=r"\s+").astype(
+    df = pd.DataFrame(
+        [["chr1", 3, 5, pd.NA, pd.NA, pd.NA, pd.NA]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_", "distance"],
+    ).astype(
         {
-            "chrom_": "O",
             "start_": pd.Int64Dtype(),
             "end_": pd.Int64Dtype(),
             "distance": pd.Int64Dtype(),
         }
     )
     pd.testing.assert_frame_equal(
         df,
@@ -1212,21 +1464,19 @@
 
     df2 = pd.DataFrame(
         [
             ["chr1", 1, 2],
         ],
         columns=["chrom", "start", "end"],
     )
-
-    d = """chrom  start  end chrom_  start_  end_  distance
-        0    chr1        3      5    NaN        NaN      NaN         NaN
-        """
-    df = pd.read_csv(StringIO(d), sep=r"\s+").astype(
+    df = pd.DataFrame(
+        [["chr1", 3, 5, pd.NA, pd.NA, pd.NA, pd.NA]],
+        columns=["chrom", "start", "end", "chrom_", "start_", "end_", "distance"],
+    ).astype(
         {
-            "chrom_": "O",
             "start_": pd.Int64Dtype(),
             "end_": pd.Int64Dtype(),
             "distance": pd.Int64Dtype(),
         }
     )
     pd.testing.assert_frame_equal(
         df,
@@ -1495,22 +1745,76 @@
                 ["chr1", 4, 7],
             ],
             columns=["chrom", "start", "end"],
         )
         .sort_values(["chrom", "start", "end"])
         .reset_index(drop=True)
     )
-
     pd.testing.assert_frame_equal(
         df_result.astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()}),
         bioframe.subtract(df1, df2)
         .sort_values(["chrom", "start", "end"])
         .reset_index(drop=True),
     )
 
+    # Test the case when substraction from point bioframe
+    df1 = pd.DataFrame([["chr1", 1, 1]], columns=["chrom", "start", "end"]).astype(
+        {"start": pd.Int64Dtype(), "end": pd.Int64Dtype()}
+    )
+
+    df2 = pd.DataFrame([["chr1", 0, 2]], columns=["chrom", "start", "end"]).astype(
+        {"start": pd.Int64Dtype(), "end": pd.Int64Dtype()}
+    )
+
+    df_result = (
+        pd.DataFrame(
+            [
+                ["chr1", 0, 1],
+                ["chr1", 1, 2],
+            ],
+            columns=["chrom", "start", "end"],
+        )
+        .sort_values(["chrom", "start", "end"])
+        .reset_index(drop=True)
+    )
+    pd.testing.assert_frame_equal(
+        df_result.astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()}),
+        bioframe.subtract(df2, df1)
+        .sort_values(["chrom", "start", "end"])
+        .reset_index(drop=True),
+    )
+
+    # Test the case when substraction from point is at the beginning bioframe
+
+    df1 = pd.DataFrame([["chr1", 1, 1]], columns=["chrom", "start", "end"]).astype(
+        {"start": pd.Int64Dtype(), "end": pd.Int64Dtype()}
+    )
+
+    df2 = pd.DataFrame([["chr1", 1, 2]], columns=["chrom", "start", "end"]).astype(
+        {"start": pd.Int64Dtype(), "end": pd.Int64Dtype()}
+    )
+
+    df_result = (
+        pd.DataFrame(
+            [
+                ["chr1", 1, 2],
+            ],
+            columns=["chrom", "start", "end"],
+        )
+        .sort_values(["chrom", "start", "end"])
+        .reset_index(drop=True)
+    )
+
+    pd.testing.assert_frame_equal(
+        df_result.astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()}),
+        bioframe.subtract(df2, df1)
+        .sort_values(["chrom", "start", "end"])
+        .reset_index(drop=True),
+    )
+
     # subtract should ignore null rows
     df1 = pd.DataFrame(
         [[pd.NA, pd.NA, pd.NA], ["chr1", 1, 5]],
         columns=["chrom", "start", "end"],
     ).astype({"start": pd.Int64Dtype(), "end": pd.Int64Dtype()})
 
     df2 = pd.DataFrame(
```

### Comparing `bioframe-0.6.3/tests/test_ops_select.py` & `bioframe-0.6.4/tests/test_ops_select.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,41 +2,32 @@
 import pytest
 
 import bioframe
 
 
 def test_select():
     df = pd.DataFrame(
-        [["chrX", 3, 8],
-         ["chr1", 4, 5],
-         ["chrX", 1, 5]],
+        [["chrX", 3, 8], ["chr1", 4, 5], ["chrX", 1, 5]],
         columns=["chrom", "start", "end"],
     )
 
-    result = pd.DataFrame(
-        [["chr1", 4, 5]],
-        columns=["chrom", "start", "end"]
-    )
+    result = pd.DataFrame([["chr1", 4, 5]], columns=["chrom", "start", "end"])
     pd.testing.assert_frame_equal(
         result, bioframe.select(df, "chr1:4-10").reset_index(drop=True)
     )
 
     result = pd.DataFrame(
-        [["chrX", 3, 8],
-         ["chrX", 1, 5]],
-         columns=["chrom", "start", "end"]
+        [["chrX", 3, 8], ["chrX", 1, 5]], columns=["chrom", "start", "end"]
     )
     pd.testing.assert_frame_equal(
         result, bioframe.select(df, "chrX").reset_index(drop=True)
     )
 
     result = pd.DataFrame(
-        [["chrX", 3, 8],
-         ["chrX", 1, 5]],
-         columns=["chrom", "start", "end"]
+        [["chrX", 3, 8], ["chrX", 1, 5]], columns=["chrom", "start", "end"]
     )
     pd.testing.assert_frame_equal(
         result, bioframe.select(df, "chrX:4-6").reset_index(drop=True)
     )
 
     # Query range not in the dataframe
     assert len(bioframe.select(df, "chrZ")) == 0
@@ -48,22 +39,19 @@
         bioframe.select(df, "chr1:1-0")
 
 
 def test_select__with_colnames():
     ### select with non-standard column names
     new_names = ["chr", "chrstart", "chrend"]
     df = pd.DataFrame(
-        [["chrX", 3, 8],
-         ["chr1", 4, 5],
-         ["chrX", 1, 5]],
+        [["chrX", 3, 8], ["chr1", 4, 5], ["chrX", 1, 5]],
         columns=new_names,
     )
     result = pd.DataFrame(
-        [["chrX", 3, 8],
-         ["chrX", 1, 5]],
+        [["chrX", 3, 8], ["chrX", 1, 5]],
         columns=new_names,
     )
     pd.testing.assert_frame_equal(
         result, bioframe.select(df, "chrX:4-6", cols=new_names).reset_index(drop=True)
     )
     pd.testing.assert_frame_equal(
         result, bioframe.select(df, "chrX", cols=new_names).reset_index(drop=True)
@@ -90,55 +78,40 @@
     pd.testing.assert_frame_equal(
         result, bioframe.select(df, "chr1:0-1").reset_index(drop=True)
     )
 
 
 def test_select__mask_indices_labels():
     df = pd.DataFrame(
-        [["chrX", 3, 8],
-         ["chr1", 4, 5],
-         ["chrX", 1, 5]],
+        [["chrX", 3, 8], ["chr1", 4, 5], ["chrX", 1, 5]],
         columns=["chrom", "start", "end"],
     )
 
     region = "chr1:4-10"
-    answer = pd.DataFrame(
-        [["chr1", 4, 5]],
-        columns=["chrom", "start", "end"]
-    )
+    answer = pd.DataFrame([["chr1", 4, 5]], columns=["chrom", "start", "end"])
 
     result = bioframe.select(df, region)
-    pd.testing.assert_frame_equal(
-        answer, result.reset_index(drop=True)
-    )
+    pd.testing.assert_frame_equal(answer, result.reset_index(drop=True))
     mask = bioframe.select_mask(df, region)
-    pd.testing.assert_frame_equal(
-        answer, df.loc[mask].reset_index(drop=True)
-    )
+    pd.testing.assert_frame_equal(answer, df.loc[mask].reset_index(drop=True))
     labels = bioframe.select_labels(df, region)
-    pd.testing.assert_frame_equal(
-        answer, df.loc[labels].reset_index(drop=True)
-    )
+    pd.testing.assert_frame_equal(answer, df.loc[labels].reset_index(drop=True))
     idx = bioframe.select_indices(df, region)
-    pd.testing.assert_frame_equal(
-        answer, df.iloc[idx].reset_index(drop=True)
-    )
+    pd.testing.assert_frame_equal(answer, df.iloc[idx].reset_index(drop=True))
 
 
 def test_select__query_intervals_are_half_open():
-    df = pd.DataFrame({
-        "chrom": ["chr1", "chr1",
-                  "chr2", "chr2", "chr2", "chr2", "chr2", "chr2"],
-        "start": [0, 10,
-                  10, 20, 30, 40, 50, 60],
-        "end":  [10, 20,
-                 20, 30, 40, 50, 60, 70],
-        "name": ["a", "b",
-                 "A", "B", "C", "D", "E", "F"],
-    })
+    df = pd.DataFrame(
+        {
+            "chrom": ["chr1", "chr1", "chr2", "chr2", "chr2", "chr2", "chr2", "chr2"],
+            "start": [0, 10, 10, 20, 30, 40, 50, 60],
+            "end": [10, 20, 20, 30, 40, 50, 60, 70],
+            "name": ["a", "b", "A", "B", "C", "D", "E", "F"],
+        }
+    )
 
     result = bioframe.select(df, "chr1")
     assert (result["name"] == ["a", "b"]).all()
 
     result = bioframe.select(df, "chr2:20-70")
     assert (result["name"] == ["B", "C", "D", "E", "F"]).all()
 
@@ -168,24 +141,22 @@
 
     result = bioframe.select(df, "chr2:25-51")
     assert (result["name"] == ["B", "C", "D", "E"]).all()
 
 
 def test_select__with_point_intervals():
     # Dataframe containing "point intervals"
-    df = pd.DataFrame({
-        "chrom": ["chr1", "chr1",
-                  "chr2", "chr2", "chr2", "chr2", "chr2", "chr2"],
-        "start": [0, 10,
-                  10, 20, 30, 40, 50, 60],
-        "end":  [10, 10,
-                 20, 30, 40, 50, 50, 70],
-        "name": ["a", "b",
-                 "A", "B", "C", "D", "E", "F"],
-    })
+    df = pd.DataFrame(
+        {
+            "chrom": ["chr1", "chr1", "chr2", "chr2", "chr2", "chr2", "chr2", "chr2"],
+            "start": [0, 10, 10, 20, 30, 40, 50, 60],
+            "end": [10, 10, 20, 30, 40, 50, 50, 70],
+            "name": ["a", "b", "A", "B", "C", "D", "E", "F"],
+        }
+    )
     result = bioframe.select(df, "chr1")
     assert (result["name"] == ["a", "b"]).all()
 
     result = bioframe.select(df, "chr1:4-10")
     assert (result["name"] == ["a"]).all()
 
     result = bioframe.select(df, "chr1:4-4")
@@ -209,17 +180,15 @@
     result = bioframe.select(df, "chr2:50-50")
     assert (result["name"] == ["E"]).all()
 
 
 def test_select__with_points():
     # Dataframe of points
     df = pd.DataFrame(
-        [["chrX", 3, "A"],
-         ["chr1", 4, "C"],
-         ["chrX", 1, "B"]],
+        [["chrX", 3, "A"], ["chr1", 4, "C"], ["chrX", 1, "B"]],
         columns=["chrom", "pos", "name"],
     )
 
     result = bioframe.select(df, "chr1:4-10", cols=["chrom", "pos", "pos"])
     assert (result["name"] == ["C"]).all()
 
     result = bioframe.select(df, "chr1:3-10", cols=["chrom", "pos", "pos"])
```

### Comparing `bioframe-0.6.3/tests/test_resources.py` & `bioframe-0.6.4/tests/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     db = "hg38"
     for provider in ["local", "ucsc"]:
         chromsizes = bioframe.fetch_chromsizes(db, provider=provider)
         assert isinstance(chromsizes, pd.Series)
         assert chromsizes.name == "length"
         assert len(chromsizes) == 25
 
-        chromsizes_df = bioframe.fetch_chromsizes(
-            db, provider=provider, as_bed=True
-        )
+        chromsizes_df = bioframe.fetch_chromsizes(db, provider=provider, as_bed=True)
         assert isinstance(chromsizes_df, pd.DataFrame)
         assert list(chromsizes_df.columns) == ["chrom", "start", "end"]
         assert len(chromsizes_df) == 25
 
     # Check synonymous local assemblies
     assert bioframe.fetch_chromsizes("hg38", provider="local").equals(
         bioframe.fetch_chromsizes("GRCh38", provider="local")
```

### Comparing `bioframe-0.6.3/tests/test_vis.py` & `bioframe-0.6.4/tests/test_vis.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     bioframe.to_ucsc_colorstring("none") == "0"
     bioframe.to_ucsc_colorstring(np.nan) == "0"
     bioframe.to_ucsc_colorstring(pd.NA) == "0"
 
     with pytest.raises(ValueError):
         bioframe.to_ucsc_colorstring("notacolor")
 
-    df = bioframe.from_any([
-        ["chr1", 0, 10, "red"],
-        ["chr1", 10, 20, "blue"],
-        ["chr2", 0, 10, "green"],
-        ["chr2", 10, 20, None],
-    ])
+    df = bioframe.from_any(
+        [
+            ["chr1", 0, 10, "red"],
+            ["chr1", 10, 20, "blue"],
+            ["chr2", 0, 10, "green"],
+            ["chr2", 10, 20, None],
+        ]
+    )
     df["itemRgb"] = df["name"].apply(bioframe.to_ucsc_colorstring)
     assert df["itemRgb"].tolist() == ["255,0,0", "0,0,255", "0,128,0", "0"]
```

### Comparing `bioframe-0.6.3/LICENSE` & `bioframe-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/README.md` & `bioframe-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.3/pyproject.toml` & `bioframe-0.6.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bioframe"
+version = "0.6.4"
 description = "Operations and utilities for Genomic Interval Dataframes."
 license = {text = "MIT"}
 authors = [
   {name = "Open2C", email = "open.chromosome.collective@gmail.com"},
 ]
 keywords = [
     "pandas",
@@ -30,22 +31,23 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 readme = "README.md"
-dynamic = ["version"]
 dependencies = [
     "matplotlib",
     "numpy>=1.10",
     "pandas>=1.3",
     "pyyaml",
     "requests",
     "typing-extensions ; python_version<'3.9'",
+    "importlib-metadata ; python_version<'3.8'",
+    "importlib-resources ; python_version<'3.9'",
 ]
 
 [project.optional-dependencies]
 dev = [
     "biopython",
     "isort",
     "pysam",
@@ -67,42 +69,42 @@
 
 [project.urls]
 homepage = "https://github.com/open2c/bioframe"
 documentation = "https://bioframe.readthedocs.io/en/latest"
 repository = "https://github.com/open2c/bioframe"
 changelog = "https://github.com/open2c/bioframe/blob/main/CHANGES.md"
 
-[tool.hatch.version]
-path = "bioframe/_version.py"
-
-[tool.hatch.envs.default]
-features = ["dev", "test", "docs"]
-
-[tool.hatch.envs.default.scripts]
-fix = "ruff --fix ."
-lint = "ruff bioframe tests"
-test = "pytest ."
-docs = "sphinx-autobuild docs docs/_build/html"
-
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = "bioframe"
 
 [tool.ruff]
 target-version = "py37"
 exclude = [
     ".venv",
-    "bioframe/__init__.py",
-    "bioframe/core/__init__.py",
-    "bioframe/io/__init__.py",
 ]
-extend-select = [
+lint.extend-select = [
     # "C",  # mccabe complexity
     # "D",  # pydocstyle
     "E",  # style errors
     "F",  # pyflakes
     "I",  # isort
     "RUF", # ruff-specific rules
     "UP", # pyupgrade
     "W",  # style  warnings
 ]
+
+[tool.hatch.envs.default]
+features = ["dev", "test", "docs"]
+
+[tool.hatch.envs.default.scripts]
+fix = "ruff check --fix ."
+lint = "ruff check bioframe tests"
+test = "pytest ."
+docs = "sphinx-autobuild docs docs/_build/html"
+
+[tool.hatch.envs.test]
+features = ["dev", "test"]
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.8", "3.9", "3.10", "3.11"]
```

### Comparing `bioframe-0.6.3/PKG-INFO` & `bioframe-0.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bioframe
-Version: 0.6.3
+Version: 0.6.4
 Summary: Operations and utilities for Genomic Interval Dataframes.
 Project-URL: homepage, https://github.com/open2c/bioframe
 Project-URL: documentation, https://bioframe.readthedocs.io/en/latest
 Project-URL: repository, https://github.com/open2c/bioframe
 Project-URL: changelog, https://github.com/open2c/bioframe/blob/main/CHANGES.md
 Author-email: Open2C <open.chromosome.collective@gmail.com>
 License: MIT
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: numpy>=1.10
 Requires-Dist: pandas>=1.3
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: typing-extensions; python_version < '3.9'
 Provides-Extra: dev
```

