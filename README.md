Example Code and Figures for "baker": Bayesian Analysis Kit for Etiology Research
------
> An R Package for Fitting Bayesian [Nested Partially Latent Class Models](http://biostats.bepress.com/jhubiostat/paper276/) 

Details
-------------------------------------

* `simulated_example_nplcm.R`: a simple `R` file to generate simulated data, fit the nested-partially latent class models, check the models, visualize the posterior results. Please refer to the head of the file for more details about requirements to run this example code.
* `scn_3_mixiter_1/rep_1_kfit_2`: a folder generated automatically by the example code above. It contains the automatically generated `.bug` file, model specifications, data information along with the posterior samples obtained from Gibbs sampling (done by JAGS).
* `pathogen_category_simulation.csv`: a simple data with two columns: the first column has pathogen names, the second column has pathogen types. It is for plotting the posterior for viral versus bacterial etiologies.
* `visualization figures.pdf`: a collection of figures obtained from this simulation. There are figures such as individual prediction figures, standardized log odds ratio difference (SLORD) figures not shown here.


Maintainer:
--------------------------

Zhenke Wu (zhwu@jhu.edu)

Department of Biostatistics

Johns Hopkins Bloomberg School of Public Health
