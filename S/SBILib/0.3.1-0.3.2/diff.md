# Comparing `tmp/SBILib-0.3.1.tar.gz` & `tmp/SBILib-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILib-0.3.1.tar", last modified: Thu Jul 20 16:24:58 2023, max compression
+gzip compressed data, was "SBILib-0.3.2.tar", last modified: Fri Jul 21 16:14:42 2023, max compression
```

## Comparing `SBILib-0.3.1.tar` & `SBILib-0.3.2.tar`

### file list

```diff
@@ -1,164 +1,166 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.685818 SBILib-0.3.1/
--rw-r--r--   0 patrick    (501) staff       (20)      120 2023-07-20 16:20:24.000000 SBILib-0.3.1/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)    25403 2023-07-20 16:24:58.686173 SBILib-0.3.1/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    25142 2023-07-20 15:23:10.000000 SBILib-0.3.1/README.md
--rw-r--r--   0 patrick    (501) staff       (20)     6077 2023-07-19 23:01:24.000000 SBILib-0.3.1/Scenarios.md
--rw-r--r--   0 patrick    (501) staff       (20)      103 2023-07-20 16:24:58.687463 SBILib-0.3.1/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      618 2023-07-20 15:32:57.000000 SBILib-0.3.1/setup.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.459148 SBILib-0.3.1/src/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.475565 SBILib-0.3.1/src/SBILib/
--rw-r--r--   0 patrick    (501) staff       (20)    12951 2023-07-20 15:34:37.000000 SBILib-0.3.1/src/SBILib/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.488457 SBILib-0.3.1/src/SBILib/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4500 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11699 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-07-19 22:56:14.000000 SBILib-0.3.1/src/SBILib/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-07-19 22:56:22.000000 SBILib-0.3.1/src/SBILib/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14930 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2926 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-07-19 22:56:21.000000 SBILib-0.3.1/src/SBILib/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-07-19 22:56:20.000000 SBILib-0.3.1/src/SBILib/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-07-19 22:56:23.000000 SBILib-0.3.1/src/SBILib/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.495037 SBILib-0.3.1/src/SBILib/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-07-19 22:55:56.000000 SBILib-0.3.1/src/SBILib/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-07-19 22:55:49.000000 SBILib-0.3.1/src/SBILib/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-07-19 22:55:54.000000 SBILib-0.3.1/src/SBILib/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-07-19 22:55:55.000000 SBILib-0.3.1/src/SBILib/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-07-19 22:55:55.000000 SBILib-0.3.1/src/SBILib/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-07-19 22:55:57.000000 SBILib-0.3.1/src/SBILib/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-07-19 22:55:53.000000 SBILib-0.3.1/src/SBILib/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.512529 SBILib-0.3.1/src/SBILib/databases/
--rw-r--r--   0 patrick    (501) staff       (20)      273 2023-07-19 22:56:12.000000 SBILib-0.3.1/src/SBILib/databases/AlphaFoldlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-07-19 22:56:12.000000 SBILib-0.3.1/src/SBILib/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8412 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13617 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5573 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5355 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-07-19 22:56:01.000000 SBILib-0.3.1/src/SBILib/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6713 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9123 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1795 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5733 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7098 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7063 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-07-19 22:56:07.000000 SBILib-0.3.1/src/SBILib/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7149 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.515156 SBILib-0.3.1/src/SBILib/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-07-19 22:56:09.000000 SBILib-0.3.1/src/SBILib/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4777 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8169 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.517692 SBILib-0.3.1/src/SBILib/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-07-19 22:55:48.000000 SBILib-0.3.1/src/SBILib/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-07-19 22:55:43.000000 SBILib-0.3.1/src/SBILib/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-07-19 22:55:48.000000 SBILib-0.3.1/src/SBILib/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-07-19 22:55:47.000000 SBILib-0.3.1/src/SBILib/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.521323 SBILib-0.3.1/src/SBILib/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.527999 SBILib-0.3.1/src/SBILib/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-07-19 22:57:25.000000 SBILib-0.3.1/src/SBILib/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2255 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-07-19 22:57:26.000000 SBILib-0.3.1/src/SBILib/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2223 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-07-19 22:57:25.000000 SBILib-0.3.1/src/SBILib/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.530544 SBILib-0.3.1/src/SBILib/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3324 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3606 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-07-19 22:57:32.000000 SBILib-0.3.1/src/SBILib/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      338 2023-07-19 22:57:27.000000 SBILib-0.3.1/src/SBILib/external/README.md
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-07-19 22:57:28.000000 SBILib-0.3.1/src/SBILib/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.536273 SBILib-0.3.1/src/SBILib/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9107 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12570 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23488 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-07-19 22:57:19.000000 SBILib-0.3.1/src/SBILib/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8072 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/external/blast/blast_parser.py
--rw-r--r--   0 patrick    (501) staff       (20)      312 2023-07-19 22:57:34.000000 SBILib-0.3.1/src/SBILib/external/configSBI.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.537852 SBILib-0.3.1/src/SBILib/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-07-19 22:57:36.000000 SBILib-0.3.1/src/SBILib/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-07-19 22:57:35.000000 SBILib-0.3.1/src/SBILib/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.543863 SBILib-0.3.1/src/SBILib/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6331 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15045 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-07-19 22:57:13.000000 SBILib-0.3.1/src/SBILib/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-07-19 22:57:10.000000 SBILib-0.3.1/src/SBILib/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.548851 SBILib-0.3.1/src/SBILib/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-07-19 22:57:04.000000 SBILib-0.3.1/src/SBILib/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43526 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-07-19 22:57:04.000000 SBILib-0.3.1/src/SBILib/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-07-19 22:57:05.000000 SBILib-0.3.1/src/SBILib/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.558352 SBILib-0.3.1/src/SBILib/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    25560 2023-07-20 15:29:21.000000 SBILib-0.3.1/src/SBILib/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-07-19 22:54:58.000000 SBILib-0.3.1/src/SBILib/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.570494 SBILib-0.3.1/src/SBILib/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-07-19 22:55:41.000000 SBILib-0.3.1/src/SBILib/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-07-19 22:55:42.000000 SBILib-0.3.1/src/SBILib/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-07-19 22:55:35.000000 SBILib-0.3.1/src/SBILib/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3758 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-19 22:55:40.000000 SBILib-0.3.1/src/SBILib/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.585111 SBILib-0.3.1/src/SBILib/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19964 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13264 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2763 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6877 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4988 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-07-19 22:54:38.000000 SBILib-0.3.1/src/SBILib/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.595265 SBILib-0.3.1/src/SBILib/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9010 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3408 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-07-19 22:55:14.000000 SBILib-0.3.1/src/SBILib/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.606142 SBILib-0.3.1/src/SBILib/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-07-19 22:55:19.000000 SBILib-0.3.1/src/SBILib/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3806 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-07-19 22:55:19.000000 SBILib-0.3.1/src/SBILib/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3275 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-07-19 22:55:18.000000 SBILib-0.3.1/src/SBILib/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.612848 SBILib-0.3.1/src/SBILib/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-07-19 22:55:25.000000 SBILib-0.3.1/src/SBILib/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-07-19 22:55:24.000000 SBILib-0.3.1/src/SBILib/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-07-19 22:55:24.000000 SBILib-0.3.1/src/SBILib/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.622200 SBILib-0.3.1/src/SBILib/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-07-19 22:55:11.000000 SBILib-0.3.1/src/SBILib/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-07-19 22:55:10.000000 SBILib-0.3.1/src/SBILib/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11115 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-07-19 22:55:11.000000 SBILib-0.3.1/src/SBILib/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-07-19 22:55:10.000000 SBILib-0.3.1/src/SBILib/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.627406 SBILib-0.3.1/src/SBILib/structure/geometry/
--rw-r--r--   0 patrick    (501) staff       (20)    11737 2023-07-19 22:54:32.000000 SBILib-0.3.1/src/SBILib/structure/geometry/RMSD.py
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 22:54:33.000000 SBILib-0.3.1/src/SBILib/structure/geometry/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      662 2023-07-19 22:54:32.000000 SBILib-0.3.1/src/SBILib/structure/geometry/basics.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.647374 SBILib-0.3.1/src/SBILib/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2282 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3827 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2011 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14754 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1199 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      944 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7645 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8530 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2421 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18693 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14368 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8541 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.659387 SBILib-0.3.1/src/SBILib/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19068 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19200 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-07-19 22:55:29.000000 SBILib-0.3.1/src/SBILib/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-07-19 22:55:34.000000 SBILib-0.3.1/src/SBILib/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-07-19 22:55:34.000000 SBILib-0.3.1/src/SBILib/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.667846 SBILib-0.3.1/src/SBILib/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10771 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10721 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5357 2023-07-20 15:23:10.000000 SBILib-0.3.1/src/SBILib/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-07-19 22:55:02.000000 SBILib-0.3.1/src/SBILib/structure/residue/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.480033 SBILib-0.3.1/src/SBILib.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)    25403 2023-07-20 16:24:58.000000 SBILib-0.3.1/src/SBILib.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     4930 2023-07-20 16:24:58.000000 SBILib-0.3.1/src/SBILib.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-20 16:24:58.000000 SBILib-0.3.1/src/SBILib.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-07-20 16:24:58.000000 SBILib-0.3.1/src/SBILib.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        7 2023-07-20 16:24:58.000000 SBILib-0.3.1/src/SBILib.egg-info/top_level.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-20 16:24:58.684523 SBILib-0.3.1/tests/
--rw-r--r--   0 patrick    (501) staff       (20)   156217 2023-07-19 23:01:16.000000 SBILib-0.3.1/tests/Test_1a3q.cif.gz
--rw-r--r--   0 patrick    (501) staff       (20)    47362 2023-07-19 23:01:16.000000 SBILib-0.3.1/tests/Test_pdb1a2w.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:17.000000 SBILib-0.3.1/tests/Test_pdb1a3q.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)   116164 2023-07-19 23:01:18.000000 SBILib-0.3.1/tests/Test_pdb2ram.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:21.000000 SBILib-0.3.1/tests/pdb1a3q.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)     9521 2023-07-20 15:29:43.000000 SBILib-0.3.1/tests/test_modules.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.807696 SBILib-0.3.2/
+-rw-r--r--   0 patrick    (501) staff       (20)      128 2023-07-21 15:34:16.000000 SBILib-0.3.2/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)    25858 2023-07-21 16:14:42.808001 SBILib-0.3.2/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    25597 2023-07-20 16:37:41.000000 SBILib-0.3.2/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)     6077 2023-07-19 23:01:24.000000 SBILib-0.3.2/Scenarios.md
+-rw-r--r--   0 patrick    (501) staff       (20)      103 2023-07-21 16:14:42.809348 SBILib-0.3.2/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      621 2023-07-21 16:12:19.000000 SBILib-0.3.2/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.490268 SBILib-0.3.2/src/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.507323 SBILib-0.3.2/src/SBILib/
+-rw-r--r--   0 patrick    (501) staff       (20)    12951 2023-07-21 15:36:22.000000 SBILib-0.3.2/src/SBILib/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.532662 SBILib-0.3.2/src/SBILib/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4500 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11699 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-07-19 22:56:14.000000 SBILib-0.3.2/src/SBILib/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-07-19 22:56:22.000000 SBILib-0.3.2/src/SBILib/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14930 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2926 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-07-19 22:56:21.000000 SBILib-0.3.2/src/SBILib/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-07-19 22:56:20.000000 SBILib-0.3.2/src/SBILib/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-07-19 22:56:23.000000 SBILib-0.3.2/src/SBILib/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.551570 SBILib-0.3.2/src/SBILib/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-07-19 22:55:56.000000 SBILib-0.3.2/src/SBILib/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-07-19 22:55:49.000000 SBILib-0.3.2/src/SBILib/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-07-19 22:55:54.000000 SBILib-0.3.2/src/SBILib/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-07-19 22:55:55.000000 SBILib-0.3.2/src/SBILib/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-07-19 22:55:55.000000 SBILib-0.3.2/src/SBILib/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-07-19 22:55:57.000000 SBILib-0.3.2/src/SBILib/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-07-19 22:55:53.000000 SBILib-0.3.2/src/SBILib/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.586132 SBILib-0.3.2/src/SBILib/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)      273 2023-07-19 22:56:12.000000 SBILib-0.3.2/src/SBILib/databases/AlphaFoldlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-07-19 22:56:12.000000 SBILib-0.3.2/src/SBILib/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8412 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13617 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5573 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5355 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-07-19 22:56:01.000000 SBILib-0.3.2/src/SBILib/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6713 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9123 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1795 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5733 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7098 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7063 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-07-19 22:56:07.000000 SBILib-0.3.2/src/SBILib/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7149 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.592414 SBILib-0.3.2/src/SBILib/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-07-19 22:56:09.000000 SBILib-0.3.2/src/SBILib/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4777 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8169 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.602206 SBILib-0.3.2/src/SBILib/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-07-19 22:55:48.000000 SBILib-0.3.2/src/SBILib/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-07-19 22:55:43.000000 SBILib-0.3.2/src/SBILib/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-07-19 22:55:48.000000 SBILib-0.3.2/src/SBILib/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-07-19 22:55:47.000000 SBILib-0.3.2/src/SBILib/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.608223 SBILib-0.3.2/src/SBILib/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.620227 SBILib-0.3.2/src/SBILib/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-07-19 22:57:25.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2255 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-07-19 22:57:26.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2223 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-07-19 22:57:25.000000 SBILib-0.3.2/src/SBILib/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.626122 SBILib-0.3.2/src/SBILib/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3324 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3606 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-07-19 22:57:32.000000 SBILib-0.3.2/src/SBILib/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      338 2023-07-19 22:57:27.000000 SBILib-0.3.2/src/SBILib/external/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-07-19 22:57:28.000000 SBILib-0.3.2/src/SBILib/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.638485 SBILib-0.3.2/src/SBILib/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9107 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12570 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23488 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-07-19 22:57:19.000000 SBILib-0.3.2/src/SBILib/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8072 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/blast_parser.py
+-rw-r--r--   0 patrick    (501) staff       (20)      312 2023-07-19 22:57:34.000000 SBILib-0.3.2/src/SBILib/external/configSBI.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.642582 SBILib-0.3.2/src/SBILib/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-07-19 22:57:36.000000 SBILib-0.3.2/src/SBILib/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-07-19 22:57:35.000000 SBILib-0.3.2/src/SBILib/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.653894 SBILib-0.3.2/src/SBILib/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6331 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15045 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-07-19 22:57:13.000000 SBILib-0.3.2/src/SBILib/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-07-19 22:57:10.000000 SBILib-0.3.2/src/SBILib/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.663100 SBILib-0.3.2/src/SBILib/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-07-19 22:57:04.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43526 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-07-19 22:57:04.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-07-19 22:57:05.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.673499 SBILib-0.3.2/src/SBILib/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    25560 2023-07-20 15:29:21.000000 SBILib-0.3.2/src/SBILib/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-07-19 22:54:58.000000 SBILib-0.3.2/src/SBILib/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.686040 SBILib-0.3.2/src/SBILib/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-07-19 22:55:41.000000 SBILib-0.3.2/src/SBILib/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-07-19 22:55:42.000000 SBILib-0.3.2/src/SBILib/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-07-19 22:55:35.000000 SBILib-0.3.2/src/SBILib/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3758 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-19 22:55:40.000000 SBILib-0.3.2/src/SBILib/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.699052 SBILib-0.3.2/src/SBILib/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19964 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13264 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2763 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6877 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4988 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-07-19 22:54:38.000000 SBILib-0.3.2/src/SBILib/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.707094 SBILib-0.3.2/src/SBILib/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9010 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3408 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-07-19 22:55:14.000000 SBILib-0.3.2/src/SBILib/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.719137 SBILib-0.3.2/src/SBILib/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-07-19 22:55:19.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3806 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-07-19 22:55:19.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3275 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-07-19 22:55:18.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.724194 SBILib-0.3.2/src/SBILib/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-07-19 22:55:25.000000 SBILib-0.3.2/src/SBILib/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-07-19 22:55:24.000000 SBILib-0.3.2/src/SBILib/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-07-19 22:55:24.000000 SBILib-0.3.2/src/SBILib/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.734256 SBILib-0.3.2/src/SBILib/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-07-19 22:55:11.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-07-19 22:55:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11115 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-07-19 22:55:11.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-07-19 22:55:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.738805 SBILib-0.3.2/src/SBILib/structure/geometry/
+-rw-r--r--   0 patrick    (501) staff       (20)    11737 2023-07-19 22:54:32.000000 SBILib-0.3.2/src/SBILib/structure/geometry/RMSD.py
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 22:54:33.000000 SBILib-0.3.2/src/SBILib/structure/geometry/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      662 2023-07-19 22:54:32.000000 SBILib-0.3.2/src/SBILib/structure/geometry/basics.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.762081 SBILib-0.3.2/src/SBILib/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2282 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3827 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2011 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14754 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1199 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      944 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7645 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8530 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2421 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18693 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14368 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8541 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.775417 SBILib-0.3.2/src/SBILib/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19068 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19200 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-07-19 22:55:29.000000 SBILib-0.3.2/src/SBILib/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-07-19 22:55:34.000000 SBILib-0.3.2/src/SBILib/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-07-19 22:55:34.000000 SBILib-0.3.2/src/SBILib/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.784215 SBILib-0.3.2/src/SBILib/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10771 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10721 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5357 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-07-19 22:55:02.000000 SBILib-0.3.2/src/SBILib/structure/residue/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.806880 SBILib-0.3.2/src/SBILib/tests/
+-rw-r--r--   0 patrick    (501) staff       (20)      426 2023-07-20 15:27:20.000000 SBILib-0.3.2/src/SBILib/tests/Test.py
+-rw-r--r--   0 patrick    (501) staff       (20)   156217 2023-07-19 23:01:16.000000 SBILib-0.3.2/src/SBILib/tests/Test_1a3q.cif.gz
+-rw-r--r--   0 patrick    (501) staff       (20)    47362 2023-07-19 23:01:16.000000 SBILib-0.3.2/src/SBILib/tests/Test_pdb1a2w.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:17.000000 SBILib-0.3.2/src/SBILib/tests/Test_pdb1a3q.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)   116164 2023-07-19 23:01:18.000000 SBILib-0.3.2/src/SBILib/tests/Test_pdb2ram.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 23:01:17.000000 SBILib-0.3.2/src/SBILib/tests/__ini__.py
+-rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:21.000000 SBILib-0.3.2/src/SBILib/tests/pdb1a3q.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)     9923 2023-07-21 16:09:58.000000 SBILib-0.3.2/src/SBILib/tests/test_modules.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.515944 SBILib-0.3.2/src/SBILib.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)    25858 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     5049 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        7 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/top_level.txt
```

### Comparing `SBILib-0.3.1/PKG-INFO` & `SBILib-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-Metadata-Version: 2.1
-Name: SBILib
-Version: 0.3.1
-Home-page: https://github.com/structuralbioinformatics/SBI
-Author: Patrick Gohl
-Author-email: patrick.gohl@upf.edu
-License: MIT
-Keywords: Structural Bioinformatics,Loops
-Description-Content-Type: text/markdown
-
 # Welcome to the StructuralBioInformatics pylib
 
 The **SBILib** python library is a continuous work in progress that clusters functionalities to work with data derived from [PDB][1], from creating a local PDB repository to do _real_ Blast searches over PDB sequences (i.e. sequences of the really crystallized protein sections) to perform a simply split chains (separate the sections of a PDB file).
 
 
 ## Installation:
-SBILib has been distributed on PyPi and can be installed with pip:
+SBILib has been distributed on PyPi and can be installed with pip. However due to size limits we werent able to provide the BLAST database file through PyPi. This file, which will be needed for running BLAST and passing the unit tests, is available on our github repository. The full pip installation is outlined below. Alternatively you can define your own Blast database file as outlined in the BLAST section of this tutorial. 
 
-```python
+```console
 pip install SBILib
+
+
 ```
 
+
+
+
 It can also be directly cloned from our github repo:
 
 ```console
 git clone https://github.com/structuralbioinformatics/SBI
 ```
 
 Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.
 
 
 ## Testing:
 We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should
-These scripts are located in the directory "tests".
-```python
+These scripts are located in the directory "tests". REMEMBER the BLAST database file must be installed if installation occured with pip
+```console
 python Test.py
+
 #........('TEST_PDB1A3Q_A.66.pdb', 'TEST_PDB1A3Q_A.66.dssp')
 #truncated chain!TEST_PDB1A3Q_A.66.dssp
 #.('TEST_PDB2RAM_A.38.pdb', 'TEST_PDB2RAM_A.38.dssp')
 #('TEST_PDB2RAM_B.26.pdb', 'TEST_PDB2RAM_B.26.dssp')
 #('TEST_PDB1A3Q_A.30.pdb', 'TEST_PDB1A3Q_A.30.dssp')
 #truncated chain!TEST_PDB1A3Q_A.30.dssp
 #('TEST_PDB1A3Q_B.75.pdb', 'TEST_PDB1A3Q_B.75.dssp')
```

### Comparing `SBILib-0.3.1/README.md` & `SBILib-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,49 @@
+Metadata-Version: 2.1
+Name: SBILib
+Version: 0.3.2
+Home-page: https://github.com/structuralbioinformatics/SBI
+Author: Patrick Gohl
+Author-email: patrick.gohl@upf.edu
+License: MIT
+Keywords: Structural Bioinformatics,Loops
+Description-Content-Type: text/markdown
+
 # Welcome to the StructuralBioInformatics pylib
 
 The **SBILib** python library is a continuous work in progress that clusters functionalities to work with data derived from [PDB][1], from creating a local PDB repository to do _real_ Blast searches over PDB sequences (i.e. sequences of the really crystallized protein sections) to perform a simply split chains (separate the sections of a PDB file).
 
 
 ## Installation:
-SBILib has been distributed on PyPi and can be installed with pip:
+SBILib has been distributed on PyPi and can be installed with pip. However due to size limits we werent able to provide the BLAST database file through PyPi. This file, which will be needed for running BLAST and passing the unit tests, is available on our github repository. The full pip installation is outlined below. Alternatively you can define your own Blast database file as outlined in the BLAST section of this tutorial. 
 
-```python
+```console
 pip install SBILib
+
+
 ```
 
+
+
+
 It can also be directly cloned from our github repo:
 
 ```console
 git clone https://github.com/structuralbioinformatics/SBI
 ```
 
 Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.
 
 
 ## Testing:
 We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should
-These scripts are located in the directory "tests".
-```python
+These scripts are located in the directory "tests". REMEMBER the BLAST database file must be installed if installation occured with pip
+```console
 python Test.py
+
 #........('TEST_PDB1A3Q_A.66.pdb', 'TEST_PDB1A3Q_A.66.dssp')
 #truncated chain!TEST_PDB1A3Q_A.66.dssp
 #.('TEST_PDB2RAM_A.38.pdb', 'TEST_PDB2RAM_A.38.dssp')
 #('TEST_PDB2RAM_B.26.pdb', 'TEST_PDB2RAM_B.26.dssp')
 #('TEST_PDB1A3Q_A.30.pdb', 'TEST_PDB1A3Q_A.30.dssp')
 #truncated chain!TEST_PDB1A3Q_A.30.dssp
 #('TEST_PDB1A3Q_B.75.pdb', 'TEST_PDB1A3Q_B.75.dssp')
```

### Comparing `SBILib-0.3.1/Scenarios.md` & `SBILib-0.3.2/Scenarios.md`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/setup.py` & `SBILib-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 
 setup(
     name='SBILib',
-    version='0.3.1',
+    version='0.3.2',
     license='MIT',
     author="Patrick Gohl",
     author_email='patrick.gohl@upf.edu',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     include_package_data=True,
     long_description=readme,
@@ -19,7 +19,10 @@
     keywords='Structural Bioinformatics, Loops',
     install_requires=[
           'numpy','pandas','pynion','Requests','scipy','six'
       ],
 
 )
 
+
+
+
```

### Comparing `SBILib-0.3.1/src/SBILib/__init__.py` & `SBILib-0.3.2/src/SBILib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import os
 import traceback
 import datetime
 import time
 import logging
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 class Parameters(object):
     '''
     Designed to work through all the {SBI} library.
     It contains several parameters that will control (a) the amount of data
     shown to the user during the execution of {SBI} subroutines and (b) the
```

### Comparing `SBILib-0.3.1/src/SBILib/beans/Executable.py` & `SBILib-0.3.2/src/SBILib/beans/Executable.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/beans/File.py` & `SBILib-0.3.2/src/SBILib/beans/File.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/beans/IndexedNum.py` & `SBILib-0.3.2/src/SBILib/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/beans/Path.py` & `SBILib-0.3.2/src/SBILib/beans/Path.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/beans/StorableObject.py` & `SBILib-0.3.2/src/SBILib/beans/StorableObject.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/beans/butler.py` & `SBILib-0.3.2/src/SBILib/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/beans/singleton.py` & `SBILib-0.3.2/src/SBILib/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/data/Alphabet.py` & `SBILib-0.3.2/src/SBILib/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/data/AminoAcids.py` & `SBILib-0.3.2/src/SBILib/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/data/AtomVariants.py` & `SBILib-0.3.2/src/SBILib/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/data/Element.py` & `SBILib-0.3.2/src/SBILib/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/data/Properties.py` & `SBILib-0.3.2/src/SBILib/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/data/SetDict.py` & `SBILib-0.3.2/src/SBILib/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/data/__init__.py` & `SBILib-0.3.2/src/SBILib/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/CATHlink.py` & `SBILib-0.3.2/src/SBILib/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/DrugBanklink.py` & `SBILib-0.3.2/src/SBILib/databases/DrugBanklink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/Enzymelink.py` & `SBILib-0.3.2/src/SBILib/databases/Enzymelink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/GOlink.py` & `SBILib-0.3.2/src/SBILib/databases/GOlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/PDBTMlink.py` & `SBILib-0.3.2/src/SBILib/databases/PDBTMlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/PDBeChemlink.py` & `SBILib-0.3.2/src/SBILib/databases/PDBeChemlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/PDBlink.py` & `SBILib-0.3.2/src/SBILib/databases/PDBlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/SCOPlink.py` & `SBILib-0.3.2/src/SBILib/databases/SCOPlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/TaxIDlink.py` & `SBILib-0.3.2/src/SBILib/databases/TaxIDlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/Uniprotlink.py` & `SBILib-0.3.2/src/SBILib/databases/Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/__Uniprotlink.py` & `SBILib-0.3.2/src/SBILib/databases/__Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/__init__.py` & `SBILib-0.3.2/src/SBILib/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/dblink.py` & `SBILib-0.3.2/src/SBILib/databases/dblink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/uniprot/connect.py` & `SBILib-0.3.2/src/SBILib/databases/uniprot/connect.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/databases/uniprot/uniprot.py` & `SBILib-0.3.2/src/SBILib/databases/uniprot/uniprot.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/error/BlastError.py` & `SBILib-0.3.2/src/SBILib/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/error/FileError.py` & `SBILib-0.3.2/src/SBILib/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/error/SeqAliError.py` & `SBILib-0.3.2/src/SBILib/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/CDhit/CDhit.py` & `SBILib-0.3.2/src/SBILib/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/CDhit/CDhitExe.py` & `SBILib-0.3.2/src/SBILib/external/CDhit/CDhitExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/CDhit/CDhitHomolog.py` & `SBILib-0.3.2/src/SBILib/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/CDhit/CDhitList.py` & `SBILib-0.3.2/src/SBILib/external/CDhit/CDhitList.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/DSSP/DSSP.py` & `SBILib-0.3.2/src/SBILib/external/DSSP/DSSP.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/DSSP/DSSPExe.py` & `SBILib-0.3.2/src/SBILib/external/DSSP/DSSPExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/blast/BlastExe.py` & `SBILib-0.3.2/src/SBILib/external/blast/BlastExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/blast/BlastHit.py` & `SBILib-0.3.2/src/SBILib/external/blast/BlastHit.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/blast/BlastResult.py` & `SBILib-0.3.2/src/SBILib/external/blast/BlastResult.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/external/blast/blast_parser.py` & `SBILib-0.3.2/src/SBILib/external/blast/blast_parser.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/math/stats.py` & `SBILib-0.3.2/src/SBILib/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/sequence/Fasta.py` & `SBILib-0.3.2/src/SBILib/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/sequence/IndexedSeqAli.py` & `SBILib-0.3.2/src/SBILib/sequence/IndexedSeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/sequence/SeqAli.py` & `SBILib-0.3.2/src/SBILib/sequence/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/sequence/Sequence.py` & `SBILib-0.3.2/src/SBILib/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/sequence/alignment/Needleman_Wunsch.py` & `SBILib-0.3.2/src/SBILib/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/sequence/alignment/SeqAli.py` & `SBILib-0.3.2/src/SBILib/sequence/alignment/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/sequence/alignment/SimilarityMatrix.py` & `SBILib-0.3.2/src/SBILib/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/PDB.py` & `SBILib-0.3.2/src/SBILib/structure/PDB.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/atom/Atom.py` & `SBILib-0.3.2/src/SBILib/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/atom/AtomOfAminoAcid.py` & `SBILib-0.3.2/src/SBILib/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/atom/AtomOfNucleotide.py` & `SBILib-0.3.2/src/SBILib/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/atom/AtomSeries.py` & `SBILib-0.3.2/src/SBILib/structure/atom/AtomSeries.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/chain/Chain.py` & `SBILib-0.3.2/src/SBILib/structure/chain/Chain.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/chain/ChainFrame.py` & `SBILib-0.3.2/src/SBILib/structure/chain/ChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/chain/ChainOfNucleotide.py` & `SBILib-0.3.2/src/SBILib/structure/chain/ChainOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/chain/ChainOfProtein.py` & `SBILib-0.3.2/src/SBILib/structure/chain/ChainOfProtein.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/chain/ProteinChainFrame.py` & `SBILib-0.3.2/src/SBILib/structure/chain/ProteinChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/Complex.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/Complex.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/InnerContacts.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/InnerContacts.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/contact/Contact.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/contact/ContactAA.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAA.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/contact/ContactAH.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/contact/ContactAN.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAN.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/inner/PHInnerContact.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/inner/PPInnerContact.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/interface/Interface.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/interface/PHInterface.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/interface/PNInterface.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/interface/PNInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/contacts/interface/PPInterface.py` & `SBILib-0.3.2/src/SBILib/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/geometry/RMSD.py` & `SBILib-0.3.2/src/SBILib/structure/geometry/RMSD.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/geometry/basics.py` & `SBILib-0.3.2/src/SBILib/structure/geometry/basics.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/BioMolecule.py` & `SBILib-0.3.2/src/SBILib/structure/header/BioMolecule.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/DBreference.py` & `SBILib-0.3.2/src/SBILib/structure/header/DBreference.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/Experiment.py` & `SBILib-0.3.2/src/SBILib/structure/header/Experiment.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/Header.py` & `SBILib-0.3.2/src/SBILib/structure/header/Header.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/HeteroAtom.py` & `SBILib-0.3.2/src/SBILib/structure/header/HeteroAtom.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/MiniRes.py` & `SBILib-0.3.2/src/SBILib/structure/header/MiniRes.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/Molecule.py` & `SBILib-0.3.2/src/SBILib/structure/header/Molecule.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/SecondaryStructure.py` & `SBILib-0.3.2/src/SBILib/structure/header/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/Site.py` & `SBILib-0.3.2/src/SBILib/structure/header/Site.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/header/__init__.py` & `SBILib-0.3.2/src/SBILib/structure/header/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/parse_mmCIF.py` & `SBILib-0.3.2/src/SBILib/structure/parse_mmCIF.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/parse_pdb.py` & `SBILib-0.3.2/src/SBILib/structure/parse_pdb.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/protein/Arch.py` & `SBILib-0.3.2/src/SBILib/structure/protein/Arch.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/protein/SShelper.py` & `SBILib-0.3.2/src/SBILib/structure/protein/SShelper.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/protein/SecondaryStructure.py` & `SBILib-0.3.2/src/SBILib/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/protein/Sequencer.py` & `SBILib-0.3.2/src/SBILib/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/residue/Residue.py` & `SBILib-0.3.2/src/SBILib/structure/residue/Residue.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/residue/ResidueOfAminoAcid.py` & `SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib/structure/residue/ResidueOfNucleotide.py` & `SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/src/SBILib.egg-info/PKG-INFO` & `SBILib-0.3.2/src/SBILib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: SBILib
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
 
 # Welcome to the StructuralBioInformatics pylib
 
 The **SBILib** python library is a continuous work in progress that clusters functionalities to work with data derived from [PDB][1], from creating a local PDB repository to do _real_ Blast searches over PDB sequences (i.e. sequences of the really crystallized protein sections) to perform a simply split chains (separate the sections of a PDB file).
 
 
 ## Installation:
-SBILib has been distributed on PyPi and can be installed with pip:
+SBILib has been distributed on PyPi and can be installed with pip. However due to size limits we werent able to provide the BLAST database file through PyPi. This file, which will be needed for running BLAST and passing the unit tests, is available on our github repository. The full pip installation is outlined below. Alternatively you can define your own Blast database file as outlined in the BLAST section of this tutorial. 
 
-```python
+```console
 pip install SBILib
+
+
 ```
 
+
+
+
 It can also be directly cloned from our github repo:
 
 ```console
 git clone https://github.com/structuralbioinformatics/SBI
 ```
 
 Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.
 
 
 ## Testing:
 We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should
-These scripts are located in the directory "tests".
-```python
+These scripts are located in the directory "tests". REMEMBER the BLAST database file must be installed if installation occured with pip
+```console
 python Test.py
+
 #........('TEST_PDB1A3Q_A.66.pdb', 'TEST_PDB1A3Q_A.66.dssp')
 #truncated chain!TEST_PDB1A3Q_A.66.dssp
 #.('TEST_PDB2RAM_A.38.pdb', 'TEST_PDB2RAM_A.38.dssp')
 #('TEST_PDB2RAM_B.26.pdb', 'TEST_PDB2RAM_B.26.dssp')
 #('TEST_PDB1A3Q_A.30.pdb', 'TEST_PDB1A3Q_A.30.dssp')
 #truncated chain!TEST_PDB1A3Q_A.30.dssp
 #('TEST_PDB1A3Q_B.75.pdb', 'TEST_PDB1A3Q_B.75.dssp')
```

### Comparing `SBILib-0.3.1/src/SBILib.egg-info/SOURCES.txt` & `SBILib-0.3.2/src/SBILib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -123,13 +123,15 @@
 src/SBILib/structure/protein/SecondaryStructure.py
 src/SBILib/structure/protein/Sequencer.py
 src/SBILib/structure/protein/__init__.py
 src/SBILib/structure/residue/Residue.py
 src/SBILib/structure/residue/ResidueOfAminoAcid.py
 src/SBILib/structure/residue/ResidueOfNucleotide.py
 src/SBILib/structure/residue/__init__.py
-tests/Test_1a3q.cif.gz
-tests/Test_pdb1a2w.ent.gz
-tests/Test_pdb1a3q.ent.gz
-tests/Test_pdb2ram.ent.gz
-tests/pdb1a3q.ent.gz
-tests/test_modules.py
+src/SBILib/tests/Test.py
+src/SBILib/tests/Test_1a3q.cif.gz
+src/SBILib/tests/Test_pdb1a2w.ent.gz
+src/SBILib/tests/Test_pdb1a3q.ent.gz
+src/SBILib/tests/Test_pdb2ram.ent.gz
+src/SBILib/tests/__ini__.py
+src/SBILib/tests/pdb1a3q.ent.gz
+src/SBILib/tests/test_modules.py
```

### Comparing `SBILib-0.3.1/tests/Test_1a3q.cif.gz` & `SBILib-0.3.2/src/SBILib/tests/Test_1a3q.cif.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/tests/Test_pdb1a2w.ent.gz` & `SBILib-0.3.2/src/SBILib/tests/Test_pdb1a2w.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/tests/Test_pdb1a3q.ent.gz` & `SBILib-0.3.2/src/SBILib/tests/Test_pdb1a3q.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/tests/Test_pdb2ram.ent.gz` & `SBILib-0.3.2/src/SBILib/tests/Test_pdb2ram.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/tests/pdb1a3q.ent.gz` & `SBILib-0.3.2/src/SBILib/tests/pdb1a3q.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.1/tests/test_modules.py` & `SBILib-0.3.2/src/SBILib/tests/test_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import unittest
+import unittest, subprocess, gzip, os, shutil
 
 from SBILib.structure import PDB, Complex 
 from SBILib.databases import PDBlink
 from SBILib.external.blast import BlastExe
 
 
 
@@ -60,22 +60,28 @@
 
 class Test_Blast(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.blastresults = None
 
     def setUp(self):
+        url = "ftp://ftp.ebi.ac.uk/pub/databases/uniprot/knowledgebase/uniprot_sprot.fasta.gz"
+        output = subprocess.run(["wget", url], capture_output=True, text=True)
+        with gzip.open('uniprot_sprot.fasta.gz', 'rb') as f:
+            with open('uniprot_sprot.fasta','wb') as f_out:
+                shutil.copyfileobj(f,f_out)
+        os.remove("uniprot_sprot.fasta.gz")
         self.protein = PDB("Test_pdb1a3q.ent.gz")
         self.chainA = self.protein.get_chain_by_id("A")
 
     def test_Compile_Blast(self):
         querySequence = self.chainA.protein_sequence
         queryID = self.chainA.globalID
         try:
-            blast = BlastExe(database = "../BlastDB/uniprot_sprot.fasta")
+            blast = BlastExe(database = "uniprot_sprot.fasta")
         except Exception as e:
             self.fail("BlastExe() raised ExceptionType unexpectedly!")
         try:
             self.__class__.blastresults = blast.execute_query_seq(sequenceID = queryID, sequence = querySequence)
         except Exception as e:
             self.fail("blast.execute_query_seq() raised ExceptionType unexpectedly!")
         first = self.__class__.blastresults.get_hits()[0]
```

