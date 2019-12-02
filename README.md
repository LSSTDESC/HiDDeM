# HiDDeM: HIgh-Dimensional DEsc Metrics (HiDDeM)

This repository is home to the HiDDeM project, which aims to develop and characterize metrics for the comparison of multi-dimensional distributions in a variety of LSST-DESC contexts. 

## Motivation

One common use case for the application of such metrics is validation testing for simulated catalogs, which often requires a quantitative comparison of the distributions of simulated and real data in two or more dimensions. 
There are a number of metrics that are appropriate for univariate distributions (reviewed thoroughly in [the PZ DC1 paper](https://github.com/LSSTDESC/PZDC1paper)), such as the Kolmogorv-Smirnov (KS) statistic, but options for higher dimensional spaces are limited, and no one metric will be suited to every science goal.
In the example of comparing simulated and real data, the Kullback–Leibler (KL) divergence's requirement of a notion of one distribution being closer to "the truth" than another makes it appropriate to the problem, but its sensitivity to the tails of the distributions may not match what we actually care about. 

## Scope

This project will explore new metrics that can be used to compare and characterize the nature of the differences between higher-dimensional distributions.  
Concrete examples for the use of each metric will be provided by examining their performance in [DESCQA](https://github.com/LSSTDESC/descqa) validation tests. 

Other use cases besides catalog validation are envisaged for this work. 
One example would be the comparison of the results of cosmological inference for two different probes in the full multi-dimensional cosmological parameter space.  
