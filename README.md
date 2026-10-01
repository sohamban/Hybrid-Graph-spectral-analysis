Basis Idea of the Programming

The programming implements an fMRI-based framework for ADHD classification using brain functional connectivity. The main idea is to develop a data-driven pipeline that captures individual variations in brain organization and extracts discriminative connectivity patterns.

The program consists of three major stages:

Adaptive ROI Extraction
Grouped Independent Component Analysis (ICA) and Dictionary Learning are used to identify meaningful and subject-adaptive brain regions from fMRI data.
Hybrid Graph Spectral Analysis
Functional connectivity is constructed from the extracted ROIs. Conventional graph Fourier representation and Riemannian/geodesic-based graph spectral representation are combined to obtain a hybrid spatio-spectral representation of brain connectivity.
CLSTM-Based ADHD Classification
The extracted spatio-spectral features are provided to a hybrid Convolutional Long Short-Term Memory (CLSTM) model. Convolutional layers learn spatial patterns, while LSTM layers capture sequential dependencies among the connectivity features. The learned representation is then used to classify ADHD and non-ADHD subjects.

The overall programming workflow is:

fMRI Data → Adaptive ROI Extraction → Functional Connectivity → Hybrid Graph Spectral Representation → Spatio-Spectral Features → CLSTM → ADHD Classification

The implementation is intended to provide a reproducible computational framework for investigating brain functional connectivity patterns associated with ADHD.
