# Business-Self-Sanctioning-of-Russia
### Class Project for Bayesian Machine Learning
### Authors: Elina Ribakova, Diana Morris, Carol Moore
### Data was compiled by the Kiev School of Economics (KSE) Leave Russia project and provided to the authors.  https://leave-russia.org/
### This analysis reflects the work and opinions of the authors only and is independent from KSE and the Leave Russia Project. 
### Abstract

Following Russia’s full-scale invasion of Ukraine on February 24, many countries have imposed severe financial and trade sanctions on Russia, including its access to global payments systems and the U.S. dollar, sovereign debt trading, commodity exports, and access to critical technology.  There is also an emerging phenomenon of “self-sanctioning”: multinational companies exiting the Russian market, whether partial or fully, temporarily, or permanently, despite not being explicitly forced to do so by sanctions. In this analysis, we estimate a Bayesian multinomial logistic regression model to identify the factors associated with a companies' decisions to curtail business with Russia, and to what extent. 

The database as of July 31, 2022 covers 2,479 companies across 75 countries and 55 industries. The response variable is a company’s operational status in Russia:  "Leave": explicit action to close branches in Russia or stop orders to Russia; "Stay": take no action; business as usual; "Wait": hold off planned investment ('buy time') or scale back operations.  Features included in the regression were industry (aggregated to 7 to 9 categories), presence of official sanctions by the country of the company's headquarters, global revenues, and percentage of revenues from Russia.  Due to missing values, the model with %revenue from Russian included 484 observations and the version of the model without this variable had 1,157 observations.

Markov Chain Monte Carlo estimates of the slope and intercept parameters with priors ~N(0,1) and N=1,157 found that companies in the healthcare/pharma industry had lower log odds leaving compared to the reference industry, consumer cyclicals (94% HDI for posterior probability of leaving -2.8 to -.46).  The presence of official sanctions in the home country was correlated with increased log odds of leaving and reduced log odds of staying, while waiting was about the same with and without official sanctions.   

