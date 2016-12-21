Example Code and Figures for "baker": Bayesian Analysis Kit for Etiology Research
------
> An R Package for Fitting Bayesian [Nested Partially Latent Class Models](https://academic.oup.com/biostatistics/article/2555349/Nested-partially-latent-class-models-for-dependent) 

Details
-------------------------------------


* Modify in the `simulated_example_nplcm.R` the directory path 

> `working_dir <- "~/Downloads/run_baker_example"` 

to somewhere local to you. Posterior results will be stored here. The `simulated_example_nplcm.R` will automatically create
the folder.

* `simulated_example_nplcm.R`: a simple `R` file to generate simulated data, fit the nested-partially latent class models, check the models, visualize the posterior results. Please refer to the file content for more details about the requirements to run this example code.

Then you can run the following code for replicating the results:

```{r}
source_github <- function(u) {
  # load package
  require(RCurl)
  
  # read script lines from website
  script <- getURL(u, ssl.verifypeer = FALSE)
  
  # parase lines and evealuate in the global environement
  eval(parse(text = script))
}

devtools::install_github("zhenkewu/baker")

sessionInfo()
source("https://raw.githubusercontent.com/zhenkewu/baker_example/master/simulated_example_nplcm.R")
```

* `scn_3_mixiter_1/rep_1_kfit_2`: a folder generated automatically by the example code above. It contains the automatically generated `.bug` model file, model specifications, data information, MCMC sampling settings along with the posterior samples obtained from the Gibbs sampling (done by JAGS). Some automatically generated visuals are also included; please refer to the end of `simulated_example_nplcm.R` for the code that generated the figures.

* `pathogen_category_simulation.csv`: a simple data with two columns; **It is automatically downloaded into your working folder for bacterial/viral group etiology visualization**. The first column contains pathogen names, the second column specifies the corresponding pathogen types. It is used for plotting the posterior distribution of viral versus bacterial etiologies.

* `visualization figures.pdf`: colects figures obtained from this simulation (see the figures in `scn_3_mixiter_1/rep_1_kfit_2`). Figures not shown here include individual prediction figures, standardized log odds ratio difference (SLORD) figures. 


Maintainer:
--------------------------

Zhenke Wu (zhenkewu@umich.edu)

Department of Biostatistics

University of Michigan