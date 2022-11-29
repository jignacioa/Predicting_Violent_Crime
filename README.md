Introduction

The objective of this study was to build a linear regression model that could effectively predict violent
crimes per population: total number of violent crimes per 100,000. The data set provided was Communities
& Crime Unnormalized from the UCI Machine Learning Repository. This data set includes US data from
the 1990 Census, 1990 Law Enforcement Management and Admin Stats survey, and crime data from the
1995 FBI UCR.

The following is a list of the initial predictors selected for the linear regression model:
• PolicBudgPerPop: police operating budget per population
• RacialMatchCommPol: a measure of the racial match between the community and the police force.
High values indicate proportions in community and police force are similar
• medIncome: median household income
• PctFam2Par: percentage of families (with kids) that are headed by two parents

Initial predictor selection was based on current discussions in the US in regards to crime and its relationship
to law enforcement budget, relationship between law enforcement and the communities policed, and income.
Exploratory data analysis was performed to get an insight into a possible correlation between each predictor
and violent crime. A linear regression model was fit to the data and model selection was performed using
two different techniques. One utilized the p-value of each predictor as an exclusion criterion while the second
method performed stepwise selection of the optimal model using the AIC value.

Mathematical assumptions of the model were checked through various diagnostic plots and the data was
checked for outliers and influential observations using two different mathemical values calculated from the
data, standardized residuals and Cook’s Distance. After further tuning and refining the model, confidence
and prediction intervals were calculated using the final model
