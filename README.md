Example Code and Figures for "baker": Bayesian Analysis Kit for Etiology Research
------
> An R Package for Fitting Bayesian [Nested Partially Latent Class Models](http://biostats.bepress.com/jhubiostat/paper276/) 

Details
-------------------------------------

* `simulated_example_nplcm.R`: a simple `R` file to generate simulated data, fit the nested-partially latent class models, check the models, visualize the posterior results. Please refer to the file content for more details about the requirements to run this example code.
* `scn_3_mixiter_1/rep_1_kfit_2`: a folder generated automatically by the example code above. It contains the automatically generated `.bug` model file, model specifications, data information, MCMC sampling settings along with the posterior samples obtained from the Gibbs sampling (done by JAGS).
* `pathogen_category_simulation.csv`: a simple data with two columns. The first column contains pathogen names, the second column specifies the corresponding pathogen types. It is used for plotting the posterior distribution of viral versus bacterial etiologies.
* `visualization figures.pdf`: a collection of figures obtained from this simulation. Figures not shown here include individual prediction figures, standardized log odds ratio difference (SLORD) figures.


Maintainer:
--------------------------

Zhenke Wu (zhwu@jhu.edu)

Department of Biostatistics

Johns Hopkins Bloomberg School of Public Health
