---
title: Syllabus
---

# Timeseries 1

## Summary
This course presents a comprehensive treatment of timeseries data suitable for first- and second-year graduate students in Clinical Bioinformatics and Data Sciences.
The course is arranged as 12 weeks of lectures (2h/week) with 8 weekly homework problem sets.
Two mid-semester projects will help students develop practical programming skills necessary for accessing and analyzing publicly-available data.
The course closes with a machine learning competition focused on identification and annotation of freezing of gait episodes in kinematic data of patients with Parkinson's disease.

## Prerequisites
Previous coursework in linear algebra and statistics / probability theory.
Fluency with programming in an interpreted language such as R, Matlab, or Python.

## Text
There is no dedicated text. Some material is adapted from texts by [Shumway](reference/Shumway.pdf), [Hamilton](reference/Hamilton.pdf), and [Lathi](reference/Lathi.pdf).

## Course Objectives
This course will introduce students to theoretical and applied aspects of timeseries analysis through lectures, homework, and a final project.
Following this course students should be able to: 
1. Understand time-domain representations of signals, including difference equations and AR models.
1. Understand fundamentals of sampling and aliasing.
1. Understand common sources of noise in biosignals.
1. Apply common linear and nonlinear signal conditioning approaches to noisy biosignal data.
1. Calculate common estimates of time-varying spectral energy and other summary statistics.
1. Design and train a simple classifier that can identify events in biosignal data.

## Grading
1. Homework (50%) will consist of math problems and will help students develop analytical and programming skills.
1. An end-of-semester project (25%) will provide students with practical experience in identifying health-related events in patient data. 

## Outline

![](images/noisyCosine.png)

1. __Introduction to timeseries data__
    1. Representations of time in informatics data
        1. Timescales - 1 kHz to 1 sample/year
        1. Explicit vs. implicit representations of time
        1. Time to event: censored data and survival analysis
        1. Causal and non-causal data
        1. Course focus: signals in which time is represented implicitly and sampled regularly
    1. Simple operations for discovering a signal embedded in additive noise
        1. Regression onto a hypothesized basis
        1. Moving average smoothing
        1. Frequency-domain filtering
        1. Autoregressive estimation
1. __Spectral analysis and filtering__
    1. Equivalence of frequency and time domain representations of signals
    1. Signal representation by Fourier series
    1. Aperiodic signal representation by the Fourier Transform
    1. Sampling and aliasing
        1. The sampling theorem
        1. The discrete Fourier transform (DFT)
    1. Decimation and upsampling
    1. Linear filters
    1. Impacts of windowing on frequency content
    1. Measures of signal size, energy, and power in the spectral domain
    1. Optional topics: invertible projection matrix representations
        1. DFT projection
        1. DWT projection
        1. SVD/Karhunen–Loève/PCA projection
    1. __Mid-semester project 1:__ calculation of low-frequency/high-frequency (LF/HF) ratio of heart rate variability ([McSharry](reference/McSharry.pdf)) in a publicly-available dataset. Mid-semester project 1 will be scored based on performance vs. Dr. McKay's implementation.
1. __Time series regression and autoregressive / ARIMA models__
    1. Autoregressive moving average models
    1. Difference equations
    1. Autocorrelation and partial autocorrelation
    1. Forecasting and backcasting
    1. Building ARIMA models
    1. Estimating covariance structures in longitudinal studies (e.g., [Lu](reference/Lu.pdf))
    1. __Mid-semester project 2:__ ARIMA approach for health event prediction (e.g., [avian influenza H5N1 outbreaks](reference/Kane.pdf)) in a publicly-available dataset. Mid-semester project 1 will be scored based on performance vs. Dr. McKay's implementation.
1. __Final project:__ detection of tremulous freezing episodes in unpublished kinematic data of PD patients annotated by clinical collaborators.
    1. Two lectures will cover clinical and practical aspects of Parkinson's disease.
    1. In year 1 of the class, the final project will be scored based on reconstruction of expert labels (start and stop of FOG episodes) provided by a clinical collaborator. One approach is that provided by [Moore](reference/Moore.pdf). In later years, the final project will build upon the work of previous cohorts and will identify kinematic features associated with medication state during testing (OFF and ON medication for most participants) and aspects of disease phenotype.
    
## Outline - Biomedical Signal Processing
1. Patient monitoring and data acquisition
1. Biomedical signals – ECG, SAO₂, BP, EEG, Resp, Speech …
1. Time series analysis, autocorrelation, correlation
1. Sampling, interpolation, windowing, decimation and anti-aliasing
1. Frequency analysis
1. AR spectral analysis, cepstral analysis & speech 
1. Filtering (IIR/FIR)
1. Event detection (beats, arrhythmias)
1. Feature extraction (respiration, HRV)
1. Labs (every afternoon) – ECG & PPG analysis
1. Applications (final day) – presentations on 3 research topics

### Autoregressive Models
1. A time-series tool, to predict future values from past events
    * AR modelling utilizes the time history of a signal to predict future values of the signal.
1. Can be used to derive a frequency spectrum too
    * Similar to the Fourier transform, the AR model requires that the signal be wide sense stationary (loosely, having the same variance and mean over all time) for real applications, though there is no mathematical constraint.
    * Quite nicely, as well as predicting future values, the AR model can also be used to derive a frequency spectrum, and can therefore be used as an alternative to the FFT (fast fourier transform) in the calculation of frequency spectra.
1. Data must be stationary
    * There is, of course, the question, why we would use AR rather than FFTs – but that is something we will get on to later.




