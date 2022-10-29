# 3207_Assignment2

## What the project does
This assignment involves assessing publication biases that exist among many studies that explores the relationship of Ocean acidification and Fish behaviour. It takes the data used by Clement et al. (2022), add on the results from Clark et al, (2020) to assess the biases through multi-level meta-analysis. This involved many packages such as orchaRd and metafor to complete diagrams and creation of models. 

The data itself analyses how 6 species of coral fishes react in the presence of elevated CO2 levels, leading to ocean acidification. Each study tends to follow their own methodology, refer to Clement et al. (2022) for more information. 

## Why the project is useful
This analysis brings light onto how common publication bias is, and how easily it is overlooked. It not only spreads misinformation, but it also delays the rate in which we find the truth. By exploring the presences of biases, we also acknowledge possible methodologies to alleviate these issues. 

## Methodology
The analysis started with summarising and binding of the datasets, such that both datasets have the same column names to reduce confounding. Using the escalc() function, it produces the chosen effect size (lnRR) magnitude and variance. This revealed presence of outliers, in which 10 were removed for subsequent analysis. Next, many multi-level meta-analysis models were created to assess presence of publication biases (time-lag and file-drawer bias) through funnel plots and time-lag plots, then quantified its effects using the r2_ml() function from the metafor package. 

