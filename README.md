# Analysing publication bias within an Ocean acidification report

## Background
This project involves assessing publication biases that exist among many studies that explores the relationship of Ocean acidification and Fish behaviour. It takes the data by Clement et al. (2022), including the results from Clark et al. (2020) to assess any presence of publication biases through multi-level meta-analysis. Some packages used includes: orchaRd and metafor to create appropriate diagrams and models typically seen in multi-level meta-analysis. 

The data itself analyses any changes in behaviour from six types of coral fishes in the presence of elevated CO2 levels, leading to ocean acidification. Each study tends to follow their own methodology, refer to Clement et al. (2022) for more information. 

## Why this project is useful
This analysis brings light on how common publication bias is, and how easily it can be overlooked. It not only spreads misinformation, but can mislead further research in the same field. By exploring the presences of biases, we also acknowledge other possible methodologies that may help alleviate these issues. 

## Project methodology
The analysis started with summarising and binding of the datasets, such that both datasets have the same column names to reduce confounding. Using the escalc() function, it produces an appropriate effect size (lnRR) magnitude and variance. This revealed presence of outliers, in which 10 were removed from subsequent analysis. Next, many multi-level meta-analysis models were created to assess presence of publication biases (time-lag and file-drawer bias) through funnel plots and time-lag plots, then quantified its effects using the r2_ml() function from the metafor package. 

