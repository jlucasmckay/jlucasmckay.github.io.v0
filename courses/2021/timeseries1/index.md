---
title: Syllabus
---

# Timeseries 1

## Summary
This course presents a comprehensive treatment of timeseries data suitable for first- and second-year graduate students in Bioinformatics and Data Sciences.
The course is arranged as 12 weeks of lectures (2h/week) with weekly homework and closes with a machine learning competition focused on identification and annotation of freezing of gait episodes in kinematic data of patients with Parkinson's disease.

## Prerequisites
Previous coursework in linear algebra and statistics / probability theory.
Fluency with programming in Python, Matlab, or similar.

## Text
There is no dedicated text. Some material is adapted from "Signal Processing and Linear Systems" by [Lathi](handouts/Lathi.pdf).

## Course Objectives
This course will introduce students to fundamental theory of timeseries analysis through lectures, homework, and a second-quarter project.
Following this course students should be able to: 
1. Understand fundamental duality between time- and frequency- domain representation of biosignals
1. Understand fundamentals of sampling and the potential impact of aliasing on biological data 
1. Prepare timeseries datasets for analyses that appropriately consider repeated measurements of individual patients at different nominal times
1. Apply common linear and nonlinear signal conditioning approaches to noisy data
1. Calculate common estimates of time-varying signal energy
1. Design and train a simple autoregressive classifier that can predict changes in time-varying signal energy
1. Characterize the prediction horizon of the classifier

## Grading
1. Homework (50%) will help students develop analytical and programming skills.
1. An end-of-semester project (50%) will provide students with practical experience in identifying health-related events in patient data. Students will use the PDFOG kinematic dataset to predict the onset of freezing of gait episodes identified from video recordings by an expert rater. This will be possible to do only techniques presented in the course, but students may identify and implement approaches from the literature.

## Outline

### Introduction: different representations of Time in informatics data
1. Timescales - 1 kHz to annual
    1. ECG
    1. Annual
1. Explicit vs. implicit representations of time
1. Time to event: censored data and survival analysis
1. Forecasting: data only from the past
1. Course focus: signals in which time is represented implicitly and sampled regularly, "high frequency" in statistics nomenclature

### Equivalence of time domain and frequency domain representations of signals
1. Cauchy-Schwartz inequality
1. Estimating energy
1. Transformation matrices
    1. DFT basis matrix
    1. DWT basis matrix
1. Operations in other domains
	1. De-trend
	1. Wavelet filtering

### Sampling, aliasing, and signal quality of high-frequency data
1. Sampling artifacts
1. Antialias filtering
1. Sources and types of noise
    1. Additive vs. signal-dependent noise in biological timeseries
1. Rolling averages and nonlinear operations

### Example timeseries signal statistics
1. Time domain characteristics
    1. Mean and standard deviation of heart rate
    1. Mean tremor frequency
    1. TK 
1. Frequency-domain characteristics
    1. Low-frequency/high-frequency (LF/HF) ratio of heart rate variability (ratio of power between 0.015–0.15 Hz and 0.15–0.4 Hz in the RR tachogram)
    1. "Freeze band power" in kinematic marker data

### Autoregressive models

Equivalence of Frequency domain representation of a grandma cell


Matched filters: 







Digital signal processing
1. Deconvolution with matched filters
1. Filters matched to input timeseries


Homeworks
1. Matched filters: converting "phono" signals to "line-level" signals (RIAA playback equalization)

Sampling and aliasing
1. Antialias filtering
1. Explicit, rather than implicit, representations of Time

Digital signal processing
1. Deconvolution with matched filters
1. Filters matched to input timeseries




Explicit Time
Data management
1. Wide and tall Data
1. Implicit and explicit timeseries


Additional topics
1. Additive vs. signal-dependent noise
1. Rolling averages and prediction
1. Differen

Projects
1. Detecting tremulous freezing episodes
1. Detecting arrhythmias

1. Data shapes
1. The `fog` dataset
1. The `emg` dataset
1. Frequency domain description of filters: high pass, low pass, band pass
    1. Converting "phono" signals to "line-level" signals (RIAA playback equalization)
1. Time domain description of filters: "matched filters"
    1. A single deep learning kernel
1. Nonlinear operators
1. Comparing timeseries
    1. Control chart
    1. Across groups
1. Threshold-based approaches to identify abnormalities



CS534 Machine Learning Spring 2019 
Instructor: Lee Cooper, Assistant Professor of Biomedical Engineering & Biomedical Informatics Office: Suite 4103 Woodruff Memorial Research Building Phone: (404)712-0110 
Communication & Course Materials: 
Lectures: MW 1-2:15 PM, MCS Room W303 
Text: The Elements of Statistical Learning. Friedman, Tibshirani and Hastie. Springer, Second Edition. 
Prerequisites: Previous coursework in linear algebra and statistics or probability theory. Fluency with programming in Python or Matlab. *See Homework below. 
Course Objectives: 
This course will introduce students to fundamental theory and algorithms in machine learning through lectures, homework, and a semester-long project. Following this course students should be able to: 
1. Prepare datasets for machine-learning experiments 2. Formulate rigorous validation protocols, and evaluate the rigor of validation protocols 3. Understand the bias and variance tradeoff and various strategies to mitigate overfitting 4. Understand fundamental machine-learning algorithms presented in the text 
Grading: 
Project (50%) The semester-long project is designed to provide you with practical experience in algorithm implementation and validation experiments. Projects will be presented at the end of the semester and documented in a short report. Students will work in small teams, and each student’s final project grade will be weighted using reviews from their teammates. 
Homework (50%) will help students develop analytical and programming skills. Solutions will be explained at the beginning of class on the due date and late submissions will not be accepted. A homework assignment given on the first day will test prerequisite material and graded pass/fail. A passing grade on this homework is required to pass this course. 
Academic Integrity: 
Emory University maintains an honor code that defines academic misconduct: Emory Honor Code. 
Any suspected violations of the Emory Honor Code will be referred to the honor council for a hearing. This inlcudes but is not limited to plagiarism on homeworks or class projects. Homework assignments should be completed independently and should reflect only your original work and understanding of the assignment. Code should not be copied from other students or open source libraries. 
Introduction & Supervised Learning I Theme Topics Dates Reading Introduction Review syllabus, overview of course 
topics 1/14 Random Variables & Probability 
Random variables, probability theory, conditional and joint distributions, Bayes rule 
1/14, 1/16 Handouts 
Decision Theory Machine learning as statistics 1/23 Chapters 1, 2 
Linear Regression Regression, ridge regression, LASSO 
regression, elastic net regression 1/28, 1/30 Chapter 3 Linear Classification logistic regression, LDA, QDA 2/4, 2/6 Chapter 4 
Theory & Validation Procedures Training & test error, conditional and Theory 
expected test error, bias-variance decomposition, optimism 
2/11, 2/12 Chapter 7 
Validation Validation as an estimation problem, 
validation protocols 2/18, 2/20 Chapter 7 Error Measures Error measures, class imbalance, ROC 
analysis, precision-recall 2/18 Handouts Model Selection Effective number of parameters, Akaike 
and Bayes information criterion 2/20 Chapter 7 
Supervised Learning II Practical Issues Preparing data, labeling issues, 
interpretation 3/4 Chapters 9,10 Boosting and Trees Decision trees, boosting, ADABoost, 
gradient boosting 3/6 Chapters 9,10 Neural Networks Perceptron, gradient optimization, back 
propagation 3/18, 3/20 Chapter 11 Support Vector 
Machines SVM, kernel SVM 3/25, 3/27 Chapter 12 Prototype Methods KNN 4/1 Chapter 13 
Random Forests Ensemble methods, random forests 4/3 Chapters 15, 16 Challenges with 
Curse of dimensionality, sparse High-Dimensional Data 
representation 4/8 Chapter 18 
Unsupervised Learning Dimensionality Reduction 
Principal component analysis, locally-linear embedding, manifold learning 
4/10 Chapter 14 
Clustering & Mixture Modeling 
K-means, spectral clustering, 
expectation maximization 4/15, 4/17 Chapter 14 
Project Presentations 4/22, 4/29 
4/24, 
