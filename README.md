# Project 1 Credit Card Analysis

This project explores reason to why customers may churn factors such as inactivity, card usage and time with bank. the aim of this analysis is see if which are more likely going to influence a customer to churn. using visualisations I can see if certain categories influence customers to leave. I will be to document my findings and summarise reasons.


# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Dataset Content

* The dataset I used was the BankChurners and it was a synthetic dataset from Kaggle. 
Here is the link for the dataset: https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers

## Business Requirements

* To understand reasons as to why customers churn and identify any solutions required to retain customers. To find out at what point a customer is likely to churn.

## Hypothesis and how to validate?

* List here your project hypothesis(es) and how you envision validating it (them) 
- Customers who have been with the bank longer have a higher credit limit
- Customers with more bank products are less like to churn 
- Customers with more inactive months are more likely to churn
- Customers with high inactivity and high transaction amounts are more likely to churn than other customer groups.
- Customers with higher credit utilisation rattios are less likely to churn

I will use data visualisations such as scatterplots, boxplots, linegraphs, histograms and bar charts across different variables to see if there is a corelation. (Eg. seeing if there is a corelation between how many products a customer holds and if they they churned)
## Project Plan

Data collection and set up: The synthetic dataset was downloaded from Kaggle and then saved in the Raw data folder.
Initial data exploration and cleaning: Once had imported the data I explored it by checking the contents of the data such as columns, value counts, statistical data of selected columns. After this had been done I ran to see if there were any missing rows or values, then I checked for duplicates. Any necessary cleaning was done for visualisation.
Data Visualisation: Scatterplots, boxplots, linegraphs, histograms and bar charts across different variables to create appriate graphs and help test the hypotheses.

## The rationale to map the business requirements to the Data Visualisations

- Do customers who have been with the bank longer have a higher credit limit?
 An interactive Plotly scatter plot compared ⁠ Months_on_book ⁠ against ⁠ Credit_Limit ⁠, alongside a correlation check between the two. Plotly was chosen here specifically because the relationship involves a large number of individual data points, and an interactive chart made it possible to inspect specific customers rather than relying on a static, dense scatter alone. A supporting line chart of average credit limit by tenure was added to make any underlying trend easier to read through the noise of individual points.
- Are customers with more bank products less likely to churn?
A Matplotlib bar chart compared the average number of products held by existing versus attrited customers, giving a direct headline comparison. A boxplot was added to show the full distribution behind that average, rather than the average alone.
- Are customers with more inactive months more likely to churn?
A Seaborn bar plot compared average months inactive between existing and attrited customers, and a boxplot showed the distribution of inactivity within each group, including its spread and outliers.
- Are customers with high inactivity and high transaction amounts more likely to churn than other groups?
Customers were split into four behavioural groups by combining a median split on transaction amount (⁠ Spend_Group ⁠) with a median split on inactivity (⁠ Inactive_Group ⁠). An interactive Plotly bar chart compared churn rate across these four groups directly, and a boxplot showed the transaction amount distribution within each group, to check whether the groups were meaningfully distinct before drawing conclusions from the churn-rate comparison.
## Analysis techniques used

Analysis techniques used I used visual exploratory analysis as my main method, testing each of my hypotheses with one Matplotlib, one Seaborn, and one Plotly chart. The specific chart types I used were boxplots (to compare distributions between churned and retained customers), scatter plots (to explore the relationship between two continuous variables), a histogram (to check the shape of an engineered feature), bar charts (to compare a summary statistic across groups)
I structured my analysis hypothesis by hypothesis, giving each one its own section with all three required chart types together, followed by a short written finding under each chart and an overall conclusion for that hypothesis. I chose this structure over grouping all the Matplotlib charts together, then all the Seaborn charts, and so on, because I wanted each hypothesis to be read and understood as a complete, self-contained argument, rather than making the reader piece together evidence for the same hypothesis from three different places in the notebook. I also had to reconsider Hypothesis 3 once I saw the actual result: the data showed the opposite pattern to what I had predicted, so rather than treating this as a failure, I reported the result honestly and reasoned through a possible explanation for why it might have happened.


## Ethical considerations (optional)

The dataset I used in this project was from Kaggle and was a synthetic dataset so it did not contain real personal data, However if this was a real dataset I would've autotomised the data before beginning exploration.
 
## Use of AI
- I used Chat GPT 5.5 to suggest appropriate graphs for visualisation 
- I used Chat GPT 5.5 to help put code comments within my code.

## Development Roadmap
- I want get more comfortable using feature engineering 
- Be able to incorporate AI effectively

## Main Data Analysis Libraries
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Plotly

## Credits

https://plotly.com/python/ -Plotly documentation

https://seaborn.pydata.org/ - Seaborn documentation

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)

* Thank the people who supported this project.