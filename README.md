# Elastic-Net-for-PLSR-DA
A short function for running elastic net using the 'lasso' function in MATLAB. This function is designed for use with the PLSDA/R pipeline available at https://github.com/Dolatshahi-Lab/PLSR-DA.

This function can be used prior to the PLSDA pipeline to perform feature selection in a robust and repeatable manner. The function parameters allow tuning of MATLAB's lasso function behavior, including adjustment of alpha and the number of cross-validation replicated. The wrapper function then repeats lasso feature selection a specified number of times and retains the features that were selected repeatedly, based on the threshold set by the stability parameter.

The output of this function is a list of the features that meet the selection criteria and can be used to downsample the feature matrix for future analyses.
