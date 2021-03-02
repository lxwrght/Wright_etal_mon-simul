# A comparison of monitoring designs to assess wildlife community parameters across spatial scales

### Alexander D. Wright, Evan H. Campbell Grant, and Elise F. Zipkin

### In Review

### Code/Data DOI: 

### Please contact the first author for questions about the code or data: Alexander D. Wright (adwright@msu.edu)

________________________________________________________________________________________________________________________________________

## Abstract:
Dedicated long-term monitoring at appropriate spatial and temporal scales is necessary to understand biodiversity losses and develop effective conservation plans. Wildlife monitoring is often achieved by obtaining data at a combination of spatial scales, ranging from local to broad, to understand the status, trends, and drivers of individual species or whole communities and their dynamics. However, limited resources for monitoring necessitates tradeoffs in the scope and scale of data collection. Careful consideration of the spatial and temporal allocation of finite sampling effort is crucial for monitoring programs that span multiple spatial scales. Here we evaluate the ability of five monitoring designs - stratified random, weighted effort, indicator unit, rotating panel, and split panel - to recover parameter values that describe the status (occupancy), trends (change in occupancy), and drivers (a site-specific covariate and an autologistic term) of wildlife communities at two spatial scales. Using an amphibian monitoring program that spans a network of U.S. National Parks as a motivating example, we conducted a simulation study for a regional community occupancy sampling program to compare the monitoring designs across varying levels of sampling effort (ranging from 10 to 50%). We found that the stratified random design outperformed the other designs for most parameters of interest at both scales, and was thus generally preferable in balancing the estimation of status, trends, and drivers across scales. However, we found that other designs had improved performance in specific situations. For example, (e.g., the rotating panel design performed best at estimating spatial drivers at a regional level). Thus, our results highlight the nuanced scenarios in which various design strategies may be preferred, and offer guidance as to how managers can balance common tradeoffs in large-scale and long-term monitoring programs in terms of the specific knowledge gained. Monitoring designs that reduce biases in parameter estimates are needed to guide conservation policy and management decisions in the face of broad scaled environmental challenges, but the optimal design is sensitive to the specific objectives of a monitoring program.

## Simulation Code
1. Code used to simulate and analyze datasets for each monitoring design on the High Performance Computing Cluster at Michigan State University:
   - [Data-simulation_SR.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Stratified random design
   - [Data-simulation_WE.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Weighted Effort design
   - [Data-simulation_IU.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Indicator Unit design
   - [Data-simulation_RP.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Rotating Panel design
   - [Data-simulation_SP.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Split Panel design
3.JAGS model that is fit with simulated data in the step above:
   - [jags_SR.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Stratified random design
   - [jags_WE.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Weighted Effort design
   - [jags_IU.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Indicator Unit design
   - [jags_RP.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Rotating Panel design
   - [jags_SP.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_data.R): Split Panel design
5. [Data-simulation_Results-Plots.R](https://github.com/lxwrght/Wright_etal_InReview_LandEcol/blob/master/MRCM_Results-Plots.R): Post simulation script that makes published tables, results, and figures.
