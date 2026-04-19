Before running the code in any RMD files, open the R Project file ('Using models to identify the causes of 
pre-symptomatic transmission from human infection data.Rproj') at the root of the directory to correctly set the 
working directory.

# Literature review of CHI trials

'CHI trial lit review.Rmd' contains the plotting code for Figure 1, which illustrates the data collected for 
our literature review of controlled human infection trials.

# Identifying correlates of pre-symptomatic transmission

'Fitting statistical model to human infection data.Rmd' contains the code for the analysis of 
the data from Ge *et al*., 2023 and Zhou *et al*., 2023. This includes fitting the statistical model we use
to individual viral shedding data, calculating the duration and amplitude of pre-symptomatic transmission for
each person, running linear regressions assessing e.g. the correlation between viral population growth rate 
and the duration of pre-symptomatic transmission across all the participants, and bootstrapping 
the predicted values of the linear regressions to assess statistical uncertainty. 

Data was cleaned separately and loaded in directly at the beginning of the code. For the norovirus data, 
this involved simple reformatting of the data from the noroData.rds file found in the supplementary material of 
Ge *et al*., 2023, as well as averaging viral shedding values for time points where multiple samples are 
reported to be taken. For the SARS-CoV-2 data, this involved visually data mining the shedding and 
symptom onset data from Figure 2 in Zhou *et al*., 2023 using the metaDigitise package.

# Mechanistic within-host model

'Mechanistic model.Rmd' contains the code for the simulations and analyses of the within-host model we 
employ to produce a plausible scenario of pre-symptomatic transmission informed by earlier findings vis-a-vis 
data from the Ge *et al*., 2023 and Zhou *et al*., 2023 studies. 
