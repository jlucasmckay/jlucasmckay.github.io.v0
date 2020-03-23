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
There is no dedicated text. Some material is adapted from texts by [Lathi](references/Lathi.pdf) and [Shumway](references/Shumway.pdf) 

## Course Objectives
This course will introduce students to theoretical and applied aspects of timeseries analysis through lectures, homework, and a second-quarter project.
Following this course students should be able to: 
1. Understand fundamental duality between time- and frequency- domain representation of signals
1. Understand fundamentals of sampling and aliasing
1. Prepare timeseries datasets for analyses that appropriately consider repeated measurements of individual patients at different nominal times
1. Apply common linear and nonlinear signal conditioning approaches to noisy data
1. Calculate common estimates of time-varying signal energy
1. Design and train a simple autoregressive classifier that can predict changes in time-varying signal energy
1. Characterize the prediction horizon of the classifier

## Grading
1. Homework (50%) will help students develop analytical and programming skills.
1. An end-of-semester project (50%) will provide students with practical experience in identifying health-related events in patient data. Students will use the PDFOG kinematic dataset to predict the onset of freezing of gait episodes identified from video recordings by an expert rater. This will be possible to do only techniques presented in the course, but students may identify and implement approaches from the literature.

## Outline
    
1. Introduction to timeseries data
    1. Representations of time in informatics data
        1. Timescales - 1 kHz to 1 sample/year
        1. Explicit vs. implicit representations of time
        1. Time to event: censored data and survival analysis
        1. Forecasting: data only from the past
        1. Course focus: signals in which time is represented implicitly and sampled regularly, "high frequency" in statistics nomenclature
    1. Simple operations on regularly-sampled timeseries data (examples from [Shumway](references/Shumway.pdf))
        1. Using regression to discover a signal embedded in noise
        1. Moving average smoothing
1. Equivalence of time domain and frequency domain representations of signals 
    1. Signal representation by Fourier series
    1. Aperiodic signal representation by the Fourier Transform
    1. Sampling and aliasing
        1. The sampling theorem
        1. The Discrete Fourier Transform (DFT)
    1. Projection matrix representations
        1. DFT basis matrix
        1. DWT basis matrix    
    1. Frequency domain description of ideal and real filters
    1. Impacts of windowing
1. Measures of signal size, energy, and power
    1. Kurtosis etc.
1. Projects
    1. Detecting tremulous freezing episodes
    1. Detecting arrhythmias

### Timeseries regression and ARIMA


### Sampling, aliasing, and signal quality of high-frequency data
1. Sampling artifacts
1. Antialias filtering
1. Sources and types of noise
    1. Additive vs. signal-dependent noise in biological timeseries
1. Rolling averages and nonlinear operations

### Autoregressive / ARIMA approaches
1. Comparison of ARIMA and random forest time series models for prediction of avian influenza H5N1 outbreaks [Kane](references/Kane.pdf)
1. 

### Example timeseries signal statistics
1. Time domain characteristics
    1. Mean and standard deviation of heart rate
    1. Mean tremor frequency
    1. TK 
1. Frequency-domain characteristics
    1. Low-frequency/high-frequency (LF/HF) ratio of heart rate variability ([McSharry](references/McSharry.pdf))
    1. "Freeze band power" in kinematic/kinetic data ([Moore](references/Moore.pdf))

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

