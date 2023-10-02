# Likelihood ratio based forensic text comparison system

Two types of likelihood ratio (LR)-based forensic text comparison systems are available. One is based on a deep learning (DL) approach and the other is on a machine learning (ML) approach. This repository contains the source code used in the paper presented at the 16th Biennial Conference of the International Association for Forensic & Legal Linguistics. The title of the paper is "Estimating Likelihood Ratios for Authorship Evidence with a Deep-learning-based Text Representation".

# Installation

The DL system was written in Python and the ML system was built using R.

The following libraries are required for the DL system:

  transformers==4.4
  torch==1.7
  pandas
  sklearn
  torchinfo

Python 3.7 was used
conda create -n IbnA pip python=3.7
conda activate IbnA

