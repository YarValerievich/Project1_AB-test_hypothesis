# Prioritization of hypotheses and A/B-test analysis for an online store. 

I recommend checking out the project at [the following link](https://nbviewer.org/github/YarValerievich/Project1_AB-test_hypothesis/blob/main/Project1_AB-test_hypothesis.ipynb).

## Purpose: 

Using the data of the online store, prioritize the hypotheses and evaluate the results of A/B-testing using various methods.

## Description: 

The hypotheses were prioritized using ICE and RICE frameworks. An analysis of the A/B-test results was conducted, and graphs of cumulative revenue, average check, and conversion rates were plotted by group. The statistical significance of differences in conversions and average check between raw and cleansed data was calculated.

## Result:

### Prioritization of hypotheses: 
We calculated the values for ICE and RICE frameworks. After finding differences in priorities, we explained them based on different user reach. We chose RICE as the main criterion. Hypothesis 7 received priority: Add a subscription form to all main pages to collect a customer database for email newsletters.

### A/B-test analysis: 
#### Studying cumulative metrics:
We examined cumulative metrics by preparing cumulative data for graphing. We studied cumulative revenue and average check graphs for both groups. We found that there were outliers in the data because of the "jumps" in the graphs. The metrics for the groups were practically indistinguishable. We studied the cumulative conversion graph, and Group B stabilized above Group A. This was also evident in the relative conversion ratio graph. At this stage, we noticed differences in conversion and suspected that revenue and average check did not differ significantly between the groups.

#### Outlier analysis: 
As we discovered "jumps" in the graphs in the previous step, we analyzed outliers for our metrics. For average check, we looked for outliers in order cost, and for conversion, we looked for outliers in the number of orders per user during the test period. We chose the 95th percentile as the clipping boundary.

#### Calculation of statistical significance for raw data: 
We checked the significance of differences in conversion and average check. We found statistically significant differences in conversions. There was a 13.8% increase in Group B. There were no statistically significant differences in average check, but an increase of 25.9% was detected in Group B. We suspected outliers caused this.

#### Calculation of statistical significance for clean data: 
We obtained more precise results on conversion after sieving. There was a statistically significant increase by 14.8% in Group B. The average check test showed the same result - no differences. However, after outlier removal, we saw a real picture of a relative change of -1.7%.
The results were obtained at a 95% significance level (we used alpha=0.05). 

### Decision based on the test results: 
We made the decision to stop the test and record Group B's victory since, in the alternative hypothesis, there were no changes in the average check, but the conversion increased by 15%.

## Stack of technologies: 

- python
	- pandas
	- pyplot
	- numpy
	- scipy
- A/B-testing
- statistical hypotheses testing
