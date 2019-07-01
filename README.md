# Analysis of A/B Test Results for an e-commerce website

This project analyzes the results of an A/B test run by an e-commerce website
to help decide whether to implement a new page, keep the old page,
or perhaps run the experiment longer.

The analysis uses the methods:
* probability
* A/B testing
* regression models


## Dataset
Two datasets are analyzed:
1. ab_data.csv has 294,478 records with 5 column:
- user_id
- timestamp
- group (control or treatment)
- landing_page (old_page or new_page)
- converted (1,0, with 1 meaning converted)

2. countries.csv has 290,584 records with 2 variables
- used_id
- country

The datasets were provided by Udacity as part of the Analyze A/B Test Results project

## Imports
import pandas as pd<br>
import numpy as np<br>
import random<br>
import matplotlib.pyplot as plt<br>
import statsmodels.api as sm<br>


## Conclusions

Based on the available data and consistent across the methods used in this
analysis: probability, A/B testing and regression models, there is insufficient
evidence to support that the new page is better than the old page in impacting
conversions.

Furthermore in the initial analysis, it was found that the old page had a
slightly higher conversion rate than the new page.

Additional analysis was conducted to determine whether a user's country had any
relationship with conversion, but this metric was not found to be statistically
significant.

As this experiment was run for just under a month in January, it may be
beneficial to run the experiment longer in order to account for seasonal effects
on change in behaviour due to this being the start of the year. Additionally
a longer duration for the experiment might also determine whether a novelty
effect or change aversion was at play.

This project was competed as part of the Udacity Data Analyst Nanodegree
