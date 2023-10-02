# Likelihood ratio based forensic text comparison system

Two types of likelihood ratio (LR)-based forensic text comparison systems are available. One is based on a deep learning (DL) approach and the other is on a machine learning (ML) approach. This repository contains the source code used in the paper presented at the 16th Biennial Conference of the International Association for Forensic & Legal Linguistics. The title of the paper is "Estimating Likelihood Ratios for Authorship Evidence with a Deep-learning-based Text Representation".

# Installation

The DL system was written in Python and the ML system was built using R.

The following libraries are required for the DL system:

  * transformers==4.4
  * torch==1.7
  * pandas
  * sklearn
  * torchinfo

Python 3.7 was used
  * conda create -n IbnA pip python=3.7
  * conda activate IbnA

The following libraries are required for the ML system:

 * library(fitdistrplus)
 * library(stylo)
 * library(actuar)
 * library(StatMatch)
 * library(MASS)
 * library(ROCR)
 * library(stats)
 * library(ROC)
 * library(MGLM)
 * library(usedist)
 * library(dirichlet)
 * library(Compositional)
 * library(MGLM)

# Dataset

This repository works with Amazon Database. The downloaded database which consists of 5 iterations x 5 batches (25 files) should be stored in 'amazon database' directory for the DL system. The feature values extracted from the database should be placed in 'amazon_database_feature_extracted' directory for the ML system.

# Directory structure (DL)

 * DL system

# Directory structure (ML)

The zipped file 'ml.zipped' consists of the following three directories:
 * amazon_database_feature_extracted
 * ml_experiment_outcome
 * src
 ** xxx  


