# Comparing `tmp/singlecellmultiomics-0.1.7.tar.gz` & `tmp/singlecellmultiomics-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/singlecellmultiomics-0.1.7.tar", last modified: Fri Nov 29 13:30:25 2019, max compression
+gzip compressed data, was "dist/singlecellmultiomics-0.1.9.tar", last modified: Tue May 12 15:59:10 2020, max compression
```

## Comparing `singlecellmultiomics-0.1.7.tar` & `singlecellmultiomics-0.1.9.tar`

### file list

```diff
@@ -1,184 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.151877 singlecellmultiomics-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (115)      259 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)     7887 2019-11-29 13:30:25.151877 singlecellmultiomics-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     6409 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.131877 singlecellmultiomics-0.1.7/data/
--rw-r--r--   0 runner    (1001) docker     (115)   817796 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/data/mini_nla_test.bam
--rw-r--r--   0 runner    (1001) docker     (115)   107496 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/data/mini_nla_test.bam.bai
--rw-r--r--   0 runner    (1001) docker     (115)      320 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/data/mini_test.bed
--rw-r--r--   0 runner    (1001) docker     (115)       63 2019-11-29 13:30:25.155877 singlecellmultiomics-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     4603 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.131877 singlecellmultiomics-0.1.7/singlecellmultiomics/
--rw-r--r--   0 runner    (1001) docker     (115)       99 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.131877 singlecellmultiomics-0.1.7/singlecellmultiomics/alleleTools/
--rw-r--r--   0 runner    (1001) docker     (115)       27 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/alleleTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    11998 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/alleleTools/alleleTools.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.135877 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/
--rw-r--r--   0 runner    (1001) docker     (115)       28 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     6323 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/alignment_view.py
--rw-r--r--   0 runner    (1001) docker     (115)     1007 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamDuprate.py
--rw-r--r--   0 runner    (1001) docker     (115)     3616 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamExtractRandomPrimerStats.py
--rw-r--r--   0 runner    (1001) docker     (115)     9278 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamFeatureDensityVisualisation.py
--rw-r--r--   0 runner    (1001) docker     (115)     1994 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamFilter.py
--rw-r--r--   0 runner    (1001) docker     (115)    16630 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamFunctions.py
--rw-r--r--   0 runner    (1001) docker     (115)     1581 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamMappingRate.py
--rw-r--r--   0 runner    (1001) docker     (115)     1481 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamPlateVisualisation.py
--rw-r--r--   0 runner    (1001) docker     (115)     6902 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamPlotRTstats.py
--rw-r--r--   0 runner    (1001) docker     (115)     4897 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamTabulator.py
--rw-r--r--   0 runner    (1001) docker     (115)    22455 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamToCountTable.py
--rw-r--r--   0 runner    (1001) docker     (115)     4965 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamToMethylationAndCopyNumber.py
--rw-r--r--   0 runner    (1001) docker     (115)    19590 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamToRNACounts.py
--rw-r--r--   0 runner    (1001) docker     (115)    15417 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/structureTensor.py
--rw-r--r--   0 runner    (1001) docker     (115)    25207 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/variantStats.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.135877 singlecellmultiomics-0.1.7/singlecellmultiomics/barcodeFileParser/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/barcodeFileParser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    13587 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/barcodeFileParser/barcodeFileParser.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.135877 singlecellmultiomics-0.1.7/singlecellmultiomics/countTableProcessing/
--rw-r--r--   0 runner    (1001) docker     (115)       35 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/countTableProcessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3886 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/countTableProcessing/correct_count_table_bias.py
--rw-r--r--   0 runner    (1001) docker     (115)     1560 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/countTableProcessing/downsampleDataFrame.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.135877 singlecellmultiomics-0.1.7/singlecellmultiomics/fastaProcessing/
--rw-r--r--   0 runner    (1001) docker     (115)     5644 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fastaProcessing/createMapabilityIndex.py
--rw-r--r--   0 runner    (1001) docker     (115)     2429 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fastaProcessing/fastaMaskVariants.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.135877 singlecellmultiomics-0.1.7/singlecellmultiomics/fastqProcessing/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fastqProcessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1672 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fastqProcessing/fastqHandle.py
--rw-r--r--   0 runner    (1001) docker     (115)     1554 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fastqProcessing/fastqIterator.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.135877 singlecellmultiomics-0.1.7/singlecellmultiomics/features/
--rw-r--r--   0 runner    (1001) docker     (115)       39 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4534 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/features/exonGTFtoIntronGTF.py
--rw-r--r--   0 runner    (1001) docker     (115)    44141 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/features/features.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.135877 singlecellmultiomics-0.1.7/singlecellmultiomics/fragment/
--rw-r--r--   0 runner    (1001) docker     (115)       69 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fragment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4486 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fragment/chic.py
--rw-r--r--   0 runner    (1001) docker     (115)    31405 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fragment/fragment.py
--rw-r--r--   0 runner    (1001) docker     (115)     5451 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/fragment/nlaIII.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.139877 singlecellmultiomics-0.1.7/singlecellmultiomics/libraryDetection/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/libraryDetection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     5850 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/libraryDetection/archivestats.py
--rw-r--r--   0 runner    (1001) docker     (115)     9677 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/libraryDetection/sequencingLibraryListing.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.139877 singlecellmultiomics-0.1.7/singlecellmultiomics/libraryProcessing/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/libraryProcessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    11359 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/libraryProcessing/libraryStatistics.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.139877 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/
--rw-r--r--   0 runner    (1001) docker     (115)       38 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.139877 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/
--rw-r--r--   0 runner    (1001) docker     (115)     1143 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/celseq1.bc
--rw-r--r--   0 runner    (1001) docker     (115)     4883 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2.bc
--rw-r--r--   0 runner    (1001) docker     (115)     4883 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2_noNla.bc
--rw-r--r--   0 runner    (1001) docker     (115)      471 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/illumina_RP_indices.bc
--rw-r--r--   0 runner    (1001) docker     (115)      864 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/lennart96NLA.bc
--rw-r--r--   0 runner    (1001) docker     (115)      391 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/lk_virus1.bc
--rw-r--r--   0 runner    (1001) docker     (115)     3456 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/maya_384NLA.bc
--rw-r--r--   0 runner    (1001) docker     (115)      864 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/maya_mspj1.bc
--rw-r--r--   0 runner    (1001) docker     (115)     4883 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/nla_bisulfite.bc
--rw-r--r--   0 runner    (1001) docker     (115)     4884 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/scartrace.bc
--rw-r--r--   0 runner    (1001) docker     (115)     3456 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/scartraceBarcodes.bc
--rw-r--r--   0 runner    (1001) docker     (115)    22066 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/baseDemultiplexMethods.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.143877 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/
--rw-r--r--   0 runner    (1001) docker     (115)     2059 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/BULK_ILLUMINA.py
--rw-r--r--   0 runner    (1001) docker     (115)      916 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq1.py
--rw-r--r--   0 runner    (1001) docker     (115)     4165 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq2.py
--rw-r--r--   0 runner    (1001) docker     (115)     2467 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/Hexamer.py
--rw-r--r--   0 runner    (1001) docker     (115)      838 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/MSPJI.py
--rw-r--r--   0 runner    (1001) docker     (115)     2189 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/NLAIII.py
--rw-r--r--   0 runner    (1001) docker     (115)      224 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     8968 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/restrictionbisulfite.py
--rw-r--r--   0 runner    (1001) docker     (115)     2517 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/scCHIC.py
--rw-r--r--   0 runner    (1001) docker     (115)     1541 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/scartrace.py
--rw-r--r--   0 runner    (1001) docker     (115)     2411 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexedFastqConversion.py
--rw-r--r--   0 runner    (1001) docker     (115)    14121 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexingStrategyLoader.py
--rw-r--r--   0 runner    (1001) docker     (115)    19447 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demux.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.143877 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/
--rw-r--r--   0 runner    (1001) docker     (115)      471 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_RP_indices.bc
--rw-r--r--   0 runner    (1001) docker     (115)      723 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_ThruPlex48S_indices.bc
--rw-r--r--   0 runner    (1001) docker     (115)      588 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_TruSeq_indices.bc
--rw-r--r--   0 runner    (1001) docker     (115)      760 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_i7_indices.bc
--rw-r--r--   0 runner    (1001) docker     (115)     2280 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_ThruPlex48S_RP.bc
--rw-r--r--   0 runner    (1001) docker     (115)     1422 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_iPCR_RP.bc
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.143877 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/
--rw-r--r--   0 runner    (1001) docker     (115)      297 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2882 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/chic.py
--rw-r--r--   0 runner    (1001) docker     (115)     2597 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/consensus.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.143877 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/consensus_model/
--rw-r--r--   0 runner    (1001) docker     (115)   164531 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/consensus_model/nla_140bp_pe_juan_1M.pickle
--rw-r--r--   0 runner    (1001) docker     (115)     7201 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/featureannotatedmolecule.py
--rw-r--r--   0 runner    (1001) docker     (115)     2946 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/fourthiouridine.py
--rw-r--r--   0 runner    (1001) docker     (115)    13316 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/iterator.py
--rw-r--r--   0 runner    (1001) docker     (115)    78192 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/molecule.py
--rw-r--r--   0 runner    (1001) docker     (115)     4081 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/nlaIII.py
--rw-r--r--   0 runner    (1001) docker     (115)      607 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/rna.py
--rw-r--r--   0 runner    (1001) docker     (115)    11442 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/taps.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.143877 singlecellmultiomics-0.1.7/singlecellmultiomics/pyutils/
--rw-r--r--   0 runner    (1001) docker     (115)       52 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/pyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3929 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/pyutils/handlelimiter.py
--rw-r--r--   0 runner    (1001) docker     (115)     1564 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/pyutils/pyutils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.147877 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.147877 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/_general/
--rw-r--r--   0 runner    (1001) docker     (115)     1796 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/_general/sge_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.147877 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic/
--rw-r--r--   0 runner    (1001) docker     (115)     9611 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic/Snakefile
--rw-r--r--   0 runner    (1001) docker     (115)      241 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic/config.json
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.147877 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic_allelic/
--rw-r--r--   0 runner    (1001) docker     (115)    10921 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic_allelic/Snakefile
--rw-r--r--   0 runner    (1001) docker     (115)      396 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic_allelic/config.json
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.147877 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/demux/
--rw-r--r--   0 runner    (1001) docker     (115)     1341 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/demux/demux.smk
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.147877 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/nlaIII/
--rw-r--r--   0 runner    (1001) docker     (115)     9673 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/nlaIII/Snakefile
--rw-r--r--   0 runner    (1001) docker     (115)      411 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/nlaIII/config.json
--rw-r--r--   0 runner    (1001) docker     (115)     2799 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/scmo_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.147877 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/
--rw-r--r--   0 runner    (1001) docker     (115)      364 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1360 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/allele.py
--rw-r--r--   0 runner    (1001) docker     (115)     4518 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/conversions.py
--rw-r--r--   0 runner    (1001) docker     (115)     1457 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/datatype.py
--rw-r--r--   0 runner    (1001) docker     (115)     3309 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/fragmentsize.py
--rw-r--r--   0 runner    (1001) docker     (115)     1238 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/mappingquality.py
--rw-r--r--   0 runner    (1001) docker     (115)     3395 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/methylation.py
--rw-r--r--   0 runner    (1001) docker     (115)     2037 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/oversequencing.py
--rw-r--r--   0 runner    (1001) docker     (115)     8009 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/plate.py
--rw-r--r--   0 runner    (1001) docker     (115)     5026 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/readcount.py
--rw-r--r--   0 runner    (1001) docker     (115)     1499 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/rejectionreasons.py
--rw-r--r--   0 runner    (1001) docker     (115)     2946 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/scchicligation.py
--rw-r--r--   0 runner    (1001) docker     (115)     1128 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/statistic.py
--rw-r--r--   0 runner    (1001) docker     (115)     2499 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/tag.py
--rw-r--r--   0 runner    (1001) docker     (115)      689 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/trimming.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.151877 singlecellmultiomics-0.1.7/singlecellmultiomics/tags/
--rw-r--r--   0 runner    (1001) docker     (115)       20 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     5297 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/tags/tags.py
--rw-r--r--   0 runner    (1001) docker     (115)      524 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/tags/write_tags_md.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.151877 singlecellmultiomics-0.1.7/singlecellmultiomics/tagtools/
--rw-r--r--   0 runner    (1001) docker     (115)       24 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/tagtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     8046 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/tagtools/tagtools.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.151877 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/
--rw-r--r--   0 runner    (1001) docker     (115)     2248 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/4SUtagger.py
--rw-r--r--   0 runner    (1001) docker     (115)       63 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    21503 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/bamtagmultiome.py
--rw-r--r--   0 runner    (1001) docker     (115)     1918 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/customreads.py
--rw-r--r--   0 runner    (1001) docker     (115)     6992 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/digest.py
--rw-r--r--   0 runner    (1001) docker     (115)     4859 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/mspjI.py
--rw-r--r--   0 runner    (1001) docker     (115)     6132 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/nlaIII.py
--rw-r--r--   0 runner    (1001) docker     (115)     3247 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/rna.py
--rw-r--r--   0 runner    (1001) docker     (115)     3886 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/scar.py
--rw-r--r--   0 runner    (1001) docker     (115)     5000 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/scchic.py
--rw-r--r--   0 runner    (1001) docker     (115)     2639 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/tag.py
--rw-r--r--   0 runner    (1001) docker     (115)     6707 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/taps.py
--rw-r--r--   0 runner    (1001) docker     (115)     5507 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/tapsTabulator.py
--rw-r--r--   0 runner    (1001) docker     (115)    23147 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/tapsTagger.py
--rw-r--r--   0 runner    (1001) docker     (115)    26723 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/universalBamTagger.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.151877 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/
--rw-r--r--   0 runner    (1001) docker     (115)      121 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1554 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/binning.py
--rw-r--r--   0 runner    (1001) docker     (115)     3888 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/blockzip.py
--rw-r--r--   0 runner    (1001) docker     (115)      523 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (115)      461 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/iteration.py
--rw-r--r--   0 runner    (1001) docker     (115)     3181 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/sequtils.py
--rw-r--r--   0 runner    (1001) docker     (115)     6742 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/utils/submission.py
--rw-r--r--   0 runner    (1001) docker     (115)       22 2019-11-29 13:30:10.000000 singlecellmultiomics-0.1.7/singlecellmultiomics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-29 13:30:25.131877 singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     7887 2019-11-29 13:30:25.000000 singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     7872 2019-11-29 13:30:25.000000 singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-11-29 13:30:25.000000 singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)      222 2019-11-29 13:30:25.000000 singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       21 2019-11-29 13:30:25.000000 singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.301231 singlecellmultiomics-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      259 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8687 2020-05-12 15:59:10.301231 singlecellmultiomics-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     7137 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.273231 singlecellmultiomics-0.1.9/data/
+-rw-r--r--   0 runner    (1001) docker     (116)     2253 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/data/chic_test_region.bam
+-rw-r--r--   0 runner    (1001) docker     (116)    28520 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/data/chic_test_region.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (116)   817796 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/data/mini_nla_test.bam
+-rw-r--r--   0 runner    (1001) docker     (116)   107496 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/data/mini_nla_test.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (116)      320 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/data/mini_test.bed
+-rw-r--r--   0 runner    (1001) docker     (116)       63 2020-05-12 15:59:10.301231 singlecellmultiomics-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     5772 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.273231 singlecellmultiomics-0.1.9/singlecellmultiomics/
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.273231 singlecellmultiomics-0.1.9/singlecellmultiomics/alleleTools/
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/alleleTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13609 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/alleleTools/alleleTools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3600 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/alleleTools/heterozygousSNPedit.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/
+-rw-r--r--   0 runner    (1001) docker     (116)      114 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6323 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/alignment_view.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22999 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamBinCounts.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6355 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamCopyNumber.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1007 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamDuprate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3618 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamExtractRandomPrimerStats.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3423 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamExtractSamples.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16664 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamExtractVariants.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9278 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamFeatureDensityVisualisation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2120 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamFeatures.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1946 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamFilter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29105 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1581 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamMappingRate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4048 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamMatchGATKBQSRReport.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1481 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamPlateVisualisation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6902 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamPlotRTstats.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2786 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamReadGroupFormat.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1909 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamSplitByTag.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4897 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamTabulator.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24889 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamToCountTable.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4976 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamToMethylationAndCopyNumber.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8720 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamToMethylationCalls.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19598 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamToRNACounts.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6857 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/pileup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7821 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/split_bam_by_cluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6844 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/split_double_BAM.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15417 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/structureTensor.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27994 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/variantStats.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/barcodeFileParser/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/barcodeFileParser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13587 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/barcodeFileParser/barcodeFileParser.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/countTableProcessing/
+-rw-r--r--   0 runner    (1001) docker     (116)       35 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/countTableProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3886 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/countTableProcessing/correct_count_table_bias.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1560 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/countTableProcessing/downsampleDataFrame.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/fastaProcessing/
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fastaProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5644 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fastaProcessing/createMappabilityIndex.py
+-rw-r--r--   0 runner    (1001) docker     (116)      363 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fastaProcessing/fastaHandle.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3128 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fastaProcessing/fastaMaskVariants.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/fastqProcessing/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fastqProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1704 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fastqProcessing/fastqHandle.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1554 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fastqProcessing/fastqIterator.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/features/
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4534 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/features/exonGTFtoIntronGTF.py
+-rw-r--r--   0 runner    (1001) docker     (116)    45954 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/features/features.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/
+-rw-r--r--   0 runner    (1001) docker     (116)       95 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5365 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/chic.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35199 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9716 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/nlaIII.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1758 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/scartrace.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/libraryDetection/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/libraryDetection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6847 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/libraryDetection/archivestats.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9677 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/libraryDetection/sequencingLibraryListing.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/libraryProcessing/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/libraryProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13738 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/libraryProcessing/libraryStatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.277231 singlecellmultiomics-0.1.9/singlecellmultiomics/methylation/
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/methylation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6257 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/methylation/methylation.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.281231 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.281231 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/
+-rw-r--r--   0 runner    (1001) docker     (116)     1143 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/celseq1.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     4883 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     4883 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2_noNla.bc
+-rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/illumina_RP_indices.bc
+-rw-r--r--   0 runner    (1001) docker     (116)      864 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/lennart96NLA.bc
+-rw-r--r--   0 runner    (1001) docker     (116)      391 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/lk_virus1.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     3456 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/maya_384NLA.bc
+-rw-r--r--   0 runner    (1001) docker     (116)      864 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/maya_mspj1.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     4883 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/nla_bisulfite.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     4884 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/scartrace.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     3456 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/scartraceBarcodes.bc
+-rw-r--r--   0 runner    (1001) docker     (116)    22883 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/baseDemultiplexMethods.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.281231 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/
+-rw-r--r--   0 runner    (1001) docker     (116)     2059 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/BULK_ILLUMINA.py
+-rw-r--r--   0 runner    (1001) docker     (116)      916 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq1.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5017 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2467 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/Hexamer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      838 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/MSPJI.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2189 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/NLAIII.py
+-rw-r--r--   0 runner    (1001) docker     (116)      224 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8968 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/restrictionbisulfite.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6937 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/scCHIC.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1541 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/scartrace.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2411 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexedFastqConversion.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11786 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexingStrategyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19868 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demux.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.281231 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/
+-rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_RP_indices.bc
+-rw-r--r--   0 runner    (1001) docker     (116)      723 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_ThruPlex48S_indices.bc
+-rw-r--r--   0 runner    (1001) docker     (116)      588 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_TruSeq_indices.bc
+-rw-r--r--   0 runner    (1001) docker     (116)      760 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_i7_indices.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     2280 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_ThruPlex48S_RP.bc
+-rw-r--r--   0 runner    (1001) docker     (116)     1422 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_iPCR_RP.bc
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.285231 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/
+-rw-r--r--   0 runner    (1001) docker     (116)      381 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4194 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/chic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6853 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/consensus.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.285231 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/consensus_model/
+-rw-r--r--   0 runner    (1001) docker     (116)   164531 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/consensus_model/nla_140bp_pe_juan_1M.pickle
+-rw-r--r--   0 runner    (1001) docker     (116)  3827984 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/consensus_model/sk_NR3_mf3_trained_hard_fit_9939.h5
+-rw-r--r--   0 runner    (1001) docker     (116)     8382 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/featureannotatedmolecule.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2314 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2946 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/fourthiouridine.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17613 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (116)    88355 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4046 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/nlaIII.py
+-rw-r--r--   0 runner    (1001) docker     (116)      607 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/rna.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3376 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/scartrace.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16591 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/taps.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.289231 singlecellmultiomics-0.1.9/singlecellmultiomics/pyutils/
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/pyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3929 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/pyutils/handlelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1564 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/pyutils/pyutils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.289231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.289231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/_general/
+-rw-r--r--   0 runner    (1001) docker     (116)     1545 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/_general/sge_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1547 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/_general/slurm_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.289231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/call_sc_variants/
+-rw-r--r--   0 runner    (1001) docker     (116)     3959 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/call_sc_variants/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/call_sc_variants/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.289231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/call_variants/
+-rw-r--r--   0 runner    (1001) docker     (116)     2435 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/call_variants/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      139 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/call_variants/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.289231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/chic/
+-rw-r--r--   0 runner    (1001) docker     (116)    12893 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/chic/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      356 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/chic/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/chic_allelic/
+-rw-r--r--   0 runner    (1001) docker     (116)    10921 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/chic_allelic/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      396 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/chic_allelic/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/cs2/
+-rw-r--r--   0 runner    (1001) docker     (116)     9365 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/cs2/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      308 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/cs2/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/cs2_scmo/
+-rw-r--r--   0 runner    (1001) docker     (116)     8326 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/cs2_scmo/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      281 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/cs2_scmo/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/demux/
+-rw-r--r--   0 runner    (1001) docker     (116)     1341 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/demux/demux.smk
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/merge_fastq/
+-rw-r--r--   0 runner    (1001) docker     (116)     2298 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/merge_fastq/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/mutect_bulk/
+-rw-r--r--   0 runner    (1001) docker     (116)     4014 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/mutect_bulk/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      153 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/mutect_bulk/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/nlaIII/
+-rw-r--r--   0 runner    (1001) docker     (116)     9718 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/nlaIII/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      521 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/nlaIII/config.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/scartrace/
+-rw-r--r--   0 runner    (1001) docker     (116)    11039 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/scartrace/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/scartrace/config.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2927 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/scmo_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/
+-rw-r--r--   0 runner    (1001) docker     (116)      448 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1360 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/allele.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2129 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/cellreadcount.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4518 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1457 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3309 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/fragmentsize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2067 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/lorenz.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1238 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/mappingquality.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3395 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/methylation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2037 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/oversequencing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8009 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/plate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5026 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/readcount.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1499 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/rejectionreasons.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2946 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/scchicligation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1128 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2499 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)      689 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/trimming.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/tags/
+-rw-r--r--   0 runner    (1001) docker     (116)       20 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5639 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/tags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (116)      524 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/tags/write_tags_md.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.293231 singlecellmultiomics-0.1.9/singlecellmultiomics/tagtools/
+-rw-r--r--   0 runner    (1001) docker     (116)       24 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/tagtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8046 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/tagtools/tagtools.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.297231 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/
+-rw-r--r--   0 runner    (1001) docker     (116)     2437 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/4SUtagger.py
+-rw-r--r--   0 runner    (1001) docker     (116)       87 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    45169 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/bamtagmultiome.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7917 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/bamtagmultiome_multi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1918 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/customreads.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6992 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/digest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4859 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/mspjI.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6132 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/nlaIII.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3247 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/rna.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3886 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/scar.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5000 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/scchic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2639 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7495 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6707 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/taps.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5524 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/tapsTabulator.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23161 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/tapsTagger.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26723 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/universalBamTagger.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.297231 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)      201 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    38507 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/bdbbio.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)   115297 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/bdbplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3946 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/bdbsstats.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2396 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/binning.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5443 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/blockzip.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     7927 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/copyNumberStatePlotter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1093 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (116)      461 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/iteration.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6795 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/organoidTools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1923 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5129 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1056 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3811 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/sequtils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10895 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/utils/submission.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.301231 singlecellmultiomics-0.1.9/singlecellmultiomics/variants/
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13002 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/variants/postProcessVariants.py
+-rw-r--r--   0 runner    (1001) docker     (116)      706 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/variants/variantWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1105 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/variants/vcfFilterAlleleFreq.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-05-12 15:58:59.000000 singlecellmultiomics-0.1.9/singlecellmultiomics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-12 15:59:10.273231 singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8687 2020-05-12 15:59:09.000000 singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    10692 2020-05-12 15:59:10.000000 singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-12 15:59:09.000000 singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      251 2020-05-12 15:59:09.000000 singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       21 2020-05-12 15:59:09.000000 singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/top_level.txt
```

### Comparing `singlecellmultiomics-0.1.7/PKG-INFO` & `singlecellmultiomics-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: singlecellmultiomics
-Version: 0.1.7
+Version: 0.1.9
 Summary: Tools to deal with one or more measurements from single cells
 Home-page: https://github.com/BuysDB/SingleCellMultiOmics
 Author: Buys de Barbanson
 Author-email: b.barbanson@hubrecht.eu
 License: MIT
-Download-URL: https://github.com/BuysDB/SingleCellMultiOmics/archive/v0.1.6.tar.gz
+Download-URL: https://github.com/BuysDB/SingleCellMultiOmics/archive/v0.1.9.tar.gz
 Description: [![Build Status](https://travis-ci.com/BuysDB/SingleCellMultiOmics.svg?branch=master)](https://travis-ci.com/BuysDB/SingleCellMultiOmics) [![Documentation Status](https://readthedocs.org/projects/singlecellmultiomics/badge/?version=latest)](https://singlecellmultiomics.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/singlecellmultiomics.svg)](https://badge.fury.io/py/singlecellmultiomics) [![Anaconda-Server Badge](https://anaconda.org/buysdb/singlecellmultiomics/badges/installer/conda.svg)](https://anaconda.org/buysdb/singlecellmultiomics)
         
         ## Single cell multi omics
         Single cell multi omics is a set of tools to deal with multiple measurements from the same cell. This package has been developed by the [van Oudenaarden group](https://www.hubrecht.eu/research-groups/van-oudenaarden-group/).
         
         # Installation
         ```
         git clone https://github.com/BuysDB/SingleCellMultiOmics
         pip install ./SingleCellMultiOmics
         ```
         For creating a virtual environment look [here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Python-test-and-run-environment)
         
         # Usage
-        
-        The following tools are available:
-        
-        demux.py:
+        `demux.py`:
         This tool demultiplexes raw fastq files, adapters, molecule and cell information are removed from the fastq records and encoded into the read name including their base-calling qualities.
         Additional stored inforation includes:
         - Assigned and raw illumina index
         - Library
         - Demultiplexing strategy used for demultiplexing (What kind of data the read is derived from)
         - Assigned barcode index
         
@@ -35,50 +32,62 @@
         
         For RNA seq data aligned to a transcriptome the step after this is to run featureCounts.
         
         The mapped reads are encoded in a BAM file. This BAM file still contains the encoded data and this has to be decoded in order to get a useful BAM file.
         `bamtagmultiome.py`
         1) Recodes the original read names and extracts all information previously encoded by the demultiplexer.
         2) Adds allele information. (A VCF file is required for this)
-        3) Supports multiple protocols: 
-         RNA:CELSEQ1, CELSEQ2, VASA (with 8 and 6bp UMI), 
+        3) Supports multiple protocols:
+         RNA:CELSEQ1, CELSEQ2, VASA (with 8 and 6bp UMI),
          methylation digest sequencing:SC MSPJI ,  
-         lineage tracing:SCARTRACE, 
+         lineage tracing:SCARTRACE,
          DNA digest sequencing: NLAIII, 
          histone modification sequencing: scCHIC,
          Single cell methylation : TAPs (in combination with any other supported protocol).
-         
+        
         4) Assigns reads to molecules to allow for deduplication, adds duplication BAM flag
         5) Assigns read groups
+        6) Splits libraries where multiple modalities are measured
+        7) Estimates consensus sequences of molecules
         
         All SAM tags used and written by this package are listed in [TAGS.MD](https://github.com/BuysDB/SingleCellMultiOmics/blob/master/TAGS.MD)
         
+        `bamToCountTable.py`
+        [Extracts a count table from a bam file, look here for examples.](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Bam-file-to-count-table)
+        
+        
+        `libraryStatistics.py`
+        [All statistics plots can be generated with a single script, look here for details.](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Library-statistics-plots)
         
         # Examples:
         
         Demultiplex all fastq.gz files in the current directory using NLAIII barcodes
         ```
         demux.py *.fastq.gz -use NLAIII384C8U3 --y
         ````
         
         Demultiplex only the specified sequencing index (GTTTGA), and everything 1 hamming distance away from GTTTGA  :
         ```
         demux.py -si GTTTGA *.gz --y --hdi 1
         ```
         
+        ### API: Using SingleCellMultiOmics from python
+        [All molecule and fragment information can be accessed using python](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Molecule-iteration)
+        [Documentation for the classes in available here](https://singlecellmultiomics.readthedocs.io/en/latest/py-modindex.html)
+        
         ### scCHIC
         For every fragment in input.bam find scCHIC seq fragments and deduplicate these. Fragments with the same cell barcode, umi, library and strand and starting within a range of 5 bp from each other are assigned as duplicate. The mnase cut site location is expected to be between the first base (Usually an A) this A is part of the sequencing adapter, and the second base (Usually a T). The cut site location is recorded into the DS tag. When alleles are specified using -alleles, the molecule assignment is split up by allele, this means that if two fragments map to the same location and share the same umi, but contain SNPs which indicate differing alleles, the reads are not assigned to the same molecule. For every fragment the ligation sequence is recorded into the RZ tag.
         ```
-        bamtagmultiome.py input.bam -method chic -o tagged.bam 
+        bamtagmultiome.py input.bam -method chic -o tagged.bam
         ```
         [Complete scCHIC data processing instructions from FastQ to count table here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/scCHIC-data-processing)
         ### NlaIII
         For every fragment in input.bam find NLAIII seq fragments and deduplicate these. Fragments with the same cell barcode, umi, library and strand are assigned as duplicate. The NlaIII cut site location is recorded into the DS tag. When alleles are specified using -alleles, the molecule assignment is split up by allele, this means that if two fragments map to the same location and share the same UMI, but contain SNPs which indicate differing alleles, the reads are not assigned to the same molecule. For every fragment the sequenced part of the NlaIII cut site sequence is recorded into the RZ tag, this is usually CATG, but is allowed to be shifted 1 base to ATG. In the NlaIII protocol a reverse transcription (RT) is used, generally capturing more reverse transcription reactions will yield a more accurate molecule consensus sequence. For every fragment which support the molecule the reverse transcription reaction is recorded by storing the location of the random primer used for RT and the sequence of the random primer.
         ```
-        bamtagmultiome.py input.bam -method nla -o tagged.bam 
+        bamtagmultiome.py input.bam -method nla -o tagged.bam
          ```
          [Complete NlaIII data processing instructions from FastQ to count table here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/NLA-III-data-processing)
         
         
         ### Plate visualisation
         
         Show relative abundance of reads and unique molecules across 384 well plate.
```

### Comparing `singlecellmultiomics-0.1.7/README.md` & `singlecellmultiomics-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 ```
 git clone https://github.com/BuysDB/SingleCellMultiOmics
 pip install ./SingleCellMultiOmics
 ```
 For creating a virtual environment look [here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Python-test-and-run-environment)
 
 # Usage
-
-The following tools are available:
-
-demux.py:
+`demux.py`:
 This tool demultiplexes raw fastq files, adapters, molecule and cell information are removed from the fastq records and encoded into the read name including their base-calling qualities.
 Additional stored inforation includes:
 - Assigned and raw illumina index
 - Library
 - Demultiplexing strategy used for demultiplexing (What kind of data the read is derived from)
 - Assigned barcode index
 
@@ -26,50 +23,62 @@
 
 For RNA seq data aligned to a transcriptome the step after this is to run featureCounts.
 
 The mapped reads are encoded in a BAM file. This BAM file still contains the encoded data and this has to be decoded in order to get a useful BAM file.
 `bamtagmultiome.py`
 1) Recodes the original read names and extracts all information previously encoded by the demultiplexer.
 2) Adds allele information. (A VCF file is required for this)
-3) Supports multiple protocols: 
- RNA:CELSEQ1, CELSEQ2, VASA (with 8 and 6bp UMI), 
+3) Supports multiple protocols:
+ RNA:CELSEQ1, CELSEQ2, VASA (with 8 and 6bp UMI),
  methylation digest sequencing:SC MSPJI ,  
- lineage tracing:SCARTRACE, 
+ lineage tracing:SCARTRACE,
  DNA digest sequencing: NLAIII, 
  histone modification sequencing: scCHIC,
  Single cell methylation : TAPs (in combination with any other supported protocol).
- 
+
 4) Assigns reads to molecules to allow for deduplication, adds duplication BAM flag
 5) Assigns read groups
+6) Splits libraries where multiple modalities are measured
+7) Estimates consensus sequences of molecules
 
 All SAM tags used and written by this package are listed in [TAGS.MD](https://github.com/BuysDB/SingleCellMultiOmics/blob/master/TAGS.MD)
 
+`bamToCountTable.py`
+[Extracts a count table from a bam file, look here for examples.](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Bam-file-to-count-table)
+
+
+`libraryStatistics.py`
+[All statistics plots can be generated with a single script, look here for details.](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Library-statistics-plots)
 
 # Examples:
 
 Demultiplex all fastq.gz files in the current directory using NLAIII barcodes
 ```
 demux.py *.fastq.gz -use NLAIII384C8U3 --y
 ````
 
 Demultiplex only the specified sequencing index (GTTTGA), and everything 1 hamming distance away from GTTTGA  :
 ```
 demux.py -si GTTTGA *.gz --y --hdi 1
 ```
 
+### API: Using SingleCellMultiOmics from python
+[All molecule and fragment information can be accessed using python](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Molecule-iteration)
+[Documentation for the classes in available here](https://singlecellmultiomics.readthedocs.io/en/latest/py-modindex.html)
+
 ### scCHIC
 For every fragment in input.bam find scCHIC seq fragments and deduplicate these. Fragments with the same cell barcode, umi, library and strand and starting within a range of 5 bp from each other are assigned as duplicate. The mnase cut site location is expected to be between the first base (Usually an A) this A is part of the sequencing adapter, and the second base (Usually a T). The cut site location is recorded into the DS tag. When alleles are specified using -alleles, the molecule assignment is split up by allele, this means that if two fragments map to the same location and share the same umi, but contain SNPs which indicate differing alleles, the reads are not assigned to the same molecule. For every fragment the ligation sequence is recorded into the RZ tag.
 ```
-bamtagmultiome.py input.bam -method chic -o tagged.bam 
+bamtagmultiome.py input.bam -method chic -o tagged.bam
 ```
 [Complete scCHIC data processing instructions from FastQ to count table here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/scCHIC-data-processing)
 ### NlaIII
 For every fragment in input.bam find NLAIII seq fragments and deduplicate these. Fragments with the same cell barcode, umi, library and strand are assigned as duplicate. The NlaIII cut site location is recorded into the DS tag. When alleles are specified using -alleles, the molecule assignment is split up by allele, this means that if two fragments map to the same location and share the same UMI, but contain SNPs which indicate differing alleles, the reads are not assigned to the same molecule. For every fragment the sequenced part of the NlaIII cut site sequence is recorded into the RZ tag, this is usually CATG, but is allowed to be shifted 1 base to ATG. In the NlaIII protocol a reverse transcription (RT) is used, generally capturing more reverse transcription reactions will yield a more accurate molecule consensus sequence. For every fragment which support the molecule the reverse transcription reaction is recorded by storing the location of the random primer used for RT and the sequence of the random primer.
 ```
-bamtagmultiome.py input.bam -method nla -o tagged.bam 
+bamtagmultiome.py input.bam -method nla -o tagged.bam
  ```
  [Complete NlaIII data processing instructions from FastQ to count table here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/NLA-III-data-processing)
 
 
 ### Plate visualisation
 
 Show relative abundance of reads and unique molecules across 384 well plate.
```

### Comparing `singlecellmultiomics-0.1.7/data/mini_nla_test.bam` & `singlecellmultiomics-0.1.9/data/mini_nla_test.bam`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/data/mini_nla_test.bam.bai` & `singlecellmultiomics-0.1.9/data/mini_nla_test.bam.bai`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/setup.py` & `singlecellmultiomics-0.1.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
 from setuptools import setup
 import os
 import sys
 
 _here = os.path.abspath(os.path.dirname(__file__))
 version = {}
 with open(os.path.join(_here, 'singlecellmultiomics', 'version.py')) as f:
@@ -23,31 +22,34 @@
     version=version['__version__'],
     description='Tools to deal with one or more measurements from single cells',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Buys de Barbanson',
     author_email='b.barbanson@hubrecht.eu',
     url='https://github.com/BuysDB/SingleCellMultiOmics',
-    download_url = 'https://github.com/BuysDB/SingleCellMultiOmics/archive/v0.1.6.tar.gz',
+    download_url = 'https://github.com/BuysDB/SingleCellMultiOmics/archive/v0.1.9.tar.gz',
 
     license='MIT',
     packages=['singlecellmultiomics',
 
         'singlecellmultiomics.alleleTools',
         'singlecellmultiomics.bamProcessing',
         'singlecellmultiomics.barcodeFileParser',
         'singlecellmultiomics.countTableProcessing',
         'singlecellmultiomics.features',
         'singlecellmultiomics.fragment',
         'singlecellmultiomics.fastqProcessing',
+        'singlecellmultiomics.fastaProcessing',
         'singlecellmultiomics.libraryDetection',
         'singlecellmultiomics.libraryProcessing',
         'singlecellmultiomics.modularDemultiplexer',
         'singlecellmultiomics.molecule',
+        'singlecellmultiomics.methylation',
         'singlecellmultiomics.pyutils',
+        'singlecellmultiomics.variants',
         'singlecellmultiomics.tags',
         'singlecellmultiomics.statistic',
         'singlecellmultiomics.tagtools',
         'singlecellmultiomics.universalBamTagger',
         'singlecellmultiomics.utils',
         'singlecellmultiomics.modularDemultiplexer.demultiplexModules'
         ],
@@ -55,59 +57,76 @@
 
     scripts=[
         # Demultiplexing
         'singlecellmultiomics/modularDemultiplexer/demux.py',
 
         # Fasta
         'singlecellmultiomics/fastaProcessing/fastaMaskVariants.py',
-        'singlecellmultiomics/fastaProcessing/createMapabilityIndex.py',
+        'singlecellmultiomics/fastaProcessing/createMappabilityIndex.py',
 
         # Tagging
         'singlecellmultiomics/universalBamTagger/universalBamTagger.py',
+        'singlecellmultiomics/universalBamTagger/bamtagmultiome_multi.py',
         'singlecellmultiomics/universalBamTagger/bamtagmultiome.py',
         'singlecellmultiomics/universalBamTagger/tapsTagger.py',
         'singlecellmultiomics/universalBamTagger/tapsTabulator.py',
         'singlecellmultiomics/universalBamTagger/4SUtagger.py',
 
         # Bam processing:
         'singlecellmultiomics/bamProcessing/bamTabulator.py',
+        'singlecellmultiomics/bamProcessing/bamSplitByTag.py',
+        'singlecellmultiomics/bamProcessing/bamReadGroupFormat.py',
         'singlecellmultiomics/bamProcessing/bamToCountTable.py',
+        'singlecellmultiomics/bamProcessing/bamCopyNumber.py',
+        'singlecellmultiomics/bamProcessing/bamExtractSamples.py',
         'singlecellmultiomics/bamProcessing/bamToMethylationAndCopyNumber.py',
+        'singlecellmultiomics/bamProcessing/bamToMethylationCalls.py',
         'singlecellmultiomics/bamProcessing/bamMappingRate.py',
         'singlecellmultiomics/bamProcessing/bamFilter.py',
         'singlecellmultiomics/bamProcessing/bamPlotRTstats.py',
         'singlecellmultiomics/bamProcessing/bamPlateVisualisation.py',
         'singlecellmultiomics/bamProcessing/bamFeatureDensityVisualisation.py',
         'singlecellmultiomics/bamProcessing/bamDuprate.py',
         'singlecellmultiomics/bamProcessing/bamExtractRandomPrimerStats.py',
         'singlecellmultiomics/bamProcessing/bamToRNACounts.py',
         'singlecellmultiomics/bamProcessing/structureTensor.py',
         'singlecellmultiomics/bamProcessing/variantStats.py',
+        'singlecellmultiomics/bamProcessing/bamExtractVariants.py',
+        'singlecellmultiomics/bamProcessing/bamMatchGATKBQSRReport.py',
+        'singlecellmultiomics/bamProcessing/bamBinCounts.py',
+        'singlecellmultiomics/bamProcessing/split_double_BAM.py',
+
         # Library processing:
         'singlecellmultiomics/libraryProcessing/libraryStatistics.py',
         'singlecellmultiomics/libraryDetection/archivestats.py',
+        'singlecellmultiomics/alleleTools/heterozygousSNPedit.py',
 
         # Feature conversion:
         'singlecellmultiomics/features/exonGTFtoIntronGTF.py',
 
+        # Variants:
+        'singlecellmultiomics/variants/postProcessVariants.py',
+        'singlecellmultiomics/variants/vcfFilterAlleleFreq.py',
 
         # Utility: (SGE wrapper)
         'singlecellmultiomics/utils/submission.py',
 
         #Worfklow
         'singlecellmultiomics/snakemake_workflows/scmo_workflow.py',
-        'singlecellmultiomics/snakemake_workflows/_general/sge_wrapper.py'
+        'singlecellmultiomics/snakemake_workflows/_general/sge_wrapper.py',
+        'singlecellmultiomics/snakemake_workflows/_general/slurm_wrapper.py'
 
         ],
 
   install_requires=[
-       'pysam>=0.15.3','numpy>=1.16.4','pandas>=0.25.0','colorama',
-       'pysamiterators>=1.6','more-itertools','matplotlib','tabulate',
-       'wheel','setuptools>=40.8.0','scikit-learn>=0.21.3','seaborn',
-       'biopython>=1.71','pytest>=5.0.0','pytest-runner','snakemake>=5.8.1'
+       'pysam>=0.15.3','numpy>=1.15.4','pandas>=0.25.0','colorama',
+       'pysamiterators>=1.7','more-itertools','matplotlib','tabulate',
+       'wheel','setuptools>=40.8.0','scikit-learn>=0.21.3','seaborn', 'statsmodels',
+       'biopython>=1.71','pytest>=5.0.0','pytest-runner','snakemake>=5.8.1','lxml',
+       'statsmodels' #,'tensorflow>=1.14.0'
    ],
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
 
     include_package_data=True,
 
     classifiers=[
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/alleleTools/alleleTools.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/alleleTools/alleleTools.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,24 @@
 # -*- coding: utf-8 -*-
 import pysam
 import argparse
 import collections
 import functools
 import gzip
 import os
+from singlecellmultiomics.utils import Prefetcher
 
+def get_allele_dict():
+    return collections.defaultdict(nested_set_defaultdict)
+def nested_set_defaultdict():
+    return collections.defaultdict( set_defaultdict )
+def set_defaultdict():
+    return collections.defaultdict (set)
 
-class AlleleResolver:
+class AlleleResolver(Prefetcher):
 
     def clean_vcf_name(self, vcffile):
         # Convert file name to string if it is not
         if type(vcffile) == pysam.libcbcf.VariantFile:
             vcffile = vcffile.filename.decode('ascii')
         if type(vcffile) == bytes:
             vcffile = vcffile.decode('ascii')
@@ -21,15 +28,19 @@
     def __init__(self, vcffile=None,
                  chrom=None,
                  phased=True,
                  uglyMode=False,
                  lazyLoad=False,
                  select_samples=None,
                  use_cache=False,
-                 ignore_conversions=None
+                 ignore_conversions=None,
+                 verbose=False,
+                 region_start=None,
+                 region_end=None
+
 
                  # When this flag is true a cache file is generated containing
                  # usable SNPs for every chromosome in gzipped format
                  ):
         """Initialise AlleleResolver
 
         Args:
@@ -37,29 +48,40 @@
 
             chrom (str):  contig/chromosome to prepare variants for
 
             phased(bool) : the variants in the vcf file are phased (every sample is one haplotype)
 
             uglyMode (bool) : the vcf file is invalid (not indexed) and has to be loaded to memory
 
+            verbose (bool) : Print debug information
+
             lazyLoad (bool) : the vcf file is valid and indexed and does not need to be loaded to memory
 
             select_samples (list) : Use only these samples from the VCF file
 
             use_cache (bool) : When this flag is true a cache file is generated containing usable SNPs for every chromosome in gzipped format
 
             ignore_conversions(set) : conversions to ignore {(ref, alt), ..} , for example set( ('C','T'), ('G','A') )
 
+            region_start(int) : only load variants within this range (region_start-region_end) when reading a cached variant file
+
+            region_end(int) : only load variants within this range (region_start-region_end) when reading a cached variant file
+
+
         """
+        self.args = locals().copy()
+        del self.args['self']
+
         self.ignore_conversions = ignore_conversions
         self.phased = phased
-        self.verbose = False
-        self.locationToAllele = collections.defaultdict(lambda: collections.defaultdict(
-            lambda: collections.defaultdict(set)))  # chrom -> pos-> base -> sample(s)
+        self.verbose = verbose
+        self.locationToAllele = get_allele_dict()  # chrom -> pos-> base -> sample(s)
         self.select_samples = select_samples
+        self.region_start = region_start
+        self.region_end = region_end
 
         self.lazyLoad = lazyLoad
 
         if vcffile is None:
             return
         self.vcffile = self.clean_vcf_name(vcffile)
         self.use_cache = use_cache
@@ -78,15 +100,15 @@
             if self.verbose:
                 print(
                     'Lazy loading is not supported for non proper VCFs. Loading all variants to memory.')
             if self.select_samples is not None:
                 raise NotImplementedError(
                     "Sample selection is not implemented for non proper VCF")
             lazyLoad = False
-        # self.locationToAllele = collections.defaultdict( lambda:
+
         # collections.defaultdict(set) ) #(chrom, pos)-> base -> sample(s)
 
         if uglyMode:
             foundIt = False  # If the target chromosome was found
             with open(vcffile, 'r') as f:
 
                 for line in f:
@@ -139,21 +161,46 @@
         Args:
             path (str):  path of the cache file
             chrom (str):  contig/chromosome
         """
         with gzip.open(path, 'rt') as f:
             for line in f:
                 position, base, samples = line.strip().split('\t', 3)
-                self.locationToAllele[chrom][int(
-                    position)][base] = set(samples.split(','))
+                position = int(position)
+                if self.region_start is not None and position<self.region_start:
+                    continue
+                if self.region_end is not None and position>self.region_end:
+                    break
+
+                self.locationToAllele[chrom][position][base] = set(samples.split(','))
+
+
+
+    def instance(self, arg_update):
+        if 'self' in self.args:
+            del self.args['self']
+        clone = AlleleResolver(**self.args)
+        return clone
+
+
+    def prefetch(self, contig, start, end):
+
+        clone = self.instance({'region_start':start, 'region_end':end})
+
+        #print(f'Prefetching {contig}:{start}-{end}')
+        try:
+            self.fetchChromosome(self.vcffile, contig, True)
+        except ValueError:
+            # This means the chromosome is not available
+            pass
+        return clone
 
     def fetchChromosome(self, vcffile, chrom, clear=False):
         if clear:
-            self.locationToAllele = collections.defaultdict(lambda: collections.defaultdict(
-                lambda: collections.defaultdict(set)))  # chrom -> pos-> base -> sample(s)
+            self.locationToAllele = get_allele_dict()  # chrom -> pos-> base -> sample(s)
 
         vcffile = self.clean_vcf_name(vcffile)
         # allocate:
 
         # Decide if this is an allele we would may be cache?
         write_cache_file_flag = False
         if self.use_cache:
@@ -185,45 +232,49 @@
 
         unTrusted = []
         added = 0
         if self.verbose:
             print(f'Reading variants for {chrom} ', end='')
         with pysam.VariantFile(vcffile) as v:
             try:
-                for rec in v.fetch(chrom):
+                for rec in v.fetch(chrom, start=self.region_start, stop=self.region_end):
                     used = False
                     bad = False
                     bases_to_alleles = collections.defaultdict(
                         set)  # base -> samples
 
                     if self.phased:  # variants are phased, assign a random allele
                         samples_assigned = set()
                         most_assigned_base = 0
+                        monomorphic=False
                         for sample, sampleData in rec.samples.items():
 
                             if self.select_samples is not None and sample not in self.select_samples:
                                 continue
                             for base in sampleData.alleles:
                                 if base is None:
-                                    unTrusted.append((rec.chrom, rec.pos))
+                                    # This site is monomorphic:
+                                    monomorphic=True
                                     continue
                                 if len(base) == 1:
                                     bases_to_alleles[base].add(sample)
                                     used = True
                                     samples_assigned.add(sample)
                                 else:  # This location cannot be trusted:
                                     bad = True
                         # We can prune this site if all samples are associated
                         # with the same base
                         if self.select_samples is not None and used:
                             if len(samples_assigned) != len(
                                     self.select_samples):
                                 # The site is not informative
                                 bad = True
-                        if len(bases_to_alleles) < 2:
+                        if monomorphic and len(bases_to_alleles)>0:
+                            bad=False
+                        elif len(bases_to_alleles) < 2:
                             bad = True
                             # The site is not informative
                     else:  # not phased
                         if not all(
                                 len(allele) == 1 for allele in rec.alleles):  # only select SNVs
                             bad = True
                         else:
@@ -237,16 +288,15 @@
                             ((rec.ref, base) in self.ignore_conversions for base in bases_to_alleles))
 
                     if used and not bad:
                         self.locationToAllele[rec.chrom][rec.pos -
                                                          1] = bases_to_alleles
                         added += 1
             except Exception as e:
-                print(e)
-
+                raise
         # for t in unTrusted:
         #    if t in self.locationToAllele:
         #        del self.locationToAllele[t[0]][t[1]]
         #del unTrusted
         if self.verbose:
             print(f'{added} variants [OK]')
         if self.use_cache and write_cache_file_flag:
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/alignment_view.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/alignment_view.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamDuprate.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamDuprate.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamExtractRandomPrimerStats.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamExtractRandomPrimerStats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import singlecellmultiomics
 from singlecellmultiomics.molecule import MoleculeIterator, NlaIIIMolecule
-from singlecellmultiomics.fragment import NLAIIIFragment
+from singlecellmultiomics.fragment import NlaIIIFragment
 import pysam
 import collections
 import pysamiterators
 import pandas as pd
 import numpy as np
 import re
 import more_itertools
@@ -90,16 +90,16 @@
         default='./randomer_usage.pickle.gz',
         help='Output pickle/csv path')
     args = argparser.parse_args()
 
     with pysam.AlignmentFile(args.bamfile) as alignments:
         molecule_source = MoleculeIterator(
             alignments,
-            moleculeClass=NlaIIIMolecule,
-            fragmentClass=NLAIIIFragment,
+            molecule_class=NlaIIIMolecule,
+            fragment_class=NlaIIIFragment,
         )
 
         qf = get_random_primer_histogram(
             molecule_source,
             args.min_mq,
             args.max_size,
             args.size_bin_size,
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamFeatureDensityVisualisation.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamFeatureDensityVisualisation.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamFilter.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamFilter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import os
-import pysam
-import argparse
-import sys
-
-if __name__ == '__main__':
-    argparser = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description="""Filter bam file for value of tag or multiple tags
-    """)
-    argparser.add_argument('bamfile', metavar='bamfile', type=str)
-    argparser.add_argument('expression', help="""Filter expression. All reads which yield a boolean true value for this expression will be send to the output file. For example r.get_tag("SM")=="cell1"   or r.reference_start==10   . Take care that for ALL positions you should subtract 1 because counting will start at 0. See https://pysam.readthedocs.io/en/latest/api.html#pysam.AlignedSegment for all attributes you can use for filtering. It is possible to filter for a compound expression. For example r.get_tag('BC')=='CAACTAGA' and r.reference_name=='1' """)
-    argparser.add_argument(
-        '-o',
-        type=str,
-        required=True,
-        help='output bam path')
-    argparser.add_argument(
-        '--f',
-        action='store_true',
-        help='Force overwrite of existing files')
-    argparser.add_argument('-head', type=int)
-    args = argparser.parse_args()
-
-    if os.path.exists(args.o) and not args.f:
-        raise ValueError(
-            f'The output file {args.o} already exists! Use --f or remove the file')
-
-    bamFile = pysam.AlignmentFile(args.bamfile, "rb")
-    header = bamFile.header.copy()
-    outputFile = pysam.AlignmentFile(args.o, "wb", header=header)
-
-    written = 0
-    for r in bamFile:
-        if eval(args.expression):
-
-            outputFile.write(r)
-            written += 1
-            if args.head and written >= args.head:
-                break
-
-    print(f'Filtering finished, {written} reads')
-    outputFile.close()
-    try:
-        os.system(f'samtools index {args.o}')
-    except Exception as e:
-        pass
+#!/usr/bin/env python3
+
+# -*- coding: utf-8 -*-
+import os
+import pysam
+import argparse
+import sys
+
+if __name__ == '__main__':
+    argparser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        description="""Filter bam file for value of tag or multiple tags
+    """)
+    argparser.add_argument('bamfile', metavar='bamfile', type=str)
+    argparser.add_argument('expression', help="""Filter expression. All reads which yield a boolean true value for this expression will be send to the output file. For example r.get_tag("SM")=="cell1"   or r.reference_start==10   . Take care that for ALL positions you should subtract 1 because counting will start at 0. See https://pysam.readthedocs.io/en/latest/api.html#pysam.AlignedSegment for all attributes you can use for filtering. It is possible to filter for a compound expression. For example r.get_tag('BC')=='CAACTAGA' and r.reference_name=='1' """)
+    argparser.add_argument(
+        '-o',
+        type=str,
+        required=True,
+        help='output bam path')
+    argparser.add_argument(
+        '--f',
+        action='store_true',
+        help='Force overwrite of existing files')
+    argparser.add_argument('-head', type=int)
+    args = argparser.parse_args()
+
+    if os.path.exists(args.o) and not args.f:
+        raise ValueError(
+            f'The output file {args.o} already exists! Use --f or remove the file')
+
+    bamFile = pysam.AlignmentFile(args.bamfile, "rb")
+    header = bamFile.header.copy()
+    outputFile = pysam.AlignmentFile(args.o, "wb", header=header)
+
+    written = 0
+    for r in bamFile:
+        if eval(args.expression):
+
+            outputFile.write(r)
+            written += 1
+            if args.head and written >= args.head:
+                break
+
+    print(f'Filtering finished, {written} reads')
+    outputFile.close()
+    try:
+        os.system(f'samtools index {args.o}')
+    except Exception as e:
+        pass
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamMappingRate.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamMappingRate.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamPlateVisualisation.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamPlateVisualisation.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamPlotRTstats.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamPlotRTstats.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamTabulator.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamTabulator.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamToCountTable.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamToCountTable.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pysam
 import collections
 import argparse
 import pandas as pd
 import numpy as np
 import itertools
 import singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods
+import gzip  # for loading blacklist bedfiles
 TagDefinitions = singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods.TagDefinitions
 
 
 def coordinate_to_sliding_bin_locations(dp, bin_size, sliding_increment):
     """
     Convert a single value to a list of overlapping bins
 
@@ -93,29 +94,37 @@
     except Exception as e:
         value = defective
     return value
 
 # define if a read should be used
 
 
-def read_should_be_counted(read, args):
+def read_should_be_counted(read, args, blacklist_dic = None):
     """
     Check if a read should be counted given the filter arguments
 
     Parameters
     ----------
     read : pysam.AlignedSegment or None
         read to check if it should be counted
 
     Returns
     -------
     bool
     """
 
+
 # Read is empty
+    if args.filterMP:
+        if not read.has_tag('mp'):
+            return False
+        if read.get_tag('mp')=='unique':
+            return True
+        return False
+
     if read is None or read.is_qcfail:
         return False
 
     # Mapping quality below threshold
     if read.mapping_quality < args.minMQ:
         return False
 
@@ -126,14 +135,25 @@
 
     # Read is a duplicate
     # (args.dedup and ( not read.has_tag('RC') or (read.has_tag('RC') and read.get_tag('RC')!=1))):
     if read.is_unmapped or (args.dedup and (
             read.has_tag("RR") or read.is_duplicate)):
         return False
 
+    # Read is in blacklist
+    if blacklist_dic is not None:
+        if read.reference_name in blacklist_dic:
+            # iterate through tuples of startend to check
+            for startend in blacklist_dic[read.reference_name]:
+                # start is 0-based inclusive, end is 0-based exclusive
+                start_bad = read.reference_start >= startend[0] and read.reference_start < startend[1]
+                end_bad = read.reference_end >= startend[0] and read.reference_end < startend[1]
+                if start_bad or end_bad:
+                    return False
+
     return True
 
 
 def tagToHumanName(tag, TagDefinitions):
     if tag not in TagDefinitions:
         return tag
     return TagDefinitions[tag].humanName
@@ -142,18 +162,19 @@
 def assignReads(
         read,
         countTable,
         args,
         joinFeatures,
         featureTags,
         sampleTags,
-        more_args=[]):
+        more_args=[],
+        blacklist_dic = None):
 
     assigned = 0
-    if not read_should_be_counted(read, args):
+    if not read_should_be_counted(read, args, blacklist_dic):
         return assigned
 
     # Get the sample to which this read belongs
     sample = tuple(readTag(read, tag) for tag in sampleTags)
 
     # Decide how many counts this read yields
     if args.doNotDivideFragments:
@@ -400,26 +421,49 @@
     if args.featureTags is not None:
         featureTags = args.featureTags.split(',')
 
     if args.joinedFeatureTags is not None:
         featureTags = args.joinedFeatureTags.split(',')
         joinFeatures = True
 
+        # When -byValue is used, and joined feature tags are supplied, automatically append the args.byValue tag, otherwise it will get lost
+        if args.byValue is not None and len(featureTags)>0 and args.byValue not in featureTags:
+            featureTags.append(args.byValue)
+
+
     if args.bin is not None and args.binTag not in featureTags:
         print("The bin tag was not supplied as feature, automatically appending the bin feature.")
         featureTags.append(args.binTag)
 
     if len(featureTags) == 0:
         raise ValueError(
             "No features supplied! Please supply -featureTags -joinedFeatureTags and or -binTag")
 
     sampleTags = args.sampleTags.split(',')
     countTable = collections.defaultdict(
         collections.Counter)  # cell->feature->count
 
+    if args.blacklist is not None:
+        # create blacklist dictionary {chromosome : [ (start1, end1), ..., (startN, endN) ]}
+        # used to check each read and exclude if it is within any of these start end sites
+        #
+        blacklist_dic = {}
+        print("Creating blacklist dictionary:")
+        with open(args.blacklist, mode='r') as blfile:
+            for row in blfile:
+                parts = row.strip().split()
+                chromo, start, end = parts[0], int(parts[1]), int(parts[2])
+                if chromo not in blacklist_dic:
+                    # init chromo
+                    blacklist_dic[chromo] = []  # list of tuples
+                blacklist_dic[chromo].append( (start, end) )
+        print(blacklist_dic)
+    else:
+        blacklist_dic = None
+
     assigned = 0
     for bamFile in args.alignmentfiles:
 
         with pysam.AlignmentFile(bamFile) as f:
             i = 0  # make sure i is defined
             if args.bin:
                 # Obtain the reference sequence lengths
@@ -442,39 +486,41 @@
                         break
 
                     assigned += assignReads(read,
                                             countTable,
                                             args,
                                             joinFeatures,
                                             featureTags,
-                                            sampleTags)
-            else:
+                                            sampleTags,
+                                            blacklist_dic = blacklist_dic)
+            else:  # args.bedfile is not None
                 # for adding counts associated with a bedfile
                 with open(args.bedfile, "r") as bfile:
                     #breader = csv.reader(bfile, delimiter = "\t")
                     for row in bfile:
 
                         parts = row.strip().split()
-                        chromo, start, end, bname = parts[0], int(
-                            parts[1]), int(parts[2]), parts[3]
+                        chromo, start, end, bname = parts[0], int(float(
+                            parts[1])), int(float(parts[2])), parts[3]
                         if args.contig is not None and chromo != args.contig:
                             continue
                         for i, read in enumerate(f.fetch(chromo, start, end)):
                             if i % 1_000_000 == 0:
                                 print(
                                     f"{bamFile} Processed {i} reads, assigned {assigned}, completion:{100*(i/(0.001+f.mapped+f.unmapped+f.nocoordinate))}%")
                             assigned += assignReads(read,
                                                     countTable,
                                                     args,
                                                     joinFeatures,
                                                     featureTags,
                                                     sampleTags,
                                                     more_args=[start,
                                                                end,
-                                                               bname])
+                                                               bname],
+                                                    blacklist_dic = blacklist_dic)
 
                             if args.head is not None and i > args.head:
                                 break
 
             print(
                 f"Finished: {bamFile} Processed {i} reads, assigned {assigned}")
     print(f"Finished counting, now exporting to {args.o}")
@@ -568,14 +614,20 @@
         action='store_true',
         help='When used every read is counted once, a fragment will count as two reads. 0.5 otherwise')
     multimapping_args.add_argument(
         '-minMQ',
         type=int,
         default=0,
         help="minimum mapping quality")
+
+    multimapping_args.add_argument(
+        '--filterMP',
+        action= 'store_true',
+        help="Filter reads which are not uniquely mappable")
+
     multimapping_args.add_argument(
         '--filterXA',
         action='store_true',
         help="Do not count reads where the XA (alternative hits) tag has been set for a non-alternative locus.")
 
     binning_args = argparser.add_argument_group('Binning', '')
     #binning_args.add_argument('-offset', type=int, default=0, help="Add offset to bin. If bin=1000, offset=200, f=1999 -> 1200. f=4199 -> 3200")
@@ -597,15 +649,15 @@
     # specifies the bin range in which the read was counted" ) this is now
     # always on!
     binning_args.add_argument('-binTag', default='DS')
     binning_args.add_argument(
         '-byValue',
         type=str,
         help='Extract the value from the supplied tag and use this as count to add')
-
+    binning_args.add_argument('-blacklist', metavar='BED FILE BLACKLIST TO FILTER OUT', help = 'Bedfile of blacklist regions to exclude', default=None)
     bed_args = argparser.add_argument_group('Bedfiles', '')
     bed_args.add_argument(
         '-bedfile',
         type=str,
         help="Bed file containing 3 columns, chromo, start, end to be read for fetching counts")
 
     argparser.add_argument(
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamToMethylationAndCopyNumber.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamToMethylationAndCopyNumber.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     # cell -> (context, chromosome, bin) -> methylation
     methylation_pos = collections.defaultdict(collections.Counter)
     # cell -> (context, chromosome, bin) -> methylation
     methylation_neg = collections.defaultdict(collections.Counter)
     # cell -> (allele, chromosome,   bin) -> raw_count
     fragment_read_abundance = collections.defaultdict(collections.Counter)
 
-    with pysam.AlignmentFile(args.alignmentfile) as alignments:
+    with pysam.AlignmentFile(args.alignmentfile, threads=4) as alignments:
 
         min_mq = 30
         wrote = 0
         # for chromosome in chromosomes:
         #    for i,read in enumerate(alignments.fetch(chromosome)):
         for read in alignments:
             if read.is_duplicate:
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/bamToRNACounts.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamToRNACounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,21 +124,21 @@
         identifierFields=['transcript_id'],
         store_all=True,
         head=args.hf,
         contig=contig)
 
     # What is used for assignment of molecules?
     if args.method == 'nla':
-        moleculeClass = singlecellmultiomics.molecule.AnnotatedNLAIIIMolecule
-        fragmentClass = singlecellmultiomics.fragment.NLAIIIFragment
+        molecule_class = singlecellmultiomics.molecule.AnnotatedNLAIIIMolecule
+        fragment_class = singlecellmultiomics.fragment.NlaIIIFragment
         pooling_method = 1  # all data from the same cell can be dealt with separately
         stranded = None  # data is not stranded
     elif args.method == 'vasa' or args.method == 'cs':
-        moleculeClass = singlecellmultiomics.molecule.VASA
-        fragmentClass = singlecellmultiomics.fragment.SingleEndTranscript
+        molecule_class = singlecellmultiomics.molecule.VASA
+        fragment_class = singlecellmultiomics.fragment.SingleEndTranscript
         pooling_method = 1
         stranded = 1  # data is stranded, mapping to other strand
     else:
         raise ValueError("Supply a valid method")
 
     # COUNT:
     exon_counts_per_cell = collections.defaultdict(
@@ -167,24 +167,24 @@
     for alignmentfile_path in args.alignmentfiles:
 
         i = 0
         with pysam.AlignmentFile(alignmentfile_path) as alignments:
             molecule_iterator = MoleculeIterator(
                 alignments=alignments,
                 check_eject_every=5000,
-                moleculeClass=moleculeClass,
+                molecule_class=molecule_class,
                 molecule_class_args={
                     'features': features,
                     'stranded': stranded,
                     'min_max_mapping_quality': args.minmq,
                     'reference': ref,
                     'allele_resolver': allele_resolver
                 },
 
-                fragmentClass=fragmentClass,
+                fragment_class=fragment_class,
                 fragment_class_args={
                     'umi_hamming_distance': args.umi_hamming_distance,
                     'R1_primer_length': 4,
                     'R2_primer_length': 6},
                 perform_qflag=True,
                 # when the reads have not been tagged yet, this flag is very
                 # much required
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/structureTensor.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/structureTensor.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/bamProcessing/variantStats.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/variantStats.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import pickle
 import pandas as pd
 from colorama import Fore, Style
 from singlecellmultiomics.bamProcessing.bamFunctions import sorted_bam_file, sort_and_index, get_reference_from_pysam_alignmentFile, add_readgroups_to_header, write_program_tag, GATK_indel_realign
 from singlecellmultiomics.pyutils import meanOfCounter
 import argparse
 import os
-
+import sys
+import traceback
 f'Please use an environment with python 3.6 or higher!'
 
 
 def obtain_variant_statistics(
     alignment_file_paths,
     cell_obs, statistics, cell_call_data,
     reference,
@@ -80,56 +81,62 @@
 
     for pathi, alignment_path in enumerate(alignment_file_paths):
 
         # Perform re-alignment:
         if args.realign:
             target_bam = f'align_{chromosome}_{region_start}_{region_end}.bam'
 
-            if not os.path.exist(target_bam):
+            if not os.path.exists(target_bam):
                 temp_target_bam = f'{target_bam}.temp.bam'
+                temp_target_bai = f'{target_bam}.temp.bai'
                 GATK_indel_realign(
                     alignment_path,
                     temp_target_bam,
                     chromosome,
                     region_start,
                     region_end,
                     args.indelvcf,
                     gatk_path=args.gatk3_path,
                     interval_path=None,
-                    java_cmd='java -jar -Xmx30G -Djava.io.tmpdir=./gatk_tmp',
+                    java_cmd=f'java -jar -Xmx{args.realign_mem}G -Djava.io.tmpdir=./gatk_tmp',
                     reference=reference.handle.filename.decode('utf8'),
                     interval_write_path=f'./align_{chromosome}_{region_start}_{region_end}.intervals')
+
+                print(f'Renaming {temp_target_bam} > {target_bam}')
                 os.rename(temp_target_bam,target_bam)
+                os.rename(temp_target_bai,target_bam.replace('.bam','.bai'))
             alignment_path = target_bam
 
-        with pysam.AlignmentFile(alignment_path) as alignments:
+        with pysam.AlignmentFile(alignment_path, ignore_truncation=args.ignore_bam_issues) as alignments:
 
             for molecule_id, molecule in enumerate(
                     singlecellmultiomics.molecule.MoleculeIterator(alignments,
                                                                    fragment_class_args={
                                                                        'umi_hamming_distance': umi_hamming_distance,
                                                                    },
                                                                    molecule_class_args={
                                                                        'reference': reference
                                                                    },
-                                                                   moleculeClass=singlecellmultiomics.molecule.NlaIIIMolecule,
-                                                                   fragmentClass=singlecellmultiomics.fragment.NLAIIIFragment,
+                                                                   molecule_class=singlecellmultiomics.molecule.NlaIIIMolecule,
+                                                                   fragment_class=singlecellmultiomics.fragment.NlaIIIFragment,
                                                                    start=ssnv_position - WINDOW_RADIUS,
                                                                    end=ssnv_position + WINDOW_RADIUS,
                                                                    contig=chromosome
                                                                    )):
 
                 # For every molecule obtain the consensus from which to extract
                 # the gSNV and sSNV:
                 try:
                     consensus = molecule.get_consensus()
                 except Exception as e:
                     if str(e) == 'Could not extract any safe data from molecule':
                         statistics[(chromosome, ssnv_position)
                                    ]['R2_unmapped'][True] += 1
+                    else:
+                        print(e)
                     continue
 
                 # Extract the gSNV and sSNV:
                 ssnv_state = consensus.get((chromosome, ssnv_position))
                 gsnv_state = consensus.get((chromosome, gsnv_position))
 
                 # Store all used molecules in the window for inspection:
@@ -232,15 +239,15 @@
     #
     # determine if there is an alternative base in the first place
     # a fraction of the reads in a cell need to vote for a tuple,
     # this fraction is stored in the alpha parameter , or a minimum amount of reads, stored in the beta parameter
     # determine tp*, the alleles we expect observe
     # ϴ τ α γ κ λ ν ξ ρ ϕ
     α = 0.2  # minimum relative abundance of sSNV voting reads in single sample
-    β = 10  # minimum amount of sSSNV reads in cell, or in total if α is exceeded
+    β = 3  # minimum amount of sSSNV reads in cell, or in total if α is exceeded
     γ = 0.9  # minimum amount of votes for sSNV
     ε = 2  # minimum amount of cells voting for sSNV
     ω = 0.9  # gsnv majority
 
     sSNV_votes = collections.Counter()  # { sSNV_alt_base : votes }
     total_samples_which_voted = 0
     for sample, observed_tuples in cell_read_obs.items():
@@ -267,15 +274,17 @@
             alpha_value = 0 if ref_sSNV_reads==0 else sSNV_supporting_reads/ref_sSNV_reads
 
             vote = (
                 1 if (
                     alpha_value >= α and (
                         sSNV_supporting_reads +
                         ref_sSNV_reads) >= β) or (
-                    alpha_value < α and ref_sSNV_reads >= β) else 0)
+                    alpha_value < α and sSNV_supporting_reads >= β) else 0)
+
+            print(f'{sample}\tsSNV alt:{sSNV_state}\t{sSNV_supporting_reads}\tsSNV ref:{ref_sSNV_reads}\t{ref_sSNV_reads}\tα:{alpha_value}\t{"votes" if vote else "no vote"}')
 
             if vote:
                 votes_for_this_sample.add(sSNV_state)
                 sSNV_votes[sSNV_state] += 1
                 total_samples_which_voted += 1
 
     # done voting.
@@ -310,283 +319,338 @@
     for basecall, obs in gSNV_obs_phased.most_common():
         if basecall != gSNV_ref_base:
             gSNV_alt_base = basecall
             break
 
     if sSNV_alt_base is None or gSNV_alt_base is None:
         # No phased alt base found ...
+        print(f'No phased allele found')
         return
 
     # Determine the phase (most common genotypes)
     sSNV_phase = None
     wt_allele_gSNV = None
     snv_allele_gSNV = None
     sSNV_phased_votes = sum((obs
                              for (sSNV_state, gSNV_state), obs
                              in complete_genotype_obs.most_common()
-                             if sSNV_state == sSNV_alt_base
+                             if sSNV_state == sSNV_alt_base and  gSNV_state is not None
                              ))
 
-    for (sSNV_state, gSNV_state), obs in complete_genotype_obs.most_common():
-        if sSNV_state == sSNV_alt_base:
-            sSNV_phase = (sSNV_state, gSNV_state)
-            phased_gSNV = gSNV_state
-            if gSNV_state == gSNV_ref_base:
-                # the reference allele is alt
-                wt_allele_gSNV = gSNV_alt_base
-                snv_allele_gSNV = gSNV_ref_base
-            else:
-                wt_allele_gSNV = gSNV_ref_base
-                snv_allele_gSNV = gSNV_alt_base
-                # the reference allele is ref
-            break
+    if sSNV_phased_votes==0:
+        print('No votes cast for phasing the selected alternative allele')
+        return
+    # Find the phased germline variant:
+    for (sSNV_state, gSNV_state), this_phase_obs in complete_genotype_obs.most_common():
+        if sSNV_state != sSNV_alt_base or  gSNV_state is None:
+            continue
 
-        statistics[(chromosome, ssnv_position)]['sSNV_gSNV_phase'] = snv_allele_gSNV
-        
-        if snv_allele_gSNV is None:
-            return
+        print(f'There are {sSNV_phased_votes} votes for the haplotype {sSNV_state} {gSNV_state}, ratio:{this_phase_obs / sSNV_phased_votes} ')
 
-        # Verify that at least ω votes are cast for the currently selected
-        # allele :
-        if (sSNV_phased_votes / obs) < ω:
+        if (this_phase_obs / sSNV_phased_votes) < ω:
+            print(f'This does not pass the threshold ω {ω} ')
             return
+        else:
+            print(f'This does pass the threshold ω {ω} ')
+        break
 
-        # The valid tuples are thus:
-        uninformative_allele = (sSNV_ref_base, wt_allele_gSNV)
-        informative_allele_wt = (sSNV_ref_base, snv_allele_gSNV)
-
-        valid_tuples = [sSNV_phase,  # mutated
-                        informative_allele_wt,  # wt
-                        uninformative_allele]
-
-        # As we have umi's we just have a threshold for the least amount of reads
-        # we want to observe for a molecule to be taken into account
-        # Count how often we found valid and invalid genotypes
-        valid = 0
-        invalid = 0
-        valid_var = 0
-        invalid_var = 0
-        for (ssnv, gsnv), tuple_obs in complete_genotype_obs.most_common():
-            if ssnv == sSNV_alt_base:  # variant:
-                if (ssnv, gsnv) in valid_tuples:
-                    valid_var += tuple_obs
-                else:
-                    invalid_var += tuple_obs
-
-            if (ssnv, gsnv) in valid_tuples:
-                valid += tuple_obs
-            else:
-                invalid += tuple_obs
+    sSNV_phase = (sSNV_state, gSNV_state)
+    phased_gSNV = gSNV_state
+    snv_allele_gSNV = None
+    if gSNV_state == gSNV_ref_base:
+        # the reference allele is alt
+        wt_allele_gSNV = gSNV_alt_base
+        snv_allele_gSNV = gSNV_ref_base
+    else:
+        wt_allele_gSNV = gSNV_ref_base
+        snv_allele_gSNV = gSNV_alt_base
+            # the reference allele is ref
+        # break ? why?
 
-        phase_ratio = 0
-        if valid_var + invalid_var > 0:
-            phase_ratio = valid_var / (valid_var + invalid_var)
-
-        # Score Tuples with evidence for variant
-        haplotype_scores[(chrom, pos)] = {
-            'valid_tuples': valid,
-            'invalid_tuples': invalid,
-            'valid_var_tuples': valid_var,
-            'invalid_var_tuples': invalid_var,
-            'phasing_ratio': phase_ratio,
-            'gSNV_allelic_bias': gSNV_obs[gSNV_ref_base] / (gSNV_obs[gSNV_ref_base] + gSNV_obs[gSNV_alt_base])
-        }
+    statistics[(chromosome, ssnv_position)]['sSNV_gSNV_phase'] = snv_allele_gSNV
 
-        print(f'Germline variant obs: {gSNV_ref_base} {gSNV_alt_base}')
-        print(f'sSNV obs: {sSNV_ref_base} {sSNV_alt_base}')
-        if sSNV_phase is not None:
-            print(f'sSNV variant is phased with {phased_gSNV}')
-        print(Style.BRIGHT + 'Valid tuples:' + Style.RESET_ALL)
-        for g, s in valid_tuples:
-            print(f' {g}\t{s}')
-
-        print(Style.BRIGHT + 'Scores:' + Style.RESET_ALL)
-        for name, obs in haplotype_scores[(chrom, pos)].items():
-            print(f' {name}\t{obs}')
-
-        # Create the cell call dictionary
-
-        for cell, observed_tuples in cell_read_obs.items():
-            total_reads = 0
-            phased_variant_support_reads = 0
-            unphased_variant_support_reads = 0
-            variant_neg_support_reads = 0
-            uninformative_reads = 0
-            conflict_reads = 0
-            for (sSNV_state, gSNV_state), reads in observed_tuples:
-                if sSNV_state is None:
-                    continue
-                total_reads += reads
-                if sSNV_state == sSNV_alt_base:
-                    if gSNV_state == wt_allele_gSNV:
-                        conflict_reads += reads
-                    elif gSNV_state == snv_allele_gSNV:
-                        # reads containing the sSNV and gSNV as expected
-                        phased_variant_support_reads += reads
-                    elif gSNV_state is None:
-                        # reads containing sSNV but not overlapping with gSNV
-                        unphased_variant_support_reads += reads
-
-                elif sSNV_state == sSNV_ref_base:
-                    if gSNV_state == snv_allele_gSNV:
-                        # reads on informative allele where we found evidence
-                        # of the sSNV not being present
-                        variant_neg_support_reads += reads
-
-            if conflict_reads / (total_reads) > 0.2:
-                cell_call_data[(chrom, pos)][cell] = -1  # invalid
-
-            if (unphased_variant_support_reads +
-                    phased_variant_support_reads) / total_reads > 0.1:
-                cell_call_data[(chrom, pos)][cell] = 1
-                if unphased_variant_support_reads + phased_variant_support_reads >= 3:
-                    cell_call_data[(chrom, pos)][cell] = 10
-
-            if (phased_variant_support_reads) / total_reads > 0.1:
-                cell_call_data[(chrom, pos)][cell] = 2
-                if phased_variant_support_reads >= 3:
-                    cell_call_data[(chrom, pos)][cell] = 20
-
-            if variant_neg_support_reads / total_reads > 0.1:
-                # 0.1 for ref allele obs
-                cell_call_data[(chrom, pos)][cell] += 0.1
-
-        # Annotate every molecule...
-
-        for molecule_id, (m, ssnv_state, gsnv_state) in enumerate(
-                window_molecules):
-            m.set_meta('mi', molecule_id)
-            if gsnv_state is None:
-                m.set_meta('gv', '?')
-            else:
-                m.set_meta('gv', gsnv_state)
+    if snv_allele_gSNV is None:
+        print("No germline variant was phased")
+        return
 
-            if ssnv_state is None:
-                m.set_meta('sv', '?')
+    # The valid tuples are thus:
+    uninformative_allele = (sSNV_ref_base, wt_allele_gSNV)
+    informative_allele_wt = (sSNV_ref_base, snv_allele_gSNV)
+
+    valid_tuples = [sSNV_phase,  # mutated
+                    informative_allele_wt,  # wt
+                    uninformative_allele]
+
+    # As we have umi's we just have a threshold for the least amount of reads
+    # we want to observe for a molecule to be taken into account
+    # Count how often we found valid and invalid genotypes
+    valid = 0
+    invalid = 0
+    valid_var = 0
+    invalid_var = 0
+    for (ssnv, gsnv), tuple_obs in complete_genotype_obs.most_common():
+        if ssnv == sSNV_alt_base:  # variant:
+            if (ssnv, gsnv) in valid_tuples:
+                valid_var += tuple_obs
             else:
-                m.set_meta('sv', ssnv_state)
-
-            if ssnv_state is None:
-                m.set_meta('VD', 'NO_SNV_OVERLAP')
-                continue
+                invalid_var += tuple_obs
 
-            if gsnv_state is not None and not (
-                    ssnv_state, gsnv_state) in valid_tuples:
-                m.set_meta('VD', 'INVALID_PHASE')
-                continue
-            if ssnv_state == sSNV_alt_base:
-                m.set_meta('VD', 'SNV_ALT')
-                continue
-
-            if ssnv_state == sSNV_ref_base and gsnv_state == phased_gSNV:
-                m.set_meta('VD', 'SNV_REF')
-                continue
-            if gsnv_state != phased_gSNV:
-                m.set_meta('VD', 'UNINFORMATIVE_ALLELE')
+        if (ssnv, gsnv) in valid_tuples:
+            valid += tuple_obs
+        else:
+            invalid += tuple_obs
+
+    phase_ratio = 0
+    if valid_var + invalid_var > 0:
+        phase_ratio = valid_var / (valid_var + invalid_var)
+
+    # Score Tuples with evidence for variant
+    haplotype_scores[(chrom, pos)] = {
+        'valid_tuples': valid,
+        'invalid_tuples': invalid,
+        'valid_var_tuples': valid_var,
+        'invalid_var_tuples': invalid_var,
+        'phasing_ratio': phase_ratio,
+        'gSNV_allelic_bias': gSNV_obs[gSNV_ref_base] / (gSNV_obs[gSNV_ref_base] + gSNV_obs[gSNV_alt_base])
+    }
+
+    print(f'Germline variant obs: {gSNV_ref_base} {gSNV_alt_base}')
+    print(f'sSNV obs: {sSNV_ref_base} {sSNV_alt_base}')
+    if sSNV_phase is not None:
+        print(f'sSNV variant is phased with {phased_gSNV}')
+    print(Style.BRIGHT + 'Valid tuples:' + Style.RESET_ALL)
+    for g, s in valid_tuples:
+        print(f' {g}\t{s}')
+
+    print(Style.BRIGHT + 'Scores:' + Style.RESET_ALL)
+    for name, obs in haplotype_scores[(chrom, pos)].items():
+        print(f' {name}\t{obs}')
+
+    # Create the cell call dictionary
+
+    uninformative_obs = 0 # This is important, otherwise we might use a SNP ..
+    for cell, observed_tuples in cell_read_obs.items():
+        print(cell,  observed_tuples)
+        total_reads = 0
+        phased_variant_support_reads = 0
+        unphased_variant_support_reads = 0
+        variant_neg_support_reads = 0
+        uninformative_reads = 0
+        conflict_reads = 0
+        for (sSNV_state, gSNV_state), reads in observed_tuples.items():
+            if sSNV_state is None:
                 continue
-
-            m.set_meta('VD', 'REJECTED')
-        # write
-
-        for m, ssnv_state, gsnv_state in window_molecules:
-            m.write_tags()
-            m.write_pysam(out)
-
-            # Update read groups
-            for fragment in m:
-                read_groups.add(fragment.get_read_group())
+            total_reads += reads
+            if sSNV_state == sSNV_alt_base:
+                if gSNV_state == wt_allele_gSNV:
+                    conflict_reads += reads
+                elif gSNV_state == snv_allele_gSNV:
+                    # reads containing the sSNV and gSNV as expected
+                    phased_variant_support_reads += reads
+                elif gSNV_state is None:
+                    # reads containing sSNV but not overlapping with gSNV
+                    unphased_variant_support_reads += reads
+
+            elif sSNV_state == sSNV_ref_base:
+                if gSNV_state == snv_allele_gSNV:
+                    # reads on informative allele where we found evidence
+                    # of the sSNV not being present
+                    variant_neg_support_reads += reads
+                elif gSNV_state == wt_allele_gSNV:
+                    uninformative_reads += reads
+                    uninformative_obs += 1
+
+        if total_reads==0:
+            continue
+        if variant_neg_support_reads>0:
+            cell_call_data[(chrom, pos)][cell] = 0
+
+        if (unphased_variant_support_reads +
+                phased_variant_support_reads) / total_reads > 0.1:
+            cell_call_data[(chrom, pos)][cell] = 1
+            if unphased_variant_support_reads + phased_variant_support_reads >= 3:
+                cell_call_data[(chrom, pos)][cell] = 10
+
+        if (phased_variant_support_reads) / total_reads > 0.1:
+            cell_call_data[(chrom, pos)][cell] = 2
+            if phased_variant_support_reads >= 3:
+                cell_call_data[(chrom, pos)][cell] = 20
+
+        #if uninformative_reads / total_reads > 0.1:
+        #    # 0.1 for ref allele obs
+    #        cell_call_data[(chrom, pos)][cell] += 0.1
+
+        if conflict_reads / (total_reads) > 0.2:
+            cell_call_data[(chrom, pos)][cell] = -1  # invalid
+
+
+    haplotype_scores[(chrom, pos)]['uninformative_obs'] = uninformative_obs
+    # Annotate every molecule...
+
+    for molecule_id, (m, ssnv_state, gsnv_state) in enumerate(
+            window_molecules):
+        m.set_meta('mi', molecule_id)
+        if gsnv_state is None:
+            m.set_meta('gv', '?')
+        else:
+            m.set_meta('gv', gsnv_state)
+
+        if ssnv_state is None:
+            m.set_meta('sv', '?')
+        else:
+            m.set_meta('sv', ssnv_state)
+
+        if ssnv_state is None:
+            m.set_meta('VD', 'NO_SNV_OVERLAP')
+            continue
+
+        if gsnv_state is not None and not (
+                ssnv_state, gsnv_state) in valid_tuples:
+            m.set_meta('VD', 'INVALID_PHASE')
+            continue
+        if ssnv_state == sSNV_alt_base:
+            m.set_meta('VD', 'SNV_ALT')
+            continue
+
+        if ssnv_state == sSNV_ref_base and gsnv_state == phased_gSNV:
+            m.set_meta('VD', 'SNV_REF')
+            continue
+        if gsnv_state != phased_gSNV:
+            m.set_meta('VD', 'UNINFORMATIVE_ALLELE')
+            continue
+
+        m.set_meta('VD', 'REJECTED')
+    # write
+
+    for m, ssnv_state, gsnv_state in window_molecules:
+        m.write_tags()
+        m.write_pysam(out)
+
+        # Update read groups
+        for fragment in m:
+            read_groups.add(fragment.get_read_group())
 
 
 if __name__ == '__main__':
     argparser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="""
     Known variant locations extraction tool
     """)
     argparser.add_argument('bamfiles', nargs='+')
     argparser.add_argument(
         '-ssnv',
-        help="sSNV bed file",
+        help="sSNV bed file, or single sSNV location chr:pos",
         type=str,
         required=True)
     argparser.add_argument(
         '-gsnv',
-        help="gSNV bed file",
+        help="gSNV bed file, or single gSNV location chr:pos",
         type=str,
         required=True)
     argparser.add_argument(
         '-reference',
         help="reference fasta file",
         type=str,
         required=True)
     argparser.add_argument('-head', type=int)
     argparser.add_argument('-min_read_obs', type=int, default=2)
     argparser.add_argument(
         '--realign',
         action='store_true',
         help='Perform re-alignment using GATK')
     argparser.add_argument(
+        '--ignore_bam_issues',
+        action='store_true',
+        help='')
+    argparser.add_argument(
         '-gatk3_path',
         type=str,
         default='GenomeAnalysisTK.jar')
     argparser.add_argument('-indelvcf', type=str)
+
+    argparser.add_argument('-prefix', type=str, default='')
+
     argparser.add_argument('-window_radius', type=int, default=250)
+    argparser.add_argument('-realign_mem', type=int, default=25)
+    argparser.add_argument('--cluster', action='store_true')
     args = argparser.parse_args()
 
     if args.realign and args.indelvcf is None:
         raise ValueError("supply -indelvcf")
 
     WINDOW_RADIUS = args.window_radius
     paths = args.bamfiles
 
     # Load probed variants
     probed_variants = {}
-    with open(args.ssnv) as s, \
-            open(args.gsnv) as g:
-        for i, (ssnv_line, gsnv_line) in enumerate(zip(s, g)):
-            if ssnv_line.startswith('track name'):
-                continue
-            chrom, snv_pos, _ = ssnv_line.strip().split()
-            _, gsnv_pos, __ = gsnv_line.strip().split()
-            snv_pos, gsnv_pos = int(snv_pos), int(gsnv_pos)
-            probed_variants[(chrom, snv_pos)] = gsnv_pos
+    if ':' in args.ssnv:
+        chrom, snv_pos = args.ssnv.strip().split(':')
+        chrom_g, gsnv_pos = args.gsnv.strip().split(':')
+        assert chrom==chrom_g, 'germline SNV should be on the same chromosome as the sSNV'
+        probed_variants[(chrom, int(snv_pos))] = int( gsnv_pos)
 
+    else:
+        with open(args.ssnv) as s, \
+                open(args.gsnv) as g:
+            for i, (ssnv_line, gsnv_line) in enumerate(zip(s, g)):
+                if ssnv_line.startswith('track name'):
+                    continue
+                chrom, snv_pos, _ = ssnv_line.strip().split()
+                _, gsnv_pos, __ = gsnv_line.strip().split()
+                snv_pos, gsnv_pos = int(snv_pos), int(gsnv_pos)
+                probed_variants[(chrom, snv_pos)] = gsnv_pos
+
+    if args.cluster:
+        for i,((chrom, snv_pos), gsnv_pos) in enumerate(probed_variants.items()):
+            arguments = " ".join(
+                [x for x in sys.argv if x != '--cluster' and '.bed' not in x and '-ssnv'!=x and '-gsnv'!=x ])
+
+            job_name = f'vstat_{i}'
+            out_folder = './variantStats'
+            if not os.path.exists(out_folder):
+                os.makedirs(out_folder)
+            print('submission.py' + f' -y --py36 -time 50 -t 1 -m 50 -N {job_name} "{arguments} -ssnv {chrom}:{snv_pos} -gsnv {chrom}:{gsnv_pos} -prefix {out_folder}/{chrom}_{snv_pos}" ')
+        exit()
     reference = pysamiterators.CachedFasta(pysam.FastaFile(args.reference))
 
     cell_obs = collections.defaultdict(
         lambda: collections.defaultdict(
             collections.Counter))
     statistics = collections.defaultdict(
         lambda: collections.defaultdict(
             collections.Counter))
     cell_call_data = collections.defaultdict(dict)  # location->cell->haplotype
     haplotype_scores = {}
 
     read_groups = set()  # Store unique read groups in this set
-    with sorted_bam_file('evidence.bam', origin_bam=pysam.AlignmentFile(paths[0]), read_groups=read_groups) as out:
+    with sorted_bam_file(f'{args.prefix}_evidence.bam', origin_bam=pysam.AlignmentFile(paths[0], ignore_truncation=args.ignore_bam_issues), read_groups=read_groups) as out:
 
         for variant_index, ((chromosome, ssnv_position), potential_gsnv_position) in enumerate(
                 probed_variants.items()):
 
-            obtain_variant_statistics(
-                alignment_file_paths=paths,
-                cell_obs=cell_obs,
-                cell_call_data=cell_call_data,
-                statistics=statistics,
-                reference=reference,
-                chromosome=chromosome,
-                ssnv_position=ssnv_position,
-                gsnv_position=potential_gsnv_position,
-                WINDOW_RADIUS=WINDOW_RADIUS,
-                haplotype_scores=haplotype_scores,
-                out=out, min_read_obs=args.min_read_obs,
-                read_groups=read_groups,
-                args=args,
-                umi_hamming_distance=1
-            )
+            try:
+                obtain_variant_statistics(
+                    alignment_file_paths=paths,
+                    cell_obs=cell_obs,
+                    cell_call_data=cell_call_data,
+                    statistics=statistics,
+                    reference=reference,
+                    chromosome=chromosome,
+                    ssnv_position=ssnv_position,
+                    gsnv_position=potential_gsnv_position,
+                    WINDOW_RADIUS=WINDOW_RADIUS,
+                    haplotype_scores=haplotype_scores,
+                    out=out, min_read_obs=args.min_read_obs,
+                    read_groups=read_groups,
+                    args=args,
+                    umi_hamming_distance=1
+                )
+            except Exception as e:
+                traceback.print_exc()
 
             if args.head and (variant_index > args.head - 1):
                 print(
                     f'Stopping at variant {variant_index+1} because head was supplied ')
                 break
 
     lambda_free_dict = {}
@@ -598,15 +662,15 @@
             'mean_del_pbp': meanOfCounter(stats['deletions_per_bp']),
             'mean_matches_pbp': meanOfCounter(stats['matches_per_bp']),
             'mean_alt_mapping_per_read': meanOfCounter(stats['alt_per_read']),
 
             'ssnv_ref_phred': meanOfCounter(stats['ssnv_ref_phred']),
             'ssnv_alt_phred': meanOfCounter(stats['ssnv_alt_phred']),
             'gsnv_ref_phred': meanOfCounter(stats['gsnv_ref_phred']),
-            'gsnv_alt_phred': meanOfCounter(stats['gsnv_alt_phred']),
+            'gsnv_any_alt_phred': meanOfCounter(stats['gsnv_any_alt_phred']),
 
             'mean_max_mapping_quality': meanOfCounter(stats['max_mapping_quality']),
             'mean_ivt_dups': meanOfCounter(stats['ivt_dups']),
             'mean_undigested': meanOfCounter(stats['undigested']),
             'R2_unmapped': stats['R2_unmapped'][True],
 
 
@@ -614,16 +678,24 @@
             'mean_reads': meanOfCounter(stats['reads']),
             'total_reads': sum((amount * frequency for amount, frequency in stats['reads'].most_common())),
             'total_molecules': sum((amount * frequency for amount, frequency in stats['molecules'].most_common()))
 
         }
 
     print('Writing final site table')
-    site_stats = pd.DataFrame(lambda_free_dict).T.join(
-        pd.DataFrame(haplotype_scores).T)
-    site_stats.to_pickle('site_stats.pickle.gz')
-    site_stats.to_csv('site_stats.csv')
+    try:
+        site_stats = pd.DataFrame(lambda_free_dict).T.join(
+            pd.DataFrame(haplotype_scores).T)
+    except Exception as e:
+        print(e)
+        site_stats = pd.DataFrame(lambda_free_dict).T
+
+    site_stats.to_pickle(f'{args.prefix}_site_stats.pickle.gz')
+    site_stats.to_csv(f'{args.prefix}_site_stats.csv')
 
     print('Writing final cell table')
-    cell_call_df = pd.DataFrame(cell_call_data)
-    cell_call_df.to_pickle('cell_calls.pickle.gz')
-    cell_call_df.to_csv('cell_calls.csv')
+    try:
+        cell_call_df = pd.DataFrame(cell_call_data)
+        cell_call_df.to_pickle(f'{args.prefix}_cell_calls.pickle.gz')
+        cell_call_df.to_csv(f'{args.prefix}_cell_calls.csv')
+    except Exception as e:
+        print(e)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/barcodeFileParser/barcodeFileParser.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/barcodeFileParser/barcodeFileParser.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/countTableProcessing/correct_count_table_bias.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/countTableProcessing/correct_count_table_bias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import singlecellmultiomics
 from singlecellmultiomics.molecule import MoleculeIterator, NlaIIIMolecule
-from singlecellmultiomics.fragment import NLAIIIFragment
+from singlecellmultiomics.fragment import NlaIIIFragment
 import pysam
 import collections
 import pysamiterators
 import pandas as pd
 import seaborn as sns
 import numpy as np
 import re
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/countTableProcessing/downsampleDataFrame.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/countTableProcessing/downsampleDataFrame.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/fastaProcessing/createMapabilityIndex.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/fastaProcessing/createMappabilityIndex.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,20 +129,20 @@
 
             # Assing a wrong annotation to the target site:
             if key_mapped not in sites:
                 sites[key_mapped] = {'correct': 0, 'wrong_gain': 0, 'lost': 0}
             sites[key_mapped]['wrong_gain'] += 1
 
     print("Writing site statistics ...")
-    outtab = f'simulated_{args.digest_sequence}_single_{r1_read_length}.mapability.stats.bgzf'
-    outtabsafe = f'simulated_{args.digest_sequence}_single_{r1_read_length}.mapability.safe.bgzf'
+    outtab = f'simulated_{args.digest_sequence}_single_{r1_read_length}.mappability.stats.bgzf'
+    outtabsafe = f'simulated_{args.digest_sequence}_single_{r1_read_length}.mappability.safe.bgzf'
 
     with BlockZip(outtab, 'w') as stats, BlockZip(outtabsafe, 'w') as safe:
         for (contig, pos, strand), measured in sites.items():
             stats.write(
                 contig,
                 pos,
                 strand,
-                f'{measured["correct"]}\t{measured["lost"]}\t{measured["wrong_gain"]}\n')
+                f'{measured["correct"]}\t{measured["lost"]}\t{measured["wrong_gain"]}')
 
             if measured['wrong_gain'] == 0 and measured['lost'] == 0 and measured['correct'] == 1:
                 safe.write(contig, pos, strand, 'ok')
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/fastaProcessing/fastaMaskVariants.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/fastaProcessing/fastaMaskVariants.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pysam
 import numpy as np
 import argparse
 import os
 import itertools
 import gzip
 import pandas as pd
+import multiprocessing
 
 if __name__ == '__main__':
     argparser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="""Convert genome FASTA file to convert alternative bases to Ns""")
     argparser.add_argument(
         'fasta',
@@ -22,14 +23,19 @@
         type=str,
         help='VCF file(s) to extract variants from')
     argparser.add_argument(
         '-o',
         type=str,
         default='./masked.fasta.gz',
         help='output file')
+    argparser.add_argument(
+        '-t',
+        type=int,
+        default=10,
+        help='Amount of contigs to process in parallel')
     args = argparser.parse_args()
 
     try:
         faIn = pysam.FastaFile(args.fasta)
     except ValueError as e:
         print('FAI index missing. Now creating...')
         os.system(f'samtools faidx {args.fasta}')
@@ -37,43 +43,56 @@
         raise
 
     try:
         faIn = pysam.FastaFile(args.fasta)
     except Exception as e:
         raise
 
-    outputHandle = gzip.open(args.o, 'wb')
+    if args.o.endswith('.gz'):
+        outputHandle = gzip.open(args.o, 'wb')
+    else:
+        outputHandle = open(args.o, 'wb')
     referenceNames = faIn.references
     referenceLengths = dict(zip(referenceNames, faIn.lengths))
-
-    # wholeGenome = {
-    #    ref:faIn.fetch(ref) for ref in referenceNames
-    # }
-    warnedMissing = set()
     totalMasked = 0
-    variants = pysam.VariantFile(args.vcf)
-    for chrom in referenceNames:
-        try:
+
+    def get_masked_bytearray( jargs ):
+
+        totalMasked = 0
+        (chrom, fasta_file_path, variant_file_path) = jargs
+        with pysam.FastaFile(fasta_file_path) as faIn, pysam.VariantFile(variant_file_path, threads=4) as  variants:
+
             chrom_seq = bytearray(faIn.fetch(chrom), 'ascii')
-            for rec in variants.fetch(chrom):
-                if rec.start >= (referenceLengths[rec.chrom]):
-                    print(
-                        f"WARNING record {rec.chrom} {rec.pos} defines a variant outside the supplied fasta file!")
-                    continue
-
-                if len(rec.alleles) == 1 and len(rec.alleles[0]) == 1:
-                    chrom_seq[rec.pos - 1] = 78  # ord N
-                    totalMasked += 1
-                elif len(rec.alleles[0]) == 1 and len(rec.alleles[1]) == 1:
-
-                    chrom_seq[rec.pos - 1] = 78  # ord N
-                    totalMasked += 1
-
-        except ValueError:
-            print(f"No variants for {chrom}")
-            pass
+            if chrom in variants.index:
+                print(f'masking {chrom}')
+                for rec in variants.fetch(chrom):
+                    if rec.start >= (referenceLengths[rec.chrom]):
+                        print(
+                            f"WARNING: record {rec.chrom} {rec.pos} defines a variant outside the supplied fasta file!")
+                        continue
+
+                    if len(rec.alleles) == 1 and len(rec.alleles[0]) == 1:
+                        chrom_seq[rec.pos-1] = 78  # ord N
+                        totalMasked += 1
+                    elif len(rec.alleles[0]) == 1 and len(rec.alleles[1]) == 1:
+
+                        chrom_seq[rec.pos-1] = 78  # ord N
+                        totalMasked += 1
+            print(f'Masked {totalMasked} bases of {chrom}')
+            return chrom_seq
+
+
+    workers = multiprocessing.Pool(args.t)
+
+
+    for chrom, chrom_seq in zip(
+                referenceNames,
+                workers.imap(
+                    get_masked_bytearray,
+                    ((chrom, args.fasta, args.vcf )
+                    for chrom in referenceNames ))):
         # Write chromsome
         outputHandle.write(f'>{chrom}\n'.encode('ascii'))
         outputHandle.write(chrom_seq)
         outputHandle.write('\n'.encode('ascii'))
 
     outputHandle.close()
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/fastqProcessing/fastqHandle.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/fastqProcessing/fastqHandle.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,31 @@
         self.path = path
         if not self.sc:
             if pairedEnd:
                 self.handles = [
                     gzip.open(
                         path +
                         'R1.fastq.gz',
-                        'wt'),
+                        'wt',compresslevel=1),
                     gzip.open(
                         path +
                         'R2.fastq.gz',
-                        'wt')]
+                        'wt',compresslevel=1)]
             else:
                 self.handles = [gzip.open(path + 'reads.fastq.gz', 'wt')]
         else:
 
             self.handles = HandleLimiter(
                 compressionLevel=1, maxHandles=maxHandles)
 
     def write(self, records):
         if self.sc:
             for readIdx, record in zip(('R1', 'R2'), records):
                 # Obtain cell from record:
-                cell = f"{record.tags.get('BI','no_cell_id')}.{record.tags.get('MX','unk')}"
+                cell = f"{record.tags.get('bi','no_cell_id')}.{record.tags.get('MX','unk')}"
                 self.handles.write(
                     f'{self.path}.{cell}.{readIdx}.fastq.gz',
                     str(record),
                     method=1)
         else:
             for handle, record in zip(self.handles, records):
                 handle.write(str(record))
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/fastqProcessing/fastqIterator.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/fastqProcessing/fastqIterator.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/features/exonGTFtoIntronGTF.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/features/exonGTFtoIntronGTF.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/features/features.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/features/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 import gzip
 import itertools
 import re
 import functools
 import pysam
-
+from singlecellmultiomics.utils import Prefetcher
+from copy import copy
 
 def get_gene_id_to_gene_name_conversion_table(annotation_path_exons,
                                               featureTypes=['gene_name']):
     """Create a dictionary converting a gene id to other gene features,
         such as gene_name/gene_biotype etc.
 
     Arguments:
         annotation_path_exons(str) : path to GTF file (can be gzipped)
         featureTypes(list) : list of features to convert to, for example ['gene_name','gene_biotype']
 
     Returns:
         conversion_dict(dict) : { gene_id : 'firstFeature_secondFeature'}
-        """
+    """
     conversion_table = {}
     with (gzip.open(annotation_path_exons, 'rt') if annotation_path_exons.endswith('.gz') else open(annotation_path_exons, 'r')) as t:
         for i, line in enumerate(t):
             parts = line.rstrip().split(None, 8)
             keyValues = {}
             for part in parts[-1].split(';'):
                 kv = part.strip().split()
@@ -37,44 +38,91 @@
                 conversion_table[keyValues['gene_id']] = '_'.join([
                     keyValues.get(feature, 'None')
                     for feature in featureTypes])
 
     return conversion_table
 
 
-class FeatureContainer:
+class FeatureContainer(Prefetcher):
 
     def __init__(self):
+        self.args = locals().copy()
         self.startCoordinates = {}  # dict of np.array()
         self.features = {}
         self.endCoordinates = {}
         self.sorted = True  # Flag containing if the features are all coordinate sorted
         # When set to true, the class will be (very) verbose
         self.debug = False
         self.remapKeys = {}  # {'chrMT':'chrM','MT':'chrM'}  Use this to convert chromosome names between the GTF and requested locations
         self.verbose = False
+        self.preload_list = []
 
     def debugMsg(self, msg):
         if self.verbose:
             print(msg)
 
+    def __repr__(self):
+        s= 'FeatureContainer,'
+        if len(self.preload_list):
+            s+= ' Preloaded files:\n'
+            for f in self.preload_list:
+                s+=str(f)+'\n'
+        if len(self.features):
+            s+=f'Features in memory for {len(self.features)} contigs\n'
+        else:
+            s+='No features in memory\n'
+        return s
+
     def __len__(self):
         return sum(len(f) for f in self.features.values())
 
+
+    def preload_GTF(self, **kwargs):
+        self.preload_list.append( {'gtf':kwargs} )
+
+
+    def instance(self, arg_update):
+        if 'self' in self.args:
+            del self.args['self']
+        clone = FeatureContainer(**self.args)
+        for cmd in self.preload_list:
+            for preload_type, kwargs in cmd.items():
+                kwargs_copy = copy(kwargs)
+                kwargs_copy.update(arg_update)
+                if preload_type=='gtf':
+                    clone.loadGTF(**kwargs_copy)
+                else:
+                    raise ValueError()
+        return clone
+
+
+    def prefetch(self, contig, start, end):
+        return self.instance( {'contig':contig, 'region_start':start,  'region_end':end})
+
+
     def loadGTF(self, path, thirdOnly=None, identifierFields=['gene_id'],
                 ignChr=False, select_feature_type=None, exon_select=None,
-                head=None, store_all=False, contig=None):
+                head=None, store_all=False, contig=None, offset=-1,
+                region_start=None, region_end=None):
         """Load annotations from a GTF file.
         ignChr: ignore the chr part of the Annotation chromosome
         """
+        if region_end is not None or region_start is not None:
+            assert contig is not None and region_end is not None and region_start is not None
+
         self.loadedGtfFeatures = thirdOnly
         #pattern = '^(.*) "(.*).*"'
         #prog = re.compile(pattern)
         if self.verbose:
-            print("Loading %s" % path)
+            if contig is None:
+                print(f"Loading {path} completely")
+            elif region_start is None:
+                print(f"Loading {path}, for contig {contig}")
+            else:
+                print(f"Loading {path}, for contig {contig}:{region_start}-{region_end}")
         added = 0
         with (gzip.open(path, 'rt') if path.endswith('.gz') else open(path, 'r')) as f:
             for line_id, line in enumerate(f):
                 if head is not None and added > head:
                     break
                 if line[0] != '#':
                     parts = line.rstrip().split(None, 8)
@@ -136,29 +184,32 @@
                         else:
                             featureName = ','.join(
                                 [parts[2], parts[3], parts[4], keyValues['transcript_id']])
                     else:
                         featureName = ','.join(
                             [keyValues.get(i, 'none') for i in identifierFields if i in keyValues])
 
+
+                    start = int( parts[3] ) + offset
+                    end = int( parts[4] ) + offset
+
+                    if region_end is not None and region_start is not None and ( end<region_start or start>region_end):
+                        continue
+
                     if store_all:
                         keyValues['type'] = parts[2]
                         self.addFeature(
                             self.remapKeys.get(
-                                chromosome, chromosome), int(
-                                parts[3]), int(
-                                parts[4]), strand=parts[6], name=featureName, data=tuple(
+                                chromosome, chromosome),start,end, strand=parts[6], name=featureName, data=tuple(
                                 keyValues.items()))
 
                     else:
                         self.addFeature(
                             self.remapKeys.get(
-                                chromosome, chromosome), int(
-                                parts[3]), int(
-                                parts[4]), strand=parts[6], name=featureName, data=','.join(
+                                chromosome, chromosome), start,end, strand=parts[6], name=featureName, data=','.join(
                                 (':'.join(
                                     ('type', parts[2])), ':'.join(
                                     ('gene_id', keyValues['gene_id'])))))
                     added += 1
 
             if self.verbose:
                 print("Loaded %s features, now sorting" %
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/fragment/chic.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/chic.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,32 @@
 class CHICFragment(Fragment):
     def __init__(self,
                  reads,
                  R1_primer_length=4,
                  R2_primer_length=6,
                  assignment_radius=1_000,
                  umi_hamming_distance=1,
-                 invert_strand=True
+                 invert_strand=True,
+                 no_umi_cigar_processing=False,
+                 **kwargs
                  ):
         self.invert_strand = invert_strand
         Fragment.__init__(self,
                           reads,
                           assignment_radius=assignment_radius,
                           R1_primer_length=R1_primer_length,
                           R2_primer_length=R2_primer_length,
-                          umi_hamming_distance=umi_hamming_distance
+                          umi_hamming_distance=umi_hamming_distance,
+                          max_NUC_stretch = 18,
+                          **kwargs
+
+                )
 
-                          )
         # set CHIC cut site given reads
+        self.no_umi_cigar_processing = no_umi_cigar_processing
         self.strand = None
         self.ligation_motif = None
         self.site_location = None
         self.cut_site_strand = None
         self.identify_site()
         if self.is_valid():
             self.match_hash = (
@@ -75,39 +81,58 @@
         is_trimmed = (R1.has_tag('MX') and R1.get_tag(
             'MX').startswith('scCHIC'))
 
         if R1.is_unmapped:
             self.set_rejection_reason("R1_unmapped")
             return(None)
 
-        # if R1.seq[0]=='T': # Site on the start of R1, R2 should map behind
+        # Identify the start coordinate of Read 1 by reading the amount of softclips on the start of the read
+        r1_start =(R1.reference_end if R1.is_reverse else R1.reference_start)
+        if not self.no_umi_cigar_processing:
+            if R1.is_reverse:
+                if R1.cigartuples[-1][0]==4: # softclipped at end
+                    r1_start+=R1.cigartuples[-1][1]
+            else:
+                if R1.cigartuples[0][0]==4: # softclipped at start
+                    r1_start-=R1.cigartuples[0][1]
+
         if is_trimmed:
             # The first base of the read has been taken off and the lh tag is
             # already set, this can be copied to RZ
 
             self.set_site(
                 site_strand=R1.is_reverse if not self.invert_strand else not R1.is_reverse,
                 # We sequence the other strand (Starting with a T, this is an A in the molecule), the digestion thus happened on the other strand
                 # On the next line we asume that the mnsase cut is one base after the ligated A, but it can be more bases upstream
                 site_chrom=R1.reference_name,
-                site_pos=(R1.reference_end if R1.is_reverse else R1.reference_start),
+                site_pos=r1_start,
                 is_trimmed=True
-
             )
+
         else:
 
             self.set_site(
                 site_strand=R1.is_reverse if not self.invert_strand else not R1.is_reverse,
                 # We sequence the other strand (Starting with a T, this is an A in the molecule), the digestion thus happened on the other strand
                 # On the next line we asume that the mnsase cut is one base after the ligated A, but it can be more bases upstream
                 site_chrom=R1.reference_name,
-                site_pos=(R1.reference_end - 1 if R1.is_reverse else R1.reference_start + 1),
+                site_pos=(r1_start - 1 if R1.is_reverse else r1_start + 1),
                 is_trimmed=False)
 
     def is_valid(self):
+        if self.qcfail:
+            return False
+
+        if self.max_fragment_size is not None:
+            try:
+                size = self.get_fragment_size()
+                if size>self.max_fragment_size:
+                    return False
+            except Exception:
+                pass
         return self.site_location is not None
 
     def get_site_location(self):
         return self.site_location
 
     def __repr__(self):
         return Fragment.__repr__(
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/fragment/fragment.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/fragment/fragment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 from singlecellmultiomics.utils.sequtils import hamming_distance
 import pysamiterators.iterators
 import singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods
 from singlecellmultiomics.utils import style_str
+from singlecellmultiomics.bamProcessing import get_read_group_from_read
 complement = str.maketrans('ATCGN', 'TAGCN')
 
 
 class Fragment():
     """
     This class holds 1 or more reads which are derived from the same cluster
 
@@ -42,15 +43,18 @@
 
     """
 
     def __init__(self, reads, assignment_radius=3, umi_hamming_distance=1,
                  R1_primer_length=0,
                  R2_primer_length=6,
                  tag_definitions=None,
-                 mapping_dir=(False, True)  # R1 forward, R2 reverse
+                 max_fragment_size = None,
+                 mapping_dir=(False, True),
+                 max_NUC_stretch = None,
+                 read_group_format=0  # R1 forward, R2 reverse
                  ):
         """
         Initialise Fragment
 
             Args:
                 reads( list ):
                     list containing pysam AlignedSegment reads
@@ -66,18 +70,22 @@
 
                 R2_primer_length(int):
                     length of R2 primer, these bases are not taken into account when calculating a consensus
 
                 tag_definitions(list):
                     sam TagDefinitions
 
+                max_fragment_size (int):
+                    When specified, fragments with a fragment size larger than the specified value are flagged as qcfail
+
                 mapping_dir( tuple ):
                     expected mapping direction of mates,
                     True for reverse, False for forward. This parameter is used in dovetail detection
 
+                read_group_format(int) : see get_read_group()
             Returns:
                 html(string) : html representation of the fragment
         """
         self.R1_primer_length = R1_primer_length
         self.R2_primer_length = R2_primer_length
         if tag_definitions is None:
             tag_definitions = singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods.TagDefinitions
@@ -92,27 +100,44 @@
         # Check for multimapping
         self.is_multimapped = True
         self.mapping_quality = 0
         self.match_hash = None
         self.safe_span = None  # wether the span of the fragment could be determined
         self.unsafe_trimmed = False  # wether primers have been trimmed off
         self.random_primer_sequence = None
+        self.max_fragment_size = max_fragment_size
+        self.read_group_format = read_group_format
+        self.max_NUC_stretch = max_NUC_stretch
+        self.qcfail = False
+
         # Span:\
         self.span = [None, None, None]
 
         self.umi = None
 
         # Force R1=read1 R2=read2:
+
         for i, read in enumerate(self.reads):
 
             if read is None:
                 continue
+
+            if self.max_NUC_stretch is not None and (
+                self.max_NUC_stretch*'A' in read.seq or \
+                self.max_NUC_stretch*'G' in read.seq or \
+                self.max_NUC_stretch*'T' in read.seq or \
+                self.max_NUC_stretch*'C' in read.seq ):
+                self.set_rejection_reason('HomoPolymer', set_qcfail=True)
+                self.qcfail=True
+                break
+
             if read.has_tag('rS'):
                 self.random_primer_sequence = read.get_tag('rS')
                 self.unsafe_trimmed = True
+                self.R2_primer_length = 0 # Set R2 primer length to zero, as the primer has been removed
             if not read.is_unmapped:
                 self.is_mapped = True
             if read.mapping_quality > 0:
                 self.is_multimapped = False
             self.mapping_quality = max(
                 self.mapping_quality, read.mapping_quality)
             if i == 0:
@@ -121,14 +146,16 @@
                 read.is_read1 = True
                 read.is_read2 = False
             elif i == 1:
                 read.is_read1 = False
                 read.is_read2 = True
 
         self.set_sample()
+        if self.qcfail:
+            return
         self.set_strand(self.identify_strand())
         self.update_span()
         self.update_umi()
 
     def write_tensor(self, chromosome=None, span_start=None, span_end=None, height=30, index_start=0,
                      base_content_table=None,
                      base_mismatches_table=None,
@@ -270,47 +297,59 @@
 
             used_reads += 1
         if skip_missing_reads:
             return used_reads + index_start + 1
         else:
             return ri + index_start + 1
 
-    def get_read_group(self):
-        """
-        Obtain read group for this fragment
-        Returns:
-            read_group(str) : Read group containing flow cell lane and unique sample id
-        """
-        rg = None
+
+    def get_read_group(self, with_attr_dict=False):
+
+
+        rg_id=None
         for read in self.reads:
-            if read is not None:
-                rg = f"{read.get_tag('Fc') if read.has_tag('Fc') else 'NONE'}.{read.get_tag('La') if read.has_tag('La') else 'NONE'}.{read.get_tag('SM') if read.has_tag('SM') else 'NONE'}"
-                break
-        return rg
+            if read is None:
+                continue
+
+            r = get_read_group_from_read(read,
+                    format=self.read_group_format,
+                    with_attr_dict=with_attr_dict)
+
+            break
+
+        return r
+
 
     def set_duplicate(self, is_duplicate):
         """Define this fragment as duplicate, sets the corresponding bam bit flag
         Args:
             value(bool) : is_duplicate
         """
         for read in self.reads:
             if read is not None:
                 read.is_duplicate = is_duplicate
 
+    def get_fragment_size(self):
+        return abs(self.span[2] - self.span[1])
+
     def write_tags(self):
         self.set_meta('MQ', self.mapping_quality)
         self.set_meta('MM', self.is_multimapped)
         self.set_meta('RG', self.get_read_group())
         if self.has_valid_span():
             # Write fragment size:
-            self.set_meta('fS', abs(self.span[2] - self.span[1]))
+            self.set_meta('fS', self.get_fragment_size())
             self.set_meta('fe', self.span[1])
             self.set_meta('fs', self.span[2])
 
+        else:
+            self.set_rejection_reason('FS', set_qcfail=True)
+
         # Set qcfail bit when the fragment is not valid
+
         if not self.is_valid():
             for read in self:
                 if read is not None:
                     read.is_qcfail = True
 
     def write_pysam(self, pysam_handle):
         """Write all associated reads to the target file
@@ -335,43 +374,44 @@
             if self.get_R2().is_unmapped:
                 return None
             return not self.get_R2().is_reverse
         return None
 
     def get_random_primer_hash(self):
         """Obtain hash describing the random primer
-        this assumes the random primer is on the end of R2 and has a length of 6BP
+        this assumes the random primer is on the end of R2 and has a length of self.R2_primer_length
         When the rS tag is set, the value of this tag is used as random primer sequence
         Returns None,None when the random primer cannot be described
 
         Returns:
+            reference_name (str) or None
             reference_start (int) : Int or None
             sequence (str) : Int or None
         """
         R2 = self.get_R2()
 
         if R2 is None or R2.query_sequence is None:
-            return None, None
+            return None, None, None
         # The read was not mapped
         if R2.is_unmapped:
             # Guess the orientation does not matter
             if self.random_primer_sequence is not None:
-                return None, self.random_primer_sequence
-            return None, R2.query_sequence[:self.R2_primer_length]
+                return None, None, self.random_primer_sequence
+            return None, None, R2.query_sequence[:self.R2_primer_length]
 
         if R2.is_reverse:
             global complement
             if self.random_primer_sequence is not None:
-                return R2.reference_end, self.random_primer_sequence
+                return R2.reference_name, R2.reference_end, self.random_primer_sequence
 
-            return(R2.reference_end, R2.query_sequence[-self.R2_primer_length:][::-1].translate(complement))
+            return(R2.reference_name, R2.reference_end, R2.query_sequence[-self.R2_primer_length:][::-1].translate(complement))
         else:
             if self.random_primer_sequence is not None:
-                return R2.reference_start, self.random_primer_sequence
-            return(R2.reference_start, R2.query_sequence[:self.R2_primer_length])
+                return R2.reference_name, R2.reference_start, self.random_primer_sequence
+            return(R2.reference_name, R2.reference_start, R2.query_sequence[:self.R2_primer_length])
         raise ValueError()
 
     def set_meta(self, key, value, as_set=False):
         self.meta[key] = value
         for read in self:
             if read is not None:
                 if as_set and read.has_tag(key):
@@ -428,48 +468,59 @@
         if len(self.reads) < 2:
             return False
         return self.reads[1] is not None
 
     def update_span(self):
         """
         Update the span (the location the fragment maps to) stored in Fragment
-        """
 
-        if self.mapping_dir != (False, True):
-            raise NotImplementedError("Sorry only FW RV is implemented")
+        The span is a single stretch of coordinates on a single contig.
+        The contig is determined by the reference_name assocated to the first
+        mapped read in self.reads
+
+        """
 
         contig = None
+
+        start = None
+        end = None
         for read in self.reads:
             if read is not None and not read.is_unmapped:
-                contig = read.reference_name
+                if contig is None:
+                    contig = read.reference_name
+                if contig == read.reference_name:
+
+                    if start is None:
+                        start = read.reference_start
+                    else:
+                        start = min(start, read.reference_start)
+
+                    if end is None:
+                        end = read.reference_end
+                    else:
+                        end = max(end, read.reference_end)
+
+        self.span = (contig, start, end)
 
-        try:
-            surfaceStart, surfaceEnd = pysamiterators.iterators.getPairGenomicLocations(
-                self.get_R1(),
-                self.get_R2(),
-                R1PrimerLength=self.R1_primer_length,
-                R2PrimerLength=self.R2_primer_length,
-                allow_unsafe=True
-            )
-            self.span = (contig, surfaceStart, surfaceEnd)
-            self.safe_span = True
-        except Exception as e:
-
-            if self.has_R1() and not self.get_R1().is_unmapped:
-                self.span = (
-                    contig,
-                    self.get_R1().reference_start,
-                    self.get_R1().reference_end)
-            self.safe_span = False
 
     def get_span(self):
         return self.span
 
     def has_valid_span(self):
-        return not any([x is None for x in self.get_span()])
+
+        # Check if the span could be calculated:
+        defined_span = not any([x is None for x in self.get_span()])
+        if not defined_span:
+            return False
+
+        if self.max_fragment_size is not None and self.get_fragment_size()>self.max_fragment_size:
+            return False
+
+
+        return True
 
     def set_sample(self, sample=None):
         """Force sample name or obtain sample name from associated reads"""
         if sample is not None:
             self.sample = sample
         else:
             for read in self.reads:
@@ -688,14 +739,16 @@
                 0 : Read 1
                 1: Read 2
                 ..
         """
         return self.reads[index]
 
     def is_valid(self):
+        if self.qcfail:
+            return False
         return self.has_valid_span()
 
     def get_strand_repr(self):
         s = self.get_strand()
         if s is None:
             return '?'
         if s:
@@ -798,14 +851,22 @@
 
 
 class SingleEndTranscript(Fragment):
     def __init__(self, reads, **kwargs):
         Fragment.__init__(self, reads, **kwargs)
 
 
+        self.match_hash = (
+            self.sample,
+            self.strand,
+            reads[1].reference_end if self.strand else reads[1].reference_start,
+            )
+
+
+
 class FeatureCountsSingleEndFragment(Fragment):
     """ Class for fragments annotated with featureCounts
 
     Extracts annotated gene from the XT tag.
     Deduplicates using XT tag and UMI
     Reads without XT tag are flagged as invalid
 
@@ -813,23 +874,24 @@
 
     def __init__(self,
                  reads,
                  R1_primer_length=4,
                  R2_primer_length=6,
                  assignment_radius=100_000,
                  umi_hamming_distance=1,
-                 invert_strand=False
+                 invert_strand=False,
+                 **kwargs
                  ):
 
         Fragment.__init__(self,
                           reads,
                           assignment_radius=assignment_radius,
                           R1_primer_length=R1_primer_length,
                           R2_primer_length=R2_primer_length,
-                          umi_hamming_distance=umi_hamming_distance)
+                          umi_hamming_distance=umi_hamming_distance,**kwargs)
 
         self.strand = None
         self.gene = None
         self.identify_gene()
 
         if self.is_valid():
             self.match_hash = (self.strand, self.gene, self.sample)
@@ -853,14 +915,78 @@
         for read in self.reads:
             if read is not None and read.has_tag('XT'):
                 self.gene = read.get_tag('XT')
                 self.valid = True
                 return self.gene
 
 
+
+class FeatureCountsFullLengthFragment(FeatureCountsSingleEndFragment):
+    """ Class for fragments annotated with featureCounts, with multiple reads covering a gene
+
+    Extracts annotated gene from the XT tag.
+    Deduplicates using XT tag and UMI
+    Reads without XT tag are flagged as invalid
+
+    """
+
+    def __init__(self,
+                 reads,
+                 R1_primer_length=4,
+                 R2_primer_length=6,
+                 assignment_radius=10_000,
+                 umi_hamming_distance=1,
+                 invert_strand=False,
+                 **kwargs
+                 ):
+
+        FeatureCountsSingleEndFragment.__init__(self,
+                          reads,
+                          assignment_radius=assignment_radius,
+                          R1_primer_length=R1_primer_length,
+                          R2_primer_length=R2_primer_length,
+                          umi_hamming_distance=umi_hamming_distance,
+                          **kwargs
+
+                          )
+
+    def __eq__(self, other):
+        # Make sure fragments map to the same strand, cheap comparisons
+        if self.match_hash != other.match_hash:
+            return False
+
+        #Calculate distance
+        if min(abs(self.span[1] -
+                   other.span[1]), abs(self.span[2] -
+                                       other.span[2])) > self.assignment_radius:
+            return False
+
+        # Make sure UMI's are similar enough, more expensive hamming distance
+        # calculation
+        return self.umi_eq(other)
+
+
+class FragmentWithoutPosition(Fragment):
+    """ Fragment without a specific location on a contig"""
+    def get_site_location(self):
+        if self.has_valid_span():
+            return self.span[0], 0
+        else:
+            return '*', 0
+
+class FragmentStartPosition(Fragment):
+    """ Fragment without a specific location on a contig"""
+    def get_site_location(self):
+        for read in self:
+            if read is not None and not read.is_unmapped:
+                return read.reference_name, read.reference_start
+        return None
+
+
+
 class FragmentWithoutUMI(Fragment):
     """
     Use this class when no UMI information is available
     """
 
     def __init__(self, reads, **kwargs):
         Fragment.__init__(self, reads, **kwargs)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/libraryDetection/sequencingLibraryListing.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/libraryDetection/sequencingLibraryListing.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/libraryProcessing/libraryStatistics.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/libraryProcessing/libraryStatistics.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,34 +5,38 @@
 import matplotlib.pyplot as plt
 import os
 import sys
 import pysam
 import collections
 import argparse
 
+from singlecellmultiomics.bamProcessing import bam_is_processed_by_program
+
 from colorama import Fore
 from colorama import Back
 from colorama import Style
 import singlecellmultiomics.pyutils as pyutils
 from singlecellmultiomics.tagtools import tagtools
 import pysamiterators.iterators as pysamIterators
 import gzip
 import pickle
 import subprocess
+from glob import glob
 
 import matplotlib
 matplotlib.rcParams['figure.dpi'] = 160
 matplotlib.use('Agg')
 
 
 def select_bam_file(lookup):
     for l in lookup:
-        print(f'Found file at {l}')
         if os.path.exists(l):
+            print(f'Found file at {l}')
             return l
+
     return None
 
 
 def select_fastq_file(lookup):
     for paths in lookup:
         if isinstance(paths, tuple):
             for path in paths:
@@ -56,43 +60,65 @@
                            help="type of staistics to produce. options are \
             'demult-stats', 'meth-stats', 'chic-stats' and 'all-stats'")
     argparser.add_argument('-o', type=str, help="output file prefix")
     argparser.add_argument(
         '--plotsOnly',
         action='store_true',
         help="only make plots")
+
+    argparser.add_argument(
+        '--sl',
+        action='store_true',
+        help="Show lookup paths")
+
+
+    argparser.add_argument(
+        '--tablesOnly',
+        action='store_true',
+        help="only make tables")
+
     argparser.add_argument('-head', type=int)
     argparser.add_argument(
         '-tagged_bam',
         type=str,
         help='Alias of subpath to tagged bam file. For example /tagged/sorted.bam')
     argparser.add_argument('--v', action='store_true')
     argparser.add_argument('--nort', action='store_true')
+    argparser.add_argument('--nolorenz', action='store_true')
     args = argparser.parse_args()
 
     for library in args.libraries:
         library_name = library
         if library.endswith('.bam'):
             # the library is a bam file..
             bamFile = os.path.abspath(library)
             library = os.path.dirname(os.path.abspath(bamFile))
             library_name = os.path.basename(os.path.abspath(bamFile))
             print("Bam file was supplied:")
             print(bamFile)
         else:
+            print("A library was supplied, automatically detecting files ..")
             bamFile = None
         rc = ReadCount(args)  # Is also mappability
 
         statistics = [
             rc,
             FragmentSizeHistogram(args),
             RejectionReasonHistogram(args),
             MappingQualityHistogram(args),
-            OversequencingHistogram(args)
+            OversequencingHistogram(args),
+            CellReadCount(args)
         ]
+
+
+        full_file_statistics = []
+
+        if not args.nolorenz:
+            full_file_statistics.append( Lorenz(args) )
+
         if(args.t in ['meth-stats', 'all-stats']):
             statistics.extend([
                 MethylationContextHistogram(args),
                 ConversionMatrix(args)
             ])
 
         if(args.t in ['chic-stats', 'all-stats']):
@@ -119,32 +145,61 @@
             (f'{library}/rejectsR1.fastq.gz', f'{library}/rejectsR2.fastq.gz'),
             (f'{library}/rejectsR1.fastq', f'{library}/rejectsR2.fastq'),
             (f'{library}/rejectsR1.fq.gz', f'{library}/rejectsR2.fq.gz'),
             (f'{library}/rejectsR1.fq', f'{library}/rejectsR2.fq'),
         ]
 
         taggedFilesLookup = [
-            f'{library}/tagged.bam'
+            f'{library}/tagged.bam',
             f'{library}/tagged/tagged.bam',
             f'{library}/tagged/marked_duplicates.bam',
             f'{library}/tagged/resorted.featureCounts.bam',
             f'{library}/tagged/STAR_mappedAligned.sortedByCoord.out.featureCounts.bam',
             f'{library}/tagged/STAR_mappedAligned.sortedByCoord.out.bam',
             f'{library}/tagged/sorted.bam']
         if args.tagged_bam:
             taggedFilesLookup = [
                 library + '/' + args.tagged_bam] + taggedFilesLookup
 
+        if args.sl:
+            print(f'{Style.BRIGHT}Demux file lookup paths{Style.RESET_ALL}')
+            print(demuxFastqFilesLookup)
+            print(f'{Style.BRIGHT}Reject fastq file lookup paths{Style.RESET_ALL}')
+            print(rejectFilesLookup)
+            print(f'{Style.BRIGHT}Tagged bam lookup paths{Style.RESET_ALL}')
+            print(taggedFilesLookup)
+
         if 'cluster' in library:
             continue
         print(f'{Style.BRIGHT}Library {library}{Style.RESET_ALL}')
         # Check if the bam file is present
         if bamFile is None:
             bamFile = select_bam_file(taggedFilesLookup)
 
+        if bamFile is None:
+            # Perform glob expansion
+            bams = list(glob(f'{library}/*.bam'))+list(glob(f'{library}/*/*.bam'))
+            for bam_path in bams:
+                print(f"Trying {bam_path}",end="\t")
+                try:
+                    with pysam.AlignmentFile(bam_path) as a:
+                        if bam_is_processed_by_program(a, program='bamtagmultiome'):
+                            bamFile = bam_path
+                            print("[TAGGED]")
+                            break
+                        else:
+                            print("[NOT TAGGED]")
+                except Exception as e:
+                    print(f"[ERROR] {e}")
+
+        if bamFile is None:
+            print(f'{Fore.RED}BAM FILE MISSING {library}{Style.RESET_ALL}')
+            exit()
+        else:
+            print(f'{Fore.GREEN}Bam file at {bamFile}{Style.RESET_ALL}')
 
         demuxFastqFiles = select_fastq_file(demuxFastqFilesLookup)
         rejectFastqFiles = select_fastq_file(rejectFilesLookup)
 
         print("Selected files:")
         print(f'demultiplexed reads: {demuxFastqFiles}')
         print(f'rejected reads: {rejectFastqFiles}')
@@ -232,54 +287,67 @@
                 print(f'\t\t{statistic}\n')
                 statDict[statistic.__class__.__name__] = dict(statistic)
                 print(dict(statistic))
             except Exception as e:
                 if args.v:
                     print(e)
 
+        if bamFile is not None:
+            for statistic in full_file_statistics:
+                try:
+                    with pysam.AlignmentFile(bamFile ) as alignments:
+                        statistic.process_file(alignments)
+                except Exception as e:
+                    if args.v:
+                        print(e)
+
+
+
         # Make plots:
         if args.o is None:
             plot_dir = f'{library}/plots'
             table_dir = f'{library}/tables'
             statFile = f'{library}/statistics.pickle.gz'
         else:
             plot_dir = args.o
             table_dir = f'{args.o}/tables'
             statFile = f'{args.o}/statistics.pickle.gz'
 
-        if not os.path.exists(plot_dir):
-            os.makedirs(plot_dir)
-        for statistic in statistics:
-            if not hasattr(statistic, 'plot'):
-                print(
-                    f'Not making a plot for {statistic.__class__.__name__} as no plot method is defined')
-                continue
-            try:
-                statistic.plot(
-                    f'{plot_dir}/{statistic.__class__.__name__}.png',
-                    title=library_name)
-            except Exception as e:
-                if args.v:
-                    import traceback
-                    traceback.print_exc()
+        if not args.tablesOnly:
+
+            if not os.path.exists(plot_dir):
+                os.makedirs(plot_dir)
+            for statistic in statistics + full_file_statistics:
+                if not hasattr(statistic, 'plot'):
+                    print(
+                        f'Not making a plot for {statistic.__class__.__name__} as no plot method is defined')
+                    continue
+                try:
+                    statistic.plot(
+                        f'{plot_dir}/{statistic.__class__.__name__}.png',
+                        title=library_name)
+                except Exception as e:
+                    if args.v:
+                        import traceback
+                        traceback.print_exc()
 
         # Make tables:
         if not args.plotsOnly:
             with gzip.open(statFile, 'wb') as f:
                 pickle.dump(statDict, f)
             if os.path.exists(statFile):
                 with gzip.open(statFile, 'rb') as f:
                     try:
                         statDict.update(pickle.load(f))
                     except Exception as e:
                         pass
 
             if not os.path.exists(table_dir):
                 os.makedirs(table_dir)
-            for statistic in statistics:
+            for statistic in statistics + full_file_statistics:
                 if not hasattr(statistic, 'to_csv'):
                     print(
                         f'Not making a table for {statistic.__class__.__name__} as to_csv method is not defined')
                     continue
                 try:
                     statistic.to_csv(
                         f'{table_dir}/{statistic.__class__.__name__}_{library_name}.csv')
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/celseq1.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/celseq1.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2_noNla.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/celseq2_noNla.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/lennart96NLA.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/lennart96NLA.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/maya_384NLA.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/maya_384NLA.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/maya_mspj1.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/maya_mspj1.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/nla_bisulfite.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/nla_bisulfite.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/scartrace.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/scartrace.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/barcodes/scartraceBarcodes.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/barcodes/scartraceBarcodes.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/baseDemultiplexMethods.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/baseDemultiplexMethods.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 
     if tag == 'chrom':
         return read.reference_name
 
     if read.has_tag(tag):
         return read.get_tag(tag)
 
+    # Backwards compatibility with BI > bi tag:
+    if tag=='BI' and read.has_tag('bi'):
+        return read.get_tag('bi')
+
+    # Forwards compatibility:
+    if tag=='bi' and read.has_tag('BI'):
+        return read.get_tag('BI')
+
     try:
         return getattr(read, tag)
     except Exception as e:
         pass
         # print(e)
 
     return None
@@ -120,15 +128,15 @@
                 raise ValueError()
             baseQualities = self.qualities
 
         header = ";".join([f"{attribute}:{value}" for attribute, value in self.tags.items(
         ) if not self.tagDefinitions[attribute].doNotWrite])
         if len(header) > 255:  # the header length is stored as uint_8 and includes a null character. The maximum length is thus 255
             raise ValueError(
-                f"The length of the demultiplexed header is longer than 255 characters. Reduce the length of the header. For example by using -merge _ which will not put the flow cell in the sample name. The header looks like this: {header}")
+                f"The length of the demultiplexed header is longer than 255 characters. Try to keep your library name below 60 characters. Reduce the length of the header. For example by using -merge _ which will not put the flow cell in the sample name. The header looks like this: {header}")
         return "@%s\n%s\n%s\n%s\n" % (
             header,
             sequence,
             dirAtt,
             baseQualities
         )
 
@@ -196,17 +204,25 @@
             'CX': clusterXpos,
             'CY': clusterYpos,
             'RP': readPairNumber,
             'Fi': isFiltered,
             'CN': controlNumber
         })
 
+
+
+
         if indexFileParser is not None and indexFileAlias is not None:
-            indexIdentifier, correctedIndex, hammingDistance = indexFileParser.getIndexCorrectedBarcodeAndHammingDistance(
-                alias=indexFileAlias, barcode=indexSequence)
+            # Check if the index is an integer:
+            try:
+                indexInteger = int(indexSequence)
+                indexIdentifier, correctedIndex, hammingDistance = indexSequence, indexSequence, 0
+            except Exception:
+                indexIdentifier, correctedIndex, hammingDistance = indexFileParser.getIndexCorrectedBarcodeAndHammingDistance(
+                    alias=indexFileAlias, barcode=indexSequence)
 
             self.addTagByTag('aa', indexSequence, isPhred=False)
             if correctedIndex is not None:
                 #
                 #self.addTagByTag('aA',correctedIndex, isPhred=False)
                 #self.addTagByTag('aI',indexIdentifier, isPhred=False)
                 self.tags.update({'aA': correctedIndex, 'aI': indexIdentifier})
@@ -268,24 +284,36 @@
 
         except NonMultiplexable:
 
             # Its bulk
             self.tags['BK'] = True
 
         # Add sample tag: (If possible)
-        # If the BI tag is present it means we know the index of the cell
-        # if no BI tag is present, assume the sample is bulk
-        if 'BI' in self.tags:
+        # If the bi tag is present it means we know the index of the cell
+        # if no bi tag is present, assume the sample is bulk
+        if 'bi' in self.tags:
+            self.addTagByTag(
+                'SM',
+                f'{self.tags["LY"]}_{self.tags["bi"]}',
+                isPhred=False)
+        elif 'BI' in self.tags:
             self.addTagByTag(
                 'SM',
                 f'{self.tags["LY"]}_{self.tags["BI"]}',
                 isPhred=False)
+
+            # Remove BI tag
+            self.tags['bi'] = self.tags["BI"]
+            del self.tags['BI']
         else:
             self.addTagByTag('SM', f'{self.tags["LY"]}_BULK', isPhred=False)
 
+
+
+
         # Now we defined the desired values of the tags. Write them to the
         # record:
         for tag, value in self.tags.items():
             # print(tag,value)
             if self.tagDefinitions[tag].isPhred:
                 value = fastqHeaderSafeQualitiesToPhred(value, method=3)
             read.set_tag(tag, value)
@@ -531,21 +559,21 @@
             else:
                 tr.addTagByTag('RX', umi, isPhred=False, make_safe=False)
                 tr.addTagByTag('RQ', umiQual, isPhred=True)
                 #tr.addTagByTag('MI', barcode+umi, isPhred=False)
                 #tr.addTagByTag('QM', barcodeQual+umiQual, isPhred=True)
 
             """ These can be updated at once
-            tr.addTagByTag('BI', barcodeIdentifier, isPhred=False)
+            tr.addTagByTag('bi', barcodeIdentifier, isPhred=False)
             tr.addTagByTag('bc', rawBarcode, isPhred=False)
             tr.addTagByTag('MX', self.shortName, isPhred=False)
             tr.addTagByTag('BC', barcode, isPhred=False )
             """
             tr.tags.update({
-                'BI': barcodeIdentifier,
+                'bi': barcodeIdentifier,
                 'bc': rawBarcode,
                 'MX': self.shortName,
                 'BC': barcode
             })
             #tr.addTagByTag('hd', hammingDistance, isPhred=False)
             if random_primer is not None:
                 tr.addTagByTag('rS',
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/BULK_ILLUMINA.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/BULK_ILLUMINA.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq1.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq1.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq2.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/CELSeq2.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,17 +20,37 @@
             barcodeFileParser=barcodeFileParser,
             **kwargs)
         self.shortName = 'CS2C8U6'
         self.longName = 'CELSeq 2, CB: 8bp, UMI: 6bp'
         self.autoDetectable = True
         self.description = 'R1 starts with a 6bp UMI  followed by a 8bp cell barcode. R2 ends with a 6bp random primer'
 
-# Reversed case:
 
+class CELSeq2_c8_u6_NH(UmiBarcodeDemuxMethod):
+    def __init__(self, barcodeFileParser, **kwargs):
+        self.barcodeFileAlias = 'celseq2'
+        UmiBarcodeDemuxMethod.__init__(
+            self,
+            umiRead=0,
+            umiStart=0,
+            umiLength=6,
+            barcodeRead=0,
+            barcodeStart=6,
+            barcodeLength=8,
+            random_primer_read=None,
+            random_primer_length=None,
+            barcodeFileAlias=self.barcodeFileAlias,
+            barcodeFileParser=barcodeFileParser,
+            **kwargs)
+        self.shortName = 'CS2C8U6NH'
+        self.longName = 'CELSeq 2, CB: 8bp, UMI: 6bp, NO random primer'
+        self.autoDetectable = False
+        self.description = 'R1 starts with a 6bp UMI  followed by a 8bp cell barcode. R2 has no random primer. Use this demultiplexing method for VASA'
 
+# Reversed case:
 class CELSeq2_c8_u6_swapped_reads(UmiBarcodeDemuxMethod):
     def __init__(self, barcodeFileParser, **kwargs):
         self.barcodeFileAlias = 'celseq2'
         UmiBarcodeDemuxMethod.__init__(
             self,
             umiRead=1,
             umiStart=0,
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/Hexamer.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/Hexamer.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/MSPJI.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/MSPJI.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/NLAIII.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/NLAIII.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/restrictionbisulfite.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/restrictionbisulfite.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             else:
                 tr.addTagByTag('RX', umi, isPhred=False, make_safe=False)
                 tr.addTagByTag('RQ', umiQual, isPhred=True)
                 #tr.addTagByTag('MI', barcode+umi, isPhred=False)
                 #tr.addTagByTag('QM', barcodeQual+umiQual, isPhred=True)
 
             tr.addTagByTag(
-                'BI',
+                'bi',
                 barcodeIdentifier,
                 isPhred=False,
                 make_safe=False)
             tr.addTagByTag('bc', rawBarcode, isPhred=False, make_safe=False)
             #tr.addTagByTag('hd', hammingDistance, isPhred=False)
 
             tr.addTagByTag('BC', barcode, isPhred=False, make_safe=False)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexModules/scartrace.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexModules/scartrace.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexedFastqConversion.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexedFastqConversion.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demultiplexingStrategyLoader.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demultiplexingStrategyLoader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,323 +1,294 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import os
-import collections
-import glob
-import sys
-from colorama import Fore
-from colorama import Back
-from colorama import Style
-import importlib
-import inspect
-import traceback
-import singlecellmultiomics.modularDemultiplexer.demultiplexModules as dm
-import singlecellmultiomics.fastqProcessing.fastqIterator as fastqIterator
-from singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods import NonMultiplexable, IlluminaBaseDemultiplexer
-import logging
-
-
-class DemultiplexingStrategyLoader:
-    def __init__(
-            self,
-            barcodeParser,
-            moduleSearchDir='demultiplexModules',
-            indexParser=None,
-            ignoreMethods=None,
-            indexFileAlias=None):
-        package = f'singlecellmultiomics.modularDemultiplexer.{moduleSearchDir}'
-        moduleSearchPath = os.path.join(
-            os.path.dirname(
-                os.path.realpath(__file__)),
-            moduleSearchDir).replace(
-            '/./',
-            '/')
-        self.barcodeParser = barcodeParser
-        self.indexParser = indexParser
-        moduleSearchPath = moduleSearchPath
-
-        #print(f'{Style.DIM}Current script location: {__file__}')
-        #print(f'Searchdir: {moduleSearchDir}')
-        #print(f'Looking for modules in {moduleSearchPath}{Style.RESET_ALL}')
-        self.demultiplexingStrategies = []
-        self.demux_classes = [
-            dm.CELSeq2_c8_u8,
-            dm.MSPJI_c8_u3,
-            dm.ScartraceR1,
-            dm.CELSeq2_c8_u8_NNLAIII,
-            dm.ScartraceR2,
-            dm.NLAIII_384w_c8_u3,
-            dm.CELSeq1_c8_u4,
-            dm.NLAIII_96w_c8_u3,
-            dm.Nla_384w_u8_c8_ad3_is15,
-            dm.CELSeq2_c8_u6,
-            IlluminaBaseDemultiplexer,
-            dm.CELSeq2_c8_u6_swapped_reads,
-            dm.SCCHIC_384w_c8_u3
-        ]
-        for c in self.demux_classes:
-            self.demultiplexingStrategies.append(c(
-                barcodeFileParser=barcodeParser,
-                indexFileParser=indexParser,
-                indexFileAlias=indexFileAlias)
-            )
-
-        """
-        for modulePath in glob.glob(f'{moduleSearchPath}/*.py'):
-            #print(f"Found {modulePath}")
-            try:
-                module = (modulePath.split('/')[-1].replace('.py',''))
-                #print(f"Module:{module}, package:{package}")
-
-                if ignoreMethods is not None and module in ignoreMethods:
-                    print(f"{Style.DIM}Ignoring demultiplex method {module}, use -ignoreMethods none to re-enable{Style.RESET_ALL}")
-                    continue
-                if module=='__init__':
-                    continue
- #modulePath.replace('\\','/').replace('/','.').replace('..','').replace('.py','').lstrip('.').split('.')[-1]
-
-                loadedModule = importlib.import_module(f'.{module}', package)
-                # Only obtain classes defined in the module, not imported ones:
-                is_class_member = lambda member: inspect.isclass(member) and member.__module__ == f'{package}.{module}'
-                for className, classDetails in inspect.getmembers(sys.modules[f'{package}.{module}'], is_class_member):
-                    # Obtain a handle to the class and instatiate the strategy
-                    if 'Base_' in className:
-                        continue
-
-                    class_ = getattr(loadedModule, className)
-                    initiatedDemultiplexingStrategy = class_( barcodeFileParser=barcodeParser, indexFileParser=indexParser,indexFileAlias=indexFileAlias)
-                    self.demultiplexingStrategies.append(initiatedDemultiplexingStrategy)
-                    #print(initiatedDemultiplexingStrategy.name)
-
-            except Exception as e:
-
-                print(f"{Fore.RED}{Style.BRIGHT}FAILED LOADING {module} at {modulePath}\nException: {e}{Style.RESET_ALL}\nTraceback for the error:\n")
-                import traceback
-                traceback.print_exc()
-
-                from os import stat
-                from pwd import getpwuid
-
-                print(f'Contact {Style.BRIGHT}%s{Style.RESET_ALL} for help\n' % getpwuid(stat(modulePath).st_uid).pw_name)
-                print('The error only affects this module.\nProceeding to load more modules...\n')
-        """
-
-    def getSelectedStrategiesFromStringList(self, strList):
-        selectedStrategies = []
-
-        resolved = {part: False for part in strList}
-        for strategy in self.demultiplexingStrategies:
-            if strategy.shortName in strList:
-                selectedStrategies.append(strategy)
-                print('Selected strategy %s' % strategy)
-                resolved[strategy.shortName] = True
-
-        if any([v is False for v in resolved.values()]):
-            for strat in strList:
-                if resolved[strat] is False:
-                    print(f'{Fore.RED}Could not resolve {strat}{Style.RESET_ALL}')
-                    print('Available:')
-                    for s in self.demultiplexingStrategies:
-                        print(s.shortName)
-                    raise ValueError(f'Strategy {strat} not found')
-
-            raise ValueError()
-        return selectedStrategies
-
-    def list(self):
-        print(f"{Style.BRIGHT}Available demultiplexing strategies:{Style.RESET_ALL}")
-        #print('Name, alias, will be auto detected, description')
-        for strategy in self.demultiplexingStrategies:
-
-            try:
-                print(
-                    f'{Style.BRIGHT}{strategy.shortName}{Style.RESET_ALL}\t{strategy.longName}\t' +
-                    (
-                        f'{Fore.GREEN}Will be autodetected' if strategy.autoDetectable else f'{Fore.RED}Will not be autodetected') +
-                    Style.RESET_ALL +
-                    Style.DIM +
-                    f' {strategy.barcodeFileParser.getTargetCount(strategy.barcodeFileAlias) if hasattr(strategy,"barcodeFileParser") else "NA"} targets\n ' +
-                    Style.DIM +
-                    strategy.description +
-                    '\n' +
-                    strategy.getParserSummary() +
-                    Style.RESET_ALL +
-                    '\n')
-            except Exception as e:
-                print(
-                    f"{Fore.RED}{Style.BRIGHT}Error in: {strategy.shortName}\nException: {e}{Style.RESET_ALL}\nTraceback for the error:\n")
-                import traceback
-                traceback.print_exc()
-                from os import stat
-                from pwd import getpwuid
-                try:
-                    modulePath = sys.modules[strategy.__module__].__file__
-
-                    print(
-                        f'Contact {Style.BRIGHT}%s{Style.RESET_ALL} for help\n' %
-                        getpwuid(
-                            stat(modulePath).st_uid).pw_name)
-                    print(
-                        'The error only affects this module.\nProceeding to load more modules...\n')
-                except Exception as e:
-                    pass
-
-    def getAutodetectStrategies(self):
-        return [
-            strategy for strategy in self.demultiplexingStrategies if strategy.autoDetectable]
-
-    def getDemultiplexingSelectedStrategies(self):
-        if self.selectedStrategies is None:
-            raise ValueError('No strategies selected')
-        return self.selectedStrategies
-
-    def demultiplex(
-            self,
-            fastqfiles,
-            maxReadPairs=None,
-            strategies=None,
-            library=None,
-            targetFile=None,
-            rejectHandle=None,
-            log_handle=None,
-            probe=None):
-
-        useStrategies = strategies if strategies is not None else self.getAutodetectStrategies()
-        strategyYields = collections.Counter()
-        processedReadPairs = 0
-        baseDemux = IlluminaBaseDemultiplexer(
-            indexFileParser=self.indexParser,
-            barcodeParser=self.barcodeParser,
-            probe=probe)
-
-        for processedReadPairs, reads in enumerate(
-                fastqIterator.FastqIterator(*fastqfiles)):
-            for strategy in useStrategies:
-                try:
-                    recodedRecords = strategy.demultiplex(
-                        reads, library=library, probe=probe)
-
-                    if targetFile is not None:
-                        targetFile.write(recodedRecords)
-
-                except NonMultiplexable as reason:
-                    # print('NonMultiplexable')
-                    if rejectHandle is not None:
-
-                        try:
-                            to_write = baseDemux.demultiplex(
-                                reads, library=library, reason=reason)
-                            rejectHandle.write(to_write)
-
-                        except NonMultiplexable as e:
-                            # we cannot read the header of the read..
-                            reads = [
-                                '\n'.join(
-                                    (read.header +
-                                     f';RR:{reason};Rr:{e}',
-                                     read.sequence,
-                                     read.plus,
-                                     read.qual)) for read in reads]
-                            rejectHandle.write(reads)
-
-                    continue
-                except Exception as e:
-                    print(traceback.format_exc())
-                    print(
-                        f'{Fore.RED}Fatal error. While demultiplexing strategy {strategy.longName} yielded an error, the error message was: {e}')
-                    print('The read(s) causing the error looked like this:')
-                    for read in reads:
-                        print(str(read))
-                    print(Style.RESET_ALL)
-                    if log_handle is not None:
-                        log_handle.write(
-                            f"Error occured using {strategy.longName}\n")
-                # print(recodedRecord)
-                strategyYields[strategy.shortName] += 1
-            if (maxReadPairs is not None and (
-                    1 + processedReadPairs) >= maxReadPairs):
-                break
-        # write yields to log file if applicable:
-        if log_handle is not None:
-            log_handle.write(f'processed {processedReadPairs+1} read pairs\n')
-            log_handle.write(f'Reads obtained per protocol\n')
-            log_handle.write(f'Strategy\tReads\n')
-            for strategy, used_reads in strategyYields.items():
-                log_handle.write(f'{strategy}\t{used_reads}\n')
-        return processedReadPairs + 1, strategyYields
-
-    def detectLibYields(
-            self,
-            libraries,
-            strategies=None,
-            testReads=100000,
-            maxAutoDetectMethods=1,
-            minAutoDetectPct=5,
-            verbose=False):
-        libYields = dict()
-
-        for lib, lanes in libraries.items():
-            for lane, readPairs in lanes.items():
-
-                for readPair in readPairs:
-                    if len(readPairs) == 1:
-                        processedReadPairs, strategyYields = self.demultiplex(
-                            [readPairs['R1'][0]], maxReadPairs=testReads, strategies=strategies, probe=True)
-                    elif len(readPairs) == 2:
-                        processedReadPairs, strategyYields = self.demultiplex(
-                            (readPairs['R1'][0], readPairs['R2'][0]), maxReadPairs=testReads, strategies=strategies, probe=True)
-                    else:
-                        raise ValueError('Error: %s' % readPairs.keys())
-
-                if verbose:
-                    print(f'Report for {lib}:')
-                    self.strategyYieldsToFormattedReport(
-                        processedReadPairs,
-                        strategyYields,
-                        maxAutoDetectMethods=maxAutoDetectMethods,
-                        minAutoDetectPct=minAutoDetectPct)
-                libYields[lib] = {
-                    'processedReadPairs': processedReadPairs,
-                    'strategyYields': strategyYields}
-                break
-        return processedReadPairs, libYields
-
-    def strategyYieldsToFormattedReport(
-            self,
-            processedReadPairs,
-            strategyYields,
-            selectedStrategies=None,
-            maxAutoDetectMethods=1,
-            minAutoDetectPct=5):
-        print(
-            f'Analysed {Style.BRIGHT}{processedReadPairs}{Style.RESET_ALL} read pairs')
-
-        if selectedStrategies is None:
-            selectedStrategies = {}
-        #selectedStrategies = self.selectedStrategiesBasedOnYield(processedReadPairs, strategyYields)
-        for i, (strategy, strategyYield) in enumerate(
-                strategyYields.most_common()):
-            yieldRatio = strategyYield / (0.001 + processedReadPairs)
-            print(
-                (
-                    Style.BRIGHT +
-                    Fore.GREEN if (
-                        (strategy in selectedStrategies) or i < maxAutoDetectMethods) else (
-                        Fore.YELLOW if yieldRatio *
-                        100 >= minAutoDetectPct else Style.DIM)) +
-                f'\t {strategy}:%.2f%%{Style.RESET_ALL}' %
-                (100.0 *
-                 yieldRatio))
-
-    def selectedStrategiesBasedOnYield(
-            self,
-            processedReadPairs,
-            strategyYields,
-            maxAutoDetectMethods=1,
-            minAutoDetectPct=0.05):
-        selectedStrategies = []
-        for strategy, strategyYield in strategyYields.most_common(
-                maxAutoDetectMethods):
-            yieldRatio = strategyYield / (0.001 + processedReadPairs) * 100.0
-            if yieldRatio >= minAutoDetectPct:
-                selectedStrategies.append(strategy)
-        return selectedStrategies
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import os
+import collections
+import glob
+import sys
+from colorama import Fore
+from colorama import Back
+from colorama import Style
+import importlib
+import inspect
+import traceback
+import singlecellmultiomics.modularDemultiplexer.demultiplexModules as dm
+import singlecellmultiomics.fastqProcessing.fastqIterator as fastqIterator
+from singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods import NonMultiplexable, IlluminaBaseDemultiplexer
+import logging
+
+
+class DemultiplexingStrategyLoader:
+    def __init__(
+            self,
+            barcodeParser,
+            moduleSearchDir='demultiplexModules',
+            indexParser=None,
+            ignoreMethods=None,
+            indexFileAlias=None):
+        package = f'singlecellmultiomics.modularDemultiplexer.{moduleSearchDir}'
+        moduleSearchPath = os.path.join(
+            os.path.dirname(
+                os.path.realpath(__file__)),
+            moduleSearchDir).replace(
+            '/./',
+            '/')
+        self.barcodeParser = barcodeParser
+        self.indexParser = indexParser
+        moduleSearchPath = moduleSearchPath
+
+        #print(f'{Style.DIM}Current script location: {__file__}')
+        #print(f'Searchdir: {moduleSearchDir}')
+        #print(f'Looking for modules in {moduleSearchPath}{Style.RESET_ALL}')
+        self.demultiplexingStrategies = []
+        self.demux_classes = [
+            IlluminaBaseDemultiplexer,
+
+            dm.CELSeq1_c8_u4,
+            dm.CELSeq2_c8_u6,
+            dm.CELSeq2_c8_u6_NH,
+            dm.CELSeq2_c8_u8,
+            dm.CELSeq2_c8_u8_NNLAIII,
+            dm.CELSeq2_c8_u6_swapped_reads,
+
+            dm.NLAIII_384w_c8_u3,
+            dm.NLAIII_96w_c8_u3,
+            dm.Nla_384w_u8_c8_ad3_is15,
+
+            dm.SCCHIC_384w_c8_u3,
+            dm.SCCHIC_384w_c8_u3_cs2,
+            dm.SCCHIC_384w_c8_u3_pdt,
+            dm.MSPJI_c8_u3,
+            dm.ScartraceR2,
+            dm.ScartraceR1
+
+        ]
+        for c in self.demux_classes:
+            self.demultiplexingStrategies.append(c(
+                barcodeFileParser=barcodeParser,
+                indexFileParser=indexParser,
+                indexFileAlias=indexFileAlias)
+            )
+
+
+    def getSelectedStrategiesFromStringList(self, strList, verbose=True):
+        selectedStrategies = []
+
+        resolved = {part: False for part in strList}
+        for strategy in self.demultiplexingStrategies:
+            if strategy.shortName in strList:
+                selectedStrategies.append(strategy)
+                if verbose:
+                    print('Selected strategy %s' % strategy)
+                resolved[strategy.shortName] = True
+
+        if any([v is False for v in resolved.values()]):
+            for strat in strList:
+                if resolved[strat] is False:
+                    print(f'{Fore.RED}Could not resolve {strat}{Style.RESET_ALL}')
+                    print('Available:')
+                    for s in self.demultiplexingStrategies:
+                        print(s.shortName)
+                    raise ValueError(f'Strategy {strat} not found')
+
+            raise ValueError()
+        return selectedStrategies
+
+    def list(self):
+        print(f"{Style.BRIGHT}Available demultiplexing strategies:{Style.RESET_ALL}")
+        #print('Name, alias, will be auto detected, description')
+        for strategy in self.demultiplexingStrategies:
+
+            try:
+                print(
+                    f'{Style.BRIGHT}{strategy.shortName}{Style.RESET_ALL}\t{strategy.longName}\t' +
+                    (
+                        f'{Fore.GREEN}Will be autodetected' if strategy.autoDetectable else f'{Fore.RED}Will not be autodetected') +
+                    Style.RESET_ALL +
+                    Style.DIM +
+                    f' {strategy.barcodeFileParser.getTargetCount(strategy.barcodeFileAlias) if hasattr(strategy,"barcodeFileParser") else "NA"} targets\n ' +
+                    Style.DIM +
+                    strategy.description +
+                    '\n' +
+                    strategy.getParserSummary() +
+                    Style.RESET_ALL +
+                    '\n')
+            except Exception as e:
+                print(
+                    f"{Fore.RED}{Style.BRIGHT}Error in: {strategy.shortName}\nException: {e}{Style.RESET_ALL}\nTraceback for the error:\n")
+                import traceback
+                traceback.print_exc()
+                from os import stat
+                from pwd import getpwuid
+                try:
+                    modulePath = sys.modules[strategy.__module__].__file__
+
+                    print(
+                        f'Contact {Style.BRIGHT}%s{Style.RESET_ALL} for help\n' %
+                        getpwuid(
+                            stat(modulePath).st_uid).pw_name)
+                    print(
+                        'The error only affects this module.\nProceeding to load more modules...\n')
+                except Exception as e:
+                    pass
+
+    def getAutodetectStrategies(self):
+        return [
+            strategy for strategy in self.demultiplexingStrategies if strategy.autoDetectable]
+
+    def getDemultiplexingSelectedStrategies(self):
+        if self.selectedStrategies is None:
+            raise ValueError('No strategies selected')
+        return self.selectedStrategies
+
+    def demultiplex(
+            self,
+            fastqfiles,
+            maxReadPairs=None,
+            strategies=None,
+            library=None,
+            targetFile=None,
+            rejectHandle=None,
+            log_handle=None,
+            probe=None):
+
+        useStrategies = strategies if strategies is not None else self.getAutodetectStrategies()
+        strategyYields = collections.Counter()
+        processedReadPairs = 0
+        baseDemux = IlluminaBaseDemultiplexer(
+            indexFileParser=self.indexParser,
+            barcodeParser=self.barcodeParser,
+            probe=probe)
+
+        for p, reads in enumerate(
+                fastqIterator.FastqIterator(*fastqfiles)):
+            processedReadPairs = p+1
+
+            for strategy in useStrategies:
+                try:
+                    recodedRecords = strategy.demultiplex(
+                        reads, library=library, probe=probe)
+
+                    if targetFile is not None:
+                        targetFile.write(recodedRecords)
+
+                except NonMultiplexable as reason:
+                    # print('NonMultiplexable')
+                    if rejectHandle is not None:
+
+                        try:
+                            to_write = baseDemux.demultiplex(
+                                reads, library=library, reason=reason)
+                            rejectHandle.write(to_write)
+
+                        except NonMultiplexable as e:
+                            # we cannot read the header of the read..
+                            reads = [
+                                '\n'.join(
+                                    (read.header +
+                                     f';RR:{reason};Rr:{e}',
+                                     read.sequence,
+                                     read.plus,
+                                     read.qual)) for read in reads]
+                            rejectHandle.write(reads)
+
+                    continue
+                except Exception as e:
+                    print(traceback.format_exc())
+                    print(
+                        f'{Fore.RED}Fatal error. While demultiplexing strategy {strategy.longName} yielded an error, the error message was: {e}')
+                    print('The read(s) causing the error looked like this:')
+                    for read in reads:
+                        print(str(read))
+                    print(Style.RESET_ALL)
+                    if log_handle is not None:
+                        log_handle.write(
+                            f"Error occured using {strategy.longName}\n")
+                # print(recodedRecord)
+                strategyYields[strategy.shortName] += 1
+            if (maxReadPairs is not None and (
+                    processedReadPairs) >= maxReadPairs):
+                break
+        # write yields to log file if applicable:
+        if log_handle is not None:
+            log_handle.write(f'processed {processedReadPairs+1} read pairs\n')
+            log_handle.write(f'Reads obtained per protocol\n')
+            log_handle.write(f'Strategy\tReads\n')
+            for strategy, used_reads in strategyYields.items():
+                log_handle.write(f'{strategy}\t{used_reads}\n')
+        return processedReadPairs, strategyYields
+
+    def detectLibYields(
+            self,
+            libraries,
+            strategies=None,
+            testReads=100000,
+            maxAutoDetectMethods=1,
+            minAutoDetectPct=5,
+            verbose=False):
+        libYields = dict()
+
+        for lib, lanes in libraries.items():
+            for lane, readPairs in lanes.items():
+
+                for readPair in readPairs:
+                    if len(readPairs) == 1:
+                        processedReadPairs, strategyYields = self.demultiplex(
+                            [readPairs['R1'][0]], maxReadPairs=testReads, strategies=strategies, probe=True)
+                    elif len(readPairs) == 2:
+                        processedReadPairs, strategyYields = self.demultiplex(
+                            (readPairs['R1'][0], readPairs['R2'][0]), maxReadPairs=testReads, strategies=strategies, probe=True)
+                    else:
+                        raise ValueError('Error: %s' % readPairs.keys())
+
+                if verbose:
+                    print(f'Report for {lib}:')
+                    self.strategyYieldsToFormattedReport(
+                        processedReadPairs,
+                        strategyYields,
+                        maxAutoDetectMethods=maxAutoDetectMethods,
+                        minAutoDetectPct=minAutoDetectPct)
+                libYields[lib] = {
+                    'processedReadPairs': processedReadPairs,
+                    'strategyYields': strategyYields}
+                break
+        return processedReadPairs, libYields
+
+    def strategyYieldsToFormattedReport(
+            self,
+            processedReadPairs,
+            strategyYields,
+            selectedStrategies=None,
+            maxAutoDetectMethods=1,
+            minAutoDetectPct=5):
+        print(
+            f'Analysed {Style.BRIGHT}{processedReadPairs}{Style.RESET_ALL} read pairs')
+
+        if selectedStrategies is None:
+            selectedStrategies = {}
+        #selectedStrategies = self.selectedStrategiesBasedOnYield(processedReadPairs, strategyYields)
+        for i, (strategy, strategyYield) in enumerate(
+                strategyYields.most_common()):
+            yieldRatio = strategyYield / (0.001 + processedReadPairs)
+            print(
+                (
+                    Style.BRIGHT +
+                    Fore.GREEN if (
+                        (strategy in selectedStrategies) or i < maxAutoDetectMethods) else (
+                        Fore.YELLOW if yieldRatio *
+                        100 >= minAutoDetectPct else Style.DIM)) +
+                f'\t {strategy}:%.2f%%{Style.RESET_ALL}' %
+                (100.0 *
+                 yieldRatio))
+
+    def selectedStrategiesBasedOnYield(
+            self,
+            processedReadPairs,
+            strategyYields,
+            maxAutoDetectMethods=1,
+            minAutoDetectPct=0.05):
+        selectedStrategies = []
+        for strategy, strategyYield in strategyYields.most_common(
+                maxAutoDetectMethods):
+            yieldRatio = strategyYield / (0.001 + processedReadPairs) * 100.0
+            if yieldRatio >= minAutoDetectPct:
+                selectedStrategies.append(strategy)
+        return selectedStrategies
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/demux.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/demux.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 from colorama import init
 from singlecellmultiomics.modularDemultiplexer.demultiplexingStrategyLoader import DemultiplexingStrategyLoader
 import singlecellmultiomics.libraryDetection.sequencingLibraryListing as sequencingLibraryListing
 import singlecellmultiomics.barcodeFileParser.barcodeFileParser as barcodeFileParser
 from singlecellmultiomics.fastqProcessing.fastqHandle import FastqHandle
 import argparse
 from colorama import Style
-from colorama import Back
 from colorama import Fore
-import gzip
-import re
 import sys
 import os
 f"!!! PLEASE USE PYTHON 3.6 OR HIGHER !!!"
 
 if __name__ == '__main__':
 
     # Location of this script
@@ -313,15 +310,15 @@
                 args.use.split(','))
 
         print(f'Library {library} will be demultiplexed using:')
         for stra in selectedStrategies:
             print(f'\t{Fore.GREEN}{str(stra)}{Style.RESET_ALL}')
         if len(selectedStrategies) == 0:
             print(
-                f'{Fore.RED}NONE! The library will not be demultiplexed!{Style.RESET_ALL}')
+                f'{Fore.RED}NONE! The library will not be demultiplexed! The used barcodes could not be detected automatically. Please supply the desired method using the -use flag or increase the -dsize parameter to use more reads for detecting the library type.{Style.RESET_ALL}')
 
         if not args.y:
             print(f"\n{Style.BRIGHT}--y not supplied, execute the command below to run demultiplexing on the cluster:{Style.RESET_ALL}")
             arguments = " ".join(
                 [x for x in sys.argv if x != '--dry' and '--y' not in x and '-submit' not in x and '.fastq' not in x and '.fq' not in x]) + " --y"
 
             submit_in_chunks = (not args.scsepf and not args.nochunk)
@@ -338,53 +335,56 @@
 
                 if submit_in_chunks:
                     job_name = f'DMX_{library}_{group_id}'
                     submitted_jobs.append(job_name)
 
                     print(
                         'submission.py' +
-                        f' -y --py36 -time 50 -t 1 -m 8 -N {job_name} "%s  -g {group_id} -use {",".join([x.shortName for x in selectedStrategies])}"\n' %
+                        f' -y -sched auto --py36 -time 50 -t 1 -m 8 -N {job_name} "%s  -g {group_id} -use {",".join([x.shortName for x in selectedStrategies])}"\n' %
                         ('%s %s' %
                          (arguments,
                           " ".join(files_to_submit))))
                 group_id += 1
 
             final_jobs = []
             if not submit_in_chunks:
                 job_name = f'DMX_{library}'
                 print(
                     'submission.py' +
-                    f' -y --py36 -time 50 -t 1 -m 8 -N {job_name} "%s -use {",".join([x.shortName for x in selectedStrategies])}"\n' %
+                    f' -y --py36 -time 50 -t 1 -m 8 -sched auto -N {job_name} "%s -use {",".join([x.shortName for x in selectedStrategies])}"\n' %
                     ('%s %s' %
                      (arguments,
                       " ".join(filesForLib))))
                 final_jobs.append(job_name)
             else:
                 # we need a job which glues everything back together
                 # f'{args.o}/{library}/{prefix}demultiplexed
                 # f'{args.o}/{library}/{prefix}rejects
                 cmds = [
                     f'cat {args.o}/{library}/*_TEMP_demultiplexedR1.fastq.gz  > {args.o}/{library}/demultiplexedR1.fastq.gz && rm {args.o}/{library}/*_TEMP_demultiplexedR1.fastq.gz',
                     f'cat {args.o}/{library}/*_TEMP_demultiplexedR2.fastq.gz  > {args.o}/{library}/demultiplexedR2.fastq.gz && rm {args.o}/{library}/*_TEMP_demultiplexedR2.fastq.gz',
-                    f'cat {args.o}/{library}/*_TEMP_rejectsR1.fastq.gz  > {args.o}/{library}/rejectsR1.fastq.gz && rm {args.o}/{library}/*_TEMP_rejectsR1.fastq.gz',
-                    f'cat {args.o}/{library}/*_TEMP_rejectsR2.fastq.gz  > {args.o}/{library}/rejectsR2.fastq.gz && rm {args.o}/{library}/*_TEMP_rejectsR2.fastq.gz',
                     f'cat {args.o}/{library}/*_TEMP_demultiplexing.log  > {args.o}/{library}/demultiplexing.log && rm {args.o}/{library}/*_TEMP_demultiplexing.log']
+                if not args.norejects:
+                    cmds += [
+                        f'cat {args.o}/{library}/*_TEMP_rejectsR1.fastq.gz  > {args.o}/{library}/rejectsR1.fastq.gz && rm {args.o}/{library}/*_TEMP_rejectsR1.fastq.gz',
+                        f'cat {args.o}/{library}/*_TEMP_rejectsR2.fastq.gz  > {args.o}/{library}/rejectsR2.fastq.gz && rm {args.o}/{library}/*_TEMP_rejectsR2.fastq.gz'
+                    ]
 
                 for i, cmd in enumerate(cmds):
                     job_name = f'glue_{library}_{i}'
                     print(
                         'submission.py' +
-                        f' -y --silent --py36 -time 4 -t 1 -m 2 -N "glue_{library}" "{cmd}" -hold {",".join(submitted_jobs)}')
+                        f' -y -sched auto --silent --py36 -time 4 -t 1 -m 2 -N "glue_{library}" "{cmd}" -hold {",".join(submitted_jobs)}')
                     final_jobs.append(job_name)
 
             # Execute last command if applicable
             if args.nextcmd is not None:
                 print(
                     'submission.py' +
-                    f' -y --silent -time 1 -t 1 -m 1 -N "NEXT_{library}" "{cmd}" -hold {",".join(final_jobs)}')
+                    f' -y --silent -sched auto -time 1 -t 1 -m 1 -N "NEXT_{library}" "{cmd}" -hold {",".join(final_jobs)}')
 
         if args.y:
 
             targetDir = f'{args.o}/{library}'
             if not os.path.exists(targetDir):
                 try:
                     os.makedirs(targetDir)
@@ -393,16 +393,19 @@
 
             prefix = '' if args.g is None else f'{args.g}_TEMP_'
             handle = FastqHandle(
                 f'{args.o}/{library}/{prefix}demultiplexed',
                 True,
                 single_cell=args.scsepf,
                 maxHandles=args.fh)
-            rejectHandle = FastqHandle(
-                f'{args.o}/{library}/{prefix}rejects', True)
+            if args.norejects:
+                rejectHandle = None
+            else:
+                rejectHandle = FastqHandle(
+                    f'{args.o}/{library}/{prefix}rejects', True)
             """Set up statistic file"""
 
             log_location = os.path.abspath(
                 f'{args.o}/{library}/{prefix}demultiplexing.log')
             log_handle = open(log_location, 'w')
             log_handle.write(" ".join(sys.argv) + '\n')
             log_handle.write(
@@ -430,9 +433,10 @@
                     processedReadPairsForThisLib += processedReadPairs
                     log_handle.write(
                         f"done, processed:\t{processedReadPairsForThisLib} reads\n")
 
                     if args.n and processedReadPairsForThisLib >= args.n:
                         break
             handle.close()
-            rejectHandle.close()
+            if not args.norejects:
+                rejectHandle.close()
             log_handle.write(f'Demultiplexing finished\n')
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_ThruPlex48S_indices.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_ThruPlex48S_indices.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_TruSeq_indices.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_TruSeq_indices.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_i7_indices.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_i7_indices.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_ThruPlex48S_RP.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_ThruPlex48S_RP.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_iPCR_RP.bc` & `singlecellmultiomics-0.1.9/singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_iPCR_RP.bc`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/chic.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/scartrace.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,88 @@
 from singlecellmultiomics.molecule.molecule import Molecule
-from singlecellmultiomics.molecule.featureannotatedmolecule import FeatureAnnotatedMolecule
-import collections
+from singlecellmultiomics.utils.sequtils import phred_to_prob
+import numpy as np
 
-class CHICMolecule(Molecule):
-    """CHIC Molecule class
+class ScarTraceMolecule(Molecule):
+    """ScarTrace Molecule class
 
     Args:
         fragments (singlecellmultiomics.fragment.Fragment): Fragments to associate to the molecule
+
         **kwargs: extra args
 
     """
 
     def __init__(self, fragment,
                  **kwargs):
         Molecule.__init__(self, fragment, **kwargs)
-        self.ligation_motif = None
+
+        # Run code to obtain scar description
+        assert len(self) == 1, 'only implemented for molecules with a single associated fragment'
+
+        scarDescription = set()
+        qualities = []
+        for read in self.iter_reads():
+            if read is None:
+                continue
+            if read.is_unmapped:
+                continue
+            firstCigarOperation, firstCigarLen = read.cigartuples[0]
+            insertPos = 0
+            lastNonNoneRefPos = read.reference_start if firstCigarOperation != 4 else read.reference_start - firstCigarLen
+
+            expandedCigar = []
+            for cigarOperation, cigarLen in read.cigartuples:
+                expandedCigar += [cigarOperation] * cigarLen
+
+            for queryPos, referencePos in read.get_aligned_pairs(
+                    matches_only=False):
+                if queryPos is not None:
+                    qualities.append(phred_to_prob(read.qual[queryPos]))
+
+                if queryPos is None and referencePos is None:
+                    continue
+
+                if referencePos is not None:
+                    lastNonNoneRefPos = referencePos
+                    insertPos = 0
+                    if queryPos is not None:  # If both the reference and query match, there is not scar information
+                        continue
+
+                if queryPos is None:
+                    scarDescription.add(f'{referencePos}.D')
+                elif referencePos is None:  # insert or clip:
+                    operation = expandedCigar[queryPos]
+                    if operation == 1:
+                        if lastNonNoneRefPos is None:
+                            raise ValueError('Unsolvable :(')
+                        queryBase = read.seq[queryPos]
+                        scarDescription.add(
+                            f'{queryBase}.{insertPos+lastNonNoneRefPos}.I')
+                        insertPos += 1
+
+        scarDescription = ','.join(sorted(list(scarDescription)))
+
+        # Add average base calling quality excluding primers:
+        meanQ = np.mean(qualities) if len(qualities)>0 else 0
+        for read in self.iter_reads():
+            read.set_tag('SQ', 1 - meanQ)
+            if len(scarDescription) == 0:
+                scarDescription = 'WT'
+            #@todo when collapsing into molecule:
+            read.set_tag('SD', scarDescription)
+            #@todo when collapsing into molecule:
+        if self[0].get_R1() is not None:
+            self.set_meta('DS', self[0].get_R1().reference_start)
+            self.set_meta('RZ', 'SCAR')
+            self.set_meta('DT', 'SCAR')
+
 
     def write_tags(self):
         Molecule.write_tags(self)
 
-    def is_valid(self, set_rejection_reasons=False):
-
-        try:
-            chrom, start, strand = self.get_cut_site()
-        except Exception as e:
-            if set_rejection_reasons:
-                self.set_rejection_reason(f'no_cut_site_found')
+    def is_valid(self, set_rejection_reasons=False, reference=None):
+        if not any( fragment.is_valid() for fragment in self ):
+            self.set_rejection_reason('all_fragments_rejected')
             return False
 
         return True
-
-    def get_fragment_span_sequence(self, reference=None):
-        """Obtain the sequence between the start and end of the molecule
-        Args:
-            reference(pysam.FastaFile) : reference  to use.
-                If not specified self.reference is used
-        Returns:
-            sequence (str)
-        """
-        if reference is None:
-            if self.reference is None:
-                raise ValueError('Please supply a reference (PySAM.FastaFile)')
-        reference = self.reference
-        return reference.fetch(
-            self.chromosome,
-            self.spanStart,
-            self.spanEnd).upper()
-
-    def __finalise__(self):
-        # Obtain ligation motif(s)
-        self.update_ligation_motif()
-        Molecule.__finalise__(self)
-
-    def update_ligation_motif(self):
-        """
-        Extract lh tag from associated reads and set most common one to the RZ tag
-        """
-        ligation_motif_counts = collections.Counter()
-        for fragment in self:
-            if fragment.ligation_motif is not None:
-                ligation_motif_counts[fragment.ligation_motif]+=1
-        if len(ligation_motif_counts)>0:
-            self.ligation_motif = ligation_motif_counts.most_common(1)[0][0]
-            self.set_meta('RZ', self.ligation_motif)
-
-
-class AnnotatedCHICMolecule(FeatureAnnotatedMolecule, CHICMolecule):
-    """Chic Molecule which is annotated with features (genes/exons/introns, .. )
-
-    Args:
-        fragments (singlecellmultiomics.fragment.Fragment): Fragments to associate to the molecule
-        features (singlecellmultiomics.features.FeatureContainer) : container to use to obtain features from
-        **kwargs: extra args
-
-    """
-
-    def write_tags(self):
-        CHICMolecule.write_tags(self)
-        FeatureAnnotatedMolecule.write_tags(self)
-
-    def __init__(self, fragment, features, **kwargs):
-        FeatureAnnotatedMolecule.__init__(self, fragment, features, **kwargs)
-        CHICMolecule.__init__(self, fragment, **kwargs)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/consensus_model/nla_140bp_pe_juan_1M.pickle` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/consensus_model/nla_140bp_pe_juan_1M.pickle`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/featureannotatedmolecule.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/featureannotatedmolecule.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,29 +9,34 @@
 
     def __init__(
             self,
             fragment,
             features,
             stranded=None,
             auto_set_intron_exon_features=False,
+            capture_locations=False,
             **kwargs):
         """
             Args:
                 fragments (singlecellmultiomics.fragment.Fragment): Fragments to associate to the molecule
                 features (singlecellmultiomics.features.FeatureContainer) : container to use to obtain features from
                 stranded : None; not stranded, False: same strand as R1, True: other strand
+                capture_locations (bool) : Store information about the locations of the aligned features
                 auto_set_intron_exon_features(bool) : obtain intron_exon_features upon initialising
                 **kwargs: extra args
 
         """
         Molecule.__init__(self, fragment, **kwargs)
         self.features = features
         self.hits = collections.defaultdict(set)  # feature -> hit_bases
         self.stranded = stranded
         self.is_annotated = False
+        self.capture_locations = capture_locations
+        if capture_locations:
+            self.feature_locations = {} #feature->locations (chrom,start,end, strand)
 
         self.junctions = set()
         self.genes = set()
         self.introns = set()
         self.exons = set()
         self.exon_hit_gene_names = set()  # readable names
         self.is_spliced = None
@@ -57,14 +62,15 @@
         # (gene, transcript) -> set( exon_id  .. )
         exon_hits = collections.defaultdict(set)
         intron_hits = collections.defaultdict(set)
 
         for hit, locations in self.hits.items():
             if not isinstance(hit, tuple):
                 continue
+
             meta = dict(list(hit))
             if 'gene_id' not in meta:
                 continue
             if meta.get('type') == 'exon':
                 if 'transcript_id' not in meta:
                     continue
                 self.genes.add(meta['gene_id'])
@@ -125,39 +131,53 @@
                 location_dict.update(meta)
                 tabulated_hits.append(location_dict)
 
         return pd.DataFrame(tabulated_hits)
 
     def write_tags(self):
         Molecule.write_tags(self)
-
+        
         if len(self.exons) > 0:
             self.set_meta('EX', ','.join(sorted([str(x) for x in self.exons])))
+        else:
+            self.set_meta('EX',None)
+
         if len(self.introns) > 0:
             self.set_meta('IN', ','.join(
                 sorted([str(x) for x in self.introns])))
+        else:
+            self.set_meta('IN',None)
+
         if len(self.genes) > 0:
             self.set_meta('GN', ','.join(sorted([str(x) for x in self.genes])))
+        else:
+            self.set_meta('GN',None)
+
         if len(self.junctions) > 0:
             self.set_meta('JN', ','.join(
                 sorted([str(x) for x in self.junctions])))
             # Is transcriptome
             self.set_meta('IT', 1)
         elif len(self.genes) > 0:
             # Maps to gene but not junction
             self.set_meta('IT', 0.5)
+            self.set_meta('JN',None)
         else:
             # Doesn't map to gene
             self.set_meta('IT', 0)
+            self.set_meta('JN', None)
+
         if self.is_spliced is True:
             self.set_meta('SP', True)
         elif self.is_spliced is False:
             self.set_meta('SP', False)
         if len(self.exon_hit_gene_names):
             self.set_meta('gn', ';'.join(list(self.exon_hit_gene_names)))
+        else:
+            self.set_meta('gn',None)
 
     def annotate(self, method=0):
         """
             Args:
                 method (int) : 0, obtain blocks and then obtain features. 1, try to obtain features for every aligned base
 
         """
@@ -173,19 +193,29 @@
                 for start, end in self.get_aligned_blocks():
                     for hit in self.features.findFeaturesBetween(
                             chromosome=self.chromosome, sampleStart=start, sampleEnd=end, strand=strand):
                         hit_start, hit_end, hit_id, hit_strand, hit_ids = hit
                         self.hits[hit_ids].add(
                             (self.chromosome, (hit_start, hit_end)))
 
+                        if self.capture_locations:
+                            if not hit_id in self.feature_locations:
+                                self.feature_locations[hit_id] = []
+                            self.feature_locations[hit_id].append( (hit_start, hit_end, hit_strand))
+
             except TypeError:
                 # This happens when no reads map
                 pass
         else:
 
             for read in self.iter_reads():
                 for q_pos, ref_pos in read.get_aligned_pairs(
                         matches_only=True, with_seq=False):
                     for hit in self.features.findFeaturesAt(
                             chromosome=read.reference_name, lookupCoordinate=ref_pos, strand=strand):
                         hit_start, hit_end, hit_id, hit_strand, hit_ids = hit
                         self.hits[hit_ids].add((read.reference_name, ref_pos))
+
+                        if self.capture_locations:
+                            if not hit_id in self.feature_locations:
+                                self.feature_locations[hit_id] = []
+                            self.feature_locations[hit_id].append( (hit_start, hit_end, hit_strand))
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/fourthiouridine.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/fourthiouridine.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/iterator.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/iterator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from singlecellmultiomics.molecule import Molecule
 from singlecellmultiomics.fragment import Fragment
+from singlecellmultiomics.utils.prefetch import initialise_dict, initialise
 from singlecellmultiomics.universalBamTagger import QueryNameFlagger
 import pysamiterators.iterators
 import collections
 import pysam
 
 
+class ReadIterator(pysamiterators.iterators.MatePairIterator):
+    def __next__(self):
+
+        try:
+            rec = next(self.iterator)
+            return tuple((rec, None))
+        except StopIteration:
+            raise
+
 class MoleculeIterator():
     """Iterate over molecules in pysam.AlignmentFile or reads from a generator or list
 
     Example:
         >>> !wget https://github.com/BuysDB/SingleCellMultiOmics/blob/master/data/mini_nla_test.bam?raw=true -O mini_nla_test.bam
         >>> !wget https://github.com/BuysDB/SingleCellMultiOmics/blob/master/data/mini_nla_test.bam.bai?raw=true -O mini_nla_test.bam.bai
         >>> import pysam
         >>> from singlecellmultiomics.molecule import NlaIIIMolecule, MoleculeIterator
-        >>> from singlecellmultiomics.fragment import NLAIIIFragment
+        >>> from singlecellmultiomics.fragment import NlaIIIFragment
         >>> import pysamiterators
         >>> alignments = pysam.AlignmentFile('mini_nla_test.bam')
         >>> for molecule in MoleculeIterator(
         >>>             alignments=alignments,
-        >>>             moleculeClass=singlecellmultiomics.molecule.NlaIIIMolecule,
-        >>>             fragmentClass=singlecellmultiomics.fragment.NLAIIIFragment,
+        >>>             molecule_class=singlecellmultiomics.molecule.NlaIIIMolecule,
+        >>>             fragment_class=singlecellmultiomics.fragment.NlaIIIFragment,
         >>>         ):
         >>>     break
         >>> molecule
         NlaIIIMolecule
         with 1 assinged fragments
         Allele :No allele assigned
             Fragment:
@@ -109,97 +119,136 @@
                     umi:CAT
                     span:chr1 100-105
                     strand:+
                     has R1: yes
                     has R2: no
                     randomer trimmed: no
 
+
+    In the next example the molecules overlapping with a single location on chromosome `'1'` position `420000` are extracted
+    Don't forget to supply `check_eject_every = None`, this allows non-sorted data to be passed to the MoleculeIterator.
+
+    Example:
+
+        >>> from singlecellmultiomics.bamProcessing import mate_pileup
+        >>> from singlecellmultiomics.molecule import MoleculeIterator
+        >>> with pysam.AlignmentFile('example.bam') as alignments:
+        >>>     for molecule in MoleculeIterator(
+        >>>         mate_pileup(alignments, contig='1', position=420000, check_eject_every=None)
+        >>>     ):
+        >>>         pass
+
+
     Warning:
-        Always make sure the reads being supplied to the MoleculeIterator sorted by genomic coordinate!
+        Make sure the reads being supplied to the MoleculeIterator sorted by genomic coordinate! If the reads are not sorted set `check_eject_every=None`
     """
 
-    def __init__(self, alignments, moleculeClass=Molecule,
-                 fragmentClass=Fragment,
+    def __init__(self, alignments, molecule_class=Molecule,
+                 fragment_class=Fragment,
                  check_eject_every=10_000,  # bigger sizes are very speed benificial
-
                  molecule_class_args={},  # because the relative amount of molecules
                  # which can be ejected will be much higher
                  fragment_class_args={},
                  perform_qflag=True,
                  pooling_method=1,
                  yield_invalid=False,
-                 queryNameFlagger=None,
+                 yield_overflow=True,
+                 query_name_flagger=None,
                  every_fragment_as_molecule=False,
+                 yield_secondary =  False,
+                 yield_supplementary= False,
+                 max_buffer_size=None,  #Limit the amount of stored reads, when this value is exceeded, a MemoryError is thrown
+                 iterator_class = pysamiterators.iterators.MatePairIterator,
+                 skip_contigs=None,
+                 progress_callback_function=None,
+                 min_mapping_qual = None,
+
                  **pysamArgs):
         """Iterate over molecules in pysam.AlignmentFile
 
         Args:
             alignments (pysam.AlignmentFile) or iterable yielding tuples: Alignments to extract molecules from
 
-            moleculeClass (pysam.FastaFile): Class to use for molecules.
+            molecule_class (pysam.FastaFile): Class to use for molecules.
 
-            fragmentClass (pysam.FastaFile): Class to use for fragments.
+            fragment_class (pysam.FastaFile): Class to use for fragments.
 
-            check_eject_every (int): Check for yielding every N reads.
+            check_eject_every (int): Check for yielding every N reads. When None is supplied, all reads are kept into memory making coordinate sorted data not required.
 
-            molecule_class_args (dict): arguments to pass to moleculeClass.
+            molecule_class_args (dict): arguments to pass to molecule_class.
 
-            fragment_class_args (dict): arguments to pass to fragmentClass.
+            fragment_class_args (dict): arguments to pass to fragment_class.
 
             perform_qflag (bool):  Make sure the sample/umi etc tags are copied
                 from the read name into bam tags
 
             pooling_method(int) : 0: no  pooling, 1: only compare molecules with the same sample id and hash
 
             yield_invalid (bool) : When true all fragments which are invalid will be yielded as a molecule
 
-            queryNameFlagger(class) : class which contains the method digest(self, reads) which accepts pysam.AlignedSegments and adds at least the SM and RX tags
+            yield_overflow(bool) : When true overflow fragments are yielded as separate molecules
+
+            query_name_flagger(class) : class which contains the method digest(self, reads) which accepts pysam.AlignedSegments and adds at least the SM and RX tags
 
             every_fragment_as_molecule(bool): When set to true all valid fragments are emitted as molecule with one associated fragment, this is a way to disable deduplication.
 
+            yield_secondary (bool):  When true all secondary alignments will be yielded as a molecule
+
+            iterator_class : Class name of class which generates mate-pairs out of a pysam.AlignmentFile either (pysamIterators.MatePairIterator or pysamIterators.MatePairIteratorIncludingNonProper)
+
+            skip_contigs (set) : Contigs to skip
+
+            min_mapping_qual(int) : Dont process reads with a mapping quality lower than this value. These reads are not yielded as molecules!
+
             **kwargs: arguments to pass to the pysam.AlignmentFile.fetch function
 
         Yields:
             molecule (Molecule): Molecule
         """
-        if queryNameFlagger is None:
-            queryNameFlagger = QueryNameFlagger()
-        self.queryNameFlagger = queryNameFlagger
-
+        if query_name_flagger is None:
+            query_name_flagger = QueryNameFlagger()
+        self.query_name_flagger = query_name_flagger
+        self.skip_contigs = skip_contigs if skip_contigs is not None else set()
         self.alignments = alignments
-        self.moleculeClass = moleculeClass
-        self.fragmentClass = fragmentClass
+        self.molecule_class = molecule_class
+        self.fragment_class = fragment_class
         self.check_eject_every = check_eject_every
-        self.molecule_class_args = molecule_class_args
-        self.fragment_class_args = fragment_class_args
+        self.molecule_class_args = initialise_dict(molecule_class_args)
+        self.fragment_class_args = initialise_dict(fragment_class_args)
         self.perform_qflag = perform_qflag
         self.pysamArgs = pysamArgs
         self.matePairIterator = None
         self.pooling_method = pooling_method
         self.yield_invalid = yield_invalid
+        self.yield_overflow = yield_overflow
         self.every_fragment_as_molecule = every_fragment_as_molecule
+        self.progress_callback_function = progress_callback_function
+        self.iterator_class = iterator_class
+        self.max_buffer_size=max_buffer_size
+        self.min_mapping_qual = min_mapping_qual
+
         self._clear_cache()
 
     def _clear_cache(self):
         """Clear cache containing non yielded molecules"""
         self.waiting_fragments = 0
         self.yielded_fragments = 0
-        self.yielded_molecules = 0
+        self.deleted_fragments = 0
         self.check_ejection_iter = 0
         if self.pooling_method == 0:
             self.molecules = []
         elif self.pooling_method == 1:
             self.molecules_per_cell = collections.defaultdict(
                 list)  # {hash:[], :}
         else:
             raise NotImplementedError()
 
     def __repr__(self):
-        return f"""Molecule Iterator, generates fragments from {self.fragmentClass} into molecules based on {self.moleculeClass}.
-        Yielded {self.yielded_fragments} fragments, {self.waiting_fragments} fragments are waiting to be ejected.
+        return f"""Molecule Iterator, generates fragments from {self.fragment_class} into molecules based on {self.molecule_class}.
+        Yielded {self.yielded_fragments} fragments, {self.waiting_fragments} fragments are waiting to be ejected. {self.deleted_fragments} fragments rejected.
         {self.get_molecule_cache_size()} molecules cached.
         Mate pair iterator: {str(self.matePairIterator)}"""
 
     def get_molecule_cache_size(self):
         if self.pooling_method == 0:
             return len(self.molecules)
         elif self.pooling_method == 1:
@@ -207,85 +256,124 @@
                        cell_molecules in self.molecules_per_cell.items())
 
         else:
             raise NotImplementedError()
 
     def __iter__(self):
         if self.perform_qflag:
-            qf = self.queryNameFlagger
+            qf = self.query_name_flagger
 
         self._clear_cache()
         self.waiting_fragments = 0
         # prepare the source iterator which generates the read pairs:
         if isinstance(self.alignments, pysam.libcalignmentfile.AlignmentFile):
-            self.matePairIterator = pysamiterators.iterators.MatePairIterator(
+            self.matePairIterator = self.iterator_class(
                 self.alignments,
                 performProperPairCheck=False,
                 **self.pysamArgs)
         else:
             # If an iterable is provided use this as read source:
             self.matePairIterator = self.alignments
 
-        for reads in self.matePairIterator:
+        for iteration,reads in enumerate(self.matePairIterator):
+
+            if self.progress_callback_function is not None and iteration%500==0:
+                self.progress_callback_function(iteration, self, reads)
 
             if isinstance(reads, pysam.AlignedSegment):
                 R1 = reads
                 R2 = None
             elif len(reads) == 2:
                 R1, R2 = reads
             elif (isinstance(reads, list) or isinstance(reads, tuple)) and len(reads) == 1:
                 R1 = reads[0]
                 R2 = None
             else:
                 raise ValueError(
                     'Iterable not understood, supply either  pysam.AlignedSegment or lists of  pysam.AlignedSegment')
+
+            # skip_contigs
+            if len(self.skip_contigs)>0:
+                keep = False
+                for read in reads:
+                    if read is not None and read.reference_name not in self.skip_contigs:
+                        keep = True
+                if not keep:
+                    continue
+
+            if self.min_mapping_qual is not None:
+                keep = True
+                for read in reads:
+                    if read is not None and read.mapping_quality<self.min_mapping_qual:
+                        self.deleted_fragments+=1
+                        keep=False
+                if not keep:
+                    continue
+
             # Make sure the sample/umi etc tags are placed:
             if self.perform_qflag:
                 qf.digest([R1, R2])
 
-            fragment = self.fragmentClass([R1, R2], **self.fragment_class_args)
+            fragment = self.fragment_class([R1, R2], **self.fragment_class_args)
 
             if not fragment.is_valid():
                 if self.yield_invalid:
-                    m = self.moleculeClass(
+                    m = self.molecule_class(
                         fragment, **self.molecule_class_args)
                     m.__finalise__()
                     yield m
+                else:
+                    self.deleted_fragments+=1
                 continue
 
             if self.every_fragment_as_molecule:
-                m = self.moleculeClass(fragment, **self.molecule_class_args)
+                m = self.molecule_class(fragment, **self.molecule_class_args)
                 m.__finalise__()
                 yield m
                 continue
 
             added = False
-            if self.pooling_method == 0:
-                for molecule in self.molecules:
-                    if molecule.add_fragment(fragment, use_hash=False):
-                        added = True
-                        break
-            elif self.pooling_method == 1:
-                for molecule in self.molecules_per_cell[fragment.match_hash]:
-                    if molecule.add_fragment(fragment, use_hash=True):
-                        added = True
-                        break
+            try:
+                if self.pooling_method == 0:
+                    for molecule in self.molecules:
+                        if molecule.add_fragment(fragment, use_hash=False):
+                            added = True
+                            break
+                elif self.pooling_method == 1:
+                    for molecule in self.molecules_per_cell[fragment.match_hash]:
+                        if molecule.add_fragment(fragment, use_hash=True):
+                            added = True
+                            break
+            except OverflowError:
+                # This means the fragment does belong to a molecule, but the molecule does not accept any more fragments.
+                if self.yield_overflow:
+                    m = self.molecule_class(fragment, **self.molecule_class_args)
+                    m.set_rejection_reason('overflow')
+                    m.__finalise__()
+                    yield m
+                else:
+                    self.deleted_fragments+=1
+                continue
 
             if not added:
                 if self.pooling_method == 0:
-                    self.molecules.append(self.moleculeClass(
+                    self.molecules.append(self.molecule_class(
                         fragment, **self.molecule_class_args))
                 else:
                     self.molecules_per_cell[fragment.match_hash].append(
-                        self.moleculeClass(fragment, **self.molecule_class_args)
+                        self.molecule_class(fragment, **self.molecule_class_args)
                     )
 
             self.waiting_fragments += 1
             self.check_ejection_iter += 1
-            if self.check_ejection_iter > self.check_eject_every:
+
+            if self.max_buffer_size is not None and self.waiting_fragments>self.max_buffer_size:
+                raise MemoryError(f'max_buffer_size exceeded with {self.waiting_fragments} waiting fragments')
+
+            if self.check_eject_every is not None and self.check_ejection_iter > self.check_eject_every:
                 current_chrom, _, current_position = fragment.get_span()
                 if current_chrom is None:
                     continue
 
                 self.check_ejection_iter = 0
                 if self.pooling_method == 0:
                     to_pop = []
@@ -323,7 +411,9 @@
         else:
 
             for hash_group, molecules in self.molecules_per_cell.items():
                 for i, m in enumerate(molecules):
                     m.__finalise__()
                     yield m
         self._clear_cache()
+
+
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/molecule.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/molecule.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,88 @@
 import singlecellmultiomics.alleleTools
 import functools
 import typing
 import pysam
 import pysamiterators
 from singlecellmultiomics.utils import find_ranges, create_MD_tag
 import pandas as pd
+from uuid import uuid4
 
 
+###############
+
+# Variant validation function
+def detect_alleles(molecules,
+                   contig,
+                   position,
+                   min_cell_obs=3,
+                   base_confidence_threshold=None,
+                   classifier=None): # [ alleles]
+    """
+    Detect the alleles (variable bases) present at the selected location
+
+    Args:
+
+        molecules : generator to extract molecules from
+
+        variant_location(tuple) : (contig, position) zero based location of the location to test
+
+        min_cell_obs (int) : minimum amount of cells containing the allele to be emitted
+
+        confidence_threshold(float) : minimum confidence of concensus base-call to be taken into account
+
+        classifier (obj) : classifier used for consensus call, when no classifier is supplied a mayority vote is used
+
+    """
+    observed_alleles = collections.defaultdict(set) # cell -> { base_call , .. }
+    for molecule in molecules:
+        base_call = molecule.get_consensus_base(contig, position, classifier=classifier)
+
+        #confidence = molecule.get_mean_base_quality(*variant_location, base_call)
+        if base_call is not None:
+            observed_alleles[base_call].add(molecule.sample)
+
+    return [allele for allele, cells in observed_alleles.items() if len(cells)>=min_cell_obs]
+
+
+def get_variant_phase(molecules, contig, position, variant_base, allele_resolver, phasing_ratio_threshold=None): # (location,base) -> [( location, base, idenfifier)]
+    alleles = [ variant_base ]
+    phases = collections.defaultdict(collections.Counter) # Allele_id -> variant->obs
+    for molecule in molecules:
+        #allele_obs = molecule.get_allele(return_allele_informative_base_dict=True,allele_resolver=allele_resolver)
+        allele = list( molecule.get_allele(allele_resolver) )
+        if allele is None or len(allele)>1 or len(allele)==0:
+            continue
+        allele=allele[0]
+
+        base  = molecule.get_consensus_base(contig, position)
+        if base in alleles:
+            phases[base][allele] += 1
+        else:
+            pass
+
+
+    if len(phases[variant_base])==0:
+        raise ValueError("Phasing not established, no gSNVS available")
+
+    phased_allele_id = phases[variant_base].most_common(1)[0][0]
+
+    # Check if the phasing noise is below the threshold:
+    if phasing_ratio_threshold is not None:
+        correct = phases[variant_base].most_common(1)[0][1]
+        total = sum( phases[variant_base].values() )
+        phasing_ratio = correct/total
+        if correct/total < phasing_ratio_threshold:
+            raise ValueError(f'Phasing ratio not met. ({phasing_ratio}) < {phasing_ratio_threshold}')
+    # Check if the other allele i
+
+    return phased_allele_id
+
+###############
+
 @functools.lru_cache(maxsize=1000)
 def might_be_variant(chrom, pos, variants, ref_base=None):
     """Returns True if a variant exists at the given coordinate"""
     if ref_base == 'N':
         return False
     for record in variants.fetch(chrom, pos, pos + 1):
         return True
@@ -33,40 +105,40 @@
         primer_read=2,
         max_N_distance=0):
     rp = collections.defaultdict(list)
 
     # First add all reactions without a N in the sequence:
     for fragment in molecule:
 
-        hstart, hseq = fragment.get_random_primer_hash()
+        h_contig, hstart, hseq = fragment.get_random_primer_hash()
         if hseq is None:
             # This should really not happen with freshly demultiplexed data, it means we cannot extract the random primer sequence
             # which should be present as a tag (rP) in the record
-            rp[None, None].append(fragment)
+            rp[None, None, None].append(fragment)
         elif 'N' not in hseq:
-            rp[hstart, hseq].append(fragment)
+            rp[h_contig, hstart, hseq].append(fragment)
 
     # Try to match reactions with N with reactions without a N
     for fragment in molecule:
 
-        hstart, hseq = fragment.get_random_primer_hash()
+        h_contig, hstart, hseq = fragment.get_random_primer_hash()
         if hseq is not None and 'N' in hseq:
             # find nearest
-            for other_start, other_seq in rp:
-                if other_start != hstart:
+            for other_contig, other_start, other_seq in rp:
+                if other_contig!=h_contig or other_start != hstart:
                     continue
 
                 if hseq.count('N') > max_N_distance:
                     continue
 
                 if 'N' in other_seq:
                     continue
 
                 if hamming_distance(hseq, other_seq) == 0:
-                    rp[other_start, other_seq].append(fragment)
+                    rp[other_contig, other_start, other_seq].append(fragment)
     return rp
 
 
 class Molecule():
     """Molecule class, contains one or more associated fragments
 
     Attributes:
@@ -94,14 +166,15 @@
                  cache_size: int = 10_000,
                  reference: typing.Union[pysam.FastaFile, pysamiterators.CachedFasta] = None,
                  # When all fragments have a mappin quality below this value
                  # the is_valid method will return False,
                  min_max_mapping_quality: typing.Optional[int] = None,
                  mapability_reader: typing.Optional[singlecellmultiomics.bamProcessing.MapabilityReader] = None,
                  allele_resolver: typing.Optional[singlecellmultiomics.alleleTools.AlleleResolver] = None,
+                 max_associated_fragments=None,
                  **kwargs
 
                  ):
         """Initialise Molecule
 
         Parameters
         ----------
@@ -112,30 +185,34 @@
 
         allele_resolver :  alleleTools.AlleleResolver or None. Supply an allele resolver in order to assign an allele to the molecule
 
         mapability_reader : singlecellmultiomics.bamProcessing.MapabilityReader, supply a mapability_reader to set mapping_quality of 0 to molecules mapping to locations which are not mapping uniquely during in-silico library generation.
 
         cache_size (int): radius of molecule assignment cache
 
+        max_associated_fragments(int) : Maximum amount of fragments associated to molecule. If more fragments are added using add_fragment() they are not added anymore to the molecule
+
         """
 
         self.reference = reference
         self.fragments = []
         self.spanStart = None
         self.spanEnd = None
         self.chromosome = None
         self.cache_size = cache_size
         self.strand = None
         self.umi = None
+        self.overflow_fragments = 0
         self.umi_hamming_distance = None
         # when set, when comparing to a fragment the fragment to be added has
         # to match this hash
         self.fragment_match = None
         self.min_max_mapping_quality = min_max_mapping_quality
         self.umi_counter = collections.Counter()  # Observations of umis
+        self.max_associated_fragments = max_associated_fragments
         if fragments is not None:
             if isinstance(fragments, list):
                 for frag in fragments:
                     self.add_fragment(frag)
             else:
                 self.add_fragment(fragments)
 
@@ -191,14 +268,46 @@
                 for read in self.iter_reads():
                     read.mapping_quality = 0
         elif mapable is True:
             self.set_meta('mp', 'unique')
         else:
             self.set_meta('mp', 'unknown')
 
+    def calculate_consensus(self, consensus_model, molecular_identifier, out, **model_kwargs):
+        """
+        Create consensus read for molecule
+
+        Args:
+
+            consensus_model
+
+            molecular_identifier (str) : identier for this molecule, will be suffixed to the reference_id
+
+            out(pysam.AlingmentFile) : target bam file
+
+            **model_kwargs : arguments passed to the consensus model
+
+        """
+        try:
+            consensus_reads = self.deduplicate_to_single_CIGAR_spaced(
+                out,
+                f'c_{self.get_a_reference_id()}_{molecular_identifier}',
+                consensus_model,
+                NUC_RADIUS=model_kwargs['consensus_k_rad']
+            )
+            for consensus_read in consensus_reads:
+                consensus_read.set_tag('RG', self[0].get_read_group())
+                consensus_read.set_tag('mi', molecular_identifier)
+                out.write(consensus_read)
+
+        except Exception as e:
+
+            self.set_rejection_reason('CONSENSUS_FAILED', set_qcfail=True)
+            self.write_pysam(out)
+
     def get_a_reference_id(self):
         """
         Obtain a reference id for a random associated mapped read
         """
         for read in self.iter_reads():
             if not read.is_unmapped:
                 return read.reference_id
@@ -254,14 +363,15 @@
         cread.query_qualities = phred_score_array
         cread.is_supplementary = supplementary
         if cigarstring is not None:
             cread.cigarstring = cigarstring
         else:
             cread.cigarstring = f'{len(sequence)}M'
         cread.mapping_quality = self.get_max_mapping_qual()
+
         cread.is_reverse = self.strand
         if mdstring is not None:
             cread.set_tag('MD', mdstring)
 
         self.write_tags_to_psuedoreads((cread,))
 
         return cread
@@ -324,14 +434,58 @@
             try:
                 tags_obs[tag][value] += 1
             except TypeError:
                 # Dont count arrays for example
                 pass
         return tags_obs
 
+    def write_tags(self):
+        """ Write BAM tags to all reads associated to this molecule
+
+        This function sets the following tags:
+            - mI : most common umi
+            - DA : allele
+            - af : amount of associated fragments
+            - rt : rt_reaction_index
+            - rd : rt_duplicate_index
+            - TR : Total RT reactions
+            - ap : phasing information (if allele_resolver is set)
+            - TF : total fragments
+        """
+        self.is_valid(set_rejection_reasons=True)
+        if self.umi is not None:
+            self.set_meta('mI', self.umi)
+        if self.allele is not None:
+            self.set_meta('DA', str(self.allele))
+
+        # Set total amount of associated fragments
+        self.set_meta('TF',len(self.fragments) + self.overflow_fragments )
+
+        # associatedFragmentCount :
+        self.set_meta('af', len(self))
+        for rc, frag in  enumerate(self):
+            frag.set_meta('RC', rc)
+            if rc>0:
+                # Set duplicate bit
+                for read in frag:
+                    if read is not None:
+                        read.is_duplicate = True
+
+        # Write RT reaction tags (rt: rt reaction index, rd rt duplicate index)
+        rt_reaction_index = None
+        for rt_reaction_index, (_, frags) in enumerate(
+                self.get_rt_reactions().items()):
+            for rt_duplicate_index, frag in enumerate(frags):
+                frag.set_meta('rt', rt_reaction_index)
+                frag.set_meta('rd', rt_duplicate_index)
+        self.set_meta('TR', 0 if (rt_reaction_index is None) else rt_reaction_index+1 )
+
+        if self.allele_resolver is not None:
+            self.write_allele_phasing_information_tag()
+
     def write_tags_to_psuedoreads(self, reads):
         """
         Write molecule information to the supplied reads as BAM tags
         """
         # write methylation tags to new reads if applicable:
         if self.methylation_call_dict is not None:
             self.set_methylation_call_tags(
@@ -346,14 +500,15 @@
                 read.set_tag('RX', self.umi)
                 bc = list(self.get_barcode_sequences())[0]
                 read.set_tag('BC', bc)
                 read.set_tag('MI', bc + self.umi)
 
             # Store total amount of RT reactions:
             read.set_tag('TR', len(self.get_rt_reactions()))
+            read.set_tag('TF', len(self.fragments) + self.overflow_fragments)
 
             if self.allele is not None:
                 read.set_tag('DA', self.allele)
 
         if self.allele_resolver is not None:
             self.write_allele_phasing_information_tag(
                 self.allele_resolver, reads=reads)
@@ -376,34 +531,37 @@
             read (pysam.AlignedSegment) : Pseudo-read containing aggregated information
         """
         # Set all associated reads to duplicate
         for read in self.iter_reads():
             read.is_duplicate = True
 
         features = self.get_base_calling_feature_matrix(reference=reference)
-        predicted_sequence = classifier.predict(features)
-        #predicted_sequence[ features[:, [ x*8 for x in range(4) ] ].sum(1)==0 ] ='N'
-        phred_scores = np.rint(-10 * np.log10(np.clip(1 - classifier.predict_proba(
-            features).max(1), 0.000000001, 0.999999999))).astype('B')
+
+        # We only use the proba:
+        base_calling_probs = classifier.predict_proba(features)
+        predicted_sequence = [ 'ACGT'[i] for i in np.argmax( base_calling_probs ,1) ]
+        phred_scores = np.rint(-10 * np.log10(np.clip(1 - base_calling_probs.max(1), 0.000000001, 0.999999999))).astype('B')
 
         read = self.get_consensus_read(
             read_name=read_name,
             target_file=target_bam,
             consensus=''.join(predicted_sequence),
             phred_scores=phred_scores)
         read.is_read1 = True
         return read
 
     def deduplicate_to_single_CIGAR_spaced(
             self,
             target_bam,
             read_name,
-            classifier,
+            classifier=None,
             max_N_span=300,
-            reference=None):
+            reference=None,
+            **feature_matrix_args
+            ):
         """
         Deduplicate all associated reads to a single pseudoread, when the span is larger than max_N_span
         the read is split up in multi-segments. Uncovered locations are spaced using N's in the CIGAR.
 
         Args:
             target_bam (pysam.AlignmentFile) : file to associate the read with
             read_name (str) : name of the pseudoread
@@ -412,28 +570,32 @@
             reads( list [ pysam.AlignedSegment ] )
 
         """
         # Set all associated reads to duplicate
         for read in self.iter_reads():
             read.is_duplicate = True
 
-        features, reference_bases, CIGAR, alignment_start, alignment_end = self.get_base_calling_feature_matrix_spaced(
-            True, reference=reference)
+        if classifier is not None:
+            features, reference_bases, CIGAR, alignment_start, alignment_end = self.get_base_calling_feature_matrix_spaced(
+                True, reference=reference, **feature_matrix_args)
 
-        predicted_sequence = classifier.predict(features)
-        reference_sequence = ''.join(
-            [base for chrom, pos, base in reference_bases])
-        #predicted_sequence[ features[:, [ x*8 for x in range(4) ] ].sum(1)==0 ] ='N'
-        predicted_sequence = ''.join(predicted_sequence)
+            base_calling_probs = classifier.predict_proba(features)
+            predicted_sequence = [ 'ACGT'[i] for i in np.argmax( base_calling_probs ,1) ]
 
-        phred_scores = np.rint(
-            -10 * np.log10(np.clip(1 - classifier.predict_proba(features).max(1),
-                                   0.000000001,
-                                   0.999999999)
-                           )).astype('B')
+
+            reference_sequence = ''.join(
+                [base for chrom, pos, base in reference_bases])
+            #predicted_sequence[ features[:, [ x*8 for x in range(4) ] ].sum(1)==0 ] ='N'
+            predicted_sequence = ''.join(predicted_sequence)
+
+            phred_scores = np.rint(
+                -10 * np.log10(np.clip(1 - base_calling_probs.max(1),
+                                       0.000000001,
+                                       0.999999999)
+                               )).astype('B')
 
         reads = []
 
         query_index_start = 0
         query_index_end = 0
         reference_position = alignment_start  # pointer to current position
         reference_start = alignment_start  # pointer to alignment start of current read
@@ -500,67 +662,126 @@
 
         # Write NH tag (the amount of records with the same query read):
         for read in reads:
             read.set_tag('NH', len(reads))
 
         return reads
 
-    def base_calling_matrix_to_df(
+
+
+    def extract_stretch_from_dict(self, base_call_dict, alignment_start, alignment_end):
+        base_calling_probs = np.array([base_call_dict.get( (self.chromosome, pos), ('N',0))[1] for pos in range(alignment_start, alignment_end)])
+        predicted_sequence = [base_call_dict.get( (self.chromosome, pos), ('N',0))[0] for pos in range(alignment_start, alignment_end)]
+        predicted_sequence = ''.join(predicted_sequence)
+        phred_scores = np.rint(
+            -10 * np.log10(np.clip(1 -base_calling_probs,
+                                   0.000000001,
+                                   0.999999999)
+                           )).astype('B')
+        return predicted_sequence,phred_scores
+
+
+    def deduplicate_majority(self, target_bam, read_name, max_N_span=300 ):
+
+        # Convert (contig, position) -> (base_call) into:
+        # (contig, position) -> (base_call, confidence)
+        base_call_dict ={
+            (contig, position): (base, 0.95) for (contig, position), base in self.get_consensus().items()
+        }
+
+        reads = self.deduplicate_to_single_CIGAR_spaced_from_dict(target_bam, read_name, base_call_dict, max_N_span=300)
+        self.write_tags_to_psuedoreads([read for read in reads if read is not None])
+        return reads
+
+
+    def deduplicate_to_single_CIGAR_spaced_from_dict(
             self,
-            x,
-            ref_info=None,
-            NUC_RADIUS=1,
-            USE_RT=True):
+            target_bam,
+            read_name,
+            base_call_dict, #(contig, position) -> (base_call, confidence)
+            max_N_span=300,
+            ):
         """
-        Convert numpy base calling feature matrix to pandas dataframe with annotated columns
+        Deduplicate all associated reads to a single pseudoread, when the span is larger than max_N_span
+        the read is split up in multi-segments. Uncovered locations are spaced using N's in the CIGAR.
 
         Args:
-            x(np.array) : feature matrix
-            ref_info(list) : reference position annotations (will be used as index)
-            NUC_RADIUS(int) : generate kmer features target nucleotide
-            USE_RT(bool) : use RT reaction features
-
+            target_bam (pysam.AlignmentFile) : file to associate the read with
+            read_name (str) : name of the pseudoread
+            classifier (sklearn classifier) : classifier for consensus prediction
         Returns:
-            df (pd.DataFrame)
+            reads( list [ pysam.AlignedSegment ] )
+
         """
-        df = pd.DataFrame(x)
-        # annotate the columns
-        BASE_COUNT = 5
-        RT_INDEX = 7 if USE_RT else None
-        STRAND_INDEX = 0
-        PHRED_INDEX = 1
-        RC_INDEX = 2
-        MATE_INDEX = 3
-        CYCLE_INDEX = 4
-        MQ_INDEX = 5
-        FS_INDEX = 6
-        COLUMN_OFFSET = 0
-        features_per_block = 8 - (not USE_RT)
-
-        block_header = ["?"] * features_per_block
-        block_header[STRAND_INDEX] = 'strand'
-        block_header[PHRED_INDEX] = 'phred'
-        block_header[RC_INDEX] = 'read_count'
-        block_header[MATE_INDEX] = 'mate'
-        block_header[CYCLE_INDEX] = 'cycle'
-        block_header[MQ_INDEX] = 'mq'
-        block_header[FS_INDEX] = 'fragment_size'
-        block_header[RT_INDEX] = 'rt_reactions'
-        k_header = []
-        for k in range(NUC_RADIUS * 2 + 1):
-            for base in 'ACGTN':
-                k_header += [(k, b, base) for b in block_header]
+        # Set all associated reads to duplicate
+        for read in self.iter_reads():
+            read.is_duplicate = True
 
-        try:
-            df.columns = pd.MultiIndex.from_tuples(k_header)
-        except ValueError:  # the dataframe is a concateenation of multiple molecules
-            pass
-        if ref_info is not None:
-            df.index = pd.MultiIndex.from_tuples(ref_info)
-        return df
+        CIGAR, alignment_start, alignment_end = self.get_CIGAR()
+
+        reads = []
+
+        query_index_start = 0
+        query_index_end = 0
+        reference_position = alignment_start  # pointer to current position
+        reference_start = alignment_start  # pointer to alignment start of current read
+        supplementary = False
+        partial_CIGAR = []
+        partial_MD = []
+
+
+        for operation, amount in CIGAR:
+
+            if operation == 'N':
+                # Consume reference:
+                reference_position += amount
+
+            if operation == 'M':  # Consume query and reference
+                query_index_end += amount
+                reference_start = reference_position
+                reference_position += amount
+                reference_end = reference_position
+
+                partial_CIGAR.append(f'{amount}{operation}')
+
+                predicted_sequence, phred_scores = self.extract_stretch_from_dict( base_call_dict, reference_start, reference_end  ) #[start .. end)
+
+                consensus_read = self.get_consensus_read(
+                    read_name=read_name,
+                    target_file=target_bam,
+                    consensus=predicted_sequence,
+                    phred_scores=phred_scores,
+                    cigarstring=''.join(partial_CIGAR),
+                    mdstring=create_MD_tag(
+                                self.reference.fetch(self.chromosome,reference_start,reference_end),
+                                predicted_sequence
+                    ),
+                    start=reference_start,
+                    supplementary=supplementary
+                )
+                reads.append(consensus_read)
+                if not supplementary:
+                    consensus_read.is_read1 = True
+
+                supplementary = True
+                reference_start = reference_position
+                partial_CIGAR = []
+
+
+
+        # Write last index tag to last read ..
+        if supplementary:
+            reads[-1].is_read2 = True
+            reads[0].is_read1 = True
+
+        # Write NH tag (the amount of records with the same query read):
+        for read in reads:
+            read.set_tag('NH', len(reads))
+
+        return reads
 
     def get_base_calling_feature_matrix(
             self,
             return_ref_info=False,
             start=None,
             end=None,
             reference=None,
@@ -658,15 +879,15 @@
                             features[row_index][RC_INDEX + COLUMN_OFFSET +
                                                 features_per_block * block_index] += 1
 
                             # Update mate index
                             features[row_index][MATE_INDEX +
                                                 COLUMN_OFFSET +
                                                 features_per_block *
-                                                block_index] += read.is_reverse
+                                                block_index] += read.is_read2
 
                             # Update fragment sizes:
                             features[row_index][FS_INDEX +
                                                 COLUMN_OFFSET +
                                                 features_per_block *
                                                 block_index] += abs(fragment.span[1] -
                                                                     fragment.span[2])
@@ -742,14 +963,48 @@
             if return_ref_info:
                 ref_info = [
                     (self.chromosome, ref_pos, ref_bases.get(ref_pos, 'N'))
                     for ref_pos in range(origin_start, origin_end + 1)]
                 return features, ref_info
             return features
 
+
+
+    def get_CIGAR(self, reference=None):
+        """ Get alignment of all associated reads
+
+        Returns:
+            y : reference bases
+            CIGAR : alignment of feature matrix to reference tuples (operation, count)
+            reference(pysam.FastaFile) : reference to fetch reference bases from, if not supplied the MD tag is used
+        """
+
+        X = None
+
+        CIGAR = []
+        prev_end = None
+        alignment_start = None
+        alignment_end = None
+        for start, end in self.get_aligned_blocks():
+
+            if prev_end is not None:
+                CIGAR.append(('N', start - prev_end - 1))
+            CIGAR.append(('M', (end - start + 1)))
+            prev_end = end
+
+            if alignment_start is None:
+                alignment_start = start
+                alignment_end = end
+            else:
+                alignment_start = min(alignment_start, start)
+                alignment_end = max(alignment_end, end)
+
+        return CIGAR, alignment_start, alignment_end
+
+
     @functools.lru_cache(maxsize=4)
     def get_base_calling_feature_matrix_spaced(
             self,
             return_ref_info=False,
             reference=None,
             **feature_matrix_args):
         """
@@ -846,14 +1101,15 @@
         """
         if self.spanStart is not None and self.spanEnd is not None:
             return True
         return False
 
     def get_strand_repr(self, unknown='?'):
         """Get string representation of mapping strand
+
         Args:
             unknown (str) :  set what character/string to return
                              when the strand is not available
 
         Returns:
             strand_repr (str) : + forward, - reverse, ? unknown
         """
@@ -861,50 +1117,14 @@
         if s is None:
             return unknown
         if s:
             return '-'
         else:
             return '+'
 
-    def write_tags(self):
-        """ Write BAM tags to all reads associated to this molecule
-
-        This function sets the following tags:
-            - mI : most common umi
-            - DA : allele
-            - af : amount of associated fragments
-            - rt : rt_reaction_index
-            - rd : rt_duplicate_index
-            - ap : phasing information (if allele_resolver is set)
-        """
-        self.is_valid(set_rejection_reasons=True)
-        if self.umi is not None:
-            self.set_meta('mI', self.umi)
-        if self.allele is not None:
-            self.set_meta('DA', str(self.allele))
-
-        # associatedFragmentCount :
-        self.set_meta('af', len(self))
-        for rc, frag in  enumerate(self):
-            frag.set_meta('RC', rc)
-            if rc>0:
-                # Set duplicate bit
-                for read in frag:
-                    if read is not None:
-                        read.is_duplicate = True
-
-        # Write RT reaction tags (rt: rt reaction index, rd rt duplicate index)
-        for rt_reaction_index, (_, frags) in enumerate(
-                self.get_rt_reactions().items()):
-            for rt_duplicate_index, frag in enumerate(frags):
-                frag.set_meta('rt', rt_reaction_index)
-                frag.set_meta('rd', rt_duplicate_index)
-
-        if self.allele_resolver is not None:
-            self.write_allele_phasing_information_tag()
 
     def set_rejection_reason(self, reason, set_qcfail=False):
         """ Add rejection reason to all fragments associated to this molecule
 
         Args:
             reason (str) : rejection reason to set
 
@@ -1002,24 +1222,26 @@
                              window_radius=20,
                              centroid=None,
                              mask_centroid=False,
                              refence_backed=False,
                              skip_missing_reads=False
                              ):
         """ Obtain a tensor representation of the molecule alignment around the given centroid
+
         Args:
             max_reads (int) : maximum amount of reads returned in the tensor, this will be the amount of rows/4 of the returned feature matrix
 
             window_radius (int) : radius of bp around centroid
 
             centroid(int) : center of extracted window, when not specified the cut location of the molecule is used
 
             mask_centroid(bool) : when True, mask reference base at centroid with N
 
             refence_backed(bool) : when True the molecules reference is used to emit reference bases instead of the MD tag
+
         Returns:
             tensor_repr(np.array) : (4*window_radius*2*max_reads) dimensional feature matrix
         """
         reference = None
         if refence_backed:
             reference = self.reference
             if self.reference is None:
@@ -1211,19 +1433,27 @@
         """
         for fragment in self.fragments:
             if not fragment.is_multimapped:
                 return False
         return True
 
     def _add_fragment(self, fragment):
+
+        # Do not process the fragment when the max_associated_fragments threshold is exceeded
+        if self.max_associated_fragments is not None and len(self.fragments)>=(self.max_associated_fragments):
+            self.overflow_fragments += 1
+            raise OverflowError()
+
         self.match_hash = fragment.match_hash
 
         # if we already had a fragment, this fragment is a duplicate:
         if len(self.fragments) > 1:
             fragment.set_duplicate(True)
+
+
         self.fragments.append(fragment)
 
         # Update span:
         add_span = fragment.get_span()
         self.spanStart = add_span[1] if self.spanStart is None else min(
             add_span[1], self.spanStart)
         self.spanEnd = add_span[2] if self.spanEnd is None else max(
@@ -1232,49 +1462,72 @@
         self.span = (self.chromosome, self.spanStart, self.spanEnd)
         if fragment.strand is not None:
             self.strand = fragment.strand
         self.umi_counter[fragment.umi] += 1
         self.umi_hamming_distance = fragment.umi_hamming_distance
         self.saved_base_obs = None
         self.update_umi()
+        return True
 
     def get_safely_aligned_length(self):
         """Get the amount of safely aligned bases (excludes primers)
         Returns:
             aligned_bases (int) : Amount of safely aligned bases
              or None when this cannot be determined because both mates are not mapped
         """
         if self.spanStart is None or self.spanEnd is None:
             return None
-        return abs(self.spanEnd - self.spanStart)
+
+        start = None
+        end = None
+        contig = None
+        for fragment in self:
+            if contig is None:
+                contig = fragment.span[0]
+            if contig == fragment.span[0]:
+                f_start, f_end = fragment.get_safe_span()
+                if start is None:
+                    start = f_start
+                    end = f_end
+                else:
+                    start = min(f_start, start)
+                    end = min(f_end, end)
+
+        return abs(end - start)
 
     def add_fragment(self, fragment, use_hash=True):
         """Associate a fragment with this Molecule
 
         Args:
             fragment (singlecellmultiomics.fragment.Fragment) : Fragment to associate
         Returns:
             has_been_added (bool) : Returns False when the fragments which have already been associated to the molecule refuse the fragment
+
+        Raises:
+            OverflowError : when too many fragments have been associated already
+                            control this with .max_associated_fragments attribute
         """
 
         if len(self.fragments) == 0:
             self._add_fragment(fragment)
             self.sample = fragment.sample
             return True
 
         if use_hash:
             if self == fragment:
                 self._add_fragment(fragment)
                 return True
+
         else:
             for f in self.fragments:
                 if f == fragment:
                     # it matches this molecule:
                     self._add_fragment(fragment)
                     return True
+
         return False
 
     def can_be_yielded(self, chromosome, position):
         """Check if the molecule is far enough away from the supplied location to be ejected from a buffer.
 
         Args:
             chromosome (str) : chromosome / contig of location to test
@@ -1316,15 +1569,15 @@
 
         # this obtains the maximum fragment size:
         frag_chrom, frag_start, frag_end = pysamiterators.iterators.getListSpanningCoordinates(
             [v for v in itertools.chain.from_iterable(self) if v is not None])
 
         # Obtain the fragment sizes of all RT reactions:
         rt_sizes = []
-        for (rt_end, hexamer), fragments in rt_reactions.items():
+        for (rt_contig, rt_end, hexamer), fragments in rt_reactions.items():
 
             if rt_end is None:
                 continue
 
             rt_chrom, rt_start, rt_end = pysamiterators.iterators.getListSpanningCoordinates(itertools.chain.from_iterable(
                 [fragment for fragment in fragments if fragment is not None and fragment.get_random_primer_hash()[0] is not None]))
 
@@ -1337,22 +1590,28 @@
         Returns:
             mean_rt_size (float)
         """
         return np.nanmean(
             self.get_rt_reaction_fragment_sizes()
         )
 
-    def write_pysam(self, target_file):
+    def write_pysam(self, target_file, consensus=False):
         """Write all associated reads to the target file
 
         Args:
             target_file (pysam.AlignmentFile) : Target file
         """
-        for fragment in self:
-            fragment.write_pysam(target_file)
+        if consensus:
+            reads = self.deduplicate_majority(target_file,f'molecule_{uuid4()}')
+            for read in reads:
+                target_file.write(read)
+        else:
+            for fragment in self:
+                fragment.write_pysam(target_file)
+
 
     def set_methylation_call_tags(self,
                                   call_dict, bismark_call_tag='XM',
                                   total_methylated_tag='MC',
                                   total_unmethylated_tag='uC',
                                   total_methylated_CPG_tag='sZ',
                                   total_unmethylated_CPG_tag='sz',
@@ -1653,28 +1912,19 @@
         '''
 
         base_obs = collections.defaultdict(collections.Counter)
 
         used = 0  # some alignments yielded valid calls
         ignored = 0
         for fragment in self:
-            R1 = fragment.get_R1()
-            R2 = fragment.get_R2()
-            try:
-                start, end = pysamiterators.iterators.getPairGenomicLocations(
-                    R1=R1,
-                    R2=R2,
-                    allow_unsafe=(R1 is None or fragment.unsafe_trimmed))
-            except ValueError as e:
-                ignored += 1
-                continue
-            used += 1
-            for read in [R1, R2]:
+            _ ,start, end = fragment.span
+            for read in fragment:
                 if read is None:
                     continue
+
                 for cycle, query_pos, ref_pos in pysamiterators.iterators.ReadCycleIterator(
                         read, with_seq=False):
 
                     if query_pos is None or ref_pos is None or ref_pos < start or ref_pos > end:
                         continue
                     query_base = read.seq[query_pos]
                     if query_base == 'N' and not allow_N:
@@ -1682,15 +1932,17 @@
                     base_obs[(read.reference_name, ref_pos)][query_base] += 1
 
         if used == 0 and ignored > 0:
             raise ValueError('Could not extract any safe data from molecule')
 
         return base_obs
 
-    def get_base_observation_dict(self, return_refbases=False, allow_N=False):
+
+
+    def get_base_observation_dict(self, return_refbases=False, allow_N=False,allow_unsafe=True):
         '''
         Obtain observed bases at reference aligned locations
 
         Args:
             return_refbases ( bool ):
                 return both observed bases and reference bases
             allow_N (bool): Keep N base calls in observations
@@ -1710,48 +1962,55 @@
                     return self.saved_base_obs
 
         base_obs = collections.defaultdict(collections.Counter)
 
         ref_bases = {}
         used = 0  # some alignments yielded valid calls
         ignored = 0
+        error=None
         for fragment in self:
-            R1 = fragment.get_R1()
-            R2 = fragment.get_R2()
-            try:
-                start, end = pysamiterators.iterators.getPairGenomicLocations(
-                    R1=R1,
-                    R2=R2,
-                    R1PrimerLength=fragment.R1_primer_length,
-                    R2PrimerLength=fragment.R2_primer_length,
-                    allow_unsafe=(R1 is None))
-            except ValueError as e:
-                ignored += 1
-                continue
+            _, start, end = fragment.span
+
             used += 1
-            for read in [R1, R2]:
+            for read in fragment:
                 if read is None:
                     continue
-                for cycle, query_pos, ref_pos, ref_base in pysamiterators.iterators.ReadCycleIterator(
-                        read, with_seq=True, reference=self.reference):
 
-                    if query_pos is None or ref_pos is None or ref_pos < start or ref_pos > end:
-                        continue
-                    query_base = read.seq[query_pos]
-                    #query_qual = read.qual[query_pos]
-                    if query_base == 'N':
-                        continue
-                    base_obs[(read.reference_name, ref_pos)][query_base] += 1
+                if allow_unsafe:
+                    for  query_pos, ref_pos, ref_base in read.get_aligned_pairs(matches_only=True, with_seq=True):
+                        if query_pos is None or ref_pos is None: #or ref_pos < start or ref_pos > end:
+                            continue
+                        query_base = read.seq[query_pos]
+                        #query_qual = read.qual[query_pos]
+                        if query_base == 'N':
+                            continue
+                        base_obs[(read.reference_name, ref_pos)][query_base] += 1
+
+                        if return_refbases:
+                            ref_bases[(read.reference_name, ref_pos)
+                                      ] = ref_base.upper()
+
+                else:
+                    for cycle, query_pos, ref_pos, ref_base in pysamiterators.iterators.ReadCycleIterator(
+                            read, with_seq=True, reference=self.reference):
+
+                        if query_pos is None or ref_pos is None: #or ref_pos < start or ref_pos > end:
+                            continue
+                        query_base = read.seq[query_pos]
+                        #query_qual = read.qual[query_pos]
+                        if query_base == 'N':
+                            continue
+                        base_obs[(read.reference_name, ref_pos)][query_base] += 1
 
-                    if return_refbases:
-                        ref_bases[(read.reference_name, ref_pos)
-                                  ] = ref_base.upper()
+                        if return_refbases:
+                            ref_bases[(read.reference_name, ref_pos)
+                                      ] = ref_base.upper()
 
         if used == 0 and ignored > 0:
-            raise ValueError('Could not extract any safe data from molecule')
+            raise ValueError(f'Could not extract any safe data from molecule {error}')
 
         self.saved_base_obs = (base_obs, ref_bases)
 
         if return_refbases:
             return base_obs, ref_bases
 
         return base_obs
@@ -1788,14 +2047,15 @@
 
     def get_consensus(
             self,
             base_obs=None,
             classifier=None,
             store_consensus=True,
             reuse_cached_consensus=True,
+            allow_unsafe=False,
             allow_N=False):
         """Get dictionary containing consensus calls in respect to reference.
         By default mayority voting is used to determine the consensus base. If a classifier is supplied the classifier is used to determine the consensus base.
 
         Args:
             base_obs (collections.defaultdict(collections.Counter)) :
                 { genome_location (tuple) : base (string) : obs (int) }
@@ -1817,20 +2077,22 @@
             features, reference_bases, CIGAR, alignment_start, alignment_end = self.get_base_calling_feature_matrix_spaced(
                 True)
 
             if features is None:
                 # We cannot determine the consensus as there are no features...
                 return dict()
 
-            predicted_sequence = classifier.predict(features)
+            base_calling_probs = classifier.predict_proba(features)
+            predicted_sequence = [ 'ACGT'[i] for i in np.argmax( base_calling_probs ,1) ]
+
             reference_sequence = ''.join(
                 [base for chrom, pos, base in reference_bases])
 
             phred_scores = np.rint(
-                -10 * np.log10(np.clip(1 - classifier.predict_proba(features).max(1),
+                -10 * np.log10(np.clip(1 - base_calling_probs.max(1),
                                        0.000000001,
                                        0.999999999)
                                )).astype('B')
 
             consensus = {(chrom, pos): consensus_base for (
                 chrom, pos, ref_base), consensus_base in zip(reference_bases, predicted_sequence)}
 
@@ -1838,29 +2100,51 @@
                 self.classifier_consensus = consensus
                 self.classifier_phred_scores = phred_scores
             return consensus
 
         if base_obs is None:
             try:
                 base_obs, ref_bases = self.get_base_observation_dict(
-                    return_refbases=True, allow_N=allow_N)
+                    return_refbases=True, allow_N=allow_N, allow_unsafe=allow_unsafe)
             except ValueError as e:
                 # We cannot determine safe regions
                 raise
 
         for location, obs in base_obs.items():
             votes = obs.most_common()
             if len(votes) == 1 or votes[1][1] < votes[0][1]:
                 consensus[location] = votes[0][0]
 
         if store_consensus:
             self.majority_consensus = consensus
 
         return consensus
 
+    def get_consensus_base(self, contig, position, classifier=None):
+        """Obtain base call at single position of the molecule
+
+        Args:
+            contig (str) : contig to extract base call from
+
+            position (int) : position to extract base call from (zero based)
+
+            classifier (obj) : base calling classifier
+
+        Returns:
+
+            base_call (str) : base call, or None when no base call could be made
+        """
+
+        try:
+            c = self.get_consensus(classifier)
+        except ValueError:
+            return None
+        return c.get(  (contig, position), None)
+
+
     # when enabled other calls (non ref non alt will be set None)
     def check_variants(self, variants, exclude_other_calls=True):
         """Verify variants in molecule
 
         Args:
             variants (pysam.VariantFile) : Variant file handle to extract variants from
 
@@ -1874,26 +2158,16 @@
                 self.spanEnd):
             variant_dict[(variant.chrom, variant.pos - 1)
                          ] = (variant.ref, variant.alts)
 
         variant_calls = collections.defaultdict(collections.Counter)
         for fragment in self:
 
-            R1 = fragment.get_R1()
-            R2 = fragment.get_R2()
-            start, end = pysamiterators.iterators.getPairGenomicLocations(
-                R1=R1,
-                R2=R2,
-                R1PrimerLength=fragment.R1_primer_length,
-                R2PrimerLength=fragment.R2_primer_length,
-
-                allow_unsafe=(R1 is None))
-            if start is None or end is None:
-                continue
 
+            _, start, end = fragment.span
             for read in fragment:
                 if read is None:
                     continue
 
                 for cycle, query_pos, ref_pos in pysamiterators.iterators.ReadCycleIterator(
                         read):
 
@@ -1946,14 +2220,15 @@
             singlecellmultiomics.fragment.Fragment
         """
         for fragment in self.fragments:
             yield fragment
 
     def get_methylated_count(self, context=3):
         """Get the total amount of methylated bases
+
         Args:
             context (int) : 3 or 4 base context
 
         Returns:
             r (collections.Counter) : sum of methylated bases in contexts
         """
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/nlaIII.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/nlaIII.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         return True
 
     def get_fragment_span_sequence(self, reference=None):
         """Obtain the sequence between the start and end of the molecule
         Args:
             reference(pysam.FastaFile) : reference  to use.
-                If not specified self.reference is used
+                If not specified `self.reference` is used
         Returns:
             sequence (str)
         """
         if reference is None:
             if self.reference is None:
                 raise ValueError('Please supply a reference (PySAM.FastaFile)')
         reference = self.reference
@@ -67,26 +67,23 @@
             self.spanStart,
             self.spanEnd).upper()
 
     def get_undigested_site_count(self, reference=None):
         """
         Obtain the amount of undigested sites in the span of the molecule
 
-        Parameters
-        ----------
-        reference : pysam.FastaFile or similiar
-
-        Returns
-        -------
-        undigested_site_count : int
+        Args:
+            reference(pysam.FastaFile) : reference handle
+
+        Returns:
+            undigested_site_count : int
             amount of undigested cut sites in the mapping span of the molecule
 
         Raises:
-        -------
-        ValueError : when the span of the molecule is not properly defined
+            ValueError : when the span of the molecule is not properly defined
         """
         if reference is None:
             if self.reference is None:
                 raise ValueError('Please supply a reference (PySAM.FastaFile)')
         reference = self.reference
 
         seq = self.get_fragment_span_sequence(reference)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/molecule/rna.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/molecule/rna.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/pyutils/handlelimiter.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/pyutils/handlelimiter.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/pyutils/pyutils.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/pyutils/pyutils.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/_general/sge_wrapper.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/_general/slurm_wrapper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from singlecellmultiomics.utils.submission import submit_job
 
 import os
 import sys
 import re
 import subprocess
 import uuid
 from snakemake.utils import read_job_properties
@@ -19,56 +20,37 @@
 try:
     threads = job_properties['threads']
 except KeyError:
     threads = 1
 n = threads
 
 try:
-    time = job_properties['cluster']['time'] # runtime is time in hours
+    time = int( job_properties['resources']['time'])
 except KeyError:
     try:
-        time = job_properties['params']['runtime'].replace('h','') + ':00:00'
+        time = int(job_properties['cluster']['time']) # runtime is time in hours
     except KeyError:
-        time = '12:00:00'
+        try:
+            time = job_properties['params']['runtime'].replace('h','')
+        except KeyError:
+            time = '12'
 
 
 try:
     mem = job_properties['cluster']['mem']
 except KeyError:
     try:
         mem = int( int(job_properties['resources']['mem_mb'])/1000 )
     except KeyError:
         mem = 10
 
 
 # removing 'special' characters in log paths (default for snakemake)
 base_path = os.path.dirname(job_script)
 
-try:
-    os.makedirs(base_path+'/cluster_jobs')
-except Exception as e :
-    pass
-
-job_id = uuid.uuid4()
-std_out =  f'{base_path}/cluster_jobs/{job_id}.o'
-std_err = f'{base_path}/cluster_jobs/{job_id}.e' 
-
+cluster_file_folder= base_path+'/cluster_jobs'
 
 # formatting qsub command
-cmd = "qsub -V -pe threaded {n} -l h_vmem={mem}G -l h_rt={time} -o {std_out} -e {std_err} {job_script}"
-cmd = cmd.format(n=n, mem=mem, time=time, std_out=std_out, std_err=std_err, job_script=job_script)
-
-# subprocess job: qsub
-try:
-    res = subprocess.run(cmd, check=True, shell=True, stdout=subprocess.PIPE)
-except subprocess.CalledProcessError as e:
-    raise e
-
-# get qsub job ID
-res = res.stdout.decode()
-try:
-    m = re.search("Your job (\d+)", res)
-    jobid = m.group(1)
-    print(jobid)
-except Exception as e:
-    print(e)
-    raise
+job_id = submit_job(f'sh {job_script};', prefix='snake', target_directory=cluster_file_folder,  working_directory='.',
+               threads_n=n, memory_gb=mem, time_h=time, scheduler='slurm', copy_env=True,
+               email=None, mail_when_finished=False, hold=None,submit=True)
+print(job_id)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic/Snakefile` & `singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/nlaIII/Snakefile`

 * *Files 2% similar despite different names*

```diff
@@ -110,71 +110,78 @@
         -a "IlluminaMultiplexingPCRPrimer=GGAACTCCAGTCACN{{6}}TCTCGTATGCCGTCTTCTGCTTG;min_overlap=5" \
         -A "Aseq=TGGCACCCGAGAATTCCA" -a "Aseq=TGGCACCCGAGAATTCCA"  \
         -a "illuminaSmallRNAAdapter=TCGTATGCCGTCTTCTGCTTGT" > {log.stdout} 2> {log.stderr}'
 
 
 rule map:
     input:
-        ref=config['reference_file'],
         r1="processed/{library}/trimmed.R1.fastq.gz",
         r2="processed/{library}/trimmed.R2.fastq.gz"
+
+    params:
+        ref=config['reference_file_for_mapper']
+        
     output:
         bam = temp("processed/{library}/sorted.bam"),
         bam_index = temp("processed/{library}/sorted.bam.bai")
 
     log:
         stdout="log/map/{library}.stdout",
         stderr="log/map/{library}.stderr"
-
+           
     threads: 8
     params: runtime="30h"
     resources:
         mem_mb=lambda wildcards, attempt: attempt * 8000
 
     run:
         # https://stackoverflow.com/questions/40996597/snakemake-remove-output-file this is probably pretier
         if config['mapper']=='bwa':
             # The sorting and mapping has been disconnected
             shell(
-                "bwa mem -t {threads} {input.ref} {input.r1} {input.r2}  2> {log.stderr} |  samtools view -bS - > processed/{wildcards.library}/unsorted.bam; \
+                "bwa mem -t {threads} {params.ref} {input.r1} {input.r2}  2> {log.stderr} |  samtools view -bS - > processed/{wildcards.library}/unsorted.bam; \
                 samtools sort -T processed/{wildcards.library}/temp_sort -@ {threads} processed/{wildcards.library}/unsorted.bam > processed/{wildcards.library}/sorted.unfinished.bam; \
                 mv processed/{wildcards.library}/sorted.unfinished.bam {output.bam}; rm processed/{wildcards.library}/unsorted.bam; samtools index {output.bam} > {log.stdout}"
                 )
         elif config['mapper']=='bowtie2':
             shell(
-                "bowtie2 -p {threads} -q --no-unal --local --sensitive-local -N 1 -x {input.ref} -1 {input.r1} -2 {input.r2} | samtools view -Sb > processed/{wildcards.library}/unsorted.bam; \
+                "bowtie2 -p {threads} -q --no-unal --local --sensitive-local -N 1 -x {params.ref} -1 {input.r1} -2 {input.r2} | samtools view -Sb > processed/{wildcards.library}/unsorted.bam; \
                 samtools sort -T processed/{wildcards.library}/temp_sort -@ {threads} processed/{wildcards.library}/unsorted.bam > processed/{wildcards.library}/sorted.unfinished.bam; \
                 mv processed/{wildcards.library}/sorted.unfinished.bam {output.bam}; rm processed/{wildcards.library}/unsorted.bam; samtools index {output.bam} > {log.stdout} 2> {log.stderr} "
                 )
 
 
-rule SCMO_tagmultiome_ChiC_parallel_scatter:
+rule SCMO_tagmultiome_NLA_parallel_scatter:
     input:
         bam = "processed/{library}/sorted.bam",
         bam_index = "processed/{library}/sorted.bam.bai"
 
     output:
         bam = temp("processed/{library}/TEMP_CONTIG/{contig}.bam"),
         bam_index = temp("processed/{library}/TEMP_CONTIG/{contig}.bam.bai")
 
     log:
         stdout="log/tag_scatter/{library}_{contig}.stdout",
         stderr="log/tag_scatter/{library}_{contig}.stderr"
-        
+
 
     threads: 1
-    params: runtime="20h"
+    params:
+        runtime="20h",
+        alleles = config['alleles'],
+        allele_samples = config['allele_samples']
+
     resources:
-        mem_mb=lambda wildcards, attempt: attempt * 6000 # The amount of memory reqiored is dependent on wether alleles or consensus caller are used
+        mem_mb=lambda wildcards, attempt: attempt * 10000
 
     shell:
-        "bamtagmultiome.py -method chic -contig {wildcards.contig} {input.bam} -o {output.bam} > {log.stdout} 2> {log.stderr}"
+        "bamtagmultiome.py -method nla -allele_samples {params.allele_samples} -alleles {params.alleles} -contig {wildcards.contig} {input.bam} -o {output.bam} > {log.stdout} 2> {log.stderr}"
 
 
-rule SCMO_tagmultiome_ChiC_parallel_gather:
+rule SCMO_tagmultiome_NLA_parallel_gather:
     input:
         chr_bams =  expand("processed/{{library}}/TEMP_CONTIG/{contig}.bam", contig=contigs),
         chr_bams_indices =  expand("processed/{{library}}/TEMP_CONTIG/{contig}.bam.bai", contig=contigs)
     output:
         bam = "processed/{library}/tagged.bam",
         bam_index = "processed/{library}/tagged.bam.bai"
     log:
@@ -206,14 +213,15 @@
 
     threads: 1
     params: runtime="30h"
 
     shell:
         "libraryStatistics.py processed/{wildcards.library} -tagged_bam /tagged.bam > {log.stdout} 2> {log.stderr}"
 
+
 rule SCMO_count_table:
     input:
         bam = "processed/{library}/tagged.bam"
     output:
         "processed/{library}/count_table_{counting_bin_size}_{counting_sliding_window_increment}.csv"
 
     threads: 1
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/chic_allelic/Snakefile` & `singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/chic_allelic/Snakefile`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/demux/demux.smk` & `singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/demux/demux.smk`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/nlaIII/Snakefile` & `singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/cs2/Snakefile`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 from singlecellmultiomics.libraryDetection.sequencingLibraryListing import SequencingLibraryLister
 from glob import glob
 import collections
 from singlecellmultiomics.utils import get_contig_list_from_fasta
 
 """
+CelSeq2 pipeline based on the version of Marijn van Loenhout (2018)
+
+Dependencies:
+# STAR
+# samtools
+# umi-tools
+# cutadapt (trimgalore/atropos)
+# subread
+# colorama
+# SingleCellMultiOmics package
+
 This workflow:
-    Starts off from a folder containing fastq files
+    Starts off from a folder containing all fastq files
     - Detects libraries
     - Demultiplexes per library, automatically detecting the right barcodes
     - Trims using cutadapt
-    - Maps, sorts and indexes the reads per library
-    - Deduplicates and identifies molecules in parallel per contig
-    - Creates QC plots
-    - Creates count tables
+    - Maps using STAR, sorts and indexes the reads per library
+    - uses featureCounting
+    - Tags and demultiplexes
+    - Creates library statistics plots for quality control
+    - Creates count tables for deduplicated and non-deduplicated counts:
+       -> Count table containing rows with gene information and columns with cell information 
 """
 ################## configuration ##################
 configfile: "config.json"
-# config
-counting_bin_sizes = config['counting_bin_sizes']
-counting_sliding_window_increments = config['counting_sliding_window_increments']
-
-# Obtain contigs:
-contigs = get_contig_list_from_fasta(config['reference_file'])
-# If you want to select on which chromosomes to run, change and  uncomment the next line:
-# contigs = ['chr1','chr2']
 
 # This code detects which libraries are present in the current folder:
 l = SequencingLibraryLister()
 LIBRARIES = l.detect(glob('*.fastq.gz'), merge='_')
 # Flatten to library:[fastqfile, fastqfile, ...]
 fastq_per_lib = collections.defaultdict(list)
 for lib,lane_dict in LIBRARIES.items():
@@ -54,52 +59,54 @@
 def get_target_tagged_bam_list():
     return [f"processed/{library}/tagged.bam" for library in libraries]
 
 rule all:
     input:
         # get_target_demux_list() use this for demux only
         get_target_tagged_bam_list(),
-        expand("processed/{library}/count_table_{counting_bin_size}_{counting_sliding_window_increment}.csv",
-            library=libraries,
-            counting_bin_size=counting_bin_sizes,
-            counting_sliding_window_increment=counting_sliding_window_increments),
+        expand("processed/{library}/count_table_not_deduplicated.csv",
+            library=libraries),
+        expand("processed/{library}/count_table_deduplicated.csv",
+            library=libraries),
 
         expand("processed/{library}/plots/ReadCount.png", library=libraries)
 
+
+#### 1. Demultiplexing 
 rule SCMO_demux:
     input:
         fastqfiles = get_fastq_file_list
     output:
         temp("processed/{library}/demultiplexedR1.fastq.gz"),
         temp("processed/{library}/demultiplexedR2.fastq.gz"),
         temp("processed/{library}/rejectsR1.fastq.gz"),
         temp("processed/{library}/rejectsR2.fastq.gz")
-
     log:
         stdout="log/demux/{library}.stdout",
         stderr="log/demux/{library}.stderr"
     params: runtime="30h"
     resources:
         mem_mb=lambda wildcards, attempt: attempt * 4000
+    
     shell:
-        "demux.py -merge _ {input.fastqfiles} -o processed --y > {log.stdout} 2> {log.stderr}"
-
+        "demux.py -merge _ {input.fastqfiles} -o processed --y -use CS2C8U6 > {log.stdout} 2> {log.stderr}"
 
+#### 2. Trimming
 rule Trim:
     input:
         r1="processed/{library}/demultiplexedR1.fastq.gz",
-        r2="processed/{library}/demultiplexedR2.fastq.gz"
-    log:
-        stdout="log/trim/{library}.stdout",
-        stderr="log/trim/{library}.stderr"
+        r2="processed/{library}/demultiplexedR2.fastq.gz" 
     output:
         r1=temp("processed/{library}/trimmed.R1.fastq.gz"),
         r2=temp("processed/{library}/trimmed.R2.fastq.gz")
-
-    params: runtime="30h"
+    log:
+        stdout="log/trim/{library}.stdout",
+        stderr="log/trim/{library}.stderr"
+    params: 
+        runtime="30h"
     resources:
         mem_mb=lambda wildcards, attempt: attempt * 4000
 
     shell:
         'cutadapt -o {output.r1} -p {output.r2} \
         {input.r1} {input.r2} \
         -m 3 -a "IlluminaSmallAdapterConcatBait=GGAACTCCAGTCACNNNNNNATCTCGTATGCCGTCTTCTGCTT" \
@@ -107,97 +114,84 @@
         -A "IlluminaPairedEndPCRPrimer2.0=AGATCGGAAGAGCGN{{6}}CAGGAATGCCGAGACCGATCTCGTATGCCGTCTTCTGCTTG;min_overlap=5" \
         -A "universalPrimer=GATCGTCGGACTGTAGAACTCTGAACGTGTAGATCTCGGTGGTCGCCGTATCATT;min_overlap=5" \
         -a  "IlluminaGEX=TTTTTAATGATACGGCGACCACCGAGATCTACACGTTCAGAGTTCTACAGTCCGACGATC;min_overlap=5" \
         -a "IlluminaMultiplexingPCRPrimer=GGAACTCCAGTCACN{{6}}TCTCGTATGCCGTCTTCTGCTTG;min_overlap=5" \
         -A "Aseq=TGGCACCCGAGAATTCCA" -a "Aseq=TGGCACCCGAGAATTCCA"  \
         -a "illuminaSmallRNAAdapter=TCGTATGCCGTCTTCTGCTTGT" > {log.stdout} 2> {log.stderr}'
 
-
+#### 3. Mapping with STAR 
 rule map:
     input:
-        ref=config['reference_file'],
-        r1="processed/{library}/trimmed.R1.fastq.gz",
         r2="processed/{library}/trimmed.R2.fastq.gz"
+    params:
+        ref=config['STAR_index'],
+        output_dir = "processed/{library}/"
+        
     output:
-        bam = temp("processed/{library}/sorted.bam"),
-        bam_index = temp("processed/{library}/sorted.bam.bai")
-
+        bam = temp("processed/{library}/Aligned.sortedByCoord.out.bam"),
+        SJtemp = temp("processed/{library}/SJ.out.tab")
     log:
         stdout="log/map/{library}.stdout",
         stderr="log/map/{library}.stderr"
-
     threads: 8
-    params: runtime="30h"
+    params: 
+        runtime="30h",
+        output_dir = "processed/{library}/"
     resources:
         mem_mb=lambda wildcards, attempt: attempt * 8000
+        
+    shell:
+      "STAR --runThreadN 8 --outSAMtype BAM SortedByCoordinate --outFilterMultimapNmax 20 --outMultimapperOrder Random --outSAMattributes All --outSAMmultNmax 1 --readFilesCommand zcat  --readFilesIn {input.r2} \
+      --genomeDir {params.ref} --outFileNamePrefix {params.output_dir} > {log.stdout} 2> {log.stderr}"
 
-    run:
-        # https://stackoverflow.com/questions/40996597/snakemake-remove-output-file this is probably pretier
-        if config['mapper']=='bwa':
-            # The sorting and mapping has been disconnected
-            shell(
-                "bwa mem -t {threads} {input.ref} {input.r1} {input.r2}  2> {log.stderr} |  samtools view -bS - > processed/{wildcards.library}/unsorted.bam; \
-                samtools sort -T processed/{wildcards.library}/temp_sort -@ {threads} processed/{wildcards.library}/unsorted.bam > processed/{wildcards.library}/sorted.unfinished.bam; \
-                mv processed/{wildcards.library}/sorted.unfinished.bam {output.bam}; rm processed/{wildcards.library}/unsorted.bam; samtools index {output.bam} > {log.stdout}"
-                )
-        elif config['mapper']=='bowtie2':
-            shell(
-                "bowtie2 -p {threads} -q --no-unal --local --sensitive-local -N 1 -x {input.ref} -1 {input.r1} -2 {input.r2} | samtools view -Sb > processed/{wildcards.library}/unsorted.bam; \
-                samtools sort -T processed/{wildcards.library}/temp_sort -@ {threads} processed/{wildcards.library}/unsorted.bam > processed/{wildcards.library}/sorted.unfinished.bam; \
-                mv processed/{wildcards.library}/sorted.unfinished.bam {output.bam}; rm processed/{wildcards.library}/unsorted.bam; samtools index {output.bam} > {log.stdout} 2> {log.stderr} "
-                )
-
-
-rule SCMO_tagmultiome_NLA_parallel_scatter:
-    input:
-        bam = "processed/{library}/sorted.bam",
-        bam_index = "processed/{library}/sorted.bam.bai"
-
-    output:
-        bam = temp("processed/{library}/TEMP_CONTIG/{contig}.bam"),
-        bam_index = temp("processed/{library}/TEMP_CONTIG/{contig}.bam.bai")
-
+#### 4. Feature counting
+rule featureCounting:
+  input:
+        bam = "processed/{library}/Aligned.sortedByCoord.out.bam"
+  output:
+        bam = temp("processed/{library}/Aligned.sortedByCoord.out.bam.featureCounts.bam"),
+        log = temp("processed/{library}/fCounts.txt")
+  params:
+    GTF = config['GTF']
+  log:
+    stdout="log/featureCounts/{library}.stdout",
+    stderr="log/featureCounts/{library}.stderr"
+  threads: 4
+  params: runtime="30h"
+  resources:
+      mem_mb=lambda wildcards, attempt: attempt * 8000
+  
+  shell:
+    'featureCounts -s 1 -T 1 -R BAM -a {params.GTF} -o processed/{wildcards.library}/fCounts.txt {input.bam} > {log.stdout} 2> {log.stderr}'
+
+
+#### 5. Tagging and deduplication
+rule SCMO_tagmultiome_CS2:
+    input:
+      bam = "processed/{library}/Aligned.sortedByCoord.out.bam.featureCounts.bam"
+    output:
+      bamSorted = temp("processed/{library}/sorted.bam"),
+      bamSorted_index = temp("processed/{library}/sorted.bam.bai"),
+      bam = "processed/{library}/tagged.bam",
+      bam_index = "processed/{library}/tagged.bam.bai"
     log:
-        stdout="log/tag_scatter/{library}_{contig}.stdout",
-        stderr="log/tag_scatter/{library}_{contig}.stderr"
-
-
+        stdout="log/tagging/{library}.stdout",
+        stderr="log/tagging/{library}.stderr"
     threads: 1
     params:
-        runtime="20h",
-        alleles = config['alleles'],
-        allele_samples = config['allele_samples']
-
+        runtime="20h"
     resources:
         mem_mb=lambda wildcards, attempt: attempt * 10000
 
     shell:
-        "bamtagmultiome.py -method nla -allele_samples {params.allele_samples} -alleles {params.alleles} -contig {wildcards.contig} {input.bam} -o {output.bam} > {log.stdout} 2> {log.stderr}"
-
-
-rule SCMO_tagmultiome_NLA_parallel_gather:
-    input:
-        chr_bams =  expand("processed/{{library}}/TEMP_CONTIG/{contig}.bam", contig=contigs),
-        chr_bams_indices =  expand("processed/{{library}}/TEMP_CONTIG/{contig}.bam.bai", contig=contigs)
-    output:
-        bam = "processed/{library}/tagged.bam",
-        bam_index = "processed/{library}/tagged.bam.bai"
-    log:
-        stdout="log/tag_gather/{library}.stdout",
-        stderr="log/tag_gather/{library}.stderr"
-
-    threads: 1
-    params: runtime="8h"
-    message:
-        'Merging contig BAM files'
-
-    shell:
-        "samtools merge -c {output.bam} {input.chr_bams} > {log.stdout} 2> {log.stderr}; samtools index {output.bam}"
-
+        "samtools sort -T processed/{wildcards.library}/temp_sort -@ {threads} {input.bam} > processed/{wildcards.library}/sorted.unfinished.bam; \
+        mv processed/{wildcards.library}/sorted.unfinished.bam {output.bamSorted}; samtools index {output.bamSorted}; \
+        bamtagmultiome.py -method cs_feature_counts -umi_hamming_distance 0 {output.bamSorted} -o {output.bam} > {log.stdout} 2> {log.stderr}"
 
+#### 6. Library statistics
 rule SCMO_library_stats:
     input:
         bam = "processed/{library}/tagged.bam",
         r1="processed/{library}/demultiplexedR1.fastq.gz", # Its need these to count how many raw reads were present in the lib.
         r2="processed/{library}/demultiplexedR2.fastq.gz",
         r1_rejects="processed/{library}/rejectsR1.fastq.gz",
         r2_rejects="processed/{library}/rejectsR2.fastq.gz"
@@ -210,32 +204,45 @@
 
     threads: 1
     params: runtime="30h"
 
     shell:
         "libraryStatistics.py processed/{wildcards.library} -tagged_bam /tagged.bam > {log.stdout} 2> {log.stderr}"
 
-
-rule SCMO_count_table:
+#### 7. Make dedup and no dedup count tables
+#### a. Make count tables of non-deduplicated bam files
+rule SCMO_count_table_nondedup:
     input:
         bam = "processed/{library}/tagged.bam"
     output:
-        "processed/{library}/count_table_{counting_bin_size}_{counting_sliding_window_increment}.csv"
-
+        countTable = "processed/{library}/count_table_not_deduplicated.csv"
     threads: 1
     params:
-        runtime="50h",
-        counting_min_mq = config['counting_min_mq']
-
+        runtime="10h"
     log:
-        stdout="log/count_table/{library}_{counting_bin_size}_{counting_sliding_window_increment}.stdout",
-        stderr="log/count_table/{library}_{counting_bin_size}_{counting_sliding_window_increment}.stderr"
+        stdout="log/count_table/{library}_not_deduplicated.stdout",
+        stderr="log/count_table/{library}_not_deduplicated.stderr"
+    resources:
+        mem_mb=lambda wildcards, attempt: attempt * 8000
+
+    shell:
+        "bamToCountTable.py --noNames {input.bam} -o {output.countTable} -joinedFeatureTags XT,chrom -sampleTags SM > {log.stdout} 2> {log.stderr}"
 
+#### b. Make count tables of deduplicated bam files
+# This works exactly the same as step a
+rule SCMO_count_table_filtered:
+    input:
+        bam = "processed/{library}/tagged.bam"
+    output:
+        countTable = "processed/{library}/count_table_deduplicated.csv"
+    threads: 1
+    params:
+        runtime="10h"
+    log:
+        stdout="log/count_table/{library}_deduplicated.stdout",
+        stderr="log/count_table/{library}_deduplicated.stderr"
     resources:
         mem_mb=lambda wildcards, attempt: attempt * 8000
 
     shell:
-        "bamToCountTable.py -bin {wildcards.counting_bin_size} \
-        -sliding {wildcards.counting_sliding_window_increment} \
-        -minMQ {params.counting_min_mq} \
-        --noNames \
-        {input.bam} -sampleTags SM -joinedFeatureTags reference_name -binTag DS -o {output} --dedup > {log.stdout} 2> {log.stderr}"
+        "bamToCountTable.py --dedup --noNames {input.bam} -o {output.countTable} -joinedFeatureTags XT,chrom -sampleTags SM > {log.stdout} 2> {log.stderr}"
+
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/snakemake_workflows/scmo_workflow.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/snakemake_workflows/scmo_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,13 +55,15 @@
 
     else:
         deploy_workflow_files(args.alias, clean=args.clean)
         deploy_workflow_files('_general', clean=args.clean)
 
         print(f"""\nEdit config.json and then run either;\n
         On local computer:\n
-        {Fore.BLUE}snakemake -np{Style.RESET_ALL}\n
+        {Fore.BLUE}snakemake{Style.RESET_ALL}\n
         On SGE cluster:\n
         {Fore.BLUE}snakemake --cluster sge_wrapper.py  --jobs 20 --restart-times 3{Style.RESET_ALL}\n
+        On SLURM cluster:\n
+        {Fore.BLUE}snakemake --cluster slurm_wrapper.py  --jobs 20 --restart-times 3{Style.RESET_ALL}\n
         On SGE cluster with controller as a job:\n
         {Fore.BLUE}submission.py "snakemake --cluster sge_wrapper.py  --jobs 20 --restart-times 3" -y -time 50 -m 2 -N SCMOCONTROL{Style.RESET_ALL}\n
         """)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/allele.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/allele.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/conversions.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/conversions.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/datatype.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/datatype.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/fragmentsize.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/fragmentsize.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/mappingquality.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/mappingquality.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/methylation.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/methylation.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/oversequencing.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/oversequencing.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/plate.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/plate.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/readcount.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/readcount.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/rejectionreasons.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/rejectionreasons.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/scchicligation.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/scchicligation.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/statistic.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/statistic.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/tag.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/tag.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/statistic/trimming.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/statistic/trimming.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/tags/tags.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/tags/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,17 +38,24 @@
     SamTag('aa', 'rawIlluminaIndexSequence'),
     SamTag('ah', 'hammingDistanceToIndex'),
     SamTag('BC', 'barcode'),
     SamTag('CB', 'cellBarcode'),  # Same as bc
     SamTag('QX', 'barcodeQual', isPhred=True),
     SamTag('bc', 'rawBarcode'),
     SamTag('hd', 'hammingDistanceRawBcAssignedBc'),
-    SamTag('BI', 'barcodeIndex'),
+
+    SamTag('bi', 'barcodeIndex'),
+
+    #Those are insertion/deletion base qualities, where N=45, which is the default quality score for indels assigned by the BaseRecalibrator
+    SamTag('BI', 'gatk_insert_deletion_base_qualities'),
+    SamTag('BD', 'gatk_insert_deletion_base_qualities'),
+
     SamTag('QT', 'sampleBarcodeQuality', isPhred=True),
     SamTag('RX', 'umi'),
+    SamTag('tu', 'second_umi'),
     SamTag('uL', 'umiLength'),
     SamTag('RQ', 'umiQual', isPhred=True),
     SamTag('BX', 'umiCorrected'),
     SamTag('BZ', 'umiCorrectedQuality', isPhred=True),
     SamTag('MI', 'molecularIdentifier'),
     SamTag('QM', 'molecularIdentifierQuality', isPhred=True),
     SamTag('DS', 'siteCoordinate'),
@@ -128,15 +135,15 @@
     SamTag('sX', 'Total CHG methylated'),
     SamTag('sx', 'Total CHG unmethylated'),
 
 
     SamTag('rS', 'randomPrimerStart'),
     SamTag('rP', 'randomPrimerSequence'),
     SamTag('TR', 'totalRTreactions'),
-
+    SamTag('TF', 'totalAssociatedFragments'),
 
     SamTag('AI', 'AssignedIntrons'),
     SamTag('AE', 'AssingedExons'),
     SamTag('iH', 'IntronHits amount of bases aligned to intron'),
     SamTag('eH', 'ExonHits amount of bases aligned to exon'),
     SamTag('SP', 'IsSpliced'),
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/tags/write_tags_md.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/tags/write_tags_md.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/tagtools/tagtools.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/tagtools/tagtools.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/4SUtagger.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/4SUtagger.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,54 +9,55 @@
 import glob
 import pickle
 import pandas as pd
 import argparse
 
 from singlecellmultiomics.bamProcessing.bamFunctions import sorted_bam_file, sort_and_index, get_reference_from_pysam_alignmentFile, add_readgroups_to_header, write_program_tag
 
-argparser = argparse.ArgumentParser(
-    formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    description="""
-4FU detection tool
-""")
-argparser.add_argument('bamfile')
-argparser.add_argument('-head', type=int)
-argparser.add_argument(
-    '-ref',
-    type=str,
-    help='reference (autodetected if not supplied)')
-args = argparser.parse_args()
-
-
-with pysam.AlignmentFile(args.bamfile, "rb") as alignments:
-
-    reference = None
-    if args.ref is None:
-        args.ref = get_reference_from_pysam_alignmentFile(alignments)
-
-    if args.ref is not None:
-        reference = pysamiterators.iterators.CachedFasta(
-            pysam.FastaFile(args.ref))
-
-    fragment_class_args = {'umi_hamming_distance': 0}
-    molecule_class_args = {'reference': reference}
-    converted_base_frequencies = collections.defaultdict(
-        lambda: collections.defaultdict(collections.Counter))
-
-    with sorted_bam_file(f'{args.bamfile}.4SU_tagged.bam', origin_bam=alignments) as out:
-        test_iter = MoleculeIterator(
-            alignments,
-            fragment_class_args=fragment_class_args,
-            molecule_class_args={
-                'reference': reference},
-            moleculeClass=FourThiouridine,
-            fragmentClass=FeatureCountsSingleEndFragment)
-        for i, molecule in enumerate(test_iter):
-            molecule.write_tags()
-            molecule.set_meta('mi', i)
-            molecule.write_pysam(out)
-            converted_base_frequencies[molecule.sample][molecule.gene][molecule.converted_bases] += 1
-            if args.head is not None and i > (args.head - 1):
-                break
+if __name__ == '__main__':
+    argparser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        description="""
+    4FU detection tool
+    """)
+    argparser.add_argument('bamfile')
+    argparser.add_argument('-head', type=int)
+    argparser.add_argument(
+        '-ref',
+        type=str,
+        help='reference (autodetected if not supplied)')
+    args = argparser.parse_args()
+
+
+    with pysam.AlignmentFile(args.bamfile, "rb") as alignments:
+
+        reference = None
+        if args.ref is None:
+            args.ref = get_reference_from_pysam_alignmentFile(alignments)
+
+        if args.ref is not None:
+            reference = pysamiterators.iterators.CachedFasta(
+                pysam.FastaFile(args.ref))
+
+        fragment_class_args = {'umi_hamming_distance': 0}
+        molecule_class_args = {'reference': reference}
+        converted_base_frequencies = collections.defaultdict(
+            lambda: collections.defaultdict(collections.Counter))
+
+        with sorted_bam_file(f'{args.bamfile}.4SU_tagged.bam', origin_bam=alignments) as out:
+            test_iter = MoleculeIterator(
+                alignments,
+                fragment_class_args=fragment_class_args,
+                molecule_class_args={
+                    'reference': reference},
+                molecule_class=FourThiouridine,
+                fragment_class=FeatureCountsSingleEndFragment)
+            for i, molecule in enumerate(test_iter):
+                molecule.write_tags()
+                molecule.set_meta('mi', i)
+                molecule.write_pysam(out)
+                converted_base_frequencies[molecule.sample][molecule.gene][molecule.converted_bases] += 1
+                if args.head is not None and i > (args.head - 1):
+                    break
 
-    for sample, data in converted_base_frequencies.items():
-        pd.DataFrame(data).to_csv(f'{args.bamfile}.{sample}.counts.csv')
+        for sample, data in converted_base_frequencies.items():
+            pd.DataFrame(data).to_csv(f'{args.bamfile}.{sample}.counts.csv')
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/bamtagmultiome.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/tapsTagger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,286 +1,209 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import pysam
-from singlecellmultiomics.molecule import MoleculeIterator
-import singlecellmultiomics
 import singlecellmultiomics.molecule
 import singlecellmultiomics.fragment
-from singlecellmultiomics.bamProcessing.bamFunctions import sorted_bam_file, get_reference_from_pysam_alignmentFile, write_program_tag, MapabilityReader, verify_and_fix_bam
-
-from singlecellmultiomics.utils import is_main_chromosome
-import singlecellmultiomics.alleleTools
-from singlecellmultiomics.universalBamTagger.customreads import CustomAssingmentQueryNameFlagger
-import singlecellmultiomics.features
-import pysamiterators
+import gzip
+import collections
+import matplotlib.pyplot as plt
+import pandas as pd
 import argparse
-import uuid
-import os
+import pysamiterators
 import sys
+import os
+import uuid
+import singlecellmultiomics.bamProcessing.bamFunctions as bf
+import singlecellmultiomics.features
 import colorama
-import sklearn
-import pkg_resources
-import pickle
-from datetime import datetime
-
-argparser = argparse.ArgumentParser(
-    formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    description='Assign molecules, set sample tags, set alleles')
-argparser.add_argument('bamin', type=str)
-argparser.add_argument('-o', type=str, help="output bam file", required=True)
-argparser.add_argument(
-    '-method',
-    type=str,
-    default=None,
-    help="Protocol to tag, select from:nla, qflag, chic, nla_transcriptome, vasa, cs, nla_taps ,chic_taps")
-argparser.add_argument(
-    '-qflagger',
-    type=str,
-    default=None,
-    help="Query flagging algorithm")
-argparser.add_argument('-custom_flags', type=str, default="MI,RX,BI,SM")
-argparser.add_argument(
-    '-ref',
-    type=str,
-    default=None,
-    help="Path to reference fast (autodected if not supplied)")
-argparser.add_argument('-umi_hamming_distance', type=int, default=1)
-argparser.add_argument('-head', type=int)
-argparser.add_argument('-contig', type=str, help='Contig to only process')
-argparser.add_argument('-region_start', type=int, help='Zero based start coordinate of region to process')
-argparser.add_argument('-region_end', type=int, help='Zero based end coordinate of region to process')
-
-argparser.add_argument('-alleles', type=str, help="Phased allele file (VCF)")
-argparser.add_argument(
-    '-allele_samples',
-    type=str,
-    help="Comma separated samples to extract from the VCF file. For example B6,SPRET")
-argparser.add_argument(
-    '-unphased_alleles',
-    type=str,
-    help="Unphased allele file (VCF)")
-argparser.add_argument(
-    '--every_fragment_as_molecule',
-    action='store_true',
-    help='Assign every fragment as a molecule, this effectively disables UMI deduplication')
-
-argparser.add_argument(
-    '-mapfile',
-    type=str,
-    help='Path to *.safe.bgzf file, used to decide if molecules are uniquely mappable, generate one using createMapabilityIndex.py ')
-
-argparser.add_argument(
-    '-annotmethod',
-    type=int,
-    default=1,
-    help="Annotation resolving method. 0: molecule consensus aligned blocks. 1: per read per aligned base")
-cluster = argparser.add_argument_group('cluster execution')
-cluster.add_argument(
-    '--cluster',
-    action='store_true',
-    help='split by chromosomes and submit the job on cluster')
-cluster.add_argument(
-    '--no_rejects',
-    action='store_true',
-    help='Write rejected reads to output file')
-cluster.add_argument(
-    '-mem',
-    default=40,
-    type=int,
-    help='Memory requested per job')
-cluster.add_argument(
-    '-time',
-    default=52,
-    type=int,
-    help='Time requested per job')
-
-tr = argparser.add_argument_group('transcriptome specific settings')
-tr.add_argument('-exons', type=str, help='Exon GTF file')
-tr.add_argument(
-    '-introns',
-    type=str,
-    help='Intron GTF file, use exonGTF_to_intronGTF.py to create this file')
-
-cg = argparser.add_argument_group('molecule consensus specific settings')
-cg.add_argument(
-    '--consensus',
-    action='store_true',
-    help='Calculate molecule consensus read, this feature is _VERY_ experimental')
-cg.add_argument('-consensus_mask_variants', type=str,
-                help='variants to mask during training (VCF file)')
-cg.add_argument(
-    '-consensus_model',
-    type=str,
-    help='Name of or path to consensus classifier',
-    default=None)
-cg.add_argument(
-    '-consensus_n_train',
-    type=int,
-    help='Amount of bases used for training',
-    default=500_000)
-cg.add_argument('--no_source_reads', action='store_true',
-                help='Do not write original reads, only consensus ')
-
-cg.add_argument('--consensus_allow_train_location_oversampling', action='store_true',
-                help='Allow to train the consensus model multiple times for a single genomic location')
-
-
-
-
-def run_multiome_tagging_cmd(commandline):
-    args = argparser.parse_args(commandline)
-    run_multiome_tagging(args)
-
-
-def run_multiome_tagging(args):
-    """
-    Run multiome tagging adds molecule information
-
-    Arguments:
-
-        bamin (str) : bam file to process
-
-        o(str) : path to output bam file
-
-        method(str): Protocol to tag, select from:nla, qflag, chic, nla_transcriptome, vasa, cs, nla_taps ,chic_taps
-
-        qflagger(str): Query flagging algorithm to use, this algorithm extracts UMI and sample information from your reads. When no query flagging algorithm is specified, the `singlecellmultiomics.universalBamTagger.universalBamTagger.QueryNameFlagger` is used
-
-        method(str) : Method name, what kind of molecules need to be extracted. Select from:
-            nla
-            qflag
-            chic
-            nla_transcriptome
-            vasa
-            cs
-            nla_taps
-            chic_taps
-
-
-        custom_flags(str): Arguments passed to the query name flagger, comma separated "MI,RX,BI,SM"
-
-        ref(str) : Path to reference fasta file, autodected from bam header when not supplied
-
-        umi_hamming_distance(int) : Max hamming distance on UMI's
-
-        head (int) : Amount of molecules to process
-
-        contig (str) : only process this contig
-
-        region_start(int) : Zero based start coordinate of single region to process
-
-        region_end(int) : Zero based end coordinate of single region to process, None: all contigs when contig is not set, complete contig when contig is set.
-
-        alleles (str) : path to allele VCF
-
-        allele_samples(str): Comma separated samples to extract from the VCF file. For example B6,SPRET
-
-        unphased_alleles(str) : Path to VCF containing unphased germline SNPs
-
-        mapfile (str) : 'Path to *.safe.bgzf file, used to decide if molecules are uniquely mappable, generate one using createMapabilityIndex.py
-
-        annotmethod (int) : Annotation resolving method. 0: molecule consensus aligned blocks. 1: per read per aligned base
-
-        cluster (bool) : Run contigs in separate cluster jobs
-
-        no_rejects(bool) : Do not write rejected reads
-
-        mem (int) : Amount of gigabytes to request for cluster jobs
-
-        time(int) : amount of wall clock hours to request for cluster jobs
-
-        exons(str): Path to exon annotation GTF file
-
-        introns(str): Path to intron annotation GTF file
-
-        consensus(bool) : Calculate molecule consensus read, this feature is _VERY_ experimental
-
-        consensus_model(str) : Path to consensus calling model, when none specified, this is learned based on the supplied bam file, ignoring sites supplied by -consensus_mask_variants
-
-        consensus_mask_variants(str): Path VCF file masked for training on consensus caller
-
-        consensus_n_train(int) : Amount of bases used for training the consensus model
-
-        no_source_reads(bool) :  Do not write original reads, only consensus
-    """
-
-    MISC_ALT_CONTIGS_SCMO = 'MISC_ALT_CONTIGS_SCMO'
-    every_fragment_as_molecule = args.every_fragment_as_molecule
-
-    if not args.o.endswith('.bam'):
-        raise ValueError(
-            "Supply an output which ends in .bam, for example -o output.bam")
-
-    # Verify wether the input file is indexed and sorted...
-    verify_and_fix_bam(args.bamin)
-
-    if os.path.exists(args.o):
-        print(f"Removing existing file {args.o}")
-        os.remove(args.o)
+import numpy as np
 
-    input_bam = pysam.AlignmentFile(args.bamin, "rb")
 
-    # autodetect reference:
-    reference = None
-    if args.ref is None:
-        args.ref = get_reference_from_pysam_alignmentFile(input_bam)
+class Fraction:
+    def __init__(self):
+        self.values = [0, 0]
 
-    if args.ref is not None:
-        try:
-            reference = pysamiterators.iterators.CachedFasta(
-                pysam.FastaFile(args.ref))
-        except Exception as e:
-            print("Error when loading the reference file, continuing without a reference")
-            reference = None
-
-    ##### Define fragment and molecule class arguments and instances: ####
-
-    queryNameFlagger = None
-    if args.qflagger is not None:
-        if args.qflagger == 'custom_flags':
-            queryNameFlagger = CustomAssingmentQueryNameFlagger(
-                args.custom_flags.split(','))
-        else:
-            raise ValueError("Select from 'custom_flags, ..' ")
+    def __setitem__(self, key, value):
+        self.values[key] = value
 
-    molecule_class_args = {
-        'umi_hamming_distance': args.umi_hamming_distance,
-        'reference': reference
-    }
+    def __getitem__(self, key):
+        return self.values[key]
 
-    fragment_class_args = {}
-    yield_invalid = True  # if invalid reads should be written
+    def __float__(self):
+        if sum(self.values) == 0:
+            return np.nan
+        return self.values[1] / (self.values[1] + self.values[0])
 
-    if args.no_rejects:
-        yield_invalid = False
 
-    ignore_conversions = None
-    if args.method == 'nla_taps' or args.method == 'chic_taps':
-        ignore_conversions = set([('C', 'T'), ('G', 'A')])
-
-    if args.alleles is not None:
-        molecule_class_args['allele_resolver'] = singlecellmultiomics.alleleTools.AlleleResolver(
-            args.alleles,
-            select_samples=args.allele_samples.split(',') if args.allele_samples is not None else None,
-            lazyLoad=True,
-            ignore_conversions=ignore_conversions)
-
-    if args.mapfile is not None:
-        molecule_class_args['mapability_reader'] = MapabilityReader(
-            args.mapfile)
+if __name__ == '__main__':
 
-    ### Transcriptome configuration ###
-    if args.method in ('nla_transcriptome', 'cs', 'vasa'):
+    argparser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        description='Add methylation information to BAM file')
+
+    argparser.add_argument('alignmentfile', type=str)
+    argparser.add_argument(
+        '-o',
+        type=str,
+        help="output BAM path",
+        required=True)
+    argparser.add_argument(
+        '-bed',
+        type=str,
+        help="output bed file (base-level methylation status)",
+        default=None,
+        required=False)
+    # these options need to go <- VB
+    argparser.add_argument(
+        '-table',
+        type=str,
+        help="output table alias",
+        default=None,
+        required=False)
+    argparser.add_argument('-bin_size', type=int, default=250_000)
+    argparser.add_argument('-sliding_increment', type=int, default=50_000)
+    #
+    argparser.add_argument(
+        '-ref',
+        type=str,
+        required=False,
+        help='path to reference fasta file ')
+    argparser.add_argument(
+        '-min_mq',
+        default=20,
+        type=int,
+        help='Min mapping qual')
+    argparser.add_argument('-uhd', default=1, type=int,
+                           help='Umi hamming distance')
+    argparser.add_argument(
+        '-mem',
+        default=40,
+        type=int,
+        help='Memory used per job')
+    argparser.add_argument(
+        '-time',
+        default=52,
+        type=int,
+        help='Time requested per job')
+    argparser.add_argument('-head', type=int)
+    argparser.add_argument('-contig', type=str, help='contig to run on')
+    argparser.add_argument('-method', type=str, help='nla or chic')
+    argparser.add_argument(
+        '-samples',
+        type=str,
+        help='Samples to select, separate with comma. For example CellA,CellC,CellZ',
+        default=None)
+    argparser.add_argument(
+        '-context',
+        type=str,
+        help='Context to select, separate with comma. For example Z,H,X',
+        default=None)
+
+    argparser.add_argument('--stranded', action='store_true')
+    argparser.add_argument(
+        '--cluster',
+        action='store_true',
+        help='split by chromosomes and submit the job on cluster')
+    argparser.add_argument(
+        '--no_sort_index',
+        action='store_true',
+        help='do not sort and index the output bam')
+
+    # Transcriptome splitting mode
+    tr = argparser.add_argument_group('transcriptome specific settings')
+    tr.add_argument(
+        '--transcriptome',
+        action='store_true',
+        help='Label transcripts, requires exons and introns')
+    tr.add_argument('-exons', type=str, help='Exon GTF file')
+    tr.add_argument(
+        '-introns',
+        type=str,
+        help='Intron GTF file, use exonGTF_to_intronGTF.py to create this file')
+    tr.add_argument(
+        '-recovery_umi_pool_radius',
+        type=int,
+        help='BP radius. When assigning transcripts without NLA site found, use this radius for molecule pooling',
+        default=4)
+    args = argparser.parse_args()
+
+    samples = None if args.samples is None else set(args.samples.split(','))
+    contexts = None if args.context is None else set(args.context.split(','))
+#    set(
+#        [x.upper() for x in  args.context.split(',')] +
+#        [x.lower() for x in  args.context.split(',')])
+
+    alignments = pysam.AlignmentFile(args.alignmentfile)
+    # Auto detect reference:
+    if args.ref is None:
+        args.ref = bf.get_reference_from_pysam_alignmentFile(alignments)
+        if args.ref is None:
+            raise ValueError("Supply reference, -ref")
+
+    if args.transcriptome:
         print(
             colorama.Style.BRIGHT +
-            'Running in transcriptome annotation mode' +
+            'Running in transcriptome recovery mode' +
             colorama.Style.RESET_ALL)
         if args.exons is None or args.introns is None:
             raise ValueError("Please supply both intron and exon GTF files")
 
+    if args.cluster:
+        if args.contig is None:
+            # Create jobs for all chromosomes:
+            temp_prefix = os.path.abspath(
+                os.path.dirname(args.o)) + '/' + str(uuid.uuid4())
+            hold_merge = []
+            for chrom in alignments.references:
+                if chrom.startswith('KN') or chrom.startswith('KZ') or chrom.startswith(
+                        'chrUn') or chrom.endswith('_random') or 'ERCC' in chrom:
+                    continue
+                temp_bam_path = f'{temp_prefix}_{chrom}.bam'
+                temp_bed_path = f'{temp_prefix}_{chrom}.bed'
+
+                arguments = " ".join([x for x in sys.argv if not x == args.o and x != '-o']) + \
+                    f" -contig {chrom} -o {temp_bam_path} -bed {temp_bed_path}"
+
+                job = f'TAPS_{str(uuid.uuid4())}'
+                os.system(
+                    f'submission.py --silent' +
+                    f' -y --py36 -time {args.time} -t 1 -m {args.mem} -N {job} " {arguments};"')
+                hold_merge.append(job)
+
+            hold = ','.join(hold_merge)
+            os.system(
+                f'submission.py --silent' +
+                f' -y --py36 -time {args.time} -t 1 -m 10 -N {job} -hold {hold} " samtools merge {args.o} {temp_prefix}*.bam; samtools index {args.o}; rm {temp_prefix}*.ba*; cat {temp_prefix}*.bed > {args.bed}; rm {temp_prefix}*.bed"')
+            exit()
+
+    reference = pysamiterators.iterators.CachedFasta(pysam.FastaFile(args.ref))
+    taps = singlecellmultiomics.molecule.TAPS(reference=reference)
+    temp_out = f'{args.o}.temp.out.bam'
+
+    # Obtain contig sizes:
+    ref_lengths = {r: alignments.get_reference_length(
+        r) for r in alignments.references}
+
+    # Methylation dictionary: site->cell->value
+    binned_data = collections.defaultdict(
+        lambda: collections.defaultdict(Fraction))
+    cell_count = collections.Counter()
+
+    # Define molecule class arguments
+    molecule_class_args = {
+        'reference': reference,
+        'taps': taps,
+        'min_max_mapping_quality': args.min_mq
+    }
+
+    fragment_class_args = {'umi_hamming_distance': args.uhd}
+
+    # transcriptome mode specific arguments: ####
+    if args.transcriptome:
+
         transcriptome_features = singlecellmultiomics.features.FeatureContainer()
         print("Loading exons", end='\r')
         transcriptome_features.loadGTF(
             args.exons,
             select_feature_type=['exon'],
             identifierFields=(
                 'exon_id',
@@ -295,267 +218,355 @@
             select_feature_type=['intron'],
             identifierFields=['transcript_id'],
             store_all=True,
             contig=args.contig,
             head=None)
         print("All features loaded")
 
+        rejected_reads = []  # Store all rejected, potential transcript reads
+
         # Add more molecule class arguments
         molecule_class_args.update({
-            'features': transcriptome_features,
-            'auto_set_intron_exon_features': True
+            'features': transcriptome_features
         })
 
-    ### Method specific configuration ###
-    if args.method == 'qflag':
-        moleculeClass = singlecellmultiomics.molecule.Molecule
-        fragmentClass = singlecellmultiomics.fragment.Fragment
-        # Write all reads
-        yield_invalid = True
-
+    # Method specific arguments
+    if args.method == 'nla':
+        molecule_class_args.update({'site_has_to_be_mapped': True})
     elif args.method == 'chic':
-        moleculeClass = singlecellmultiomics.molecule.CHICMolecule
-        fragmentClass = singlecellmultiomics.fragment.CHICFragment
-
-    elif args.method == 'nla':
-        moleculeClass = singlecellmultiomics.molecule.NlaIIIMolecule
-        fragmentClass = singlecellmultiomics.fragment.NLAIIIFragment
-
-    elif args.method == 'nla_transcriptome':
-        moleculeClass = singlecellmultiomics.molecule.AnnotatedNLAIIIMolecule
-        fragmentClass = singlecellmultiomics.fragment.NLAIIIFragment
-
-        molecule_class_args.update({
-            'pooling_method': 1,  # all data from the same cell can be dealt with separately
-            'stranded': None  # data is not stranded
-        })
-
-    elif args.method == 'nla_taps':
-        moleculeClass = singlecellmultiomics.molecule.TAPSNlaIIIMolecule
-        fragmentClass = singlecellmultiomics.fragment.NLAIIIFragment
-
-        molecule_class_args.update({
-            'reference': reference,
-            'taps': singlecellmultiomics.molecule.TAPS(reference=reference)
-        })
-
-    elif args.method == 'chic_taps':
-
-        molecule_class_args.update({
-            'reference': reference,
-            'taps': singlecellmultiomics.molecule.TAPS(reference=reference)
-        })
-        moleculeClass = singlecellmultiomics.molecule.TAPSCHICMolecule
-        fragmentClass = singlecellmultiomics.fragment.CHICFragment
-
-    elif args.method == 'vasa' or args.method == 'cs':
-        moleculeClass = singlecellmultiomics.molecule.VASA
-        fragmentClass = singlecellmultiomics.fragment.SingleEndTranscript
+        fragment_class_args.update({'invert_strand': True})
 
-        molecule_class_args.update({
-            'pooling_method': 1,  # all data from the same cell can be dealt with separately
-            'stranded': 1  # data is stranded
-        })
-
-    else:
-        raise ValueError("Supply a valid method")
-
-    # This decides what molecules we will traverse
-    if args.contig == MISC_ALT_CONTIGS_SCMO:
-        contig = None
-    else:
-        contig = args.contig
-
-    # This decides to only extract a single genomic region:
-    if args.region_start is not None:
-        if args.region_end is None:
-            raise ValueError('When supplying -region_start then also supply -region_end')
-        region_start = args.region_start
-        region_end = args.region_end
-    else:
-        region_start = None
-        region_end = None
-
-    molecule_iterator_args = {
-        'alignments': input_bam,
-        'queryNameFlagger': queryNameFlagger,
-        'moleculeClass': moleculeClass,
-        'fragmentClass': fragmentClass,
-        'molecule_class_args': molecule_class_args,
-        'fragment_class_args': fragment_class_args,
-        'yield_invalid': yield_invalid,
-        'start':region_start,
-        'end':region_end,
-        'contig': contig,
-        'every_fragment_as_molecule': every_fragment_as_molecule
-    }
-
-    if args.contig == MISC_ALT_CONTIGS_SCMO:
-        # When MISC_ALT_CONTIGS_SCMO is set as argument, all molecules with reads
-        # mapping to a contig returning True from the is_main_chromosome
-        # function are used
-
-        def Misc_contig_molecule_generator(molecule_iterator_args):
-            for reference in input_bam.references:
-                if not is_main_chromosome(reference):
-                    molecule_iterator_args['contig'] = reference
-                    yield from MoleculeIterator(**molecule_iterator_args)
-
-        molecule_iterator = Misc_contig_molecule_generator(
-            molecule_iterator_args)
+    if args.transcriptome:
+        if args.method == 'nla':
+            molecule_class = singlecellmultiomics.molecule.AnnotatedTAPSNlaIIIMolecule
+            fragment_class = singlecellmultiomics.fragment.NlaIIIFragment
+        elif args.method == 'chic':
+            molecule_class = singlecellmultiomics.molecule.AnnotatedTAPSCHICMolecule
+            fragment_class = singlecellmultiomics.fragment.CHICFragment
+        else:
+            raise ValueError("Supply 'nla' or 'chic' for -method")
     else:
-        molecule_iterator = MoleculeIterator(**molecule_iterator_args)
+        if args.method == 'nla':
+            molecule_class = singlecellmultiomics.molecule.TAPSNlaIIIMolecule
+            fragment_class = singlecellmultiomics.fragment.NlaIIIFragment
+        elif args.method == 'chic':
+            molecule_class = singlecellmultiomics.molecule.TAPSCHICMolecule
+            fragment_class = singlecellmultiomics.fragment.CHICFragment
+        else:
+            raise ValueError("Supply 'nla' or 'chic' for -method")
 
-    #####
-    consensus_model_path = None
+    ###############################################
+    statistics = collections.defaultdict(collections.Counter)
+    mcs = collections.Counter()  # methylation calls seen
+    print(
+        colorama.Style.BRIGHT +
+        "Running TAPS tagging" +
+        colorama.Style.RESET_ALL)
+    if args.bed is not None:
+        bed = open(args.bed, "w")
+    with pysam.AlignmentFile(temp_out, "wb", header=alignments.header) as output:
+        for i, molecule in enumerate(
+                singlecellmultiomics.molecule.MoleculeIterator(
+                    alignments=alignments,
+                    molecule_class=molecule_class,
+                    fragment_class=fragment_class,
+                    fragment_class_args=fragment_class_args,
+                    yield_invalid=True,
+                    molecule_class_args=molecule_class_args,
+                    contig=args.contig
+                )):
+
+            if args.head is not None and i >= args.head:
+                print(
+                    colorama.Style.BRIGHT +
+                    colorama.Fore.RED +
+                    f"Head was supplied, stopped at {i} molecules" +
+                    colorama.Style.RESET_ALL)
+                break
+            statistics['Input']['molecules'] += 1
+            statistics['Input']['fragments'] += len(molecule)
 
-    if args.consensus:
-        # Load from path if available:
+            # Set (chromosome) unique identifier
+            molecule.set_meta('mi', f'NLA_{i}')
+            if args.transcriptome:
+                molecule.set_intron_exon_features()
+
+            if samples is not None and molecule.sample not in samples:
+                molecule.set_rejection_reason('sample_not_selected')
+                if output is not None:
+                    molecule.write_pysam(output)
+                continue
+
+            if args.transcriptome:
+                if not molecule.is_valid():
+                    if molecule.is_multimapped() or molecule.get_max_mapping_qual() < args.min_mq:
+                        molecule.set_meta('RF', 'rejected_molecule_mq')
+                        molecule.write_tags()
+                        molecule.write_pysam(output)
+                        statistics['Filtering']['low mapping quality'] += 1
+                        statistics['Filtering']['rejected'] += 1
+                        continue
 
-        if args.consensus_model is not None:
-            if os.path.exists(args.consensus_model):
-                model_path = args.consensus_model
-            else:
-                model_path = pkg_resources.resource_filename(
-                    'singlecellmultiomics', f'molecule/consensus_model/{args.consensus_model}')
-            with open(model_path, 'rb') as f:
-                consensus_model = pickle.load(f)
-        else:
-            skip_already_covered_bases = not args.consensus_allow_train_location_oversampling
-            if args.consensus_mask_variants is None:
-                mask_variants = None
+                    rejected_reads.append(molecule[0].reads)
+                    continue
+                statistics['Filtering'][f'valid {args.method} molecule'] += 1
+                if len(molecule.junctions):
+                    molecule.set_meta('RF', 'transcript_junction')
+                    molecule.set_meta('dt', 'RNA')
+                    statistics['Data type detection']['RNA because junction found'] += 1
+                else:
+                    if len(molecule.genes) == 0:
+                        molecule.set_meta('dt', 'DNA')
+                        statistics['Data type detection']['DNA not mapping to gene'] += 1
+                    else:
+                        # Check if NLA III sites are skipped...
+                        if args.method == 'nla':
+                            skipped = molecule.get_undigested_site_count()
+                            if skipped == 0:
+                                molecule.set_meta('dt', 'DNA')
+                            else:
+                                molecule.set_meta('dt', 'RNA or DNA')
+                        else:
+                            molecule.set_meta('dt', 'RNA or DNA')
             else:
-                mask_variants = pysam.VariantFile(args.consensus_mask_variants)
-            print("Fitting consensus model, this may take a long time")
-            consensus_model = singlecellmultiomics.molecule.train_consensus_model(
-                molecule_iterator,
-                mask_variants=mask_variants,
-                n_train=args.consensus_n_train,
-                skip_already_covered_bases=skip_already_covered_bases
-                )
-            # Write the consensus model to disk
-            consensus_model_path = os.path.abspath(
-                os.path.dirname(args.o)) + '/consensus_model.pickle.gz'
-            print(f'Writing consensus model to {consensus_model_path}')
-            with open(consensus_model_path, 'wb') as f:
-                pickle.dump(consensus_model, f)
-
-    # We needed to check if every argument is properly placed. If so; the jobs
-    # can be sent to the cluster
-    if args.cluster:
-        if args.contig is None:
-            # Create jobs for all chromosomes:
-            temp_prefix = os.path.abspath(os.path.dirname(
-                args.o)) + '/SCMO_' + str(uuid.uuid4())
-            hold_merge = []
-
-            found_alts = 0
-            for chrom in list(input_bam.references) + [MISC_ALT_CONTIGS_SCMO]:
-                if not is_main_chromosome(chrom):
-                    found_alts += 1
+                if not molecule.is_valid():
+                    statistics['Filtering'][f'not valid {args.method}'] += 1
+                    molecule.set_meta('RF', 'rejected_molecule')
+                    molecule.write_tags()
+                    molecule.write_pysam(output)
                     continue
-                if chrom == MISC_ALT_CONTIGS_SCMO and found_alts == 0:
+                statistics['Filtering'][f'valid {args.method} molecule'] += 1
+                molecule.set_meta('RF', 'accepted_molecule')
+
+            got_context_hit = False
+            methylated_hits = 0
+            unmethylated_hits = 0
+            readString = []
+            genomeString = []
+            for (chromosome, location), call in molecule.methylation_call_dict.items():
+                if call['context'] == '.':  # Only use calls concerning C's
                     continue
-                temp_bam_path = f'{temp_prefix}_{chrom}.bam'
-                arguments = " ".join(
-                    [x for x in sys.argv if not x == args.o and x != '-o']) + f" -contig {chrom} -o {temp_bam_path}"
-                if consensus_model_path is not None:
-                    arguments += f' -consensus_model {consensus_model_path}'
-                job = f'SCMULTIOMICS_{str(uuid.uuid4())}'
-                os.system(
-                    f'submission.py --silent' +
-                    f' -y --py36 -time {args.time} -t 1 -m {args.mem} -N {job} " {arguments};"')
-                hold_merge.append(job)
 
-            hold = ','.join(hold_merge)
-            os.system(
-                f'submission.py --silent' +
-                f' -y --py36 -time {args.time} -t 1 -m 10 -N {job} -hold {hold} " samtools merge -c {args.o} {temp_prefix}*.bam; samtools index {args.o}; rm {temp_prefix}*.ba*"')
-            exit()
+                got_context_hit += 1
+                mcs[call['context']] += 1
+                if call['context'].isupper():
+                    methylated_hits += 1
+                    readString.append(call['consensus'])
+                    genomeString.append(call['reference_base'])
+                else:
+                    unmethylated_hits += 1
+# NEED TO REMOVE THIS CODE ENTIRELY!! <- VB
+                if args.table is not None:
+                    for binIdx in singlecellmultiomics.utils.coordinate_to_bins(
+                            location, args.bin_size, args.sliding_increment):
+                        bin_start, bin_end = binIdx
+                        if bin_start < 0 or bin_end > ref_lengths[molecule.chromosome]:
+                            continue
+
+                        if args.stranded:
+                            binned_data[(chromosome, molecule.get_strand_repr(
+                            ), binIdx)][molecule.get_sample()][call['context'].isupper()] += 1
+                            cell_count[molecule.get_sample()] += 1
+                        else:
+                            binned_data[(chromosome, binIdx)][molecule.get_sample(
+                            )][call['context'].isupper()] += 1
+                            cell_count[molecule.get_sample()] += 1
+###
+                if args.bed is not None:
+                    # Skip non-selected contexts only for table
+                    if contexts is not None and call['context'] not in contexts:
+                        continue
+                    else:
+                        # name = cell barcode + context
+                        name = ":".join(
+                            [molecule.sample.split("_")[-1], call['context']])
+                        bed.write(
+                            f'{chromosome}\t{location}\t{location+1}\t{name}\t1\t{molecule.get_strand_repr()}\n')
+
+            refbase = '' if not genomeString else max(
+                set(genomeString), key=genomeString.count)
+            readbase = '' if not readString else max(
+                set(readString), key=readString.count)
+
+            readConversionString = None
+            genomeConversionString = None
+            # OT
+            readConversionString = None
+            genomeConversionString = None
+            if readbase == 'T' and refbase == 'C' and molecule.get_strand() == 1:  # '+'
+                readConversionString = 'CT'
+                genomeConversionString = 'CT'
+            # OB
+            elif readbase == 'A' and refbase == 'G' and molecule.get_strand() == 0:  # '-'
+                readConversionString = 'CT'
+                genomeConversionString = 'GA'
+            # CTOT
+            elif readbase == 'A' and refbase == 'C' and molecule.get_strand() == 1:  # '+'
+                readConversionString = 'GA'
+                genomeConversionString = 'CT'
+            # CTOB
+            elif readbase == 'A' and refbase == 'G' and molecule.get_strand() == 0:  # '-'
+                readConversionString = 'GA'
+                genomeConversionString = 'GA'
+
+            if readConversionString is not None:
+                molecule.set_meta('XR', readConversionString)
+            if genomeConversionString is not None:
+                molecule.set_meta('XG', genomeConversionString)
+
+            molecule.set_meta('ME', methylated_hits)
+            molecule.set_meta('um', unmethylated_hits)
+            statistics['Methylation']['methylated Cs'] += methylated_hits
+            statistics['Methylation']['unmethylated Cs'] += unmethylated_hits
+            molecule.write_tags()
+            molecule.write_pysam(output)
+# close bed
+    if args.bed is not None:
+        bed.close()
 
-    #####
-    # Load unphased variants to memory
-    unphased_allele_resolver = None
-    if args.unphased_alleles is not None:
-        unphased_allele_resolver = singlecellmultiomics.alleleTools.AlleleResolver(
-            phased=False, ignore_conversions=ignore_conversions)
-        try:
-            for i, variant in enumerate(
-                pysam.VariantFile(
-                    args.unphased_alleles).fetch(
-                    args.contig)):
-                if 'PASS' not in list(variant.filter):
-                    continue
-                if not all(
-                        len(allele) == 1 for allele in variant.alleles) or len(
-                        variant.alleles) != 2:
-                    continue
-                if sum([len(set(variant.samples[sample].alleles))
-                        == 2 for sample in variant.samples]) < 2:
-                    # Not heterozygous
-                    continue
+    if args.transcriptome:
+        print(
+            colorama.Style.BRIGHT +
+            f"Running transcriptome recovery on {len(rejected_reads)} reads")
+        for i, molecule in enumerate(
+            singlecellmultiomics.molecule.MoleculeIterator(
+                # plug in the possible_transcripts as read source
+                alignments=rejected_reads,
+                # Drop the TAPS and NLAIII checks
+                molecule_class=singlecellmultiomics.molecule.FeatureAnnotatedMolecule,
+                # Plain fragment, no NLAIII
+                fragment_class=singlecellmultiomics.fragment.Fragment,
+                fragment_class_args={
+                    'umi_hamming_distance': args.uhd,
+                    # this is the amount of bases R1 can shift to be assigned to the same molecule
+                    'assignment_radius': args.recovery_umi_pool_radius
+                },
+
+                yield_invalid=True,
+                molecule_class_args={
+                        'features': transcriptome_features,
+                    'reference': reference,
+                            'min_max_mapping_quality': 20
+                }
+            )):
+            if not molecule.is_valid():
+                statistics['Filtering']['rejected at transcriptome recovery step'] += 1
+                statistics['Filtering']['rejected'] += 1
+                molecule.set_meta('RF', 'rejected_recovery_invalid')
+                molecule.write_tags()
+                molecule.write_pysam(output)
+                continue
+
+            molecule.set_meta('mi', f'TRAN_{i}')
+
+            # Add gene annotations:
+            molecule.annotate(0)
+            molecule.set_intron_exon_features()
+            if len(molecule.genes) == 0:
+                molecule.set_meta('RF', 'rejected_recovery_no_gene')
+                statistics['Filtering']['rejected_recovery_no_gene'] += 1
+                molecule.write_tags()
+                molecule.write_pysam(output)
+                continue
+            if len(molecule.junctions):
+                molecule.set_meta('RF', 'recovered_transcript_junction')
+                statistics['Filtering']['recovered_transcript_junction'] += 1
+                statistics['Data type detection'][
+                    f'RNA because junction found and no {args.method} site mapped'] += 1
+            else:
+                molecule.set_meta('RF', 'recovered_transcript_gene')
+                statistics['Data type detection'][
+                    f'RNA because gene found and no {args.method} site mapped'] += 1
+                statistics['Filtering']['recovered_transcript_gene'] += 1
+            molecule.set_meta('dt', 'RNA')
+            statistics['Data type detection']['RNA'] += 1
+            molecule.write_tags()
+            molecule.write_pysam(output)
 
-                unphased_allele_resolver.locationToAllele[variant.chrom][variant.pos - 1] = {
-                    variant.alleles[0]: {'U'}, variant.alleles[1]: {'V'}}
-        except Exception as e:  # todo catch this more nicely
-            print(e)
-    out_bam_path = args.o
-
-    # Copy the header
-    input_header = input_bam.header.as_dict()
-
-    # Write provenance information to BAM header
-    write_program_tag(
-        input_header,
-        program_name='bamtagmultiome',
-        command_line=" ".join(
-            sys.argv),
-        version=singlecellmultiomics.__version__,
-        description=f'SingleCellMultiOmics molecule processing, executed at {datetime.now().strftime("%d/%m/%Y %H:%M:%S")}')
-
-    print(f'Started writing to {out_bam_path}')
-    read_groups = set()  # Store unique read groups in this set
-    with sorted_bam_file(out_bam_path, header=input_header, read_groups=read_groups) as out:
-
-        for i, molecule in enumerate(molecule_iterator):
-            # Stop when enough molecules are processed
-            if args.head is not None and (i - 1) >= args.head:
-                break
+    # Show statistics:
+    print(
+        '\n' +
+        colorama.Style.BRIGHT +
+        'Statistics' +
+        colorama.Style.RESET_ALL)
+    for statistic_class in [
+        'Input',
+        'Filtering',
+        'Data type detection',
+            'Methylation']:
+        print(f'{colorama.Style.BRIGHT} {statistic_class} {colorama.Style.RESET_ALL}')
+        for statistic, value in statistics[statistic_class].most_common():
+            print(f'  {statistic}\t{value}')
+
+    print(f'{colorama.Style.BRIGHT} Methylation calls {colorama.Style.RESET_ALL}')
+    for call, description in zip('zZxXhH',
+                                 ['unmethylated C in CpG context (CG)',
+                                  'methylated C in CpG context (CG)',
+                                  'unmethylated C in CHG context ( C[ACT]G )',
+                                  'methylated C in CHG context   ( C[ACT]G )',
+                                  'unmethylated C in CHH context ( C[ACT][ACT] )',
+                                  'methylated C in CHH context ( C[ACT][ACT] )'
+                                  ]):
+
+        if call.isupper():
+            print(
+                f'  {colorama.Style.BRIGHT}{call}{colorama.Style.RESET_ALL}\t{mcs[call]}',
+                end='\t')
+        else:
+            print(f'  {call}\t{mcs[call]}', end='\t')
+        print(f'{colorama.Style.DIM}{description}{colorama.Style.RESET_ALL}')
 
-            # set unique molecule identifier
-            molecule.set_meta('mi', f'{molecule.get_a_reference_id()}_{i}')
+    print('\n')
 
-            # Write tag values
-            molecule.write_tags()
+    if args.table is not None:
+        print(
+            colorama.Style.BRIGHT +
+            'Writing raw unmethylated counts' +
+            colorama.Style.RESET_ALL)
+        # Write raw counts:
+        df = pd.DataFrame(
+            {loc: {sample: binned_data[loc][sample][0] for sample in binned_data[loc]} for loc in binned_data})
+        df.to_pickle(f'{args.table}_unmethylated_{args.contig}.pickle.gz')
+        df.to_csv(f'{args.table}_unmethylated_{args.contig}.csv')
+        del df
 
-            if unphased_allele_resolver is not None:  # write unphased allele tag:
-                molecule.write_allele_phasing_information_tag(
-                    unphased_allele_resolver, 'ua')
-
-            # Update read groups
-            for fragment in molecule:
-                read_groups.add(fragment.get_read_group())
-
-            # Calculate molecule consensus
-            if args.consensus:
-                try:
-                    consensus_reads = molecule.deduplicate_to_single_CIGAR_spaced(
-                        out,
-                        f'consensus_{molecule.get_a_reference_id()}_{i}',
-                        consensus_model)
-                    for consensus_read in consensus_reads:
-                        consensus_read.set_tag('RG', molecule[0].get_read_group())
-                        consensus_read.set_tag('mi', i)
-                        out.write(consensus_read)
-                except Exception as e:
-                    molecule.set_rejection_reason('CONSENSUS_FAILED',set_qcfail=True)
-                    molecule.write_pysam(out)
-
-
-            # Write the reads to the output file
-            if not args.no_source_reads:
-                molecule.write_pysam(out)
+        print(
+            colorama.Style.BRIGHT +
+            'Writing raw methylated counts' +
+            colorama.Style.RESET_ALL)
+        df = pd.DataFrame(
+            {loc: {sample: binned_data[loc][sample][1] for sample in binned_data[loc]} for loc in binned_data})
+        df.to_pickle(f'{args.table}_methylated_{args.contig}.pickle.gz')
+        df.to_csv(f'{args.table}_methylated_{args.contig}.csv')
+        del df
 
+        print(
+            colorama.Style.BRIGHT +
+            'Writing ratio tables' +
+            colorama.Style.RESET_ALL)
+        # cast all fractions to float
+        for loc in binned_data:
+            for sample in binned_data[loc]:
+                binned_data[loc][sample] = float(binned_data[loc][sample])
+        df = pd.DataFrame(binned_data)
+        del binned_data
+        if args.contig:
+            df.to_pickle(f'{args.table}_ratio_{args.contig}.pickle.gz')
+            df.to_csv(f'{args.table}_ratio_{args.contig}.csv')
+        else:
+            df.to_pickle(f'{args.table}_ratio.pickle.gz')
+            df.to_csv(f'{args.table}_ratio.csv')
 
-if __name__ == '__main__':
-    args = argparser.parse_args()
-    run_multiome_tagging(args)
+    print(
+        colorama.Style.BRIGHT +
+        'Sorting and indexing final file' +
+        colorama.Style.RESET_ALL)
+    # Sort and index
+    # Perform a reheading, sort and index
+    if not args.no_sort_index:
+        cmd = f"""samtools sort {temp_out} > {args.o}; samtools index {args.o};
+        rm {temp_out};
+        """
+    else:
+        cmd = f"mv {temp_out} {args.o}"
+    os.system(cmd)
+    print("All done.")
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/customreads.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/customreads.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         for read in reads:
             if read is None:
                 continue
             origin, mi_tag, cell_barcode, umi, cell_index = read.query_name.rsplit(
                 ':', 4)
             read.set_tag('MI', mi_tag)
             read.set_tag('RX', umi)
-            read.set_tag('BI', int(cell_index))
+            read.set_tag('bi', int(cell_index))
             read.set_tag('SM', cell_barcode)
 
 
 class CustomAssingmentQueryNameFlagger(DigestFlagger):
     """This query name flagger converts values between colons ":"  to tags"""
 
     def __init__(self, block_assignments, **kwargs):
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/digest.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/digest.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/mspjI.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/mspjI.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/nlaIII.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/nlaIII.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/rna.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/rna.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/scar.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/scar.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/scchic.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/scchic.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/tag.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/tag.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/taps.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/taps.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/tapsTabulator.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/tapsTabulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,29 +90,29 @@
 
     molecule_class_args = {
         'reference': reference,
         'taps': taps,
         'min_max_mapping_quality': args.minmq
     }
     if args.method == 'nla':
-        moleculeClass = singlecellmultiomics.molecule.TAPSNlaIIIMolecule
-        fragmentClass = singlecellmultiomics.fragment.NLAIIIFragment
+        molecule_class = singlecellmultiomics.molecule.TAPSNlaIIIMolecule
+        fragment_class = singlecellmultiomics.fragment.NlaIIIFragment
         molecule_class_args.update({'site_has_to_be_mapped': True})
     elif args.method == 'chic':
-        moleculeClass = singlecellmultiomics.molecule.TAPSCHICMolecule
-        fragmentClass = singlecellmultiomics.fragment.CHICFragment
+        molecule_class = singlecellmultiomics.molecule.TAPSCHICMolecule
+        fragment_class = singlecellmultiomics.fragment.CHICFragment
     else:
         raise ValueError("Supply 'nla' or 'chic' for -method")
 
     try:
         for i, molecule in enumerate(singlecellmultiomics.molecule.MoleculeIterator(
             alignments=alignments,
-            moleculeClass=moleculeClass,
+            molecule_class=molecule_class,
             yield_invalid=(output is not None),
-            fragmentClass=fragmentClass,
+            fragment_class=fragment_class,
             fragment_class_args={'umi_hamming_distance': 1},
 
                 molecule_class_args=molecule_class_args,
                 contig=args.contig)):
 
             if args.head and (i - 1) >= args.head:
                 break
@@ -143,9 +143,10 @@
                 elif args.fmt == "bed":
                     sample = molecule.sample.split("_")[-1]
                     print(
                         f'{chromosome}\t{location}\t{location+1}\t{sample}\t1\t{molecule.get_strand_repr()}')
 
     except (KeyboardInterrupt, BrokenPipeError) as e:
         pass
-if output is not None:
-    finish_bam(output, args, temp_out)
+
+    if output is not None:
+        finish_bam(output, args, temp_out)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/tapsTagger.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/universalBamTagger/universalBamTagger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,572 +1,709 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+import re
 import pysam
-import singlecellmultiomics.molecule
-import singlecellmultiomics.fragment
-import gzip
-import collections
-import matplotlib.pyplot as plt
-import pandas as pd
-import argparse
-import pysamiterators
+import time
 import sys
+import multiprocessing
+import subprocess
 import os
-import uuid
-import singlecellmultiomics.bamProcessing.bamFunctions as bf
-import singlecellmultiomics.features
-import colorama
+from singlecellmultiomics.utils.sequtils import hamming_distance, phred_to_prob
+from singlecellmultiomics.universalBamTagger.taps import TAPSFlagger
+from singlecellmultiomics.universalBamTagger.tag import TagFlagger
+from singlecellmultiomics.universalBamTagger.scar import ScarFlagger
+from singlecellmultiomics.universalBamTagger.mspjI import MSPJIFlagger
+from singlecellmultiomics.universalBamTagger.scchic import ChicSeqFlagger
+from singlecellmultiomics.universalBamTagger.nlaIII import NlaIIIFlagger
+from singlecellmultiomics.universalBamTagger.digest import DigestFlagger
+from singlecellmultiomics.universalBamTagger.rna import RNA_Flagger
+import warnings
 import numpy as np
+import math
+import singlecellmultiomics.features
+import singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods
+from singlecellmultiomics.tagtools import tagtools
+import argparse
+import pysamiterators.iterators as pysamIterators
+import gzip
+import pickle
+from singlecellmultiomics.alleleTools import alleleTools
+import uuid
+import collections
+import glob
+c = 1_000  # !!! PLEASE USE PYTHON 3.6 OR HIGHER !!!
+complement = str.maketrans('ATGC', 'TACG')
 
 
-class Fraction:
-    def __init__(self):
-        self.values = [0, 0]
-
-    def __setitem__(self, key, value):
-        self.values[key] = value
-
-    def __getitem__(self, key):
-        return self.values[key]
+warnings.warn(
+    "universalBamTagger is deprecated. Please switch to use bamtagmultiome.py ",
+    DeprecationWarning)
 
-    def __float__(self):
-        if sum(self.values) == 0:
-            return np.nan
-        return self.values[1] / (self.values[1] + self.values[0])
 
+# Modules:
 
-if __name__ == '__main__':
 
+if __name__ == "__main__":
     argparser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description='Add methylation information to BAM file')
+        description="""Add allelic NLA and/or MSPJI digest information to a demultiplexed bam file
+    Adds the following tags:
+    RC: number of oversequenced molecules
+    DT: Source type (NLA/MSPJI/RNA.. )
+    DA: Digest allele
+    RP: Recognized sequence
+    RS: Recognized strand '-','?','+'
 
-    argparser.add_argument('alignmentfile', type=str)
-    argparser.add_argument(
-        '-o',
-        type=str,
-        help="output BAM path",
-        required=True)
+    Which tags are filled in depends on which files you supply, for example if you do not supply an allelic VCF file, then no allele tag will be added
+    """)
+
+    argparser.add_argument('bamfiles', metavar='bamfile', type=str, nargs='+')
     argparser.add_argument(
-        '-bed',
-        type=str,
-        help="output bed file (base-level methylation status)",
-        default=None,
-        required=False)
-    # these options need to go <- VB
+        '--local',
+        action='store_true',
+        help='Do not qsub sorting and indexing [deprecated]')
     argparser.add_argument(
-        '-table',
+        '-tmpprefix',
+        metavar='PREFIX.nnnn.bam',
+        help='When sorting, specify temp dir to prevent home directory filling up',
+        default='~/')
+    #argparser.add_argument('--noSort', action='store_true', help='Do not sort and index')
+    #argparser.add_argument('--cluster', action='store_true', help='Do not qsub sorting and indexing')
+
+    tagAlgs = argparser.add_argument_group('Tagging algorithms', '')
+    tagAlgs.add_argument(
+        '--ftag',
+        action='store_true',
+        help='!DEPRECATED, this flag is now always used!')
+    tagAlgs.add_argument(
+        '--atag',
+        action='store_true',
+        help='Add only allele tags')
+    tagAlgs.add_argument(
+        '--mspji',
+        action='store_true',
+        help='Look for mspji digest')
+    tagAlgs.add_argument(
+        '--nla',
+        action='store_true',
+        help='Look for nlaIII digest')
+    tagAlgs.add_argument(
+        '--chic',
+        action='store_true',
+        help='Look for mnase (scCHIC) digest')
+    tagAlgs.add_argument(
+        '--scar',
+        action='store_true',
+        help='Create R1 start, cigar sequence based DS tags')
+    tagAlgs.add_argument(
+        '--taps',
+        action='store_true',
+        help='Add TAPS based methylation state ')
+    tagAlgs.add_argument(
+        '-tag',
         type=str,
-        help="output table alias",
         default=None,
-        required=False)
-    argparser.add_argument('-bin_size', type=int, default=250_000)
-    argparser.add_argument('-sliding_increment', type=int, default=50_000)
-    #
+        help='Determine oversequencing based on a tag (for example XT to count RNA oversequencing for featureCounts counted transcripts. chrom for chromosome/contig count)')
+
+    # RNA options
+    tagAlgs.add_argument(
+        '--rna',
+        action='store_true',
+        help='Assign RNA molecules, requires a intronic and exonic GTF file')
     argparser.add_argument(
-        '-ref',
+        '-introns',
         type=str,
-        required=False,
-        help='path to reference fasta file ')
+        help='Intronic GTF file, use exonGTFtoIntronGTF.py to generate such a GTF file')
+    argparser.add_argument('-exons', type=str, help='Exonic GTF file.')
+    """
+    How much bases of the fragment fall inside the intron(s)
+    How much bases of the fragment fall inside the exon(s)
+    is the fragment spliced? How many bases are spliced out?
+    """
+
     argparser.add_argument(
-        '-min_mq',
-        default=20,
+        '-moleculeRadius',
         type=int,
-        help='Min mapping qual')
-    argparser.add_argument('-uhd', default=1, type=int,
-                           help='Umi hamming distance')
+        help='Search radius for each molecule, if a cut site is found within this range with the same umi, it will be counted as the same molecule',
+        default=0)
+
     argparser.add_argument(
-        '-mem',
-        default=40,
-        type=int,
-        help='Memory used per job')
+        '-alleles',
+        type=str,
+        help='VCF file. Add allelic info flag based on vcf file')
     argparser.add_argument(
-        '-time',
-        default=52,
-        type=int,
-        help='Time requested per job')
-    argparser.add_argument('-head', type=int)
-    argparser.add_argument('-contig', type=str, help='contig to run on')
-    argparser.add_argument('-method', type=str, help='nla or chic')
+        '--loadAllelesToMem',
+        action='store_true',
+        help='Load allele data completely into memory')
+
+    argparser.add_argument('-ref', type=str, help='reference FASTA file.')
     argparser.add_argument(
-        '-samples',
+        '-o',
         type=str,
-        help='Samples to select, separate with comma. For example CellA,CellC,CellZ',
-        default=None)
+        default='./tagged',
+        help='output folder')
     argparser.add_argument(
-        '-context',
-        type=str,
-        help='Context to select, separate with comma. For example Z,H,X',
-        default=None)
+        '--dedup',
+        action='store_true',
+        help='Create deduplicated bam files')
+
+    argparser.add_argument('-chr', help='run only on this chromosome')
 
-    argparser.add_argument('--stranded', action='store_true')
     argparser.add_argument(
-        '--cluster',
+        '-head',
+        type=int,
+        default=None,
+        help='Only process first n reads of every bam file')
+
+    devArgs = argparser.add_argument_group('Development options', '')
+    devArgs.add_argument(
+        '--fatal',
         action='store_true',
-        help='split by chromosomes and submit the job on cluster')
-    argparser.add_argument(
-        '--no_sort_index',
+        help='Crash upon any encountered error')
+    devArgs.add_argument('--verbose', action='store_true', help='Be verbose')
+    devArgs.add_argument(
+        '--knh',
         action='store_true',
-        help='do not sort and index the output bam')
+        help='Keep non-headered bam file')
 
-    # Transcriptome splitting mode
-    tr = argparser.add_argument_group('transcriptome specific settings')
-    tr.add_argument(
-        '--transcriptome',
-        action='store_true',
-        help='Label transcripts, requires exons and introns')
-    tr.add_argument('-exons', type=str, help='Exon GTF file')
-    tr.add_argument(
-        '-introns',
-        type=str,
-        help='Intron GTF file, use exonGTF_to_intronGTF.py to create this file')
-    tr.add_argument(
-        '-recovery_umi_pool_radius',
-        type=int,
-        help='BP radius. When assigning transcripts without NLA site found, use this radius for molecule pooling',
-        default=4)
     args = argparser.parse_args()
 
-    samples = None if args.samples is None else set(args.samples.split(','))
-    contexts = None if args.context is None else set(args.context.split(','))
-#    set(
-#        [x.upper() for x in  args.context.split(',')] +
-#        [x.lower() for x in  args.context.split(',')])
-
-    alignments = pysam.AlignmentFile(args.alignmentfile)
-    # Auto detect reference:
-    if args.ref is None:
-        args.ref = bf.get_reference_from_pysam_alignmentFile(alignments)
-        if args.ref is None:
-            raise ValueError("Supply reference, -ref")
-
-    if args.transcriptome:
-        print(
-            colorama.Style.BRIGHT +
-            'Running in transcriptome recovery mode' +
-            colorama.Style.RESET_ALL)
-        if args.exons is None or args.introns is None:
-            raise ValueError("Please supply both intron and exon GTF files")
-
-    if args.cluster:
-        if args.contig is None:
-            # Create jobs for all chromosomes:
-            temp_prefix = os.path.abspath(
-                os.path.dirname(args.o)) + '/' + str(uuid.uuid4())
-            hold_merge = []
-            for chrom in alignments.references:
-                if chrom.startswith('KN') or chrom.startswith('KZ') or chrom.startswith(
-                        'chrUn') or chrom.endswith('_random') or 'ERCC' in chrom:
-                    continue
-                temp_bam_path = f'{temp_prefix}_{chrom}.bam'
-                temp_bed_path = f'{temp_prefix}_{chrom}.bed'
-
-                arguments = " ".join([x for x in sys.argv if not x == args.o and x != '-o']) + \
-                    f" -contig {chrom} -o {temp_bam_path} -bed {temp_bed_path}"
-
-                job = f'TAPS_{str(uuid.uuid4())}'
-                os.system(
-                    f'submission.py --silent' +
-                    f' -y --py36 -time {args.time} -t 1 -m {args.mem} -N {job} " {arguments};"')
-                hold_merge.append(job)
-
-            hold = ','.join(hold_merge)
-            os.system(
-                f'submission.py --silent' +
-                f' -y --py36 -time {args.time} -t 1 -m 10 -N {job} -hold {hold} " samtools merge {args.o} {temp_prefix}*.bam; samtools index {args.o}; rm {temp_prefix}*.ba*; cat {temp_prefix}*.bed > {args.bed}; rm {temp_prefix}*.bed"')
-            exit()
-
-    reference = pysamiterators.iterators.CachedFasta(pysam.FastaFile(args.ref))
-    taps = singlecellmultiomics.molecule.TAPS(reference=reference)
-    temp_out = f'{args.o}.temp.out.bam'
-
-    # Obtain contig sizes:
-    ref_lengths = {r: alignments.get_reference_length(
-        r) for r in alignments.references}
-
-    # Methylation dictionary: site->cell->value
-    binned_data = collections.defaultdict(
-        lambda: collections.defaultdict(Fraction))
-    cell_count = collections.Counter()
-
-    # Define molecule class arguments
-    molecule_class_args = {
-        'reference': reference,
-        'taps': taps,
-        'min_max_mapping_quality': args.min_mq
-    }
+    if not args.mspji and not args.nla and not args.chic and not args.ftag and not args.rna and args.tag is None and args.atag is None and args.taps is None:
+        raise ValueError(
+            'Please supply any or a combination of --ftag --nla --chic --mspji --taps')
+
+    if args.rna and (args.introns is None or args.exons is None):
+        raise ValueError(
+            'Please supply exonic and intronic GTF files -introns -exons')
+
+    """
+    Corrected Tags
+    BC: This should be used for the sample-barcode so that there is no conflict in case that both sample- and molecular-barcodes are used
+    QT: This should be the quality for the sample-barcode BC
+
+    New Tags
+    RX: The raw sequence bases of the molecular-barcode(s) of the read(s) can be placed in this tag
+    QX: The original qualites (as QUAL) of the bases in RX
+
+    BX: Sequence bases of the unique molecular identifier, may be corrected or raw
+    BZ: Quality score the unique molecular identifier. May be corrected or raw. See BX tag for qualities
+
+    MI: Molecular-barcode sequence or identifier, may include non-sequence bases (Here, it is BC+RX)
+    QM: Molecular-barcode qualities, QT+QX
+
+    DS: coordinate of site
+    RC: number of oversequenced molecules
+    DT: Source type (NLA/MSPJI/RNA..? )
+    DA: Digest allele
+    RP: Recognized sequence
+    RS: Recognized strand '-','?','+'
+    LI: ligation sequence
+
+    """
+
+
+# 1: read1 2: read2
+def molecule_to_random_primer_dict(molecule, primer_length=6, primer_read=2):
+    rp = collections.defaultdict(list)
+    for fragment in molecule:
+        if fragment[primer_read - 1] is not None:
+            hstart, hseq = tagtools.getRandomPrimerHash(
+                fragment[primer_read - 1], onStart=True, primerLength=6)
+            rp[hstart, hseq].append(fragment)
+    return rp
+    # for k,p in rp.items():
+    #    yield p
+
+
+class MoleculeIterator_OLD():
+    """
+    Iterate over molecules in a bam file
+
+    Parameters
+    ----------
+    alignmentfile : pysam.AlignmentFile
+        file to read the molecules from
+
+    look_around_radius : int
+        buffer to accumulate molecules in. All fragments belonging to one molecule should fit this radius
+
+    umi_hamming_distance : int
+        Edit distance on UMI, 0: only exact match, 1: single base distance
+
+    sample_select : iterable
+        Iterable of samples to only select molecules from
+
+    Yields
+    ----------
+    list of molecules : list [ pysam.AlignedSegment ]
+    [ (R1,R2), (R1,R2) ... ]
+
+    """
+
+    def __init__(self,
+                 alignmentfile,
+                 look_around_radius=100_000,
+                 umi_hamming_distance=0,  # 0: only exact match, 1: single base distance
+                 sample_select=None,  # iterable of samples to only select molecules from
+                 # when a string is supplied only a single sample is selected
+
+                 **pysam_kwargs
+                 ):
+        self.alignmentfile = alignmentfile
+        self.look_around_radius = look_around_radius
+
+        self.current_position = None
+        self.current_chromosome = None
+        self.molecules_yielded = 0
+        self.umi_hamming_distance = umi_hamming_distance
+        self.pysam_kwargs = pysam_kwargs
+
+        self.sample_select = sample_select
+        self.sample_tag = 'SM'
+        self._clear()
+
+        self.filter_function = None  # function which results given two reads if it is usable
+
+    def _clear(self):
+        self.molecule_cache = collections.defaultdict(lambda: collections.defaultdict(
+            list))  # position -> cell,umi,strand,allele.. -> reads
+
+    def sample_assignment_function(self, fragment):
+        for read in fragment:
+            if read is not None:
+                if read.has_tag(self.sample_tag):
+                    return read.get_tag(self.sample_tag)
+        return None
+
+    # Returns postion unique identifier for a fragment
+    def localisation_function(self, fragment):
+        if not fragment[0].has_tag('DS'):
+            return None
+        return fragment[0].get_tag('DS')
+
+    def __repr__(self):
+        return f"""Molecule iterator
+        current position: {self.current_chromosome}:{self.current_position}
+        yielded {self.molecules_yielded} so far
+        currently {len(self.molecule_cache)} positions cached
+        keeping {self.get_cached_fragment_count()} fragments cached
+        """
 
-    fragment_class_args = {'umi_hamming_distance': args.uhd}
+    def get_cached_fragment_count(self):
+        total_fragments = 0
+        for position, data_per_molecule in self.molecule_cache.items():
+            for molecule_id, molecule_reads in data_per_molecule.items():
+                total_fragments += len(molecule_reads)
+        return total_fragments
+
+    def assignment_function(self, fragment):
+        return fragment[0].get_tag('SM'), fragment[0].get_tag(
+            'RX'), fragment[0].get_tag('RS')
+
+    # Returns True if two fragment ids  are identical or close enough
+    def eq_function(self, assignment_a, assignment_b):
+        if assignment_a is None or assignment_b is None:
+            return False
 
-    # transcriptome mode specific arguments: ####
-    if args.transcriptome:
+        sample_A, umi_A, strand_A = assignment_a
+        sample_B, umi_B, strand_B = assignment_b
 
-        transcriptome_features = singlecellmultiomics.features.FeatureContainer()
-        print("Loading exons", end='\r')
-        transcriptome_features.loadGTF(
-            args.exons,
-            select_feature_type=['exon'],
-            identifierFields=(
-                'exon_id',
-                'gene_id'),
-            store_all=True,
-            contig=args.contig,
-            head=None)
-
-        print("Loading introns", end='\r')
-        transcriptome_features.loadGTF(
-            args.introns,
-            select_feature_type=['intron'],
-            identifierFields=['transcript_id'],
-            store_all=True,
-            contig=args.contig,
-            head=None)
-        print("All features loaded")
-
-        rejected_reads = []  # Store all rejected, potential transcript reads
-
-        # Add more molecule class arguments
-        molecule_class_args.update({
-            'features': transcriptome_features
-        })
-
-    # Method specific arguments
-    if args.method == 'nla':
-        molecule_class_args.update({'site_has_to_be_mapped': True})
-    elif args.method == 'chic':
-        fragment_class_args.update({'invert_strand': True})
-
-    if args.transcriptome:
-        if args.method == 'nla':
-            moleculeClass = singlecellmultiomics.molecule.AnnotatedTAPSNlaIIIMolecule
-            fragmentClass = singlecellmultiomics.fragment.NLAIIIFragment
-        elif args.method == 'chic':
-            moleculeClass = singlecellmultiomics.molecule.AnnotatedTAPSCHICMolecule
-            fragmentClass = singlecellmultiomics.fragment.CHICFragment
-        else:
-            raise ValueError("Supply 'nla' or 'chic' for -method")
-    else:
-        if args.method == 'nla':
-            moleculeClass = singlecellmultiomics.molecule.TAPSNlaIIIMolecule
-            fragmentClass = singlecellmultiomics.fragment.NLAIIIFragment
-        elif args.method == 'chic':
-            moleculeClass = singlecellmultiomics.molecule.TAPSCHICMolecule
-            fragmentClass = singlecellmultiomics.fragment.CHICFragment
+        if sample_A != sample_B or strand_A != strand_B:
+            return False
+
+        if self.umi_hamming_distance == 0:
+            return umi_A == umi_B
         else:
-            raise ValueError("Supply 'nla' or 'chic' for -method")
+            return hamming_distance(umi_A, umi_B) <= self.umi_hamming_distance
 
-    ###############################################
-    statistics = collections.defaultdict(collections.Counter)
-    mcs = collections.Counter()  # methylation calls seen
-    print(
-        colorama.Style.BRIGHT +
-        "Running TAPS tagging" +
-        colorama.Style.RESET_ALL)
-    if args.bed is not None:
-        bed = open(args.bed, "w")
-    with pysam.AlignmentFile(temp_out, "wb", header=alignments.header) as output:
-        for i, molecule in enumerate(
-                singlecellmultiomics.molecule.MoleculeIterator(
-                    alignments=alignments,
-                    moleculeClass=moleculeClass,
-                    fragmentClass=fragmentClass,
-                    fragment_class_args=fragment_class_args,
-                    yield_invalid=True,
-                    molecule_class_args=molecule_class_args,
-                    contig=args.contig
-                )):
-
-            if args.head is not None and i >= args.head:
-                print(
-                    colorama.Style.BRIGHT +
-                    colorama.Fore.RED +
-                    f"Head was supplied, stopped at {i} molecules" +
-                    colorama.Style.RESET_ALL)
-                break
-            statistics['Input']['molecules'] += 1
-            statistics['Input']['fragments'] += len(molecule)
-
-            # Set (chromosome) unique identifier
-            molecule.set_meta('mi', f'NLA_{i}')
-            if args.transcriptome:
-                molecule.set_intron_exon_features()
-
-            if samples is not None and molecule.sample not in samples:
-                molecule.set_rejection_reason('sample_not_selected')
-                if output is not None:
-                    molecule.write_pysam(output)
+    def _yield_all_in_current_cache(self):
+        for position, data_per_molecule in self.molecule_cache.items():
+            for molecule_id, molecule_reads in data_per_molecule.items():
+                self.molecules_yielded += 1
+                yield molecule_reads
+        self._clear()
+
+    def _purge(self):
+        drop = []
+        for pos in self.molecule_cache:
+            if pos < (self.current_position - self.look_around_radius):
+                # purge this coordinate:
+                for molecule_id, molecule_reads in self.molecule_cache[pos].items(
+                ):
+                    self.molecules_yielded += 1
+                    yield molecule_reads
+                drop.append(pos)
+
+        for pos in drop:
+            del self.molecule_cache[pos]
+
+    def get_fragment_chromosome(self, fragment):
+        for read in fragment:
+            if read is not None:
+                return read.reference_name
+
+    def __iter__(self):
+        for fragment in pysamIterators.MatePairIterator(
+                self.alignmentfile,
+                **self.pysam_kwargs,
+                performProperPairCheck=False):
+
+            if fragment[0] is None or fragment[0].reference_name is None:
                 continue
 
-            if args.transcriptome:
-                if not molecule.is_valid():
-                    if molecule.is_multimapped() or molecule.get_max_mapping_qual() < args.min_mq:
-                        molecule.set_meta('RF', 'rejected_molecule_mq')
-                        molecule.write_tags()
-                        molecule.write_pysam(output)
-                        statistics['Filtering']['low mapping quality'] += 1
-                        statistics['Filtering']['rejected'] += 1
+            # Check if we want to drop the fragment because its corresponding
+            # sample is not selected
+            if self.sample_select is not None:
+                sample = self.sample_assignment_function(fragment)
+                if isinstance(self.sample_select, str):  # single sample
+                    if self.sample_select != sample:
                         continue
-
-                    rejected_reads.append(molecule[0].reads)
-                    continue
-                statistics['Filtering'][f'valid {args.method} molecule'] += 1
-                if len(molecule.junctions):
-                    molecule.set_meta('RF', 'transcript_junction')
-                    molecule.set_meta('dt', 'RNA')
-                    statistics['Data type detection']['RNA because junction found'] += 1
-                else:
-                    if len(molecule.genes) == 0:
-                        molecule.set_meta('dt', 'DNA')
-                        statistics['Data type detection']['DNA not mapping to gene'] += 1
-                    else:
-                        # Check if NLA III sites are skipped...
-                        if args.method == 'nla':
-                            skipped = molecule.get_undigested_site_count()
-                            if skipped == 0:
-                                molecule.set_meta('dt', 'DNA')
-                            else:
-                                molecule.set_meta('dt', 'RNA or DNA')
-                        else:
-                            molecule.set_meta('dt', 'RNA or DNA')
-            else:
-                if not molecule.is_valid():
-                    statistics['Filtering'][f'not valid {args.method}'] += 1
-                    molecule.set_meta('RF', 'rejected_molecule')
-                    molecule.write_tags()
-                    molecule.write_pysam(output)
-                    continue
-                statistics['Filtering'][f'valid {args.method} molecule'] += 1
-                molecule.set_meta('RF', 'accepted_molecule')
-
-            got_context_hit = False
-            methylated_hits = 0
-            unmethylated_hits = 0
-            readString = []
-            genomeString = []
-            for (chromosome, location), call in molecule.methylation_call_dict.items():
-                if call['context'] == '.':  # Only use calls concerning C's
-                    continue
-
-                got_context_hit += 1
-                mcs[call['context']] += 1
-                if call['context'].isupper():
-                    methylated_hits += 1
-                    readString.append(call['consensus'])
-                    genomeString.append(call['reference_base'])
-                else:
-                    unmethylated_hits += 1
-# NEED TO REMOVE THIS CODE ENTIRELY!! <- VB
-                if args.table is not None:
-                    for binIdx in singlecellmultiomics.utils.coordinate_to_bins(
-                            location, args.bin_size, args.sliding_increment):
-                        bin_start, bin_end = binIdx
-                        if bin_start < 0 or bin_end > ref_lengths[molecule.chromosome]:
-                            continue
-
-                        if args.stranded:
-                            binned_data[(chromosome, molecule.get_strand_repr(
-                            ), binIdx)][molecule.get_sample()][call['context'].isupper()] += 1
-                            cell_count[molecule.get_sample()] += 1
-                        else:
-                            binned_data[(chromosome, binIdx)][molecule.get_sample(
-                            )][call['context'].isupper()] += 1
-                            cell_count[molecule.get_sample()] += 1
-###
-                if args.bed is not None:
-                    # Skip non-selected contexts only for table
-                    if contexts is not None and call['context'] not in contexts:
+                else:  # list or set of samples
+                    if sample not in self.sample_select:
                         continue
-                    else:
-                        # name = cell barcode + context
-                        name = ":".join(
-                            [molecule.sample.split("_")[-1], call['context']])
-                        bed.write(
-                            f'{chromosome}\t{location}\t{location+1}\t{name}\t1\t{molecule.get_strand_repr()}\n')
-
-            refbase = '' if not genomeString else max(
-                set(genomeString), key=genomeString.count)
-            readbase = '' if not readString else max(
-                set(readString), key=readString.count)
-
-            readConversionString = None
-            genomeConversionString = None
-            # OT
-            readConversionString = None
-            genomeConversionString = None
-            if readbase == 'T' and refbase == 'C' and molecule.get_strand() == 1:  # '+'
-                readConversionString = 'CT'
-                genomeConversionString = 'CT'
-            # OB
-            elif readbase == 'A' and refbase == 'G' and molecule.get_strand() == 0:  # '-'
-                readConversionString = 'CT'
-                genomeConversionString = 'GA'
-            # CTOT
-            elif readbase == 'A' and refbase == 'C' and molecule.get_strand() == 1:  # '+'
-                readConversionString = 'GA'
-                genomeConversionString = 'CT'
-            # CTOB
-            elif readbase == 'A' and refbase == 'G' and molecule.get_strand() == 0:  # '-'
-                readConversionString = 'GA'
-                genomeConversionString = 'GA'
-
-            if readConversionString is not None:
-                molecule.set_meta('XR', readConversionString)
-            if genomeConversionString is not None:
-                molecule.set_meta('XG', genomeConversionString)
-
-            molecule.set_meta('ME', methylated_hits)
-            molecule.set_meta('um', unmethylated_hits)
-            statistics['Methylation']['methylated Cs'] += methylated_hits
-            statistics['Methylation']['unmethylated Cs'] += unmethylated_hits
-            molecule.write_tags()
-            molecule.write_pysam(output)
-# close bed
-    if args.bed is not None:
-        bed.close()
-
-    if args.transcriptome:
-        print(
-            colorama.Style.BRIGHT +
-            f"Running transcriptome recovery on {len(rejected_reads)} reads")
-        for i, molecule in enumerate(
-            singlecellmultiomics.molecule.MoleculeIterator(
-                # plug in the possible_transcripts as read source
-                alignments=rejected_reads,
-                # Drop the TAPS and NLAIII checks
-                moleculeClass=singlecellmultiomics.molecule.FeatureAnnotatedMolecule,
-                # Plain fragment, no NLAIII
-                fragmentClass=singlecellmultiomics.fragment.Fragment,
-                fragment_class_args={
-                    'umi_hamming_distance': args.uhd,
-                    # this is the amount of bases R1 can shift to be assigned to the same molecule
-                    'assignment_radius': args.recovery_umi_pool_radius
-                },
-
-                yield_invalid=True,
-                molecule_class_args={
-                        'features': transcriptome_features,
-                    'reference': reference,
-                            'min_max_mapping_quality': 20
-                }
-            )):
-            if not molecule.is_valid():
-                statistics['Filtering']['rejected at transcriptome recovery step'] += 1
-                statistics['Filtering']['rejected'] += 1
-                molecule.set_meta('RF', 'rejected_recovery_invalid')
-                molecule.write_tags()
-                molecule.write_pysam(output)
-                continue
 
-            molecule.set_meta('mi', f'TRAN_{i}')
+            # We went to another chromsome, purge all in cache:
+            if self.get_fragment_chromosome(
+                    fragment) != self.current_chromosome and self.current_chromosome is not None:
+                for molecule in self._yield_all_in_current_cache():
+                    yield molecule
+
+            # Check if we need to purge and yield results:
+            for molecule in self._purge():
+                yield molecule
+
+            position = self.localisation_function(fragment)
+            if position is None:
+                continue
+            molecule_id = self.assignment_function(fragment)
 
-            # Add gene annotations:
-            molecule.annotate(0)
-            molecule.set_intron_exon_features()
-            if len(molecule.genes) == 0:
-                molecule.set_meta('RF', 'rejected_recovery_no_gene')
-                statistics['Filtering']['rejected_recovery_no_gene'] += 1
-                molecule.write_tags()
-                molecule.write_pysam(output)
+            # Check if there is a molecule to assign to already present:
+            assigned = False
+            for existing_molecule in self.molecule_cache[position]:
+                if self.eq_function(existing_molecule, molecule_id):
+                    assigned = True
+                    self.molecule_cache[position][existing_molecule].append(
+                        fragment)
+            if not assigned:
+                self.molecule_cache[position][molecule_id].append(fragment)
+
+            self.current_chromosome = self.get_fragment_chromosome(fragment)
+            self.current_position = self.localisation_function(
+                fragment)  # [0].reference_end
+
+        # yield everything which was not yielded yet
+        for molecule in self._yield_all_in_current_cache():
+            yield molecule
+
+
+"""
+Iterate over transcripts in a bam file
+
+Parameters
+----------
+alignmentfile : pysam.AlignmentFile
+    file to read the molecules from
+
+look_around_radius : int
+    buffer to accumulate molecules in. All fragments belonging to one molecule should fit this radius
+
+informative_read : int
+    which read is used to define the mapping coordinate of the fragment, 1 or 2.
+
+umi_hamming_distance : int
+    Edit distance on UMI, 0: only exact match, 1: single base distance, 2 base distance ...
+
+assignment_radius : int
+    tolerance on fragment starting coordinates
+
+sample_select : iterable
+    Iterable of samples to only select molecules from
+
+Yields
+----------
+list of molecules : list [ pysam.AlignedSegment ]
+[ (R1,R2), (R1,R2) ... ]
+"""
+
+
+class TranscriptIterator(MoleculeIterator_OLD):
+    def __init__(
+            self,
+            look_around_radius=100,
+            informative_read=2,
+            assignment_radius=10,
+            **kwargs):
+        MoleculeIterator_OLD.__init__(
+            self, look_around_radius=look_around_radius, **kwargs)
+        self.informative_read = informative_read
+        self.assignment_radius = assignment_radius
+
+    def assignment_function(self, fragment):
+        return fragment[self.informative_read -
+                        1].get_tag('SM'), fragment[self.informative_read -
+                                                   1].get_tag('RX'), fragment[self.informative_read -
+                                                                              1].is_reverse
+
+    def localisation_function(self, fragment):
+        return int((fragment[self.informative_read - 1].reference_start) /
+                   self.assignment_radius) * self.assignment_radius
+
+
+class QueryNameFlagger(DigestFlagger):
+    def __init__(self, **kwargs):
+        self.assignedReadGroups = set()
+        DigestFlagger.__init__(self, **kwargs)
+
+    def digest(self, reads):
+        for read in reads:
+            if read is None:
                 continue
-            if len(molecule.junctions):
-                molecule.set_meta('RF', 'recovered_transcript_junction')
-                statistics['Filtering']['recovered_transcript_junction'] += 1
-                statistics['Data type detection'][
-                    f'RNA because junction found and no {args.method} site mapped'] += 1
+            if read.has_tag('SM'):  # It is already tagged
+                return
+            if read.query_name.startswith('UMI'):  # Old format
+                import tagBamFile  # this is not included anymore
+                tagBamFile.recodeRead(read)
             else:
-                molecule.set_meta('RF', 'recovered_transcript_gene')
-                statistics['Data type detection'][
-                    f'RNA because gene found and no {args.method} site mapped'] += 1
-                statistics['Filtering']['recovered_transcript_gene'] += 1
-            molecule.set_meta('dt', 'RNA')
-            statistics['Data type detection']['RNA'] += 1
-            molecule.write_tags()
-            molecule.write_pysam(output)
-
-    # Show statistics:
-    print(
-        '\n' +
-        colorama.Style.BRIGHT +
-        'Statistics' +
-        colorama.Style.RESET_ALL)
-    for statistic_class in [
-        'Input',
-        'Filtering',
-        'Data type detection',
-            'Methylation']:
-        print(f'{colorama.Style.BRIGHT} {statistic_class} {colorama.Style.RESET_ALL}')
-        for statistic, value in statistics[statistic_class].most_common():
-            print(f'  {statistic}\t{value}')
-
-    print(f'{colorama.Style.BRIGHT} Methylation calls {colorama.Style.RESET_ALL}')
-    for call, description in zip('zZxXhH',
-                                 ['unmethylated C in CpG context (CG)',
-                                  'methylated C in CpG context (CG)',
-                                  'unmethylated C in CHG context ( C[ACT]G )',
-                                  'methylated C in CHG context   ( C[ACT]G )',
-                                  'unmethylated C in CHH context ( C[ACT][ACT] )',
-                                  'methylated C in CHH context ( C[ACT][ACT] )'
-                                  ]):
-
-        if call.isupper():
-            print(
-                f'  {colorama.Style.BRIGHT}{call}{colorama.Style.RESET_ALL}\t{mcs[call]}',
-                end='\t')
-        else:
-            print(f'  {call}\t{mcs[call]}', end='\t')
-        print(f'{colorama.Style.DIM}{description}{colorama.Style.RESET_ALL}')
+                tr = singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods.TaggedRecord(
+                    singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods.TagDefinitions
+                )
 
-    print('\n')
+                tr.fromTaggedBamRecord(read)
 
-    if args.table is not None:
-        print(
-            colorama.Style.BRIGHT +
-            'Writing raw unmethylated counts' +
-            colorama.Style.RESET_ALL)
-        # Write raw counts:
-        df = pd.DataFrame(
-            {loc: {sample: binned_data[loc][sample][0] for sample in binned_data[loc]} for loc in binned_data})
-        df.to_pickle(f'{args.table}_unmethylated_{args.contig}.pickle.gz')
-        df.to_csv(f'{args.table}_unmethylated_{args.contig}.csv')
-        del df
-
-        print(
-            colorama.Style.BRIGHT +
-            'Writing raw methylated counts' +
-            colorama.Style.RESET_ALL)
-        df = pd.DataFrame(
-            {loc: {sample: binned_data[loc][sample][1] for sample in binned_data[loc]} for loc in binned_data})
-        df.to_pickle(f'{args.table}_methylated_{args.contig}.pickle.gz')
-        df.to_csv(f'{args.table}_methylated_{args.contig}.csv')
-        del df
-
-        print(
-            colorama.Style.BRIGHT +
-            'Writing ratio tables' +
-            colorama.Style.RESET_ALL)
-        # cast all fractions to float
-        for loc in binned_data:
-            for sample in binned_data[loc]:
-                binned_data[loc][sample] = float(binned_data[loc][sample])
-        df = pd.DataFrame(binned_data)
-        del binned_data
-        if args.contig:
-            df.to_pickle(f'{args.table}_ratio_{args.contig}.pickle.gz')
-            df.to_csv(f'{args.table}_ratio_{args.contig}.csv')
-        else:
-            df.to_pickle(f'{args.table}_ratio.pickle.gz')
-            df.to_csv(f'{args.table}_ratio.csv')
+                newHeader = tr.asIlluminaHeader()
+                read.query_name = newHeader
 
-    print(
-        colorama.Style.BRIGHT +
-        'Sorting and indexing final file' +
-        colorama.Style.RESET_ALL)
-    # Sort and index
-    # Perform a reheading, sort and index
-    if not args.no_sort_index:
-        cmd = f"""samtools sort {temp_out} > {args.o}; samtools index {args.o};
-        rm {temp_out};
-        """
+                tr.tagPysamRead(read)
+                rg = f"{read.get_tag('Fc') if read.has_tag('Fc') else 'NONE'}.{read.get_tag('La') if read.has_tag('La') else 'NONE'}.{read.get_tag('SM') if read.has_tag('SM') else 'NONE'}"
+                self.assignedReadGroups.add(rg)
+                # Add read group:
+                read.set_tag('RG', rg)
+
+
+class AlleleTagger(DigestFlagger):
+
+    def __init__(self, **kwargs):
+        DigestFlagger.__init__(self, **kwargs)
+
+    def digest(self, reads):
+        nonNullReads = [read for read in reads if read is not None]
+
+        self.addAlleleInfo(nonNullReads)
+
+
+if __name__ == "__main__":
+    # These data sources are fed to all flaggers
+    flaggerArguments = {
+        'reference': None if args.ref is None else pysamIterators.CachedFasta(
+            pysam.FastaFile(args.ref)),
+        'alleleResolver': None if args.alleles is None else alleleTools.AlleleResolver(
+            args.alleles, lazyLoad=not args.loadAllelesToMem),
+        'moleculeRadius': args.moleculeRadius,
+        'verbose': args.verbose,
+        'exon_gtf': args.exons,
+        'intron_gtf': args.introns
+    }
+
+    pairedEnd = False
+    flaggers = []
+    qFlagger = None
+    # if args.ftag:
+    # Now we ALWAYS put reads through qflagger
+    qFlagger = QueryNameFlagger(**flaggerArguments)
+    flaggers.append(qFlagger)
+    if args.nla:
+        flaggers.append(NlaIIIFlagger(**flaggerArguments))
+        pairedEnd = True
+    if args.mspji:
+        flaggers.append(MSPJIFlagger(**flaggerArguments))
+        pairedEnd = True
+    if args.chic:
+        flaggers.append(ChicSeqFlagger(**flaggerArguments))
+        pairedEnd = True
+    if args.scar:
+        flaggers.append(ScarFlagger(**flaggerArguments))
+        pairedEnd = True
+    if args.tag:
+        flaggers.append(TagFlagger(tag=args.tag))
+    if args.atag:
+        print("Running allele tagging")
+        flaggers.append(AlleleTagger(**flaggerArguments))
+    if args.rna:
+        flaggers.append(RNA_Flagger(**flaggerArguments))
+    if args.taps:
+        flaggers.append(TAPSFlagger(**flaggerArguments))
+        pairedEnd = True
+
+    if args.alleles is not None:
+        # Check if the variant file is valid..
+        if not (args.alleles.endswith('.vcf.gz')
+                or args.alleles.endswith('.bcf.gz')):
+            raise ValueError(f"""Please supply an indexed (bg)zipped VCF file.
+            You can convert your file using: bcftools view {args.alleles} -O b -o {args.alleles}.gz;
+            then index using bcftools index {args.alleles}.gz """)
+        if not (
+            os.path.exists(
+                args.alleles +
+                '.csi') or os.path.exists(
+                args.alleles +
+                '.tbi')):
+            raise ValueError(f"""Please supply an indexed (bg)zipped VCF file.
+            Index using: bcftools index {args.alleles} """)
+
+    if pairedEnd:
+        print('Assuming the input is paired end')
     else:
-        cmd = f"mv {temp_out} {args.o}"
-    os.system(cmd)
-    print("All done.")
+        print('Assuming the input is single end ( Has no influence on ftag)')
+
+    if not os.path.exists(args.o):
+        try:
+            os.makedirs(args.o)
+        except Exception as e:
+            pass
+
+    # Here we walk through the bamfiles and fetch
+    tmpprefix = f'{args.tmpprefix}'
+
+    for bamFilePath in args.bamfiles:
+
+        bamFile = pysam.AlignmentFile(bamFilePath, "rb")
+        header = bamFile.header.copy()
+        outPathTemp = f'{args.o}/{os.path.basename(bamFilePath)}.unsorted'
+        outPathTempWithHeader = f'{args.o}/{os.path.basename(bamFilePath)}.unsorted.with_header.bam'
+        outPath = f"{args.o}/{os.path.basename(bamFilePath).replace('.bam', '')}.bam"
+
+        print(f'Now reading {bamFilePath}, writing to {outPath}')
+        if args.dedup:
+            dedupOutPathTemp = f'{args.o}/{os.path.basename(bamFilePath)}.dedup.unsorted'
+            dedupOutPathTempWithHeader = f'{args.o}/{os.path.basename(bamFilePath)}.dedup.with_header.bam'
+            dedupOutPath = f"{args.o}/{os.path.basename(bamFilePath).replace('.bam', '')}.dedup.bam"
+            dedupOutputFile = pysam.AlignmentFile(
+                dedupOutPathTemp, "wb", header=header)
+        outputFile = pysam.AlignmentFile(outPathTemp, "wb", header=header)
+
+        bamName = os.path.basename(bamFilePath).replace('.bam', '')
+        # if os.path.exists(outPath+'.bai'):
+        #    continue
+        i = 0
+        if pairedEnd:
+            it = pysamIterators.MatePairIterator(
+                bamFile, performProperPairCheck=False, contig=args.chr)
+
+            for i, (R1, R2) in enumerate(it):
+                for flagger in flaggers:
+                    try:
+                        flagger.digest([R1, R2])
+                    except Exception as e:
+                        print(e)
+
+                        if args.fatal:
+                            print(R1, R2)
+                            raise e
+
+                try:
+                    if R1 is not None:
+                        outputFile.write(R1)
+                    if R2 is not None:
+                        outputFile.write(R2)
+                except Exception as e:
+                    for flagger in flaggers:
+                        print(flagger)
+                    raise e
+                if args.dedup and (
+                    (R1 is not None and R1.has_tag('RC') and R1.get_tag('RC') == 1) or (
+                        R2 is not None and R2.has_tag('RC') and R2.get_tag('RC') == 1)):
+                    if R1 is not None:
+                        dedupOutputFile.write(R1)
+                    if R2 is not None:
+                        dedupOutputFile.write(R2)
+
+                if args.head is not None and i >= args.head:
+                    break
+        else:
+            iterator = bamFile.fetch(
+                contig=args.chr) if args.chr is not None else bamFile
+            for i, R1 in enumerate(iterator):
+
+                for flagger in flaggers:
+                    try:
+                        flagger.digest([R1])
+                    except Exception as e:
+                        if args.fatal:
+                            raise e
+                        print(e)
+
+                outputFile.write(R1)
+
+                if args.head is not None and i >= args.head:
+                    break
+        print(f'{bamFilePath}: processed {i} reads')
+
+        print("Finishing files (forcing close)")
+        outputFile.close()
+        if args.dedup:
+            dedupOutputFile.close()
+
+        if qFlagger is not None:
+            readGroups = {}
+
+            for readGroup in qFlagger.assignedReadGroups:
+                flowCell, lane, sampleLib = readGroup.split('.')
+                library, sample = sampleLib.rsplit('_', 1)
+                readGroups[readGroup] = {
+                    'ID': readGroup,
+                    'LB': library,
+                    'PL': 'ILLUMINA',
+                    'SM': sample,
+                    'PU': readGroup}
+
+            headerSamFilePath = outPath.replace('.bam', '') + '.header.sam'
+            hCopy = header.to_dict()
+            hCopy['RG'] = list(readGroups.values())
+            with gzip.open(outPathTemp.replace('.bam', '') + '.readGroups.pickle.gz', 'wb') as rgzip, pysam.AlignmentFile(headerSamFilePath, 'w', header=hCopy) as headerSam:
+                pickle.dump(readGroups, rgzip)
+
+                # for readGroup, fields in readGroups.items():
+                #    headerSam.write(f'@RG\tID:{readGroup}\tPL:{fields["PL"]}\tSM:{fields["SM"]}\tPU:{fields["PU"]}\tLB:{fields["LB"]}\n')
+            # Clear the read groups
+            qFlagger.assignedReadGroups = set()
+
+            # Perform a reheading, sort and index
+            rehead_cmd = f"""{{ cat {headerSamFilePath}; samtools view {outPathTemp}; }} | samtools view -b > {outPathTempWithHeader} ;
+            rm {outPathTemp};
+            samtools sort -T {tmpprefix} {outPathTempWithHeader} > {outPath}; samtools index {outPath};
+            rm {outPathTempWithHeader};
+            """
+            print(f"Adding read groups to header and sorting.")
+            os.system(rehead_cmd)
+
+            # Same procedure for dedup:
+            if args.dedup:
+                rehead_cmd = f"""{{ cat {headerSamFilePath}; samtools view {dedupOutPathTemp}; }} | samtools view -b > {dedupOutPathTempWithHeader} ;
+                rm {dedupOutPathTemp};
+                samtools sort -T {tmpprefix} {dedupOutPathTempWithHeader} > {dedupOutPath}; samtools index {dedupOutPath};
+                rm {dedupOutPathTempWithHeader};
+                """
+                print(f"Dedup file: adding read groups to header and sorting.")
+                os.system(rehead_cmd)
+
+        else:
+            # we cannot assign readgroups...
+            rehead_cmd = f"""
+            samtools sort -T {tmpprefix} {outPathTemp} > {outPath}; samtools index {outPath};
+            rm {outPathTemp};
+            """
+            print(f"Adding read groups to header and sorting.")
+            os.system(rehead_cmd)
+
+            if args.dedup:
+                rehead_cmd = f"""
+                samtools sort -T {tmpprefix} {dedupOutPathTemp} > {dedupOutPath}; samtools index {dedupOutPath};
+                rm {dedupOutPathTemp};
+                """
+                print(f"Dedup file: adding read groups to header and sorting.")
+                os.system(rehead_cmd)
+
+    """
+    Is:NS500414;RN:455;Fc:HYLVHBGX5;La:3;Ti:13601;CX:9882;CY:17671;Fi:N;CN:0;aa:CCGTCC;aA:CCGTCC;aI:16;LY:A3-P15-1-1;RX:ACG;RQ:GGG;BI:17;bc:ACTCGATG;BC:ACTCGATG;QT:GGKKKKKK;MX:NLAIII384C8U3;A2:TGG;AQ:E6E
+    for f in $(ls *.bam | cut -f 1,2,3 -d '-' | sort | uniq | grep -v bam); do submission.py -y -time 20 -t 1 "addTagsToLennartNLABam.py $f*cell*.bam"; done
+
+    """
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/universalBamTagger/universalBamTagger.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/bamProcessing/bamFunctions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,709 +1,874 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import re
+import os
 import pysam
 import time
-import sys
-import multiprocessing
-import subprocess
+import contextlib
+from shutil import which, move
+from singlecellmultiomics.utils import BlockZip, Prefetcher
+import uuid
 import os
-from singlecellmultiomics.utils.sequtils import hamming_distance, phred_to_prob
-from singlecellmultiomics.universalBamTagger.taps import TAPSFlagger
-from singlecellmultiomics.universalBamTagger.tag import TagFlagger
-from singlecellmultiomics.universalBamTagger.scar import ScarFlagger
-from singlecellmultiomics.universalBamTagger.mspjI import MSPJIFlagger
-from singlecellmultiomics.universalBamTagger.scchic import ChicSeqFlagger
-from singlecellmultiomics.universalBamTagger.nlaIII import NlaIIIFlagger
-from singlecellmultiomics.universalBamTagger.digest import DigestFlagger
-from singlecellmultiomics.universalBamTagger.rna import RNA_Flagger
-import warnings
+from collections import defaultdict, Counter
+from singlecellmultiomics.bamProcessing.pileup import pileup_truncated
 import numpy as np
-import math
-import singlecellmultiomics.features
-import singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods
-from singlecellmultiomics.tagtools import tagtools
-import argparse
-import pysamiterators.iterators as pysamIterators
-import gzip
-import pickle
-from singlecellmultiomics.alleleTools import alleleTools
-import uuid
-import collections
-import glob
-c = 1_000  # !!! PLEASE USE PYTHON 3.6 OR HIGHER !!!
-complement = str.maketrans('ATGC', 'TACG')
-
-
-warnings.warn(
-    "universalBamTagger is deprecated. Please switch to use bamtagmultiome.py ",
-    DeprecationWarning)
-
-
-# Modules:
-
-
-if __name__ == "__main__":
-    argparser = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description="""Add allelic NLA and/or MSPJI digest information to a demultiplexed bam file
-    Adds the following tags:
-    RC: number of oversequenced molecules
-    DT: Source type (NLA/MSPJI/RNA.. )
-    DA: Digest allele
-    RP: Recognized sequence
-    RS: Recognized strand '-','?','+'
-
-    Which tags are filled in depends on which files you supply, for example if you do not supply an allelic VCF file, then no allele tag will be added
-    """)
-
-    argparser.add_argument('bamfiles', metavar='bamfile', type=str, nargs='+')
-    argparser.add_argument(
-        '--local',
-        action='store_true',
-        help='Do not qsub sorting and indexing [deprecated]')
-    argparser.add_argument(
-        '-tmpprefix',
-        metavar='PREFIX.nnnn.bam',
-        help='When sorting, specify temp dir to prevent home directory filling up',
-        default='~/')
-    #argparser.add_argument('--noSort', action='store_true', help='Do not sort and index')
-    #argparser.add_argument('--cluster', action='store_true', help='Do not qsub sorting and indexing')
-
-    tagAlgs = argparser.add_argument_group('Tagging algorithms', '')
-    tagAlgs.add_argument(
-        '--ftag',
-        action='store_true',
-        help='!DEPRECATED, this flag is now always used!')
-    tagAlgs.add_argument(
-        '--atag',
-        action='store_true',
-        help='Add only allele tags')
-    tagAlgs.add_argument(
-        '--mspji',
-        action='store_true',
-        help='Look for mspji digest')
-    tagAlgs.add_argument(
-        '--nla',
-        action='store_true',
-        help='Look for nlaIII digest')
-    tagAlgs.add_argument(
-        '--chic',
-        action='store_true',
-        help='Look for mnase (scCHIC) digest')
-    tagAlgs.add_argument(
-        '--scar',
-        action='store_true',
-        help='Create R1 start, cigar sequence based DS tags')
-    tagAlgs.add_argument(
-        '--taps',
-        action='store_true',
-        help='Add TAPS based methylation state ')
-    tagAlgs.add_argument(
-        '-tag',
-        type=str,
-        default=None,
-        help='Determine oversequencing based on a tag (for example XT to count RNA oversequencing for featureCounts counted transcripts. chrom for chromosome/contig count)')
-
-    # RNA options
-    tagAlgs.add_argument(
-        '--rna',
-        action='store_true',
-        help='Assign RNA molecules, requires a intronic and exonic GTF file')
-    argparser.add_argument(
-        '-introns',
-        type=str,
-        help='Intronic GTF file, use exonGTFtoIntronGTF.py to generate such a GTF file')
-    argparser.add_argument('-exons', type=str, help='Exonic GTF file.')
-    """
-    How much bases of the fragment fall inside the intron(s)
-    How much bases of the fragment fall inside the exon(s)
-    is the fragment spliced? How many bases are spliced out?
-    """
-
-    argparser.add_argument(
-        '-moleculeRadius',
-        type=int,
-        help='Search radius for each molecule, if a cut site is found within this range with the same umi, it will be counted as the same molecule',
-        default=0)
-
-    argparser.add_argument(
-        '-alleles',
-        type=str,
-        help='VCF file. Add allelic info flag based on vcf file')
-    argparser.add_argument(
-        '--loadAllelesToMem',
-        action='store_true',
-        help='Load allele data completely into memory')
-
-    argparser.add_argument('-ref', type=str, help='reference FASTA file.')
-    argparser.add_argument(
-        '-o',
-        type=str,
-        default='./tagged',
-        help='output folder')
-    argparser.add_argument(
-        '--dedup',
-        action='store_true',
-        help='Create deduplicated bam files')
-
-    argparser.add_argument('-chr', help='run only on this chromosome')
-
-    argparser.add_argument(
-        '-head',
-        type=int,
-        default=None,
-        help='Only process first n reads of every bam file')
-
-    devArgs = argparser.add_argument_group('Development options', '')
-    devArgs.add_argument(
-        '--fatal',
-        action='store_true',
-        help='Crash upon any encountered error')
-    devArgs.add_argument('--verbose', action='store_true', help='Be verbose')
-    devArgs.add_argument(
-        '--knh',
-        action='store_true',
-        help='Keep non-headered bam file')
+import pandas as pd
+from typing import Generator
 
-    args = argparser.parse_args()
 
-    if not args.mspji and not args.nla and not args.chic and not args.ftag and not args.rna and args.tag is None and args.atag is None and args.taps is None:
-        raise ValueError(
-            'Please supply any or a combination of --ftag --nla --chic --mspji --taps')
+def get_contigs_with_reads(bam_path: str) -> Generator:
+    """
+    Get all contigs with reads mapped to them
 
-    if args.rna and (args.introns is None or args.exons is None):
-        raise ValueError(
-            'Please supply exonic and intronic GTF files -introns -exons')
+    Args:
+        bam_path(str): path to bam file
+
+    Yields:
+        contig(str)
 
     """
-    Corrected Tags
-    BC: This should be used for the sample-barcode so that there is no conflict in case that both sample- and molecular-barcodes are used
-    QT: This should be the quality for the sample-barcode BC
+    for line in pysam.idxstats(bam_path).split('\n'):
+        try:
+            contig, contig_len, mapped_reads, unmapped_reads = line.strip().split()
+            mapped_reads, unmapped_reads = int(mapped_reads), int(unmapped_reads)
+            if mapped_reads>0 or unmapped_reads>0:
+                yield contig
+        except ValueError:
+            pass
 
-    New Tags
-    RX: The raw sequence bases of the molecular-barcode(s) of the read(s) can be placed in this tag
-    QX: The original qualites (as QUAL) of the bases in RX
+def merge_bams( bams: list, output_path: str, threads: int=4 ):
+    """Merge bamfiles to output_path
 
-    BX: Sequence bases of the unique molecular identifier, may be corrected or raw
-    BZ: Quality score the unique molecular identifier. May be corrected or raw. See BX tag for qualities
+    When a single bam file is supplied, the bam file is moved to  output_path
+    All input bam files are removed
 
-    MI: Molecular-barcode sequence or identifier, may include non-sequence bases (Here, it is BC+RX)
-    QM: Molecular-barcode qualities, QT+QX
+    Args:
+        bams : list or tuple containing paths to bam files to merge
+        output_path (str): target path
 
-    DS: coordinate of site
-    RC: number of oversequenced molecules
-    DT: Source type (NLA/MSPJI/RNA..? )
-    DA: Digest allele
-    RP: Recognized sequence
-    RS: Recognized strand '-','?','+'
-    LI: ligation sequence
+    Returns:
+        output_path (str)
 
     """
+    if len(bams)==1:
+        move(bams[0], output_path)
+        move(bams[0]+'.bai', output_path+'.bai')
+    else:
+        pysam.merge(output_path, *bams, f'-@ {threads} -f -l 1')
+        pysam.index(output_path, f'-@ {threads}')
+        for o in bams:
+            os.remove(o)
+            os.remove(o+'.bai')
+    return output_path
+
+def verify_and_fix_bam(bam_path):
+    """
+    Check if the bam file is not truncated and indexed.
+    If not, apply index
+
+    Args:
+        bam_path(str) : path to bam file
+
+    Raises:
+        ValueError : when the file is corrupted and a fix could not be applied
+    """
+    index_missing = False
+    if not os.path.exists(bam_path):
+        raise ValueError(f"The bam file {bam_path} does not exist")
+
+    with pysam.AlignmentFile(bam_path, "rb") as alignments:
+        if alignments.check_truncation():
+            raise ValueError(f"The bam file {bam_path} is truncated")
+
+        # This raises and error:
+        try:
+            if not alignments.check_index():
+                # Try to index the input file..
+                print(
+                    f"The bam file {bam_path} does not have an index, attempting an index build ..")
+                index_missing = True
+        except Exception as e:
+            index_missing = True
 
+        if index_missing:
+            pysam.index(bam_path)
 
-# 1: read1 2: read2
-def molecule_to_random_primer_dict(molecule, primer_length=6, primer_read=2):
-    rp = collections.defaultdict(list)
-    for fragment in molecule:
-        if fragment[primer_read - 1] is not None:
-            hstart, hseq = tagtools.getRandomPrimerHash(
-                fragment[primer_read - 1], onStart=True, primerLength=6)
-            rp[hstart, hseq].append(fragment)
-    return rp
-    # for k,p in rp.items():
-    #    yield p
+    if index_missing:
+        with pysam.AlignmentFile(bam_path, "rb") as alignments:
+            if not alignments.check_index():
+                raise ValueError(
+                    f'The file {bam_path} is not sorted or damaged in some way')
 
 
-class MoleculeIterator_OLD():
+def _get_samples_from_bam(handle):
+    """Get a list of samples present in the bam_file
+    private: please use get_samples_from_bam()
+
+    Args:
+        bam_file(pysam.AlignmentFile) : path to bam file or pysam object
+
+    Returns:
+        samples (set) : set containing all sample names
+
     """
-    Iterate over molecules in a bam file
+    try:
+        return set([entry['SM'] for entry in handle.header.as_dict()['RG']])
+    except Exception as e:
+        samples = set()
+        for read in handle:
+            samples.add( read.get_tag('SM') )
+        return samples
+
+def get_sample_to_read_group_dict(bam):
+    """ Obtain a dictionary containing {'sample name' : ['read groupA', 'read group B'], ...}
+        Args:
+            bam_file(pysam.AlignmentFile) or path to bam file or pysam object
+    """
+
+    if isinstance(bam, str):
+        with pysam.AlignmentFile(bam) as pysam_AlignmentFile_handle:
+            return _get_sample_to_read_group_dict(pysam_AlignmentFile_handle)
+    elif isinstance(bam, pysam.AlignmentFile):
+        return _get_sample_to_read_group_dict(bam)
 
-    Parameters
-    ----------
-    alignmentfile : pysam.AlignmentFile
-        file to read the molecules from
+    else:
+        raise ValueError(
+            'Supply either a path to a bam file or pysam.AlignmentFile object')
+
+def get_read_group_to_sample_dict(bam):
+    """ Obtain a dictionary containing {'read_group' : 'sample' , ...}
+        Args:
+            bam_file(pysam.AlignmentFile) or path to bam file or pysam object
+    """
+    d = get_sample_to_read_group_dict(bam)
+    r2s = {}
+    for sample, read_groups in d.items():
+        for rg in read_groups:
+            r2s[rg] = sample
 
-    look_around_radius : int
-        buffer to accumulate molecules in. All fragments belonging to one molecule should fit this radius
+    return r2s
 
-    umi_hamming_distance : int
-        Edit distance on UMI, 0: only exact match, 1: single base distance
+def get_read_group_format(bam):
+    """Obtain read group format
 
-    sample_select : iterable
-        Iterable of samples to only select molecules from
+    Args:
+        bam (str) : path to bam file
 
-    Yields
-    ----------
-    list of molecules : list [ pysam.AlignedSegment ]
-    [ (R1,R2), (R1,R2) ... ]
+    Returns:
+        type (int) : read group format
 
+    Raises:
+        ValueError : when read group format cannot be determined
     """
+    with pysam.AlignmentFile(bam) as f:
+        d = f.header.as_dict()
+        format_type_obs = Counter()
+        for read_group_dict in d['RG']:
 
-    def __init__(self,
-                 alignmentfile,
-                 look_around_radius=100_000,
-                 umi_hamming_distance=0,  # 0: only exact match, 1: single base distance
-                 sample_select=None,  # iterable of samples to only select molecules from
-                 # when a string is supplied only a single sample is selected
+            if read_group_dict.get('LB','')==read_group_dict.get('SM',''):
+                format_type_obs[1]+=1
+            else:
+                format_type_obs[0]+=1
 
-                 **pysam_kwargs
-                 ):
-        self.alignmentfile = alignmentfile
-        self.look_around_radius = look_around_radius
+        if len(format_type_obs)==1:
+            return format_type_obs.most_common(1)[0][0]
+        raise ValueError('Failed to indentify read group format ')
 
-        self.current_position = None
-        self.current_chromosome = None
-        self.molecules_yielded = 0
-        self.umi_hamming_distance = umi_hamming_distance
-        self.pysam_kwargs = pysam_kwargs
 
-        self.sample_select = sample_select
-        self.sample_tag = 'SM'
-        self._clear()
+def _get_sample_to_read_group_dict(handle):
+    """ Obtain a dictionary containing {'sample name' : ['read groupA', 'read group B']}
+        Args:
+            bam_file(pysam.AlignmentFile) : path to bam file or pysam object
+    """
 
-        self.filter_function = None  # function which results given two reads if it is usable
+    sample_to_read_group_dict = defaultdict(list)
+    # Traverse the read groups;
+    for entry in handle.header.as_dict()['RG']:
+        sample_to_read_group_dict[ entry['SM'] ].append(entry['ID'])
+    return sample_to_read_group_dict
+
+
+def get_contig_size(bam, contig):
+    """Extract the length of a contig from a bam file
+
+    Args:
+        bam (str or pysam.AlignmentFile) : handle to bam file or path to bam file
+        contig (str)
 
-    def _clear(self):
-        self.molecule_cache = collections.defaultdict(lambda: collections.defaultdict(
-            list))  # position -> cell,umi,strand,allele.. -> reads
+    Returns:
+        length (int)
+    """
+    if type(bam) is str:
+        with pysam.AlignmentFile(bam) as a:
+            size = get_contig_size(a, contig)
+        return size
+    elif type(bam) is pysam.AlignmentFile:
+        for c,length in zip(bam.references, bam.lengths):
+            if c==contig:
+                return length
+    else:
+        raise ValueError(
+            'Supply either a path to a bam file or pysam.AlignmentFile object')
 
-    def sample_assignment_function(self, fragment):
-        for read in fragment:
-            if read is not None:
-                if read.has_tag(self.sample_tag):
-                    return read.get_tag(self.sample_tag)
-        return None
+    return None
 
-    # Returns postion unique identifier for a fragment
-    def localisation_function(self, fragment):
-        if not fragment[0].has_tag('DS'):
-            return None
-        return fragment[0].get_tag('DS')
+def get_contig_sizes(bam):
+    """Extract lengths of all contigs from a bam file
 
-    def __repr__(self):
-        return f"""Molecule iterator
-        current position: {self.current_chromosome}:{self.current_position}
-        yielded {self.molecules_yielded} so far
-        currently {len(self.molecule_cache)} positions cached
-        keeping {self.get_cached_fragment_count()} fragments cached
-        """
+    Args:
+        bam (str or pysam.AlignmentFile) : handle to bam file or path to bam file
+
+    Returns:
+        contig_lengths : dict (contig:length (int) )
+    """
+
+    if type(bam) is str:
+        with pysam.AlignmentFile(bam) as a:
+            sizes = get_contig_sizes(a)
+        return sizes
+    elif type(bam) is pysam.AlignmentFile:
+        return dict(zip(bam.references, bam.lengths))
+    else:
+        raise ValueError(
+            'Supply either a path to a bam file or pysam.AlignmentFile object')
 
-    def get_cached_fragment_count(self):
-        total_fragments = 0
-        for position, data_per_molecule in self.molecule_cache.items():
-            for molecule_id, molecule_reads in data_per_molecule.items():
-                total_fragments += len(molecule_reads)
-        return total_fragments
-
-    def assignment_function(self, fragment):
-        return fragment[0].get_tag('SM'), fragment[0].get_tag(
-            'RX'), fragment[0].get_tag('RS')
-
-    # Returns True if two fragment ids  are identical or close enough
-    def eq_function(self, assignment_a, assignment_b):
-        if assignment_a is None or assignment_b is None:
-            return False
 
-        sample_A, umi_A, strand_A = assignment_a
-        sample_B, umi_B, strand_B = assignment_b
+def get_samples_from_bam(bam):
+    """Get a list of samples present in the bam_file
 
-        if sample_A != sample_B or strand_A != strand_B:
-            return False
+    Args:
+        bam_file(str) or pysam.AlignmentFile : path to bam file or pysam object
 
-        if self.umi_hamming_distance == 0:
-            return umi_A == umi_B
-        else:
-            return hamming_distance(umi_A, umi_B) <= self.umi_hamming_distance
+    Returns:
+        samples (set) : set containing all sample names
 
-    def _yield_all_in_current_cache(self):
-        for position, data_per_molecule in self.molecule_cache.items():
-            for molecule_id, molecule_reads in data_per_molecule.items():
-                self.molecules_yielded += 1
-                yield molecule_reads
-        self._clear()
-
-    def _purge(self):
-        drop = []
-        for pos in self.molecule_cache:
-            if pos < (self.current_position - self.look_around_radius):
-                # purge this coordinate:
-                for molecule_id, molecule_reads in self.molecule_cache[pos].items(
-                ):
-                    self.molecules_yielded += 1
-                    yield molecule_reads
-                drop.append(pos)
-
-        for pos in drop:
-            del self.molecule_cache[pos]
-
-    def get_fragment_chromosome(self, fragment):
-        for read in fragment:
-            if read is not None:
-                return read.reference_name
-
-    def __iter__(self):
-        for fragment in pysamIterators.MatePairIterator(
-                self.alignmentfile,
-                **self.pysam_kwargs,
-                performProperPairCheck=False):
+    """
 
-            if fragment[0] is None or fragment[0].reference_name is None:
-                continue
+    if isinstance(bam, str):
+        with pysam.AlignmentFile(bam) as pysam_AlignmentFile_handle:
+            return _get_samples_from_bam(pysam_AlignmentFile_handle)
+    elif isinstance(bam, pysam.AlignmentFile):
+        return _get_samples_from_bam(bam)
 
-            # Check if we want to drop the fragment because its corresponding
-            # sample is not selected
-            if self.sample_select is not None:
-                sample = self.sample_assignment_function(fragment)
-                if isinstance(self.sample_select, str):  # single sample
-                    if self.sample_select != sample:
-                        continue
-                else:  # list or set of samples
-                    if sample not in self.sample_select:
-                        continue
-
-            # We went to another chromsome, purge all in cache:
-            if self.get_fragment_chromosome(
-                    fragment) != self.current_chromosome and self.current_chromosome is not None:
-                for molecule in self._yield_all_in_current_cache():
-                    yield molecule
-
-            # Check if we need to purge and yield results:
-            for molecule in self._purge():
-                yield molecule
+    else:
+        raise ValueError(
+            'Supply either a path to a bam file or pysam.AlignmentFile object')
 
-            position = self.localisation_function(fragment)
-            if position is None:
-                continue
-            molecule_id = self.assignment_function(fragment)
 
-            # Check if there is a molecule to assign to already present:
-            assigned = False
-            for existing_molecule in self.molecule_cache[position]:
-                if self.eq_function(existing_molecule, molecule_id):
-                    assigned = True
-                    self.molecule_cache[position][existing_molecule].append(
-                        fragment)
-            if not assigned:
-                self.molecule_cache[position][molecule_id].append(fragment)
-
-            self.current_chromosome = self.get_fragment_chromosome(fragment)
-            self.current_position = self.localisation_function(
-                fragment)  # [0].reference_end
-
-        # yield everything which was not yielded yet
-        for molecule in self._yield_all_in_current_cache():
-            yield molecule
-
-
-"""
-Iterate over transcripts in a bam file
-
-Parameters
-----------
-alignmentfile : pysam.AlignmentFile
-    file to read the molecules from
-
-look_around_radius : int
-    buffer to accumulate molecules in. All fragments belonging to one molecule should fit this radius
-
-informative_read : int
-    which read is used to define the mapping coordinate of the fragment, 1 or 2.
-
-umi_hamming_distance : int
-    Edit distance on UMI, 0: only exact match, 1: single base distance, 2 base distance ...
-
-assignment_radius : int
-    tolerance on fragment starting coordinates
-
-sample_select : iterable
-    Iterable of samples to only select molecules from
-
-Yields
-----------
-list of molecules : list [ pysam.AlignedSegment ]
-[ (R1,R2), (R1,R2) ... ]
-"""
-
-
-class TranscriptIterator(MoleculeIterator_OLD):
-    def __init__(
-            self,
-            look_around_radius=100,
-            informative_read=2,
-            assignment_radius=10,
-            **kwargs):
-        MoleculeIterator_OLD.__init__(
-            self, look_around_radius=look_around_radius, **kwargs)
-        self.informative_read = informative_read
-        self.assignment_radius = assignment_radius
-
-    def assignment_function(self, fragment):
-        return fragment[self.informative_read -
-                        1].get_tag('SM'), fragment[self.informative_read -
-                                                   1].get_tag('RX'), fragment[self.informative_read -
-                                                                              1].is_reverse
-
-    def localisation_function(self, fragment):
-        return int((fragment[self.informative_read - 1].reference_start) /
-                   self.assignment_radius) * self.assignment_radius
-
-
-class QueryNameFlagger(DigestFlagger):
-    def __init__(self, **kwargs):
-        self.assignedReadGroups = set()
-        DigestFlagger.__init__(self, **kwargs)
-
-    def digest(self, reads):
-        for read in reads:
-            if read is None:
+def get_reference_from_pysam_alignmentFile(
+        pysam_AlignmentFile, ignore_missing=False):
+    """Extract path to reference from pysam handle
+
+    Args:
+        pysam_AlignmentFile (pysam.AlignmentFile)
+        ignore_missing(bool) : Check if the file exists, if not return None
+    Returns:
+        path : path to bam file (if exists or ignore_missing is supplied) or None
+    """
+    try:
+        for x in pysam_AlignmentFile.header.as_dict()['PG']:
+            if x.get('ID') != 'bwa':
                 continue
-            if read.has_tag('SM'):  # It is already tagged
-                return
-            if read.query_name.startswith('UMI'):  # Old format
-                import tagBamFile  # this is not included anymore
-                tagBamFile.recodeRead(read)
-            else:
-                tr = singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods.TaggedRecord(
-                    singlecellmultiomics.modularDemultiplexer.baseDemultiplexMethods.TagDefinitions
-                )
+            for argument in x.get('CL').split():
+                if (argument.endswith('.fa') or argument.endswith('.fasta') or argument.endswith(
+                        '.fasta.gz') or argument.endswith('.fa.gz')) and (ignore_missing or os.path.exists(argument)):
+                    return argument
+    except Exception as e:
+        pass
+
+
+def get_reference_path_from_bam(bam, ignore_missing=False):
+    """Extract path to reference from bam file
+
+    Args:
+        bam(str) or pysam.AlignmentFile : path to bam file
+        ignore_missing(bool) : Check if the file exists, if not return None
+    Returns:
+        path : path to bam file (if exists or ignore_missing is supplied) or None
+    """
+    if isinstance(bam, str):
+        with pysam.AlignmentFile(bam) as pysam_AlignmentFile_handle:
+            return get_reference_from_pysam_alignmentFile(
+                pysam_AlignmentFile_handle, ignore_missing=ignore_missing)
+    elif isinstance(bam, pysam.AlignmentFile):
+        return get_reference_from_pysam_alignmentFile(
+            bam, ignore_missing=ignore_missing)
+
+    else:
+        raise ValueError(
+            'Supply either a path to a bam file or pysam.AlignmentFile object')
+
+
+@contextlib.contextmanager
+def sorted_bam_file(
+        write_path,
+        origin_bam=None,
+        header=None,
+        read_groups=None,
+        local_temp_sort=True,
+        input_is_sorted=False,
+        mode='wb',
+        fast_compression=False, # Use fast compression for merge (-1 flag)
+        **kwargs
+        ):
+    """ Get writing handle to a sorted bam file
+
+    Args:
+        write_path (str) : write to a  bam file at this path
+
+        origin_bam (pysam.AlignmentFile ) : bam file to copy
+         header for or
+        header (dict) : header for the bam file to write
+
+        read_groups(set/dict) : set or dictionary which contains read groups. The dictionary should have the format { read_group_id (str)
+                { 'ID': ID, 'LB':library,
+                'PL':platform,
+                'SM':sampleLib,
+                'PU':readGroup }
+
+        local_temp_sort(bool) : create temporary files in current directory
+
+        input_is_sorted(bool) : Assume the input is sorted, no sorting will be applied
+
+        mode (str) : Output mode, use wbu for uncompressed writing.
+
+        **kwargs : arguments to pass to the new pysam.AlignmentFile output handle
+
+    Example:
+        >>> # This example assumes molecules are generated by `molecule_iterator`
+        >>> read_groups = set() # Store unique read groups in this set
+        >>> with sorted_bam_file('test_output.bam', header=input_header,read_groups=read_groups) as out:
+        >>>     for molecule in molecule_iterator:
+        >>>         molecule.write_tags()
+        >>>         molecule.write_pysam(out)
+        >>>         for fragment in molecule:
+        >>>             read_groups.add(fragment.get_read_group())
+        test_output.bam will be written, with read groups defined, sorted and indexed.
+
+
+    Write some pysam reads to a sorted bam file
+    Example:
+        >>> import pysam
+        >>> from singlecellmultiomics.bamProcessing import sorted_bam_file
+        >>> test_sam = pysam.AlignmentFile('test.sam','w',reference_names=['chr1','chr2'],reference_lengths=[1000,1000])
+        >>> read_A = pysam.AlignedSegment(test_sam.header)
+        >>> read_A.reference_name = 'chr2'
+        >>> read_A.reference_start = 100
+        >>> read_A.query_sequence = 'TTGCA'
+        >>> read_A.query_name= 'READ_A'
+        >>> read_A.cigarstring = '5M'
+        >>> read_A.query_qualities = [30] * len(read_A.query_sequence)
+        >>> read_A.set_tag('RG','HVKCCBGXB.4.MYLIBRARY_1')
+        >>> read_B = pysam.AlignedSegment(test_sam.header)
+        >>> read_B.reference_name = 'chr1'
+        >>> read_B.reference_start = 100
+        >>> read_B.query_sequence = 'ATCGGG'
+        >>> read_B.cigarstring = '6M'
+        >>> read_B.query_name= 'READ_B'
+        >>> read_B.query_qualities = [30] * len(read_B.query_sequence)
+        >>> read_B.set_tag('RG','HVKCCBGXB.4.MYLIBRARY_2')
+        >>> read_groups = set(( 'HVKCCBGXB.4.MYLIBRARY_2','HVKCCBGXB.4.MYLIBRARY_1'))
+        >>> with sorted_bam_file('out.bam', header=test_sam.header,read_groups=read_groups) as out:
+        >>>     out.write(read_A)
+        >>>     out.write(read_B)
+        Results in the bam file:
+        @HD	VN:1.6	SO:coordinate
+        @SQ	SN:chr1	LN:1000
+        @SQ	SN:chr2	LN:1000
+        @RG	ID:HVKCCBGXB.4.MYLIBRARY_2	SM:MYLIBRARY_2	LB:MYLIBRARY	PU:HVKCCBGXB.4.MYLIBRARY_2	PL:ILLUMINA
+        @RG	ID:HVKCCBGXB.4.MYLIBRARY_1	SM:MYLIBRARY_1	LB:MYLIBRARY	PU:HVKCCBGXB.4.MYLIBRARY_1	PL:ILLUMINA
+        READ_B	0	chr1	101	0	6M	*	0	0	ATCGGG	??????	RG:Z:HVKCCBGXB.4.MYLIBRARY_2
+        READ_A	0	chr2	101	0	5M	*	0	0	TTGCA	?????	RG:Z:HVKCCBGXB.4.MYLIBRARY_1
+
 
-                tr.fromTaggedBamRecord(read)
+    """
+    unsorted_path = None
+    unsorted_alignments = None
+    target_dir = None
+
+    unsorted_path = f'{write_path}.unsorted'
+    # Create output folder if it does not exists
+    target_dir = os.path.dirname(unsorted_path)
+    if not os.path.exists(target_dir) and len(target_dir)>0 and target_dir!='.':
+        try:
+            os.makedirs(target_dir, exist_ok=True)
+        except Exception as e:
+            pass
 
-                newHeader = tr.asIlluminaHeader()
-                read.query_name = newHeader
+    if header is not None:
+        pass
+    elif type(origin_bam) is str:
+        with pysam.AlignmentFile(origin_bam) as ain:
+            header = ain.header.copy()
+    elif origin_bam is not None:
+        header = origin_bam.header.copy()
+    else:
+        raise ValueError("Supply a header or origin_bam object")
 
-                tr.tagPysamRead(read)
-                rg = f"{read.get_tag('Fc') if read.has_tag('Fc') else 'NONE'}.{read.get_tag('La') if read.has_tag('La') else 'NONE'}.{read.get_tag('SM') if read.has_tag('SM') else 'NONE'}"
-                self.assignedReadGroups.add(rg)
-                # Add read group:
-                read.set_tag('RG', rg)
-
-
-class AlleleTagger(DigestFlagger):
-
-    def __init__(self, **kwargs):
-        DigestFlagger.__init__(self, **kwargs)
-
-    def digest(self, reads):
-        nonNullReads = [read for read in reads if read is not None]
-
-        self.addAlleleInfo(nonNullReads)
-
-
-if __name__ == "__main__":
-    # These data sources are fed to all flaggers
-    flaggerArguments = {
-        'reference': None if args.ref is None else pysamIterators.CachedFasta(
-            pysam.FastaFile(args.ref)),
-        'alleleResolver': None if args.alleles is None else alleleTools.AlleleResolver(
-            args.alleles, lazyLoad=not args.loadAllelesToMem),
-        'moleculeRadius': args.moleculeRadius,
-        'verbose': args.verbose,
-        'exon_gtf': args.exons,
-        'intron_gtf': args.introns
-    }
-
-    pairedEnd = False
-    flaggers = []
-    qFlagger = None
-    # if args.ftag:
-    # Now we ALWAYS put reads through qflagger
-    qFlagger = QueryNameFlagger(**flaggerArguments)
-    flaggers.append(qFlagger)
-    if args.nla:
-        flaggers.append(NlaIIIFlagger(**flaggerArguments))
-        pairedEnd = True
-    if args.mspji:
-        flaggers.append(MSPJIFlagger(**flaggerArguments))
-        pairedEnd = True
-    if args.chic:
-        flaggers.append(ChicSeqFlagger(**flaggerArguments))
-        pairedEnd = True
-    if args.scar:
-        flaggers.append(ScarFlagger(**flaggerArguments))
-        pairedEnd = True
-    if args.tag:
-        flaggers.append(TagFlagger(tag=args.tag))
-    if args.atag:
-        print("Running allele tagging")
-        flaggers.append(AlleleTagger(**flaggerArguments))
-    if args.rna:
-        flaggers.append(RNA_Flagger(**flaggerArguments))
-    if args.taps:
-        flaggers.append(TAPSFlagger(**flaggerArguments))
-        pairedEnd = True
-
-    if args.alleles is not None:
-        # Check if the variant file is valid..
-        if not (args.alleles.endswith('.vcf.gz')
-                or args.alleles.endswith('.bcf.gz')):
-            raise ValueError(f"""Please supply an indexed (bg)zipped VCF file.
-            You can convert your file using: bcftools view {args.alleles} -O b -o {args.alleles}.gz;
-            then index using bcftools index {args.alleles}.gz """)
-        if not (
-            os.path.exists(
-                args.alleles +
-                '.csi') or os.path.exists(
-                args.alleles +
-                '.tbi')):
-            raise ValueError(f"""Please supply an indexed (bg)zipped VCF file.
-            Index using: bcftools index {args.alleles} """)
 
-    if pairedEnd:
-        print('Assuming the input is paired end')
+    try: # Try to open the temp unsorted file:
+        unsorted_alignments = pysam.AlignmentFile(
+            unsorted_path, mode, header=header, **kwargs)
+    except Exception:
+        # Raise when this fails
+        raise
+
+    # Yield a handle to the alignments,
+    # this handle will be released when the handle runs out of scope
+    yield unsorted_alignments
+    unsorted_alignments.close()
+
+    if read_groups is not None:
+        add_readgroups_to_header(unsorted_path, read_groups)
+
+    # Write, sort and index
+    if input_is_sorted is False:
+        sort_and_index(
+            unsorted_path,
+            write_path,
+            remove_unsorted=True,
+            local_temp_sort=local_temp_sort,
+            fast_compression=fast_compression
+            )
     else:
-        print('Assuming the input is single end ( Has no influence on ftag)')
+        os.rename(unsorted_path, write_path)
+
+def write_program_tag(input_header,
+                      program_name,
+                      command_line,
+                      description,
+                      version
+                      ):
+    """Write Program Tag to bam file header
+    Args:
+        input_header  (dict): header to write PG tag to
+
+        program_name (str) : value to write to PN tag
+
+        command_line (str) : value to write to CL tag
+
+        version (str) : value to write to VN tag
+
+        description (str) : value to write to DS tag
+
+    """
+    if 'PG' not in input_header:
+        input_header['PG'] = []
+
+    blocked = set()
+    for prog_entry in input_header['PG']:
+        if prog_entry.get('PN','') == program_name:
+            blocked.add( prog_entry.get('ID','') )
+
+    proposed_id = program_name
+    i = 0
+    while proposed_id in blocked:
+        proposed_id= f'{program_name}_{i}'
+        i+=1
+
+    input_header['PG'].append({
+        'ID': proposed_id,
+        'PN': program_name,
+        'CL': command_line,
+        'VN': version,
+        'DS': description
+    })
+
+
+def bam_is_processed_by_program(alignments, program='bamtagmultiome'):
+    """Check if bam file has been processed by the supplied program
+
+    This function checks if there is an entry available in the 'PG'
+    block in header of the bam file where PN matches the program supplied.
+
+    Args:
+        alignments(pysam.AlignmentFile) : handle to bam file
+        program(str) : program to look for
+
+    Returns:
+        program_present(bool) : the program was used to process the bam file
+
+    """
+    for program_dict in alignments.header.as_dict()['PG']:
+        if program_dict.get('PN','') ==  program:
+            return True
+    return False
+
+
+def sort_and_index(
+        unsorted_path,
+        sorted_path,
+        remove_unsorted=False,
+        local_temp_sort=True,
+        fast_compression=False
+        ):
+    """ Sort and index a bam file
+    Args:
+        unsorted_path (str) : path to unsorted bam file
+
+        sorted_path (str) : write sorted file here
+
+        remove_unsorted (bool) : remove the unsorted file
+
+        local_temp_sort(bool): create temporary files in target directory
+    Raises:
+        SamtoolsError when sorting or indexing fails
+    """
+    if local_temp_sort:
+        base_directory = os.path.abspath( os.path.dirname(sorted_path) )
+        prefix = f'TMP.{uuid.uuid4()}'
+        temp_path_first = f'{base_directory}/{prefix}'
+        if temp_path_first.startswith('/TMP'):
+            # Perform sort in current directory
+            temp_path_first = f'./{prefix}'
+
+
+        # Try to sort at multiple locations, if sorting fails try the next until all locations have been tried
+        temp_paths =  [temp_path_first, f'/tmp/{prefix}', f'./{prefix}' ]
+        for i, temp_path in enumerate(temp_paths):
+            failed = False
+            try:
+                pysam.sort(
+                    '-o',
+                    sorted_path,
+                    '-T',
+                    f'{temp_path}', # Current directory with a random prefix
+                    unsorted_path, ('-l 1' if fast_compression else '-l 3')
+                )
+            except Exception as e:
+                failed = True
+                if i==len(temp_paths)-1:
+                    raise
 
-    if not os.path.exists(args.o):
+            if not failed:
+                break
+    else:
+        pysam.sort("-o", sorted_path, unsorted_path, ('-l 1' if fast_compression else '-l 3'))
+    pysam.index(sorted_path, '-@ 4')
+    if remove_unsorted:
+        os.remove(unsorted_path)
+
+
+class MapabilityReader(Prefetcher):
+
+    def __init__(self, mapability_safe_file_path, read_all=False, dont_open=True):
+        self.args = locals().copy()
+        del self.args['self']
+        self.mapability_safe_file_path = mapability_safe_file_path
+        if not dont_open:
+            self.handle = BlockZip(mapability_safe_file_path, 'r')
+
+
+    def instance(self, arg_update):
+        if 'self' in self.args:
+            del self.args['self']
+        clone = MapabilityReader(**self.args, dont_open=False)
+        return clone
+
+        # Todo: exit statements
+    def prefetch(self, contig, start, end):
+        clone = self.instance()
+        clone.handle.read_contig_to_cache( contig, region_start=start, region_end=end)
+        return clone
+
+    def site_is_mapable(self, contig, ds, strand):
+
+        if self.handle is None:
+            self.handle = BlockZip(self.mapability_safe_file_path, 'r')
+
+        """ Obtain if a restriction site is mapable or not
+        Args:
+            contig (str) : contig of site to look up
+            ds (int) : zero based coordinate of site to look up
+            strand (bool) : strand of site to look up (False: FWD, True: REV)
+
+        Returns:
+            site_is_mapable (bool) : True when the site is uniquely mapable, False otherwise
+        """
+        if self.handle[contig, ds, strand] == 'ok':
+            return True
+        return False
+
+
+def GATK_indel_realign(origin_bam, target_bam,
+                       contig, region_start, region_end,
+                       known_variants_vcf_path,
+                       # realignerTargetCreatorArgs=None,
+                       # indelRealignerArgs=None,
+                       gatk_path='GenomeAnalysisTK.jar',
+                       interval_path=None,
+                       java_cmd='java -jar -Xmx40G -Djava.io.tmpdir=./gatk_tmp',
+                       reference=None,
+                       interval_write_path=None
+                       ):
+    """
+    Re-align a specified region in a bam file using GenomeAnalysisTK
+
+    origin_bam (str) :  path to extract region from to re-align
+
+    target_bam(str) : path to write re-aligned reads to
+
+    contig (str) : contig of selected region
+
+    region_start (int) : start coordinate of region to re align (1 based)
+
+    region_end (int) :end coordiante of  selected region (1 based)
+
+    known_variants_vcf_path (str) : path to vcf containing reference variants
+
+    interval_path (str) : Use this intervals to perform realignment, when not specified intervals are generated using RealignerTargetCreator
+
+    interval_write_path (str) : when interval_path is not supplied, write the interval file here
+
+    java_cmd (str) : Command to open java
+
+    gatk_path (str) : path to GenomeAnalysisTK.jar
+
+    reference (str) : path to reference Fasta file
+    """
+    if not os.path.exists('./gatk_tmp'):
         try:
-            os.makedirs(args.o)
+            os.path.makedirs('./gatk_tmp')
         except Exception as e:
             pass
 
-    # Here we walk through the bamfiles and fetch
-    tmpprefix = f'{args.tmpprefix}'
+    # Detect reference from bam file
+    if reference is None:
+        reference = get_reference_path_from_bam(origin_bam)
+    if reference is None:
+        raise ValueError('Supply a path to a reference Fasta file (reference)')
+
+    if interval_path is None:
+        if interval_write_path is None:
+            interval_write_path = f"{target_bam.replace('.bam','')}.intervals"
+
+        target_creator_cmd = f'{java_cmd} {gatk_path} \
+        -T RealignerTargetCreator \
+        -R {reference} \
+        -L {contig}:{region_start}-{region_end} \
+        -known {known_variants_vcf_path} \
+        -I {origin_bam} \
+        -o {interval_write_path}'
+
+        # Create the intervals file
+        os.system(target_creator_cmd)
+        interval_path = interval_write_path
+
+    # Perform realignment
+    realign_cmd = f'{java_cmd} {gatk_path} \
+    -T IndelRealigner \
+    -R {reference} \
+    -targetIntervals {interval_path} \
+    -known {known_variants_vcf_path} \
+    -L {contig}:{region_start}-{region_end} \
+    -I {origin_bam} \
+    -o {target_bam} \
+    -dcov 1000000 \
+    -maxReads 2000000'
+    os.system(realign_cmd)
+    return target_bam
 
-    for bamFilePath in args.bamfiles:
+def get_random_locations(bam, n):
+    """Select random locations in the supplied bam file
 
-        bamFile = pysam.AlignmentFile(bamFilePath, "rb")
-        header = bamFile.header.copy()
-        outPathTemp = f'{args.o}/{os.path.basename(bamFilePath)}.unsorted'
-        outPathTempWithHeader = f'{args.o}/{os.path.basename(bamFilePath)}.unsorted.with_header.bam'
-        outPath = f"{args.o}/{os.path.basename(bamFilePath).replace('.bam', '')}.bam"
-
-        print(f'Now reading {bamFilePath}, writing to {outPath}')
-        if args.dedup:
-            dedupOutPathTemp = f'{args.o}/{os.path.basename(bamFilePath)}.dedup.unsorted'
-            dedupOutPathTempWithHeader = f'{args.o}/{os.path.basename(bamFilePath)}.dedup.with_header.bam'
-            dedupOutPath = f"{args.o}/{os.path.basename(bamFilePath).replace('.bam', '')}.dedup.bam"
-            dedupOutputFile = pysam.AlignmentFile(
-                dedupOutPathTemp, "wb", header=header)
-        outputFile = pysam.AlignmentFile(outPathTemp, "wb", header=header)
-
-        bamName = os.path.basename(bamFilePath).replace('.bam', '')
-        # if os.path.exists(outPath+'.bai'):
-        #    continue
-        i = 0
-        if pairedEnd:
-            it = pysamIterators.MatePairIterator(
-                bamFile, performProperPairCheck=False, contig=args.chr)
-
-            for i, (R1, R2) in enumerate(it):
-                for flagger in flaggers:
-                    try:
-                        flagger.digest([R1, R2])
-                    except Exception as e:
-                        print(e)
-
-                        if args.fatal:
-                            print(R1, R2)
-                            raise e
-
-                try:
-                    if R1 is not None:
-                        outputFile.write(R1)
-                    if R2 is not None:
-                        outputFile.write(R2)
-                except Exception as e:
-                    for flagger in flaggers:
-                        print(flagger)
-                    raise e
-                if args.dedup and (
-                    (R1 is not None and R1.has_tag('RC') and R1.get_tag('RC') == 1) or (
-                        R2 is not None and R2.has_tag('RC') and R2.get_tag('RC') == 1)):
-                    if R1 is not None:
-                        dedupOutputFile.write(R1)
-                    if R2 is not None:
-                        dedupOutputFile.write(R2)
+    bam(str or pysam.AlignmentFile)
 
-                if args.head is not None and i >= args.head:
-                    break
-        else:
-            iterator = bamFile.fetch(
-                contig=args.chr) if args.chr is not None else bamFile
-            for i, R1 in enumerate(iterator):
-
-                for flagger in flaggers:
-                    try:
-                        flagger.digest([R1])
-                    except Exception as e:
-                        if args.fatal:
-                            raise e
-                        print(e)
-
-                outputFile.write(R1)
-
-                if args.head is not None and i >= args.head:
-                    break
-        print(f'{bamFilePath}: processed {i} reads')
-
-        print("Finishing files (forcing close)")
-        outputFile.close()
-        if args.dedup:
-            dedupOutputFile.close()
-
-        if qFlagger is not None:
-            readGroups = {}
-
-            for readGroup in qFlagger.assignedReadGroups:
-                flowCell, lane, sampleLib = readGroup.split('.')
-                library, sample = sampleLib.rsplit('_', 1)
-                readGroups[readGroup] = {
-                    'ID': readGroup,
-                    'LB': library,
-                    'PL': 'ILLUMINA',
-                    'SM': sample,
-                    'PU': readGroup}
-
-            headerSamFilePath = outPath.replace('.bam', '') + '.header.sam'
-            hCopy = header.to_dict()
-            hCopy['RG'] = list(readGroups.values())
-            with gzip.open(outPathTemp.replace('.bam', '') + '.readGroups.pickle.gz', 'wb') as rgzip, pysam.AlignmentFile(headerSamFilePath, 'w', header=hCopy) as headerSam:
-                pickle.dump(readGroups, rgzip)
-
-                # for readGroup, fields in readGroups.items():
-                #    headerSam.write(f'@RG\tID:{readGroup}\tPL:{fields["PL"]}\tSM:{fields["SM"]}\tPU:{fields["PU"]}\tLB:{fields["LB"]}\n')
-            # Clear the read groups
-            qFlagger.assignedReadGroups = set()
-
-            # Perform a reheading, sort and index
-            rehead_cmd = f"""{{ cat {headerSamFilePath}; samtools view {outPathTemp}; }} | samtools view -b > {outPathTempWithHeader} ;
-            rm {outPathTemp};
-            samtools sort -T {tmpprefix} {outPathTempWithHeader} > {outPath}; samtools index {outPath};
-            rm {outPathTempWithHeader};
-            """
-            print(f"Adding read groups to header and sorting.")
-            os.system(rehead_cmd)
-
-            # Same procedure for dedup:
-            if args.dedup:
-                rehead_cmd = f"""{{ cat {headerSamFilePath}; samtools view {dedupOutPathTemp}; }} | samtools view -b > {dedupOutPathTempWithHeader} ;
-                rm {dedupOutPathTemp};
-                samtools sort -T {tmpprefix} {dedupOutPathTempWithHeader} > {dedupOutPath}; samtools index {dedupOutPath};
-                rm {dedupOutPathTempWithHeader};
-                """
-                print(f"Dedup file: adding read groups to header and sorting.")
-                os.system(rehead_cmd)
+    n(int) : amount of locations to generate
+
+    returns: generator of (contig,position) tuples
+    """
+
+    cs = get_contig_sizes(bam)
+    # Obtain cumulative amount of bases per contig:
+    cumulative_size = np.cumsum([size for contig,size in cs.items()])
+    cs_contigs = np.array( list(cs.keys()) )
+
+    random_locations = np.random.randint(0, cumulative_size[-1], n)
+    indices = np.searchsorted(cumulative_size, random_locations)
+    random_positions = random_locations-np.concatenate( ([0], cumulative_size))[indices]
+    random_contigs = cs_contigs[indices]
+
+    return zip(random_contigs, random_positions)
+
+
+
+def sample_location(handle, contig, pos,dedup=True, qc=True):
+    """
+    Obtain dictionary containing the coverage for every sample
+
+    Args:
+        handle (pysam.AlignmentFile)  : File to obtain reads from
+
+        contig (str) : contig to sample
+
+        pos (int) : coordinate to sample (zero based)
+
+        dedup(bool) : ignore duplicated reads
+
+        qc(bool) : ignore qc failed reads
+
+    Returns:
+        samples (dict) : dictionary with amount of reads at the selected locations
+
+    """
+    overlap = {} # sample -> coverage
+    for column in pileup_truncated(handle, contig, pos, pos+1):
+        for pileread in column.pileups:
+            if not pileread.is_del and not pileread.is_refskip:
+                sample = pileread.alignment.get_tag('SM')
+                if dedup and pileread.alignment.is_duplicate:
+                    continue
+                if qc and pileread.alignment.is_qcfail:
+                    continue
+
+                if not sample in overlap:
+                    overlap[sample]=1
+                else:
+                    overlap[sample]+=1
+    return overlap
+
+
+def get_read_group_from_read(read, format, with_attr_dict=False):
+    rg_id=None
+    platform = read.get_tag('Fc') if read.has_tag('Fc') else 'NONE'
+    lane = read.get_tag('La') if read.has_tag('La') else 'NONE'
+    library = read.get_tag('LY') if read.has_tag('LY') else 'NONE'
+    if format==0:
+        sample = read.get_tag('SM')
+    elif format==1:
+        sample = read.get_tag('LY')
+    else:
+        raise ValueError(f'{format} is an unknown read group format')
 
+    rg_id =  f'{platform}.{lane}.{sample}'
+    if with_attr_dict:
+        rg_dict = {
+                'ID':rg_id,
+                'LB':library,
+                'PL':platform,
+                'SM':sample,
+                'PU': rg_id }
+
+    if rg_id is None:
+        raise ValueError('No read group information could be extracted')
+
+    if with_attr_dict:
+        return rg_id, rg_dict
+    return rg_id
+
+
+def random_sample_bam(bam,n,**sample_location_args):
+    """Sample a bam file at random locations
+
+    Args:
+        bam (pysam.AlignmentFile) : bam to sample from
+
+        n (int) : Amount of locations to sample
+
+        *sample_location_args : arguments to pass to sample_location
+
+    Returns:
+        samples (dict) : dictionary with amount of reads at the selected locations
+
+    """
+    r = [sample_location(bam, contig, pos,**sample_location_args)
+    for contig, pos in get_random_locations(bam, n)]
+    return pd.DataFrame(r)
+
+
+def replace_bam_header(origin_bam_path, header, target_bam_path=None, header_write_mode='auto'):
+
+    if target_bam_path is None:
+        target_bam_path = origin_bam_path
+
+    # Write the re-headered bam file to this path
+    complete_temp_path = origin_bam_path.replace('.bam', '') + '.rehead.bam'
+
+    # When header_write_mode is auto, when samtools is available, samtools
+    # will be used, otherwise pysam
+    if header_write_mode == 'auto':
+        if which('samtools') is None:
+            header_write_mode = 'pysam'
         else:
-            # we cannot assign readgroups...
-            rehead_cmd = f"""
-            samtools sort -T {tmpprefix} {outPathTemp} > {outPath}; samtools index {outPath};
-            rm {outPathTemp};
-            """
-            print(f"Adding read groups to header and sorting.")
-            os.system(rehead_cmd)
-
-            if args.dedup:
-                rehead_cmd = f"""
-                samtools sort -T {tmpprefix} {dedupOutPathTemp} > {dedupOutPath}; samtools index {dedupOutPath};
-                rm {dedupOutPathTemp};
+            header_write_mode = 'samtools'
+
+    if header_write_mode == 'pysam':
+
+        with pysam.AlignmentFile(complete_temp_path, "wb", header=header) as out, \
+             pysam.AlignmentFile(origin_bam_path) as origin:
+            for read in origin:
+                out.write(read)
+
+        os.rename(complete_temp_path, target_bam_path)
+
+    elif header_write_mode == 'samtools':
+
+        # Write the new header to this sam file:
+        headerSamFilePath = origin_bam_path.replace(
+            '.bam', '') + '.header.sam'
+
+        # Write the sam file with the complete header:
+        with pysam.AlignmentFile(headerSamFilePath, 'w', header=header):
+            pass
+
+        # Concatenate and remove origin
+        rehead_cmd = f"""{{ cat {headerSamFilePath}; samtools view {origin_bam_path}; }} | samtools view -b > {complete_temp_path} ;
+                mv {complete_temp_path } {target_bam_path};rm {headerSamFilePath};
                 """
-                print(f"Dedup file: adding read groups to header and sorting.")
-                os.system(rehead_cmd)
+        os.system(rehead_cmd)
+    else:
+        raise ValueError(
+            'header_write_mode should be either, auto, pysam or samtools')
+
 
-    """
-    Is:NS500414;RN:455;Fc:HYLVHBGX5;La:3;Ti:13601;CX:9882;CY:17671;Fi:N;CN:0;aa:CCGTCC;aA:CCGTCC;aI:16;LY:A3-P15-1-1;RX:ACG;RQ:GGG;BI:17;bc:ACTCGATG;BC:ACTCGATG;QT:GGKKKKKK;MX:NLAIII384C8U3;A2:TGG;AQ:E6E
-    for f in $(ls *.bam | cut -f 1,2,3 -d '-' | sort | uniq | grep -v bam); do submission.py -y -time 20 -t 1 "addTagsToLennartNLABam.py $f*cell*.bam"; done
+
+def add_readgroups_to_header(
+        origin_bam_path,
+        readgroups_in,
+        target_bam_path=None,
+        header_write_mode='auto'):
+    """ Add the readgroups in the set readgroups to the header of origin_bam_path.
+
+    This function first loads the header of the origin to memory.
+    The supplied readgroups are added to this header.
+    The new header is then exported to a SAM file. The SAM file is then
+    concatenated to the original bam file.
+
+    Args:
+        origin_bam_path(str) : path to bam file to which to add readgroups to header
+
+        readgroups_in(set/dict) : set or dictionary which contains read groups. The dictionary should have the format { read_group_id (str)
+                { 'ID': ID, 'LB':library,
+                'PL':platform,
+                'SM':sampleLib,
+                'PU':readGroup }
+
+        target_bam_path(str) : path to write bam file including the readgrouped header to. When not supplied the output is written to the input bam file
 
     """
+
+    # Create a read group dictionary
+    if isinstance(readgroups_in, set):
+        readGroupsDict = {}
+        for readGroup in readgroups_in:
+            flowCell, lane, sampleLib = readGroup.split('.')
+            try:
+                library, _ = sampleLib.rsplit('_', 1)
+            except Exception as e:
+                # the library is not part of the sample name:
+                library = 'undefinedLibrary'
+            readGroupsDict[readGroup] = {
+                'ID': readGroup,
+                'LB': library,
+                'PL': 'ILLUMINA',
+                'SM': sampleLib,
+                'PU': readGroup}
+    elif isinstance(readgroups_in, dict):
+        readGroupsDict = readgroups_in
+    else:
+        raise ValueError("supply a set or dict for readgroups_in")
+
+    with pysam.AlignmentFile(origin_bam_path, "rb") as origin:
+        header = origin.header.copy()
+        hCopy = header.to_dict()
+        hCopy['RG'] = list(readGroupsDict.values())
+        replace_bam_header(origin_bam_path, hCopy,
+                            target_bam_path=target_bam_path,
+                            header_write_mode=header_write_mode)
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/utils/binning.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/utils/binning.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def coordinate_to_sliding_bin_locations(dp, bin_size, sliding_increment):
     """
     Convert a single value to a list of overlapping bins
 
     Parameters
-    ----------
+    -----   -----
     point : int
         coordinate to look up
 
     bin_size : int
         bin size
 
     sliding_increment : int
@@ -56,7 +56,33 @@
     list: [(bin_start,bin_end), .. ]
 
     """
     start, end, start_id, end_id = coordinate_to_sliding_bin_locations(
         point, bin_size, sliding_increment)
     return [(i * sliding_increment, i * sliding_increment + bin_size)
             for i in range(start_id, end_id + 1)]
+
+
+def bp_chunked(job_generator, bp_per_job):
+    """ Chunk an iterator containing coordinate sorted tasks in chunks of a total size of roughly bp_per_job
+
+    Args:
+        job_generator : iterable of commands, format (contig, start, end, *task)
+        bp_per_job (int) : Amount of bp per chunk of jobs/tasks
+
+    Yields:
+        chunk(list) :  [(contig, start, end, *task),(contig, start, end, *task),..]
+
+    @todo: contig is not used, this function expects that only bins on a single contig are supplied
+    """
+    bp_current = 0
+    current_tasks = []
+    for job in job_generator:
+        start,end = job[1],job[2]
+        bp_current += abs(end-start)
+        current_tasks.append(job)
+
+        if bp_current>=bp_per_job:
+            yield current_tasks
+            bp_current=0
+            current_tasks=[]
+    yield current_tasks
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/utils/html.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/utils/html.py`

 * *Files identical despite different names*

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics/utils/sequtils.py` & `singlecellmultiomics-0.1.9/singlecellmultiomics/utils/sequtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import math
 from pysam import FastaFile
+
+
 def is_main_chromosome(chrom):
     """ Returns True when the chromsome is a main chromsome,
     not an alternative or other
 
     Args:
         chrom(str) : chromosome name
 
@@ -12,33 +14,59 @@
 
     """
     if chrom.startswith('KN') or chrom.startswith('KZ') or chrom.startswith('JH') or chrom.startswith('GL') or chrom.startswith(
             'KI') or chrom.startswith('chrUn') or chrom.endswith('_random') or 'ERCC' in chrom or chrom.endswith('_alt') or "HLA-" in chrom:
         return False
     return True
 
-def get_contig_list_from_fasta(fasta_path):
+def get_contig_list_from_fasta(fasta_path, with_length=False):
     """Obtain list of contigs froma  fasta file,
         all alternative contigs are pooled into the string MISC_ALT_CONTIGS_SCMO
 
+    Args:
+        fasta_path (str or pysam.FastaFile) : Path or handle to fasta file
+
+        with_length(bool): return list of lengths
+
     Returns:
-        contig_list (list) : List of contigs + ['MISC_ALT_CONTIGS_SCMO'] if any alt contig is present in the fasta file
+        contig_list (list ) : List of contigs + ['MISC_ALT_CONTIGS_SCMO'] if any alt contig is present in the fasta file
         """
 
     contig_list = []
     has_alt = False
-    with FastaFile(fasta_path) as fa:
-        for reference in fa.references:
-            if is_main_chromosome(reference):
-                contig_list.append(reference)
-            else:
-                has_alt = True
+    if with_length:
+        lens = []
+
+    if type(fasta_path) is str:
+        fa = FastaFile(fasta_path)
+    elif type(fasta_path) is FastaFile:
+        fa = fasta_path
+    else:
+        raise TypeError('Supply pysam.FastaFile or str')
+
+    for reference, length in zip(fa.references, fa.lengths):
+        if is_main_chromosome(reference):
+            contig_list.append(reference)
+            if with_length:
+                lens.append(length)
+        else:
+            has_alt = True
+
+    # Close handle if we just opened one
+    if type(fasta_path) is str:
+        fa.close()
 
     if has_alt:
         contig_list.append('MISC_ALT_CONTIGS_SCMO')
+        if with_length:
+            lens.append(None)
+
+    if with_length:
+        return contig_list, lens
+
     return contig_list
 
 def phred_to_prob(phred):
     """Convert a phred score (ASCII) or integer to a numeric probability
     Args:
         phred (str/int) : score to convert
     returns:
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/PKG-INFO` & `singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: singlecellmultiomics
-Version: 0.1.7
+Version: 0.1.9
 Summary: Tools to deal with one or more measurements from single cells
 Home-page: https://github.com/BuysDB/SingleCellMultiOmics
 Author: Buys de Barbanson
 Author-email: b.barbanson@hubrecht.eu
 License: MIT
-Download-URL: https://github.com/BuysDB/SingleCellMultiOmics/archive/v0.1.6.tar.gz
+Download-URL: https://github.com/BuysDB/SingleCellMultiOmics/archive/v0.1.9.tar.gz
 Description: [![Build Status](https://travis-ci.com/BuysDB/SingleCellMultiOmics.svg?branch=master)](https://travis-ci.com/BuysDB/SingleCellMultiOmics) [![Documentation Status](https://readthedocs.org/projects/singlecellmultiomics/badge/?version=latest)](https://singlecellmultiomics.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/singlecellmultiomics.svg)](https://badge.fury.io/py/singlecellmultiomics) [![Anaconda-Server Badge](https://anaconda.org/buysdb/singlecellmultiomics/badges/installer/conda.svg)](https://anaconda.org/buysdb/singlecellmultiomics)
         
         ## Single cell multi omics
         Single cell multi omics is a set of tools to deal with multiple measurements from the same cell. This package has been developed by the [van Oudenaarden group](https://www.hubrecht.eu/research-groups/van-oudenaarden-group/).
         
         # Installation
         ```
         git clone https://github.com/BuysDB/SingleCellMultiOmics
         pip install ./SingleCellMultiOmics
         ```
         For creating a virtual environment look [here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Python-test-and-run-environment)
         
         # Usage
-        
-        The following tools are available:
-        
-        demux.py:
+        `demux.py`:
         This tool demultiplexes raw fastq files, adapters, molecule and cell information are removed from the fastq records and encoded into the read name including their base-calling qualities.
         Additional stored inforation includes:
         - Assigned and raw illumina index
         - Library
         - Demultiplexing strategy used for demultiplexing (What kind of data the read is derived from)
         - Assigned barcode index
         
@@ -35,50 +32,62 @@
         
         For RNA seq data aligned to a transcriptome the step after this is to run featureCounts.
         
         The mapped reads are encoded in a BAM file. This BAM file still contains the encoded data and this has to be decoded in order to get a useful BAM file.
         `bamtagmultiome.py`
         1) Recodes the original read names and extracts all information previously encoded by the demultiplexer.
         2) Adds allele information. (A VCF file is required for this)
-        3) Supports multiple protocols: 
-         RNA:CELSEQ1, CELSEQ2, VASA (with 8 and 6bp UMI), 
+        3) Supports multiple protocols:
+         RNA:CELSEQ1, CELSEQ2, VASA (with 8 and 6bp UMI),
          methylation digest sequencing:SC MSPJI ,  
-         lineage tracing:SCARTRACE, 
+         lineage tracing:SCARTRACE,
          DNA digest sequencing: NLAIII, 
          histone modification sequencing: scCHIC,
          Single cell methylation : TAPs (in combination with any other supported protocol).
-         
+        
         4) Assigns reads to molecules to allow for deduplication, adds duplication BAM flag
         5) Assigns read groups
+        6) Splits libraries where multiple modalities are measured
+        7) Estimates consensus sequences of molecules
         
         All SAM tags used and written by this package are listed in [TAGS.MD](https://github.com/BuysDB/SingleCellMultiOmics/blob/master/TAGS.MD)
         
+        `bamToCountTable.py`
+        [Extracts a count table from a bam file, look here for examples.](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Bam-file-to-count-table)
+        
+        
+        `libraryStatistics.py`
+        [All statistics plots can be generated with a single script, look here for details.](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Library-statistics-plots)
         
         # Examples:
         
         Demultiplex all fastq.gz files in the current directory using NLAIII barcodes
         ```
         demux.py *.fastq.gz -use NLAIII384C8U3 --y
         ````
         
         Demultiplex only the specified sequencing index (GTTTGA), and everything 1 hamming distance away from GTTTGA  :
         ```
         demux.py -si GTTTGA *.gz --y --hdi 1
         ```
         
+        ### API: Using SingleCellMultiOmics from python
+        [All molecule and fragment information can be accessed using python](https://github.com/BuysDB/SingleCellMultiOmics/wiki/Molecule-iteration)
+        [Documentation for the classes in available here](https://singlecellmultiomics.readthedocs.io/en/latest/py-modindex.html)
+        
         ### scCHIC
         For every fragment in input.bam find scCHIC seq fragments and deduplicate these. Fragments with the same cell barcode, umi, library and strand and starting within a range of 5 bp from each other are assigned as duplicate. The mnase cut site location is expected to be between the first base (Usually an A) this A is part of the sequencing adapter, and the second base (Usually a T). The cut site location is recorded into the DS tag. When alleles are specified using -alleles, the molecule assignment is split up by allele, this means that if two fragments map to the same location and share the same umi, but contain SNPs which indicate differing alleles, the reads are not assigned to the same molecule. For every fragment the ligation sequence is recorded into the RZ tag.
         ```
-        bamtagmultiome.py input.bam -method chic -o tagged.bam 
+        bamtagmultiome.py input.bam -method chic -o tagged.bam
         ```
         [Complete scCHIC data processing instructions from FastQ to count table here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/scCHIC-data-processing)
         ### NlaIII
         For every fragment in input.bam find NLAIII seq fragments and deduplicate these. Fragments with the same cell barcode, umi, library and strand are assigned as duplicate. The NlaIII cut site location is recorded into the DS tag. When alleles are specified using -alleles, the molecule assignment is split up by allele, this means that if two fragments map to the same location and share the same UMI, but contain SNPs which indicate differing alleles, the reads are not assigned to the same molecule. For every fragment the sequenced part of the NlaIII cut site sequence is recorded into the RZ tag, this is usually CATG, but is allowed to be shifted 1 base to ATG. In the NlaIII protocol a reverse transcription (RT) is used, generally capturing more reverse transcription reactions will yield a more accurate molecule consensus sequence. For every fragment which support the molecule the reverse transcription reaction is recorded by storing the location of the random primer used for RT and the sequence of the random primer.
         ```
-        bamtagmultiome.py input.bam -method nla -o tagged.bam 
+        bamtagmultiome.py input.bam -method nla -o tagged.bam
          ```
          [Complete NlaIII data processing instructions from FastQ to count table here](https://github.com/BuysDB/SingleCellMultiOmics/wiki/NLA-III-data-processing)
         
         
         ### Plate visualisation
         
         Show relative abundance of reads and unique molecules across 384 well plate.
```

### Comparing `singlecellmultiomics-0.1.7/singlecellmultiomics.egg-info/SOURCES.txt` & `singlecellmultiomics-0.1.9/singlecellmultiomics.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,81 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+data/chic_test_region.bam
+data/chic_test_region.bam.bai
 data/mini_nla_test.bam
 data/mini_nla_test.bam.bai
 data/mini_test.bed
 singlecellmultiomics/__init__.py
 singlecellmultiomics/version.py
 singlecellmultiomics.egg-info/PKG-INFO
 singlecellmultiomics.egg-info/SOURCES.txt
 singlecellmultiomics.egg-info/dependency_links.txt
 singlecellmultiomics.egg-info/requires.txt
 singlecellmultiomics.egg-info/top_level.txt
 singlecellmultiomics/alleleTools/__init__.py
 singlecellmultiomics/alleleTools/alleleTools.py
+singlecellmultiomics/alleleTools/heterozygousSNPedit.py
 singlecellmultiomics/bamProcessing/__init__.py
 singlecellmultiomics/bamProcessing/alignment_view.py
+singlecellmultiomics/bamProcessing/bamBinCounts.py
+singlecellmultiomics/bamProcessing/bamCopyNumber.py
 singlecellmultiomics/bamProcessing/bamDuprate.py
 singlecellmultiomics/bamProcessing/bamExtractRandomPrimerStats.py
+singlecellmultiomics/bamProcessing/bamExtractSamples.py
+singlecellmultiomics/bamProcessing/bamExtractVariants.py
 singlecellmultiomics/bamProcessing/bamFeatureDensityVisualisation.py
+singlecellmultiomics/bamProcessing/bamFeatures.py
 singlecellmultiomics/bamProcessing/bamFilter.py
 singlecellmultiomics/bamProcessing/bamFunctions.py
 singlecellmultiomics/bamProcessing/bamMappingRate.py
+singlecellmultiomics/bamProcessing/bamMatchGATKBQSRReport.py
 singlecellmultiomics/bamProcessing/bamPlateVisualisation.py
 singlecellmultiomics/bamProcessing/bamPlotRTstats.py
+singlecellmultiomics/bamProcessing/bamReadGroupFormat.py
+singlecellmultiomics/bamProcessing/bamSplitByTag.py
 singlecellmultiomics/bamProcessing/bamTabulator.py
 singlecellmultiomics/bamProcessing/bamToCountTable.py
 singlecellmultiomics/bamProcessing/bamToMethylationAndCopyNumber.py
+singlecellmultiomics/bamProcessing/bamToMethylationCalls.py
 singlecellmultiomics/bamProcessing/bamToRNACounts.py
+singlecellmultiomics/bamProcessing/pileup.py
+singlecellmultiomics/bamProcessing/split_bam_by_cluster.py
+singlecellmultiomics/bamProcessing/split_double_BAM.py
 singlecellmultiomics/bamProcessing/structureTensor.py
 singlecellmultiomics/bamProcessing/variantStats.py
 singlecellmultiomics/barcodeFileParser/__init__.py
 singlecellmultiomics/barcodeFileParser/barcodeFileParser.py
 singlecellmultiomics/countTableProcessing/__init__.py
 singlecellmultiomics/countTableProcessing/correct_count_table_bias.py
 singlecellmultiomics/countTableProcessing/downsampleDataFrame.py
-singlecellmultiomics/fastaProcessing/createMapabilityIndex.py
+singlecellmultiomics/fastaProcessing/__init__.py
+singlecellmultiomics/fastaProcessing/createMappabilityIndex.py
+singlecellmultiomics/fastaProcessing/fastaHandle.py
 singlecellmultiomics/fastaProcessing/fastaMaskVariants.py
 singlecellmultiomics/fastqProcessing/__init__.py
 singlecellmultiomics/fastqProcessing/fastqHandle.py
 singlecellmultiomics/fastqProcessing/fastqIterator.py
 singlecellmultiomics/features/__init__.py
 singlecellmultiomics/features/exonGTFtoIntronGTF.py
 singlecellmultiomics/features/features.py
 singlecellmultiomics/fragment/__init__.py
 singlecellmultiomics/fragment/chic.py
 singlecellmultiomics/fragment/fragment.py
 singlecellmultiomics/fragment/nlaIII.py
+singlecellmultiomics/fragment/scartrace.py
 singlecellmultiomics/libraryDetection/__init__.py
 singlecellmultiomics/libraryDetection/archivestats.py
 singlecellmultiomics/libraryDetection/sequencingLibraryListing.py
 singlecellmultiomics/libraryProcessing/__init__.py
 singlecellmultiomics/libraryProcessing/libraryStatistics.py
+singlecellmultiomics/methylation/__init__.py
+singlecellmultiomics/methylation/methylation.py
 singlecellmultiomics/modularDemultiplexer/__init__.py
 singlecellmultiomics/modularDemultiplexer/baseDemultiplexMethods.py
 singlecellmultiomics/modularDemultiplexer/demultiplexedFastqConversion.py
 singlecellmultiomics/modularDemultiplexer/demultiplexingStrategyLoader.py
 singlecellmultiomics/modularDemultiplexer/demux.py
 singlecellmultiomics/modularDemultiplexer/barcodes/celseq1.bc
 singlecellmultiomics/modularDemultiplexer/barcodes/celseq2.bc
@@ -84,38 +104,57 @@
 singlecellmultiomics/modularDemultiplexer/indices/illumina_i7_indices.bc
 singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_ThruPlex48S_RP.bc
 singlecellmultiomics/modularDemultiplexer/indices/illumina_merged_iPCR_RP.bc
 singlecellmultiomics/molecule/__init__.py
 singlecellmultiomics/molecule/chic.py
 singlecellmultiomics/molecule/consensus.py
 singlecellmultiomics/molecule/featureannotatedmolecule.py
+singlecellmultiomics/molecule/filter.py
 singlecellmultiomics/molecule/fourthiouridine.py
 singlecellmultiomics/molecule/iterator.py
 singlecellmultiomics/molecule/molecule.py
 singlecellmultiomics/molecule/nlaIII.py
 singlecellmultiomics/molecule/rna.py
+singlecellmultiomics/molecule/scartrace.py
 singlecellmultiomics/molecule/taps.py
 singlecellmultiomics/molecule/consensus_model/nla_140bp_pe_juan_1M.pickle
+singlecellmultiomics/molecule/consensus_model/sk_NR3_mf3_trained_hard_fit_9939.h5
 singlecellmultiomics/pyutils/__init__.py
 singlecellmultiomics/pyutils/handlelimiter.py
 singlecellmultiomics/pyutils/pyutils.py
 singlecellmultiomics/snakemake_workflows/scmo_workflow.py
 singlecellmultiomics/snakemake_workflows/_general/sge_wrapper.py
+singlecellmultiomics/snakemake_workflows/_general/slurm_wrapper.py
+singlecellmultiomics/snakemake_workflows/call_sc_variants/Snakefile
+singlecellmultiomics/snakemake_workflows/call_sc_variants/config.json
+singlecellmultiomics/snakemake_workflows/call_variants/Snakefile
+singlecellmultiomics/snakemake_workflows/call_variants/config.json
 singlecellmultiomics/snakemake_workflows/chic/Snakefile
 singlecellmultiomics/snakemake_workflows/chic/config.json
 singlecellmultiomics/snakemake_workflows/chic_allelic/Snakefile
 singlecellmultiomics/snakemake_workflows/chic_allelic/config.json
+singlecellmultiomics/snakemake_workflows/cs2/Snakefile
+singlecellmultiomics/snakemake_workflows/cs2/config.json
+singlecellmultiomics/snakemake_workflows/cs2_scmo/Snakefile
+singlecellmultiomics/snakemake_workflows/cs2_scmo/config.json
 singlecellmultiomics/snakemake_workflows/demux/demux.smk
+singlecellmultiomics/snakemake_workflows/merge_fastq/Snakefile
+singlecellmultiomics/snakemake_workflows/mutect_bulk/Snakefile
+singlecellmultiomics/snakemake_workflows/mutect_bulk/config.json
 singlecellmultiomics/snakemake_workflows/nlaIII/Snakefile
 singlecellmultiomics/snakemake_workflows/nlaIII/config.json
+singlecellmultiomics/snakemake_workflows/scartrace/Snakefile
+singlecellmultiomics/snakemake_workflows/scartrace/config.json
 singlecellmultiomics/statistic/__init__.py
 singlecellmultiomics/statistic/allele.py
+singlecellmultiomics/statistic/cellreadcount.py
 singlecellmultiomics/statistic/conversions.py
 singlecellmultiomics/statistic/datatype.py
 singlecellmultiomics/statistic/fragmentsize.py
+singlecellmultiomics/statistic/lorenz.py
 singlecellmultiomics/statistic/mappingquality.py
 singlecellmultiomics/statistic/methylation.py
 singlecellmultiomics/statistic/oversequencing.py
 singlecellmultiomics/statistic/plate.py
 singlecellmultiomics/statistic/readcount.py
 singlecellmultiomics/statistic/rejectionreasons.py
 singlecellmultiomics/statistic/scchicligation.py
@@ -126,26 +165,41 @@
 singlecellmultiomics/tags/tags.py
 singlecellmultiomics/tags/write_tags_md.py
 singlecellmultiomics/tagtools/__init__.py
 singlecellmultiomics/tagtools/tagtools.py
 singlecellmultiomics/universalBamTagger/4SUtagger.py
 singlecellmultiomics/universalBamTagger/__init__.py
 singlecellmultiomics/universalBamTagger/bamtagmultiome.py
+singlecellmultiomics/universalBamTagger/bamtagmultiome_multi.py
 singlecellmultiomics/universalBamTagger/customreads.py
 singlecellmultiomics/universalBamTagger/digest.py
 singlecellmultiomics/universalBamTagger/mspjI.py
 singlecellmultiomics/universalBamTagger/nlaIII.py
 singlecellmultiomics/universalBamTagger/rna.py
 singlecellmultiomics/universalBamTagger/scar.py
 singlecellmultiomics/universalBamTagger/scchic.py
 singlecellmultiomics/universalBamTagger/tag.py
+singlecellmultiomics/universalBamTagger/tagging.py
 singlecellmultiomics/universalBamTagger/taps.py
 singlecellmultiomics/universalBamTagger/tapsTabulator.py
 singlecellmultiomics/universalBamTagger/tapsTagger.py
 singlecellmultiomics/universalBamTagger/universalBamTagger.py
 singlecellmultiomics/utils/__init__.py
+singlecellmultiomics/utils/bdbbio.py
+singlecellmultiomics/utils/bdbplot.py
+singlecellmultiomics/utils/bdbsstats.py
 singlecellmultiomics/utils/binning.py
 singlecellmultiomics/utils/blockzip.py
+singlecellmultiomics/utils/copyNumberStatePlotter.py
+singlecellmultiomics/utils/export.py
 singlecellmultiomics/utils/html.py
 singlecellmultiomics/utils/iteration.py
+singlecellmultiomics/utils/organoidTools.py
+singlecellmultiomics/utils/pandas.py
+singlecellmultiomics/utils/plotting.py
+singlecellmultiomics/utils/prefetch.py
 singlecellmultiomics/utils/sequtils.py
-singlecellmultiomics/utils/submission.py
+singlecellmultiomics/utils/submission.py
+singlecellmultiomics/variants/__init__.py
+singlecellmultiomics/variants/postProcessVariants.py
+singlecellmultiomics/variants/variantWrapper.py
+singlecellmultiomics/variants/vcfFilterAlleleFreq.py
```

