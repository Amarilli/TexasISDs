# Project 1

## Education Funding Analysis

### Team Members: 

- James Draper
- Kelsey Kraft
- Mariah McLelan
- Amarilli Novel
- Hisako Yamanaka

  
### Research Question to Answer:

How does the funding allocated to education impact the success of students and schools?

### Project Description:

The project aims to analyze the impact of education funding on the success of students and schools. 

Specifically, the study will focus on the relationship between state funding in Texas education, SAT/ACT scores, and dropout rates. 

Through statistical and visual analysis, we will determine whether higher funding leads to better outcomes or if there is a point where the impact of funding levels off.


### Data Sets Source:

https://tea.texas.gov/

> https://tea.texas.gov/reports-and-data/school-data/campus-and-district-type-data-search

> https://tea.texas.gov/reports-and-data/school-performance/accountability-research/c[…]-graduation-and-dropout/completion-graduation-and-dropout-data

> https://tea.texas.gov/reports-and-data/school-performance/accountability-research/ap/ib-and-sat/act

> https://tea.texas.gov/finance-and-grants/state-funding/state-funding-reports-and-data

> https://tea.texas.gov/finance-and-grants/state-funding/state-funding-reports-and-data/peims-financial-standard-reports

### Break Down of Task:

    Mariah: Visualization, Statistical Analysis, Cleaning Final Code.
    James: Finding datasets, visualization.
    Kelsey: Visualization.
    Amarilli: Cleaning and merging datasets, README, presentation. 
    Hisako: Visualization. 

### Development

We began our study by searching for suitable datasets, focusing on the Texas Education system and referring to the TEA Texas Education Agency website.

We found six relevant Excel files, which we converted to .csv files. 

Our first challenge was determining which columns to choose. 

For finance, we focused solely on total operating revenue, which Texas uses to support educational operations and facility construction in public school districts. 
This revenue comes from local, state, and federal funding sources, with the majority coming from state and local sources and only a relatively small amount from the federal government.  

State government aid is the primary funding source for elementary and secondary education, followed by local contributions (primarily property taxes). On average, 8% of revenues come from the federal government, 47% from the state, and 45% from local sources[^bignote2].
[^bignote2]:  McFarland, J., Hussar, B., Wang, X., Zhang, J., Wang, K., Rathbun, A., … Bullock Mann, F. (2018). The condition of education 2018. National Center for Education Statistics.

We selected "All Students" as the group for SAT and ACT scores, as other groups had inconsistent data. 

Then, we merged the SAT and ACT scores with the cleaned finance data frame and formatted and sorted the values. 

We then proceeded to conduct a **statistical analysis** of the data.

### Statistical Analysis:

#### Texas Total Operating Revenue Results:

*Mean* Total Operating Revenue: 85,389,382

*Median* Total Operating Revenue: 22,696,266

*Standard Deviation*: 190,478,406

*Standard Error of the Mean*: 7,049,922

*Shapiro-Wilk Normality Test*:

Test Statistic: 0.4248087406158447

P-value: 4.7223758247746335e-43

The data does not follow a normal distribution (reject the null hypothesis).

The lower quartile of the total operating revenue is: 11395018.75

The upper quartile of the total operating revenue is: 68576095.75

The interquartile range of the total operating revenue is: 57181077.0

The median of the total operating revenue is: 22696266.0 

Values below -74376596.75 could be outliers.

Values above 154347711.25 could be outliers.


#### Texas Student Count Distribution Results:

*Mean* Student Count: 6,908

*Median* Student Count: 1,687

*Standard Deviation*: 15,534

*Standard Error of the Mean*: 575

*Shapiro-Wilk Normality Test*:

Test Statistic: 0.4364619851112366

P-value: 9.388699710976274e-43

The data does not follow a normal distribution (reject the null hypothesis).

The lower quartile of the Student Count  is: 755.0

The upper quartile of the Student Count is: 5286.5

The interquartile range of the Student Count is: 4531.5

The median of the Student Count is: 1687.0 

Values below -6042.25 could be outliers.

Values above 12083.75 could be outliers.

At this point, we started the **visual analysis**:

### Visualization:

1. Total Operating Revenue vs Student Count

The scatter plot shows a positive correlation between TOR and student count.

2. Spending Ranges (per student) vs. average total SAT  score
The line plot suggests that the budget doesn't significantly affect scores, as some schools with smaller budgets scored the highest. Moreover, smaller schools tend to have higher SAT scores. And we know from the budget vs student count that the smaller the budget, the fewer students.

3. School Size vs. Average Total SAT score
The data presented in the line graph indicates a substantial decline in academic scores when the school population increases.

4. Spending Ranges (Per student) vs. average ACT Compos
As for the SAT scores, the line plot analysis suggests that the budget doesn't significantly affect scores, as some schools with smaller budgets scored the highest. Moreover, smaller schools tend to have higher ACT scores.
These findings indicate that other factors besides budget allocation may influence academic performance, and further research is needed to identify these factors.

5. School Size vs. average ACT composite
The line plot confirms what we found for SAT scores: there is a significant decline in academic scores when the school population increases.

6. "Largest Cities (by Pop.) ACT Composite" and Largest Cities (by Pop.) SAT Total
We focused on five most significant in size city in Texas  and analyzed San Antonio ISD, Austin ISD, Fort Worth ISD, Dallas ISD, and Houston ISD creating a box plot that compares the total operating revenue for every ISD and the SAT and ACT Composite scores

7. SAT Total and ACT Composite scatterplots
These two scatter plots display total operating revenue vs. act and sat scores. 
We calculate the correlation.
The correlation between Total Operating Revenue and ACT Composite scores is -0.03
The correlation between Total Operating Revenue and SAT Total scores is -0.09

8. SAT Total and ACT Composite histograms
Displays total operating revenue vs act and sat scores. 

9. Big City SAT vs ACT
Using hvplot, this scatter plot displays where big cities stand for a score in a single graph

10. Treemap
11. Dropout rates


### Conclusions:


    


