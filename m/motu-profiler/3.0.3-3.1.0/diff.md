# Comparing `tmp/motu-profiler-3.0.3.tar.gz` & `tmp/motu-profiler-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/motu-profiler-3.0.3.tar", last modified: Wed Jul 13 14:50:15 2022, max compression
+gzip compressed data, was "motu-profiler-3.1.0.tar", last modified: Thu Apr 13 15:51:34 2023, max compression
```

## Comparing `motu-profiler-3.0.3.tar` & `motu-profiler-3.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 milanese   (503) staff       (20)        0 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/
--rw-r--r--   0 milanese   (503) staff       (20)     9786 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/PKG-INFO
--rw-r--r--   0 milanese   (503) staff       (20)     7528 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/README.md
-drwxr-xr-x   0 milanese   (503) staff       (20)        0 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/motu_profiler.egg-info/
--rw-r--r--   0 milanese   (503) staff       (20)     9786 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/motu_profiler.egg-info/PKG-INFO
--rw-r--r--   0 milanese   (503) staff       (20)      590 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/motu_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 milanese   (503) staff       (20)        1 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/motu_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 milanese   (503) staff       (20)       44 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/motu_profiler.egg-info/entry_points.txt
--rw-r--r--   0 milanese   (503) staff       (20)        6 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/motu_profiler.egg-info/top_level.txt
-drwxr-xr-x   0 milanese   (503) staff       (20)        0 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/motus/
--rw-r--r--   0 milanese   (503) staff       (20)    16191 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/PEfiltering.py
--rw-r--r--   0 milanese   (503) staff       (20)    13760 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/UTIL_log.py
--rw-r--r--   0 milanese   (503) staff       (20)    19180 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/UTIL_log_col.py
--rw-r--r--   0 milanese   (503) staff       (20)    19496 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/append.py
--rw-r--r--   0 milanese   (503) staff       (20)     5629 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/convert_long_reads.py
--rw-r--r--   0 milanese   (503) staff       (20)     5623 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/downloadDB.py
--rw-r--r--   0 milanese   (503) staff       (20)    54316 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/map_genes_to_mOTUs.py
--rw-r--r--   0 milanese   (503) staff       (20)    42249 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/map_mOTUs_to_LGs.py
--rw-r--r--   0 milanese   (503) staff       (20)    12709 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/metaSNV_DistDiv.py
--rw-r--r--   0 milanese   (503) staff       (20)    13430 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/metaSNV_Filtering_2.0.py
--rw-r--r--   0 milanese   (503) staff       (20)    10311 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/motu_utilities.py
--rwxr-xr-x   0 milanese   (503) staff       (20)   104242 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/motus.py
--rw-r--r--   0 milanese   (503) staff       (20)     3004 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/msamtools_python.py
--rw-r--r--   0 milanese   (503) staff       (20)    17003 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/print_CAMI.py
--rw-r--r--   0 milanese   (503) staff       (20)    11214 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/runBWA.py
--rw-r--r--   0 milanese   (503) staff       (20)    11256 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/runBWA_for_snv.py
--rw-r--r--   0 milanese   (503) staff       (20)     7645 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/motus/test.py
--rw-r--r--   0 milanese   (503) staff       (20)       76 2022-07-13 14:50:15.000000 motu-profiler-3.0.3/setup.cfg
--rw-r--r--   0 milanese   (503) staff       (20)     1250 2022-07-13 14:49:59.000000 motu-profiler-3.0.3/setup.py
+drwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)        0 2023-04-13 15:51:34.775221 motu-profiler-3.1.0/
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    32472 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/LICENSE
+-rwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     8434 2023-04-13 15:51:34.777250 motu-profiler-3.1.0/PKG-INFO
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     7593 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/README.md
+drwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)        0 2023-04-13 15:51:34.629504 motu-profiler-3.1.0/motu_profiler.egg-info/
+-rwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     8434 2023-04-13 15:51:34.603572 motu-profiler-3.1.0/motu_profiler.egg-info/PKG-INFO
+-rwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)      598 2023-04-13 15:51:34.610455 motu-profiler-3.1.0/motu_profiler.egg-info/SOURCES.txt
+-rwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)        1 2023-04-13 15:51:34.617126 motu-profiler-3.1.0/motu_profiler.egg-info/dependency_links.txt
+-rwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)       43 2023-04-13 15:51:34.624151 motu-profiler-3.1.0/motu_profiler.egg-info/entry_points.txt
+-rwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)        6 2023-04-13 15:51:34.630833 motu-profiler-3.1.0/motu_profiler.egg-info/top_level.txt
+drwxrwx---   0 alessiom (192165) biol-micro-sunagawa-primary (200980)        0 2023-04-13 15:51:34.768767 motu-profiler-3.1.0/motus/
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    16191 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/PEfiltering.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    13757 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/UTIL_log.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    19177 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/UTIL_log_col.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    19496 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/append.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     5629 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/convert_long_reads.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     5623 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/downloadDB.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    54316 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/map_genes_to_mOTUs.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    42460 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/map_mOTUs_to_LGs.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    12709 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/metaSNV_DistDiv.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    13430 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/metaSNV_Filtering_2.0.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    10352 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/motu_utilities.py
+-rwxr-xr-x   0 alessiom (192165) biol-micro-sunagawa-primary (200980)   104242 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/motus.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     3004 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/msamtools_python.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    17003 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/print_CAMI.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    11214 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/runBWA.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)    11256 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/runBWA_for_snv.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     7645 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/motus/test.py
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)       76 2023-04-13 15:51:34.783994 motu-profiler-3.1.0/setup.cfg
+-rw-r--r--   0 alessiom (192165) biol-micro-sunagawa-primary (200980)     1250 2023-04-13 15:50:31.000000 motu-profiler-3.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `motu-profiler-3.0.3/PKG-INFO` & `motu-profiler-3.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,203 @@
 Metadata-Version: 2.1
 Name: motu-profiler
-Version: 3.0.3
+Version: 3.1.0
 Summary: Taxonomic profiling of metagenomes from diverse environments with mOTUs3
 Home-page: https://github.com/motu-tool/mOTUs
+Download-URL: https://github.com/motu-tool/mOTUs/archive/refs/tags/3.1.0.tar.gz
 Author: Alessio Milanese
 Author-email: alessiom@ethz.ch
 License: GPLv3
-Download-URL: https://github.com/motu-tool/mOTUs/archive/refs/tags/3.0.3.tar.gz
-Description: ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motu_logo.png)
-        
-        [![Build status](https://ci.appveyor.com/api/projects/status/0x4veuuoabm6018v/branch/master?svg=true)](https://ci.appveyor.com/project/AlessioMilanese/motus-v2/branch/master)
-        [![Install with Bioconda](https://anaconda.org/bioconda/motus/badges/installer/conda.svg)](https://anaconda.org/bioconda/motus)
-        [![license](https://anaconda.org/bioconda/motus/badges/license.svg)](https://github.com/motu-tool/mOTUs_v2/blob/master/LICENSE)
-        [![Install with Bioconda](https://img.shields.io/conda/dn/bioconda/motus.svg?style=flat)](https://anaconda.org/bioconda/motus)
-        
-        
-        mOTU profiler
-        ========
-        
-        The mOTU profiler is a computational tool that estimates relative taxonomic abundance of known and currently unknown microbial community members using metagenomic shotgun sequencing data.
-        
-        Check the [wiki](https://github.com/motu-tool/mOTUs/wiki) for more information.
-        
-        If you are using mOTUs, please cite:
-        
-        > Alessio Milanese, Daniel R Mende, Lucas Paoli, Guillem Salazar, Hans-Joachim Ruscheweyh, Miguelangel Cuenca,
-        > Pascal Hingamp, Renato Alves, Paul I Costea, Luis Pedro Coelho, Thomas S B Schmidt,
-        > Alexandre Almeida, Alex L Mitchell, Robert D Finn, Jaime Huerta-Cepas,
-        > Peer Bork, Georg Zeller & Shinichi Sunagawa.
-        > **Microbial abundance, activity and population genomic profiling with mOTUs2**; _Nature Communications_ **10**, Article number: 1014 (2019).
-        > PMID: 30833550;
-        > doi: [10.1038/s41467-019-08844-4](https://www.nature.com/articles/s41467-019-08844-4)
-        
-        
-        Pre-requisites
-        --------------
-        
-        The mOTU profiler requires:
-        * Python 3 (or higher)
-        * the Burrow-Wheeler Aligner v0.7.15 or higher ([bwa](https://github.com/lh3/bwa))
-        * SAMtools v1.5 or higher ([link](http://www.htslib.org/download/))
-        
-        In order to use the command ```snv_call``` you need:
-        * [metaSNV v1.0.3](https://git.embl.de/costea/metaSNV), available also on [bioconda](https://anaconda.org/bioconda/metasnv) (we assume metaSNV.py to be in the system path)
-        
-        Check [installation wiki](https://github.com/motu-tool/mOTUs/wiki/Installation) to see how to install the dependencies with conda.
-        
-        Installation
-        --------------
-        
-        mOTUs can be installed either by using `pip` or via `conda`.
-        Installation with `conda` has the advantage that it will also download and install dependencies:
-        ```bash
-        # Install in the base environment
-        conda install motus
-        
-        # OR, create a new environment
-        conda create -n motu-env motus
-        conda activate motu-env
-        ```
-        
-        Installation with `pip`:
-        ```bash
-        # Download and install mOTUs
-        pip install motu-profiler
-        # Download the mOTUs database
-        motus downloadDB
-        ```
-        
-        You can test that motus is intalled correctly with:
-        ```
-        motus profile --test
-        ```
-        
-        Basic examples
-        --------------
-        Here is a simple example on how to obtain a taxonomic profiling from a raw read file:
-        
-        ```bash
-        motus profile -s metagenomic_sample.fastq > taxonomy_profile.txt
-        ```
-        
-        You can separate the previous call as:
-        ```bash
-        motus map_tax -s metagenomic_sample.fastq -o mapped_reads.sam
-        motus calc_mgc -i mapped_reads.sam -o mgc_ab_table.count
-        motus calc_motu -i mgc_ab_table.count > taxonomy_profile.txt
-        rm mapped_reads.sam mgc_ab_table.count
-        ```
-        
-        
-        The use of multiple threads (`-t`) is recommended, since bwa will finish faster. Here is an example with Paired-End reads:
-        
-        ```bash
-        motus profile -f for_sample.fastq -r rev_sample.fastq -s no_pair.fastq -t 6 > taxonomy_profile.txt
-        ```
-        
-        You can merge taxonomy files from different samples with `mOTU merge`:
-        
-        ```shell
-        motus profile -s metagenomic_sample_1.fastq -o taxonomy_profile_1.txt
-        motus profile -s metagenomic_sample_2.fastq -o taxonomy_profile_2.txt
-        motus merge -i taxonomy_profile_1.txt,taxonomy_profile_2.txt > all_sample_profiles.txt
-        ```
-        
-        You can profile samples that have been sequenced through different runs:
-        ```shell
-        motus profile -f sample1_run1_for.fastq,sample1_run2_for.fastq -r sample1_run1_rev.fastq,sample1_run2_rev.fastq -s sample1_run1_single.fastq > taxonomy_profile.txt
-        ```
-        
-        How mOTUs works
-        --------------
-        The mOTUs tool performs taxonomic profiling of metagenomics and metatrancriptomics samples, i.e. it identifies species and their relative abundance present in a sample. It is based on a set of mOTUs (~species) contained in the mOTUs database.
-        The mOTUs database is created from reference genomes, metagenomic samples and metagenome assembled genomes (MAGs):
-        
-        ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motus_type.png)
-        
-        A mOTUs database is composed of three types of mOTUs:
-        - ref-mOTUs, which represent **known species**,
-        - meta-mOTUs, which represent **unknown species** obtained from metagenomic samples,
-        - ext-mOTUs, which represent **unknown species** obtained from MAGs.
-        
-        Note that meta- and ext-mOTUs will not have a species level annotation.
-        
-        The mOTUs database is updated periodically, e.g the latest version (2.6.1), which doubles the number of profilable species by including ~600,000 draft genomes. Major releases are represented in the following graph (where the numbers represents the number of mOTUs for each of the three groups, with the same color-code as the previous graph):
-        ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/mOTUs_versions_2.png)
-        
-        When profiling (`motus profile`) a metagenomic sample, the mOTUs tool maps the reads from the sample to the genes in the different mOTUs:
-        ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/tax_profiling.png)
-        
-        ChangeLog
-        --------------
-        **Version 3.0.3 2022-07-13 by AlessioMilanese**
-        * Add command `prep_long` to allow the profiling of long reads (more information [here](https://github.com/motu-tool/mOTUs/wiki/Profile-long-reads)).
-        
-        **Version 3.0.2 2022-01-31 by AlessioMilanese**
-        * Convert the repository to a python package and submit to PyPI
-        
-        **Version 3.0.1 2021-07-27 by AlessioMilanese**
-        * Improve ref-mOTUs taxonomy according to #76
-        * Solve bug with `-A` option
-        
-        **Version 3.0.0 2021-06-22 by AlessioMilanese**
-        * Improve code base
-        * Minor bug fixes
-        
-        **Version 2.6.1 2021-04-27 by AlessioMilanese**
-        * Minor bug fixes
-        * Improved the taxonomy of 32 ref-mOTUs (#45)
-        
-        **Version 2.6.0 2021-03-08 by AlessioMilanese**
-        * Add 19,358 new mOTUs
-        * Add taxonomic profiles of > 11k metagenomic and metatranscriptomic samples. The updated merge function can integrate those in to the users results.
-        * Minor bug fixes
-        * Change `-1` to `unassigned`
-        
-        **Version 2.5.1 2019-08-17 by AlessioMilanese**
-        * Update the taxonomy to participate to the CAMI 2 challenge
-        
-        **Version 2.5.0 2019-08-09 by AlessioMilanese**
-        * Add -db option to use a database from another directory
-        * Add -A to print all taxonomy levels together
-        * Update the database with more than 60k new reference genomes. There are 11,915 ref-mOTUs and 2,297 meta-mOTUs.
-        
-        **Version 2.1.1 2019-03-04 by AlessioMilanese**
-        * Correct problem with samtools when installing with conda
-        
-        **Version 2.1.0 2019-03-03 by AlessioMilanese**
-        * Correct error \'\t\t\' when printing -C recall
-        * Update database (gene coordinates)
-        
-        **Version 2.0.1 2018-08-23 by AlessioMilanese**
-        * Add -C to print the result in CAMI format (BioBoxes format 0.9.1)
-        * Add -K to snv_call command to keep all the directories produced by metaSNV
-        
-        **Version 2.0.0 2018-06-12 by AlessioMilanese**
-        * Set relative abundances as default (instead of counts)
-        * Add -B to print the result in BIOM format
-        * Add test directory
-        * Python2 is not supported anymore
-        * Minor bug fixes
-        
-        **Version 2.0.0-rc1 2018-05-10 by AlessioMilanese**
-        * First release supporting all basic functionality.
-        
 Keywords: bioinformatics metagenomics taxonomic profiling
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motu_logo.png)
+
+[![Build status](https://ci.appveyor.com/api/projects/status/0x4veuuoabm6018v/branch/master?svg=true)](https://ci.appveyor.com/project/AlessioMilanese/motus-v2/branch/master)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/motus/README.html)
+[![license](https://anaconda.org/bioconda/motus/badges/license.svg)](https://github.com/motu-tool/mOTUs_v2/blob/master/LICENSE)
+[![Install with Bioconda](https://img.shields.io/conda/dn/bioconda/motus.svg?style=flat)](https://anaconda.org/bioconda/motus)
+
+
+mOTU profiler
+========
+
+The mOTU profiler is a computational tool that estimates relative taxonomic abundance of known and currently unknown microbial community members using metagenomic shotgun sequencing data.
+
+Check the [wiki](https://github.com/motu-tool/mOTUs/wiki) for more information.
+
+If you are using mOTUs, please cite:
+
+> **Reference genome-independent taxonomic profiling of microbiomes with mOTUs3**
+> 
+> Hans-Joachim Ruscheweyh*, Alessio Milanese*, Lucas Paoli, Nicolai Karcher, Quentin Clayssen,
+> Marisa Isabell Metzger, Jakob Wirbel, Peer Bork, Daniel R. Mende, Georg Zeller# & Shinichi Sunagawa#
+> 
+> _Microbiome_ (2022)
+> 
+> doi: [10.1186/s40168-022-01410-z](https://microbiomejournal.biomedcentral.com/articles/10.1186/s40168-022-01410-z)
+
+
+
+
+Pre-requisites
+--------------
+
+The mOTU profiler requires:
+* Python 3 (or higher)
+* the Burrow-Wheeler Aligner v0.7.15 or higher ([bwa](https://github.com/lh3/bwa))
+* SAMtools v1.5 or higher ([link](http://www.htslib.org/download/))
+
+In order to use the command ```snv_call``` you need:
+* [metaSNV v1.0.3](https://git.embl.de/costea/metaSNV), available also on [bioconda](https://anaconda.org/bioconda/metasnv) (we assume metaSNV.py to be in the system path)
+
+Check [installation wiki](https://github.com/motu-tool/mOTUs/wiki/Installation) to see how to install the dependencies with conda.
+
+Installation
+--------------
+
+mOTUs can be installed either by using `pip` or via `conda`.
+Installation with `conda` has the advantage that it will also download and install dependencies:
+```bash
+# Install in the base environment
+conda install motus
+
+# OR, create a new environment
+conda create -n motu-env motus
+conda activate motu-env
+```
+
+Installation with `pip`:
+```bash
+# Download and install mOTUs
+pip install motu-profiler
+# Download the mOTUs database
+motus downloadDB
+```
+
+You can test that motus is intalled correctly with:
+```
+motus profile --test
+```
+
+Basic examples
+--------------
+Here is a simple example on how to obtain a taxonomic profiling from a raw read file:
+
+```bash
+motus profile -s metagenomic_sample.fastq > taxonomy_profile.txt
+```
+
+You can separate the previous call as:
+```bash
+motus map_tax -s metagenomic_sample.fastq -o mapped_reads.sam
+motus calc_mgc -i mapped_reads.sam -o mgc_ab_table.count
+motus calc_motu -i mgc_ab_table.count > taxonomy_profile.txt
+rm mapped_reads.sam mgc_ab_table.count
+```
+
+
+The use of multiple threads (`-t`) is recommended, since bwa will finish faster. Here is an example with Paired-End reads:
+
+```bash
+motus profile -f for_sample.fastq -r rev_sample.fastq -s no_pair.fastq -t 6 > taxonomy_profile.txt
+```
+
+You can merge taxonomy files from different samples with `mOTU merge`:
+
+```shell
+motus profile -s metagenomic_sample_1.fastq -o taxonomy_profile_1.txt
+motus profile -s metagenomic_sample_2.fastq -o taxonomy_profile_2.txt
+motus merge -i taxonomy_profile_1.txt,taxonomy_profile_2.txt > all_sample_profiles.txt
+```
+
+You can profile samples that have been sequenced through different runs:
+```shell
+motus profile -f sample1_run1_for.fastq,sample1_run2_for.fastq -r sample1_run1_rev.fastq,sample1_run2_rev.fastq -s sample1_run1_single.fastq > taxonomy_profile.txt
+```
+
+How mOTUs works
+--------------
+The mOTUs tool performs taxonomic profiling of metagenomics and metatrancriptomics samples, i.e. it identifies species and their relative abundance present in a sample. It is based on a set of mOTUs (~species) contained in the mOTUs database.
+The mOTUs database is created from reference genomes, metagenomic samples and metagenome assembled genomes (MAGs):
+
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motus_type.png)
+
+A mOTUs database is composed of three types of mOTUs:
+- ref-mOTUs, which represent **known species**,
+- meta-mOTUs, which represent **unknown species** obtained from metagenomic samples,
+- ext-mOTUs, which represent **unknown species** obtained from MAGs.
+
+Note that meta- and ext-mOTUs will not have a species level annotation.
+
+The mOTUs database is updated periodically, e.g the latest version (3.0.3), which doubles the number of profilable species by including ~600,000 draft genomes. Major releases are represented in the following graph (where the numbers represents the number of mOTUs for each of the three groups, with the same color-code as the previous graph):
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/mOTUs_versions_2.png)
+
+When profiling (`motus profile`) a metagenomic sample, the mOTUs tool maps the reads from the sample to the genes in the different mOTUs:
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/tax_profiling.png)
+
+ChangeLog
+--------------
+
+**Version 3.1.0 2023-03-28 by AlessioMilanese**
+* Improve database clustering algorithm and update the database (change the number of ext-mOTUs from 19,358 to 20,128)
+
+**Version 3.0.3 2022-07-13 by AlessioMilanese**
+* Add command `prep_long` to allow the profiling of long reads (more information [here](https://github.com/motu-tool/mOTUs/wiki/Profile-long-reads))
+
+**Version 3.0.2 2022-01-31 by AlessioMilanese**
+* Convert the repository to a python package and submit to PyPI
+
+**Version 3.0.1 2021-07-27 by AlessioMilanese**
+* Improve ref-mOTUs taxonomy according to #76
+* Solve bug with `-A` option
+
+**Version 3.0.0 2021-06-22 by AlessioMilanese**
+* Improve code base
+* Minor bug fixes
+
+**Version 2.6.1 2021-04-27 by AlessioMilanese**
+* Minor bug fixes
+* Improved the taxonomy of 32 ref-mOTUs (#45)
+
+**Version 2.6.0 2021-03-08 by AlessioMilanese**
+* Add 19,358 new mOTUs
+* Add taxonomic profiles of > 11k metagenomic and metatranscriptomic samples. The updated merge function can integrate those in to the users results.
+* Minor bug fixes
+* Change `-1` to `unassigned`
+
+**Version 2.5.1 2019-08-17 by AlessioMilanese**
+* Update the taxonomy to participate to the CAMI 2 challenge
+
+**Version 2.5.0 2019-08-09 by AlessioMilanese**
+* Add -db option to use a database from another directory
+* Add -A to print all taxonomy levels together
+* Update the database with more than 60k new reference genomes. There are 11,915 ref-mOTUs and 2,297 meta-mOTUs.
+
+**Version 2.1.1 2019-03-04 by AlessioMilanese**
+* Correct problem with samtools when installing with conda
+
+**Version 2.1.0 2019-03-03 by AlessioMilanese**
+* Correct error \'\t\t\' when printing -C recall
+* Update database (gene coordinates)
+
+**Version 2.0.1 2018-08-23 by AlessioMilanese**
+* Add -C to print the result in CAMI format (BioBoxes format 0.9.1)
+* Add -K to snv_call command to keep all the directories produced by metaSNV
+
+**Version 2.0.0 2018-06-12 by AlessioMilanese**
+* Set relative abundances as default (instead of counts)
+* Add -B to print the result in BIOM format
+* Add test directory
+* Python2 is not supported anymore
+* Minor bug fixes
+
+**Version 2.0.0-rc1 2018-05-10 by AlessioMilanese**
+* First release supporting all basic functionality.
```

### Comparing `motu-profiler-3.0.3/README.md` & `motu-profiler-3.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motu_logo.png)
 
 [![Build status](https://ci.appveyor.com/api/projects/status/0x4veuuoabm6018v/branch/master?svg=true)](https://ci.appveyor.com/project/AlessioMilanese/motus-v2/branch/master)
-[![Install with Bioconda](https://anaconda.org/bioconda/motus/badges/installer/conda.svg)](https://anaconda.org/bioconda/motus)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/motus/README.html)
 [![license](https://anaconda.org/bioconda/motus/badges/license.svg)](https://github.com/motu-tool/mOTUs_v2/blob/master/LICENSE)
 [![Install with Bioconda](https://img.shields.io/conda/dn/bioconda/motus.svg?style=flat)](https://anaconda.org/bioconda/motus)
 
 
 mOTU profiler
 ========
 
 The mOTU profiler is a computational tool that estimates relative taxonomic abundance of known and currently unknown microbial community members using metagenomic shotgun sequencing data.
 
 Check the [wiki](https://github.com/motu-tool/mOTUs/wiki) for more information.
 
 If you are using mOTUs, please cite:
 
-> Alessio Milanese, Daniel R Mende, Lucas Paoli, Guillem Salazar, Hans-Joachim Ruscheweyh, Miguelangel Cuenca,
-> Pascal Hingamp, Renato Alves, Paul I Costea, Luis Pedro Coelho, Thomas S B Schmidt,
-> Alexandre Almeida, Alex L Mitchell, Robert D Finn, Jaime Huerta-Cepas,
-> Peer Bork, Georg Zeller & Shinichi Sunagawa.
-> **Microbial abundance, activity and population genomic profiling with mOTUs2**; _Nature Communications_ **10**, Article number: 1014 (2019).
-> PMID: 30833550;
-> doi: [10.1038/s41467-019-08844-4](https://www.nature.com/articles/s41467-019-08844-4)
+> **Reference genome-independent taxonomic profiling of microbiomes with mOTUs3**
+> 
+> Hans-Joachim Ruscheweyh*, Alessio Milanese*, Lucas Paoli, Nicolai Karcher, Quentin Clayssen,
+> Marisa Isabell Metzger, Jakob Wirbel, Peer Bork, Daniel R. Mende, Georg Zeller# & Shinichi Sunagawa#
+> 
+> _Microbiome_ (2022)
+> 
+> doi: [10.1186/s40168-022-01410-z](https://microbiomejournal.biomedcentral.com/articles/10.1186/s40168-022-01410-z)
+
+
 
 
 Pre-requisites
 --------------
 
 The mOTU profiler requires:
 * Python 3 (or higher)
@@ -110,24 +113,28 @@
 A mOTUs database is composed of three types of mOTUs:
 - ref-mOTUs, which represent **known species**,
 - meta-mOTUs, which represent **unknown species** obtained from metagenomic samples,
 - ext-mOTUs, which represent **unknown species** obtained from MAGs.
 
 Note that meta- and ext-mOTUs will not have a species level annotation.
 
-The mOTUs database is updated periodically, e.g the latest version (2.6.1), which doubles the number of profilable species by including ~600,000 draft genomes. Major releases are represented in the following graph (where the numbers represents the number of mOTUs for each of the three groups, with the same color-code as the previous graph):
+The mOTUs database is updated periodically, e.g the latest version (3.0.3), which doubles the number of profilable species by including ~600,000 draft genomes. Major releases are represented in the following graph (where the numbers represents the number of mOTUs for each of the three groups, with the same color-code as the previous graph):
 ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/mOTUs_versions_2.png)
 
 When profiling (`motus profile`) a metagenomic sample, the mOTUs tool maps the reads from the sample to the genes in the different mOTUs:
 ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/tax_profiling.png)
 
 ChangeLog
 --------------
+
+**Version 3.1.0 2023-03-28 by AlessioMilanese**
+* Improve database clustering algorithm and update the database (change the number of ext-mOTUs from 19,358 to 20,128)
+
 **Version 3.0.3 2022-07-13 by AlessioMilanese**
-* Add command `prep_long` to allow the profiling of long reads (more information [here](https://github.com/motu-tool/mOTUs/wiki/Profile-long-reads)).
+* Add command `prep_long` to allow the profiling of long reads (more information [here](https://github.com/motu-tool/mOTUs/wiki/Profile-long-reads))
 
 **Version 3.0.2 2022-01-31 by AlessioMilanese**
 * Convert the repository to a python package and submit to PyPI
 
 **Version 3.0.1 2021-07-27 by AlessioMilanese**
 * Improve ref-mOTUs taxonomy according to #76
 * Solve bug with `-A` option
```

### Comparing `motu-profiler-3.0.3/motu_profiler.egg-info/PKG-INFO` & `motu-profiler-3.1.0/motu_profiler.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,203 @@
 Metadata-Version: 2.1
 Name: motu-profiler
-Version: 3.0.3
+Version: 3.1.0
 Summary: Taxonomic profiling of metagenomes from diverse environments with mOTUs3
 Home-page: https://github.com/motu-tool/mOTUs
+Download-URL: https://github.com/motu-tool/mOTUs/archive/refs/tags/3.1.0.tar.gz
 Author: Alessio Milanese
 Author-email: alessiom@ethz.ch
 License: GPLv3
-Download-URL: https://github.com/motu-tool/mOTUs/archive/refs/tags/3.0.3.tar.gz
-Description: ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motu_logo.png)
-        
-        [![Build status](https://ci.appveyor.com/api/projects/status/0x4veuuoabm6018v/branch/master?svg=true)](https://ci.appveyor.com/project/AlessioMilanese/motus-v2/branch/master)
-        [![Install with Bioconda](https://anaconda.org/bioconda/motus/badges/installer/conda.svg)](https://anaconda.org/bioconda/motus)
-        [![license](https://anaconda.org/bioconda/motus/badges/license.svg)](https://github.com/motu-tool/mOTUs_v2/blob/master/LICENSE)
-        [![Install with Bioconda](https://img.shields.io/conda/dn/bioconda/motus.svg?style=flat)](https://anaconda.org/bioconda/motus)
-        
-        
-        mOTU profiler
-        ========
-        
-        The mOTU profiler is a computational tool that estimates relative taxonomic abundance of known and currently unknown microbial community members using metagenomic shotgun sequencing data.
-        
-        Check the [wiki](https://github.com/motu-tool/mOTUs/wiki) for more information.
-        
-        If you are using mOTUs, please cite:
-        
-        > Alessio Milanese, Daniel R Mende, Lucas Paoli, Guillem Salazar, Hans-Joachim Ruscheweyh, Miguelangel Cuenca,
-        > Pascal Hingamp, Renato Alves, Paul I Costea, Luis Pedro Coelho, Thomas S B Schmidt,
-        > Alexandre Almeida, Alex L Mitchell, Robert D Finn, Jaime Huerta-Cepas,
-        > Peer Bork, Georg Zeller & Shinichi Sunagawa.
-        > **Microbial abundance, activity and population genomic profiling with mOTUs2**; _Nature Communications_ **10**, Article number: 1014 (2019).
-        > PMID: 30833550;
-        > doi: [10.1038/s41467-019-08844-4](https://www.nature.com/articles/s41467-019-08844-4)
-        
-        
-        Pre-requisites
-        --------------
-        
-        The mOTU profiler requires:
-        * Python 3 (or higher)
-        * the Burrow-Wheeler Aligner v0.7.15 or higher ([bwa](https://github.com/lh3/bwa))
-        * SAMtools v1.5 or higher ([link](http://www.htslib.org/download/))
-        
-        In order to use the command ```snv_call``` you need:
-        * [metaSNV v1.0.3](https://git.embl.de/costea/metaSNV), available also on [bioconda](https://anaconda.org/bioconda/metasnv) (we assume metaSNV.py to be in the system path)
-        
-        Check [installation wiki](https://github.com/motu-tool/mOTUs/wiki/Installation) to see how to install the dependencies with conda.
-        
-        Installation
-        --------------
-        
-        mOTUs can be installed either by using `pip` or via `conda`.
-        Installation with `conda` has the advantage that it will also download and install dependencies:
-        ```bash
-        # Install in the base environment
-        conda install motus
-        
-        # OR, create a new environment
-        conda create -n motu-env motus
-        conda activate motu-env
-        ```
-        
-        Installation with `pip`:
-        ```bash
-        # Download and install mOTUs
-        pip install motu-profiler
-        # Download the mOTUs database
-        motus downloadDB
-        ```
-        
-        You can test that motus is intalled correctly with:
-        ```
-        motus profile --test
-        ```
-        
-        Basic examples
-        --------------
-        Here is a simple example on how to obtain a taxonomic profiling from a raw read file:
-        
-        ```bash
-        motus profile -s metagenomic_sample.fastq > taxonomy_profile.txt
-        ```
-        
-        You can separate the previous call as:
-        ```bash
-        motus map_tax -s metagenomic_sample.fastq -o mapped_reads.sam
-        motus calc_mgc -i mapped_reads.sam -o mgc_ab_table.count
-        motus calc_motu -i mgc_ab_table.count > taxonomy_profile.txt
-        rm mapped_reads.sam mgc_ab_table.count
-        ```
-        
-        
-        The use of multiple threads (`-t`) is recommended, since bwa will finish faster. Here is an example with Paired-End reads:
-        
-        ```bash
-        motus profile -f for_sample.fastq -r rev_sample.fastq -s no_pair.fastq -t 6 > taxonomy_profile.txt
-        ```
-        
-        You can merge taxonomy files from different samples with `mOTU merge`:
-        
-        ```shell
-        motus profile -s metagenomic_sample_1.fastq -o taxonomy_profile_1.txt
-        motus profile -s metagenomic_sample_2.fastq -o taxonomy_profile_2.txt
-        motus merge -i taxonomy_profile_1.txt,taxonomy_profile_2.txt > all_sample_profiles.txt
-        ```
-        
-        You can profile samples that have been sequenced through different runs:
-        ```shell
-        motus profile -f sample1_run1_for.fastq,sample1_run2_for.fastq -r sample1_run1_rev.fastq,sample1_run2_rev.fastq -s sample1_run1_single.fastq > taxonomy_profile.txt
-        ```
-        
-        How mOTUs works
-        --------------
-        The mOTUs tool performs taxonomic profiling of metagenomics and metatrancriptomics samples, i.e. it identifies species and their relative abundance present in a sample. It is based on a set of mOTUs (~species) contained in the mOTUs database.
-        The mOTUs database is created from reference genomes, metagenomic samples and metagenome assembled genomes (MAGs):
-        
-        ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motus_type.png)
-        
-        A mOTUs database is composed of three types of mOTUs:
-        - ref-mOTUs, which represent **known species**,
-        - meta-mOTUs, which represent **unknown species** obtained from metagenomic samples,
-        - ext-mOTUs, which represent **unknown species** obtained from MAGs.
-        
-        Note that meta- and ext-mOTUs will not have a species level annotation.
-        
-        The mOTUs database is updated periodically, e.g the latest version (2.6.1), which doubles the number of profilable species by including ~600,000 draft genomes. Major releases are represented in the following graph (where the numbers represents the number of mOTUs for each of the three groups, with the same color-code as the previous graph):
-        ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/mOTUs_versions_2.png)
-        
-        When profiling (`motus profile`) a metagenomic sample, the mOTUs tool maps the reads from the sample to the genes in the different mOTUs:
-        ![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/tax_profiling.png)
-        
-        ChangeLog
-        --------------
-        **Version 3.0.3 2022-07-13 by AlessioMilanese**
-        * Add command `prep_long` to allow the profiling of long reads (more information [here](https://github.com/motu-tool/mOTUs/wiki/Profile-long-reads)).
-        
-        **Version 3.0.2 2022-01-31 by AlessioMilanese**
-        * Convert the repository to a python package and submit to PyPI
-        
-        **Version 3.0.1 2021-07-27 by AlessioMilanese**
-        * Improve ref-mOTUs taxonomy according to #76
-        * Solve bug with `-A` option
-        
-        **Version 3.0.0 2021-06-22 by AlessioMilanese**
-        * Improve code base
-        * Minor bug fixes
-        
-        **Version 2.6.1 2021-04-27 by AlessioMilanese**
-        * Minor bug fixes
-        * Improved the taxonomy of 32 ref-mOTUs (#45)
-        
-        **Version 2.6.0 2021-03-08 by AlessioMilanese**
-        * Add 19,358 new mOTUs
-        * Add taxonomic profiles of > 11k metagenomic and metatranscriptomic samples. The updated merge function can integrate those in to the users results.
-        * Minor bug fixes
-        * Change `-1` to `unassigned`
-        
-        **Version 2.5.1 2019-08-17 by AlessioMilanese**
-        * Update the taxonomy to participate to the CAMI 2 challenge
-        
-        **Version 2.5.0 2019-08-09 by AlessioMilanese**
-        * Add -db option to use a database from another directory
-        * Add -A to print all taxonomy levels together
-        * Update the database with more than 60k new reference genomes. There are 11,915 ref-mOTUs and 2,297 meta-mOTUs.
-        
-        **Version 2.1.1 2019-03-04 by AlessioMilanese**
-        * Correct problem with samtools when installing with conda
-        
-        **Version 2.1.0 2019-03-03 by AlessioMilanese**
-        * Correct error \'\t\t\' when printing -C recall
-        * Update database (gene coordinates)
-        
-        **Version 2.0.1 2018-08-23 by AlessioMilanese**
-        * Add -C to print the result in CAMI format (BioBoxes format 0.9.1)
-        * Add -K to snv_call command to keep all the directories produced by metaSNV
-        
-        **Version 2.0.0 2018-06-12 by AlessioMilanese**
-        * Set relative abundances as default (instead of counts)
-        * Add -B to print the result in BIOM format
-        * Add test directory
-        * Python2 is not supported anymore
-        * Minor bug fixes
-        
-        **Version 2.0.0-rc1 2018-05-10 by AlessioMilanese**
-        * First release supporting all basic functionality.
-        
 Keywords: bioinformatics metagenomics taxonomic profiling
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motu_logo.png)
+
+[![Build status](https://ci.appveyor.com/api/projects/status/0x4veuuoabm6018v/branch/master?svg=true)](https://ci.appveyor.com/project/AlessioMilanese/motus-v2/branch/master)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/motus/README.html)
+[![license](https://anaconda.org/bioconda/motus/badges/license.svg)](https://github.com/motu-tool/mOTUs_v2/blob/master/LICENSE)
+[![Install with Bioconda](https://img.shields.io/conda/dn/bioconda/motus.svg?style=flat)](https://anaconda.org/bioconda/motus)
+
+
+mOTU profiler
+========
+
+The mOTU profiler is a computational tool that estimates relative taxonomic abundance of known and currently unknown microbial community members using metagenomic shotgun sequencing data.
+
+Check the [wiki](https://github.com/motu-tool/mOTUs/wiki) for more information.
+
+If you are using mOTUs, please cite:
+
+> **Reference genome-independent taxonomic profiling of microbiomes with mOTUs3**
+> 
+> Hans-Joachim Ruscheweyh*, Alessio Milanese*, Lucas Paoli, Nicolai Karcher, Quentin Clayssen,
+> Marisa Isabell Metzger, Jakob Wirbel, Peer Bork, Daniel R. Mende, Georg Zeller# & Shinichi Sunagawa#
+> 
+> _Microbiome_ (2022)
+> 
+> doi: [10.1186/s40168-022-01410-z](https://microbiomejournal.biomedcentral.com/articles/10.1186/s40168-022-01410-z)
+
+
+
+
+Pre-requisites
+--------------
+
+The mOTU profiler requires:
+* Python 3 (or higher)
+* the Burrow-Wheeler Aligner v0.7.15 or higher ([bwa](https://github.com/lh3/bwa))
+* SAMtools v1.5 or higher ([link](http://www.htslib.org/download/))
+
+In order to use the command ```snv_call``` you need:
+* [metaSNV v1.0.3](https://git.embl.de/costea/metaSNV), available also on [bioconda](https://anaconda.org/bioconda/metasnv) (we assume metaSNV.py to be in the system path)
+
+Check [installation wiki](https://github.com/motu-tool/mOTUs/wiki/Installation) to see how to install the dependencies with conda.
+
+Installation
+--------------
+
+mOTUs can be installed either by using `pip` or via `conda`.
+Installation with `conda` has the advantage that it will also download and install dependencies:
+```bash
+# Install in the base environment
+conda install motus
+
+# OR, create a new environment
+conda create -n motu-env motus
+conda activate motu-env
+```
+
+Installation with `pip`:
+```bash
+# Download and install mOTUs
+pip install motu-profiler
+# Download the mOTUs database
+motus downloadDB
+```
+
+You can test that motus is intalled correctly with:
+```
+motus profile --test
+```
+
+Basic examples
+--------------
+Here is a simple example on how to obtain a taxonomic profiling from a raw read file:
+
+```bash
+motus profile -s metagenomic_sample.fastq > taxonomy_profile.txt
+```
+
+You can separate the previous call as:
+```bash
+motus map_tax -s metagenomic_sample.fastq -o mapped_reads.sam
+motus calc_mgc -i mapped_reads.sam -o mgc_ab_table.count
+motus calc_motu -i mgc_ab_table.count > taxonomy_profile.txt
+rm mapped_reads.sam mgc_ab_table.count
+```
+
+
+The use of multiple threads (`-t`) is recommended, since bwa will finish faster. Here is an example with Paired-End reads:
+
+```bash
+motus profile -f for_sample.fastq -r rev_sample.fastq -s no_pair.fastq -t 6 > taxonomy_profile.txt
+```
+
+You can merge taxonomy files from different samples with `mOTU merge`:
+
+```shell
+motus profile -s metagenomic_sample_1.fastq -o taxonomy_profile_1.txt
+motus profile -s metagenomic_sample_2.fastq -o taxonomy_profile_2.txt
+motus merge -i taxonomy_profile_1.txt,taxonomy_profile_2.txt > all_sample_profiles.txt
+```
+
+You can profile samples that have been sequenced through different runs:
+```shell
+motus profile -f sample1_run1_for.fastq,sample1_run2_for.fastq -r sample1_run1_rev.fastq,sample1_run2_rev.fastq -s sample1_run1_single.fastq > taxonomy_profile.txt
+```
+
+How mOTUs works
+--------------
+The mOTUs tool performs taxonomic profiling of metagenomics and metatrancriptomics samples, i.e. it identifies species and their relative abundance present in a sample. It is based on a set of mOTUs (~species) contained in the mOTUs database.
+The mOTUs database is created from reference genomes, metagenomic samples and metagenome assembled genomes (MAGs):
+
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/motus_type.png)
+
+A mOTUs database is composed of three types of mOTUs:
+- ref-mOTUs, which represent **known species**,
+- meta-mOTUs, which represent **unknown species** obtained from metagenomic samples,
+- ext-mOTUs, which represent **unknown species** obtained from MAGs.
+
+Note that meta- and ext-mOTUs will not have a species level annotation.
+
+The mOTUs database is updated periodically, e.g the latest version (3.0.3), which doubles the number of profilable species by including ~600,000 draft genomes. Major releases are represented in the following graph (where the numbers represents the number of mOTUs for each of the three groups, with the same color-code as the previous graph):
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/mOTUs_versions_2.png)
+
+When profiling (`motus profile`) a metagenomic sample, the mOTUs tool maps the reads from the sample to the genes in the different mOTUs:
+![alt text](https://raw.githubusercontent.com/motu-tool/mOTUs/master/pics/tax_profiling.png)
+
+ChangeLog
+--------------
+
+**Version 3.1.0 2023-03-28 by AlessioMilanese**
+* Improve database clustering algorithm and update the database (change the number of ext-mOTUs from 19,358 to 20,128)
+
+**Version 3.0.3 2022-07-13 by AlessioMilanese**
+* Add command `prep_long` to allow the profiling of long reads (more information [here](https://github.com/motu-tool/mOTUs/wiki/Profile-long-reads))
+
+**Version 3.0.2 2022-01-31 by AlessioMilanese**
+* Convert the repository to a python package and submit to PyPI
+
+**Version 3.0.1 2021-07-27 by AlessioMilanese**
+* Improve ref-mOTUs taxonomy according to #76
+* Solve bug with `-A` option
+
+**Version 3.0.0 2021-06-22 by AlessioMilanese**
+* Improve code base
+* Minor bug fixes
+
+**Version 2.6.1 2021-04-27 by AlessioMilanese**
+* Minor bug fixes
+* Improved the taxonomy of 32 ref-mOTUs (#45)
+
+**Version 2.6.0 2021-03-08 by AlessioMilanese**
+* Add 19,358 new mOTUs
+* Add taxonomic profiles of > 11k metagenomic and metatranscriptomic samples. The updated merge function can integrate those in to the users results.
+* Minor bug fixes
+* Change `-1` to `unassigned`
+
+**Version 2.5.1 2019-08-17 by AlessioMilanese**
+* Update the taxonomy to participate to the CAMI 2 challenge
+
+**Version 2.5.0 2019-08-09 by AlessioMilanese**
+* Add -db option to use a database from another directory
+* Add -A to print all taxonomy levels together
+* Update the database with more than 60k new reference genomes. There are 11,915 ref-mOTUs and 2,297 meta-mOTUs.
+
+**Version 2.1.1 2019-03-04 by AlessioMilanese**
+* Correct problem with samtools when installing with conda
+
+**Version 2.1.0 2019-03-03 by AlessioMilanese**
+* Correct error \'\t\t\' when printing -C recall
+* Update database (gene coordinates)
+
+**Version 2.0.1 2018-08-23 by AlessioMilanese**
+* Add -C to print the result in CAMI format (BioBoxes format 0.9.1)
+* Add -K to snv_call command to keep all the directories produced by metaSNV
+
+**Version 2.0.0 2018-06-12 by AlessioMilanese**
+* Set relative abundances as default (instead of counts)
+* Add -B to print the result in BIOM format
+* Add test directory
+* Python2 is not supported anymore
+* Minor bug fixes
+
+**Version 2.0.0-rc1 2018-05-10 by AlessioMilanese**
+* First release supporting all basic functionality.
```

### Comparing `motu-profiler-3.0.3/motu_profiler.egg-info/SOURCES.txt` & `motu-profiler-3.1.0/motu_profiler.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 motu_profiler.egg-info/PKG-INFO
 motu_profiler.egg-info/SOURCES.txt
 motu_profiler.egg-info/dependency_links.txt
 motu_profiler.egg-info/entry_points.txt
```

### Comparing `motu-profiler-3.0.3/motus/PEfiltering.py` & `motu-profiler-3.1.0/motus/PEfiltering.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/UTIL_log.py` & `motu-profiler-3.1.0/motus/UTIL_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,30 +43,30 @@
 ################################################################################
 # print menus
 def msg(version_tool):
     str_msg = '''
 \00
 Program: motus - a tool for marker gene-based OTU (mOTU) profiling
 Version: '''+version_tool+'''
-Reference: Milanese et al. Microbial abundance, activity and population genomic profiling with mOTUs2. Nature Communications (2019). doi: 10.1038/s41467-019-08844-4
+Reference: Ruscheweyh, Milanese et al. Reference genome-independent taxonomic profiling of microbiomes with mOTUs3. biorxiv (2022). doi: 10.1101/2021.04.20.440600
 
 Usage: motus <command> [options]
 
 Command:
       downloadDB  Download the mOTUs database
 
  -- Taxonomic profiling
       profile     Perform taxonomic profiling (map_tax + calc_mgc + calc_motu) in a single step
       merge       Merge several taxonomic profiling results into one table
 
       map_tax     Map reads to the marker gene database
       calc_mgc    Calculate marker gene cluster (MGC) abundance
       calc_motu   Summarize MGC abundances into a mOTU profile
 
-      prep_long   Prepare long reads to be sequenced by mOTUs
+      prep_long   Prepare long reads to be profiled by mOTUs
 
  -- SNV calling
       map_snv     Map reads to the marker gene database for SNV calling
       snv_call    Generate SNV profiles (using metaSNV)
 
 Type motus <command> to print the help menu for a specific command
         '''
```

### Comparing `motu-profiler-3.0.3/motus/UTIL_log_col.py` & `motu-profiler-3.1.0/motus/UTIL_log_col.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,30 +90,30 @@
 ################################################################################
 # print menus
 def msg(version_tool):
     str_msg = '''
 \00
 '''+colour("Program:","blue_bold")+''' motus - a tool for marker gene-based OTU (mOTU) profiling
 '''+colour("Version: ","blue_bold")+version_tool+'''
-'''+colour("Reference:","blue_bold")+''' Milanese et al. Microbial abundance, activity and population genomic profiling with mOTUs2. Nature Communications (2019). doi: 10.1038/s41467-019-08844-4
+'''+colour("Reference:","blue_bold")+''' Ruscheweyh, Milanese et al. Reference genome-independent taxonomic profiling of microbiomes with mOTUs3. biorxiv (2022). doi: 10.1101/2021.04.20.440600
 
 '''+colour("Usage:","blue_bold")+''' motus <command> [options]
 
 '''+colour("Command:","blue_bold")+'''
 '''+colour("      downloadDB","cyan")+'''  Download the mOTUs database
 
 '''+colour("-- Taxonomic profiling","bold")+'''
 '''+colour("      profile","cyan")+'''     Perform taxonomic profiling (map_tax + calc_mgc + calc_motu) in a single step
 '''+colour("      merge","cyan")+'''       Merge several taxonomic profiling results into one table
 
 '''+colour("      map_tax","cyan")+'''     Map reads to the marker gene database
 '''+colour("      calc_mgc","cyan")+'''    Calculate marker gene cluster (MGC) abundance
 '''+colour("      calc_motu","cyan")+'''   Summarize MGC abundances into a mOTU profile
 
-'''+colour("      prep_long","cyan")+'''   Prepare long reads to be sequenced by mOTUs
+'''+colour("      prep_long","cyan")+'''   Prepare long reads to be profiled by mOTUs
 
 '''+colour("-- SNV calling","bold")+'''
 '''+colour("      map_snv","cyan")+'''     Map reads to the marker gene database for SNV calling
 '''+colour("      snv_call","cyan")+'''    Generate SNV profiles (using metaSNV)
 
 Type motus <command> to print the help menu for a specific command
         '''
```

### Comparing `motu-profiler-3.0.3/motus/append.py` & `motu-profiler-3.1.0/motus/append.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/convert_long_reads.py` & `motu-profiler-3.1.0/motus/convert_long_reads.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/downloadDB.py` & `motu-profiler-3.1.0/motus/downloadDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #
 # Main steps:
 #    * Download the mOTUs database
 #    * Create a file with the version information
 #
 # ============================================================================ #
 
-motus_version = "3.0.3"
-link_db = "https://zenodo.org/record/5140350/files/db_mOTU_v3.0.1.tar.gz"
-md5_db = "f4fd09fad9b311fb4f21383f6101bfc3"
-DOI_db = "10.5281/zenodo.5140350"
+motus_version = "3.1.0"
+link_db = "https://zenodo.org/record/7778108/files/db_mOTU_v3.1.0.tar.gz"
+md5_db = "f841c36150025af837f7a9a358c9a3c3"
+DOI_db = "10.5281/zenodo.7778108"
 
 
 
 # function to print progress bar for python 3
 def reporthook(count, block_size, total_size):
     global start_time
     if count == 0:
```

### Comparing `motu-profiler-3.0.3/motus/map_genes_to_mOTUs.py` & `motu-profiler-3.1.0/motus/map_genes_to_mOTUs.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/map_mOTUs_to_LGs.py` & `motu-profiler-3.1.0/motus/map_mOTUs_to_LGs.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,18 @@
         counts_mOTUs_j = [float(numeric_string) for numeric_string in counts_mOTUs_j] # transform from string to float
 
         list_diff_zero = list()
         cog_type = list()
         for i in range(len(counts_mOTUs_j)):
             if counts_mOTUs_j[i]>0:
                 list_diff_zero.append(counts_mOTUs_j[i]) # find the one that are different from zero
-                cog_type.append(genes_list[i].split('.')[0]) # and save the COG type
+                # in 3.1 we have "ref_mOTU_v31_00009.COG0012"
+                # but in general I need to have COGXXXX, so I will grep for it
+                temp_cog = re.search(r'COG[0-9][0-9][0-9][0-9]', genes_list[i]).group(0)
+                cog_type.append(temp_cog) # and save the COG type
 
         rel_ab_LGs[j] = 0
         if j != 'unassigned':
             if len(list_diff_zero) >= cutoff:
                 if len(list_diff_zero) == 1:
                     rel_ab_LGs[j] = float(sum(list_diff_zero))
                 else:
```

### Comparing `motu-profiler-3.0.3/motus/metaSNV_DistDiv.py` & `motu-profiler-3.1.0/motus/metaSNV_DistDiv.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/metaSNV_Filtering_2.0.py` & `motu-profiler-3.1.0/motus/metaSNV_Filtering_2.0.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/motu_utilities.py` & `motu-profiler-3.1.0/motus/motu_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,16 @@
     all_lengths = list()
     cont_line = 1
     cont = 0
     for line in head:
         cont = cont + 1
         if zippedInput:
             line = line.decode('ascii')
-
+        line = line.rstrip('\n')
+        
         if cont_line == 1:
             if line[0] != "@": print_error_fasta("Line does not start with @",cont,fastq_file)
 
         if cont_line == 2:
             l1 = len(line)
 
         if cont_line == 3:
```

### Comparing `motu-profiler-3.0.3/motus/motus.py` & `motu-profiler-3.1.0/motus/motus.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/msamtools_python.py` & `motu-profiler-3.1.0/motus/msamtools_python.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/print_CAMI.py` & `motu-profiler-3.1.0/motus/print_CAMI.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/runBWA.py` & `motu-profiler-3.1.0/motus/runBWA.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/runBWA_for_snv.py` & `motu-profiler-3.1.0/motus/runBWA_for_snv.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/motus/test.py` & `motu-profiler-3.1.0/motus/test.py`

 * *Files identical despite different names*

### Comparing `motu-profiler-3.0.3/setup.py` & `motu-profiler-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 long_description = read('README.md')
 setup(
     name = "motu-profiler",
-    version = "3.0.3",
+    version = "3.1.0",
     author = "Alessio Milanese",
     author_email = "alessiom@ethz.ch",
     description = ("Taxonomic profiling of metagenomes from diverse environments with mOTUs3"),
     license = "GPLv3",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords = "bioinformatics metagenomics taxonomic profiling",
     url = "https://github.com/motu-tool/mOTUs",
     packages=['motus'],
-    download_url = "https://github.com/motu-tool/mOTUs/archive/refs/tags/3.0.3.tar.gz",
+    download_url = "https://github.com/motu-tool/mOTUs/archive/refs/tags/3.1.0.tar.gz",
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

