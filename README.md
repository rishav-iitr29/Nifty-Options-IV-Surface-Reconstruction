# Implied-Volatility-Surface-Reconstruction

**Objective:** Impute missing Implied Volatility (IV) values across the NIFTY 50 options chain without lookahead bias.  

## Project Summary

The core insight was that mathematics beats machine learning for this problem. The IV surface is a smooth, analytically-defined manifold — trying to approximate it with tree-based step functions introduces unnecessary variance. The best approach uses a Regime-Switching Pure Quant Interpolator: a Natural Cubic Spline for normal days, and Linear Interpolation on Expiry Day.

## Directory Structure
1. IV_Surface_Solution.ipynb contains all code and explanation for EDA and the approaches used to compute missing IV values
2. ```reproducible code/``` contains all code files to reproduce each submission that was submitted by me in the Kaggle competition - Run the file and the csv will be generated. It also contains the dataset given.


By Rishav Kumar
