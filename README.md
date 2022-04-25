# regression-bias
This code is meant to accompany Sivadas et al., 2022: Regression Bias in Solar Wind Measurements. Under Review. 


# Demonstration of Regression Bias in Solar Wind Measurements
Random uncertianty in the conditional variable, can lead to a bias in thee conditional expectation. We demonstrate this using a Gedankenexperiment[^1] in Code 1, and provide evidence for this by comparing WIND and ACE data in Code 2. 

## Contents
**Code_1_Demonstrating_regression_bias.mlx**: contains code that carries out a thought experiment by generating artificial data, introduces uncertainty in it, and then explores the bias caused by this uncertainty in the regression function. 
The [corresponding .html](https://github.com/nithinsivadas/regression-bias/blob/main/Code_1_Demonstrating_regression_bias.html) can be used to view the code and the results for those who do not have access to MATLAB 2021. 

**Code_2_Regression_bias_in_solar_wind_measurements.mlx**: contains the code that compares simultaneous, solar wind parameters propagated to the magnetospheric bow shock, measured by ACE and WIND. We carry out non-linear regression of one parameter over the other, and vice versa, and show that the origin of bias has to  be regression dilution bias.  
The [corresponding .html]{https://github.com/nithinsivadas/regression-bias/blob/main/Code_2_Regression_bias_in_solar_wind_measurements.html} can be used to view the code and the results for those who do not have access to MATLAB 2021. 

**Data.zip** contains the following data files: 

  The WIND, ACE and GEOTAIL spacecraft measurements of the solar wind parameters propagated to the bow shock: https://spdf.gsfc.nasa.gov/pub/data/omni/high_res_omni/sc_specific/.

## Instructions
Both codes require MATLAB 2021 to run. 

To run Code2 successfully please do the followign: 
  1. Unzip Data.zip within the local repository itself. 
  2. In Code_2_Regression_bias_in_solar_wind_measurements.mlx provide the correct path of the Data folder inside the variable "DataDir".

Code1 can be executed without any external input or data. 

## Acknowledgements

Code:
1) F. Carr (2022). Orthogonal Linear Regression (https://www.mathworks.com/matlabcentral/fileexchange/16800-orthogonal-linear-regression), MATLAB Central File Exchange. Retrieved April 19, 2022.

2) Circular Statistics Toolbox (Directional Statistics) [Link] P. Berens, CircStat: A Matlab Toolbox for Circular Statistics, Journal of Statistical Software, Volume 31, Issue 10, 2009 http://www.jstatsoft.org/v31/i10
Data:

3) We thank GSFC/SPDF OMNIWeb service for the WIND spacecraft measurements. The WIND spacecraft measurements of the solar wind propagated to the bow shock can be accessed from https://spdf.gsfc.nasa.gov/pub/data/omni/high_res_omni/sc_specific/. 

[^1]: https://en.wikipedia.org/wiki/Thought_experiment
