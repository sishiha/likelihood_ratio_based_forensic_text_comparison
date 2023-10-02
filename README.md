# Likelihood ratio based forensic text comparison systems

Two types of likelihood ratio (LR)-based forensic text comparison systems are available in this repository. One is based on a deep learning (DL) approach and the other is on a machine learning (ML) approach. This repository contains the source codes used in the study presented at the 16th Biennial Conference of the International Association for Forensic & Legal Linguistics. The title of the paper is [Estimating Likelihood Ratios for Authorship Evidence with a Deep-learning-based Text Representation](https://www.dropbox.com/scl/fi/bbg49qyudnze4g5yaqa2z/iafll16_ml_dl_and_ftc.pptx?rlkey=f9yibkev6d1ncazpd35lwnj4o&dl=0). In this study, these two systems are compared at first, and then the results are fused.

The pipeline for calculating LRs is given below:



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

The zipped file 'dl.zip' contains the following directories:
* amazon_database
* evaluation
* execute
* src
* trained_models

You can train the DL system as shown below:

    training.csh

The above shell script, which is stored in 'execute' directory, runs 'model_roberta_self_attention_modified.py' stored in 'src' directory. The trained model should appear in 'trained_models' directory.

You can carry a series of experiments by excecuting the following shell script which can be found in 'excecute' directory.

    evaluation.csh

All experimental results should appear in 'evaluation' directory.

# Directory structure (ML)

The zipped file 'ml.zip' consists of the following three directories:
 * amazon_database_feature_extracted
 * ml_experiment_outcome
 * src

You can run a series of experiments using the following code which is stored in 'src' directory. The lines 11-15 are for setting experimental conditions.

    batch_experiment.R

All experimental results are stored in 'ml_experiment_outcome' directory.
