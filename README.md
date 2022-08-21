# Business-Self-Sanctioning-of-Russia
### Class Project for Bayesian Machine Learning
### Authors: Elina Ribakova, Diana Morris, Carol Moore
### Data was compiled by the Kyiv School of Economics (KSE) Leave Russia project and provided to the authors.  
### See https://leave-russia.org/ to learn more about Leave Russia.
### This analysis reflects the work and opinions of the authors only and is independent from KSE and the Leave Russia Project. 
### Abstract

Following Russia’s full-scale invasion of Ukraine on February 24, 2022 many governments imposed severe financial and trade sanctions on Russia, including its access to global payments systems and the U.S. dollar, sovereign debt trading, commodity exports, and access to critical technology.  There is also an emerging phenomenon of “self-sanctioning”: multinational companies exiting the Russian market, whether partial or fully, temporarily, or permanently, despite not being explicitly directed to do so by sanctions. In this analysis, we estimate a Bayesian multinomial logistic regression model to identify the factors associated with a companies' decisions to curtail business with Russia, and to what extent. 

The database covers 2,479 companies from 55 industries and headquartered in 75 countries. The response variable is a company’s operational status with Russia as of July 31, 2022.  "Leave": explicit action to close branches in Russia or stop orders to Russia; "Stay": take no action; "Wait": hold off planned investment or scale back operations.  Features included in the regression were industry (aggregated to 7 to 9 categories), presence of official sanctions by the company's home country, global revenues, and percentage of revenues from Russia.  Due to missing values, the model with %revenue from Russia included 484 observations and the version of the model without this variable had 1,157 observations.

Markov Chain Monte Carlo estimates of the posterior slope and intercept distributions with priors ~N(0,1) and N=1,157 found that companies in the healthcare/pharma industry had lower log odds of leaving than the reference industry, consumer cyclicals (94% HDI -2.8 to -.46).  Official sanctions imposed by the home country was correlated with increased log odds of leaving (.091 to 2.33 94% HDI) and reduced log odds of staying (-2.68 to -.50), while the association with waiting not consistently postive or negative (-.68 to 1.55).   

