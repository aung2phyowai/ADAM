
[![ADAM](http://www.fahrenfort.com/images/ADAM_logo.png)](https://github.com/fahrenfort/ADAM)

# What is it?
ADAM is an open source Matlab Toolbox. It allows you to perform multivariate analyses on your EEG and/or MEG data using backward decoding (BDM) and forward encoding models (FEM).

# Features (incomplete list)
- Perform multivariate classification analyses (backward decoding) using an arbitrary number of conditions
- Compute forward encoding models, including Channel Tuning Functions (CTFs), either across time or averaged over time
- Use the same data for training and testing through a k-fold leave-one-out procedure
- Use different datasets for testing and training
- Gives the option to either do time-frequency (TFR) decomposition first (using Fieldtrip) performing the analysis on a range of frequency bands, or just work with the raw EEG
- The decoding can either be performed on induced TFR power or total TFR power
- Do trial binning if required
- Compute Generalization Across Time (GAT) matrices (King et al, TiCS 2014) or time by frequency matrices, both for classification and for CTFs (forward modeling, e.g. see Foster et al 2016 or Samaha et al. 2016)
- Compute GAT matrices for raw EEG or for any frequency (if using TFR data)
- Average over training windows, average over testing windows, average over frequency windows
- Compute, plot and do statistics on spatial topomaps for any time point based on the Haufe method (NeuroImage, 2014)
- Compute, plot and do statistics on spatial top-maps of weights obtained from the forward model
- Statistical testing, including cluster based permutation testing and FDR on the resulting GAT matrices or on the 2D vectors, either per condition or between conditions
- Visualization of the results (2D graphs, 3D color scale maps, topoplots etc)
- The computation-intensive part of the toolbox has been optimized for use on UNIX computing clusters, to enable fast computation of large datasets (many subjects in parallel), but can also be ran locally on any computer with reasonable specs

# Why should I use this toolbox?
One of the big advantages of this toolbox is that it takes generic input formats for which many import functions are available (EEGLAB or FieldTrip), allowing researchers to do their own pre-processing any which way they like. The toolbox takes care of the intricacies of multivariate analyses (data handling), allowing a wealth of possibilities as specified above, and always has a group analysis as its endpoint. Although everything is scripted, the scripts are easy to use, doable also for novices.

# Requirements
- A recent version of Matlab (>2012b, lower versions might or might not work)
- A recent version of [EEGLAB](https://sccn.ucsd.edu/eeglab/downloadtoolbox.php) (>13, lower versions might or might not work)
- A recent install of [FieldTrip](http://www.fieldtriptoolbox.org/download) (>2015, lower versions might or might not work)
- A reasonably modern computer (>=8GB memory, enough HD space, modern processor, more is better)
