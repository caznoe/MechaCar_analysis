# MechaCar Analysis
Project for mock company to analyze design test data. Used RStudio to design a linear model to predict the MPG and a statistical evaluation and T-Test of the suspension coil's pound-per-inch based on the provided datasets. Propose a final study to further evaluate the car design options. Project for UC Berkeley Data Analytics Boot Camp.

### Data Analysis
#### MPG Regression
The results of the multiple linear regression analysis on the MechaCar data shows that the vehicle length (Pr=2.60e-12) and the ground clearance (Pr=5.21e-08) both provide a non-random amount of variance to the mpg measure. Since the intercept (Pr=5.08e-08) is also non-random, there are other variables from the car which were not a part of the analysis that are influencing the mpg.

With the amount of variables, it is dificult to plot a multiple linear regressin model. The slope of our multiple linear regression model is not considered to be zero, and the null hypothesis is rejected since the p-value is much smaller than our assumed significance level of .05% and our r-squared value is high at .7. Our coeficient table shows the slope coefficient for each independent variable to the dependent variable, mpg.

Our r squared value is high at .7 and p-value (5.35e-11) is less than the significance level so the multiple linear regression is sufficient for predicting mpg of MechaCar prototypes on the given data. However, the lack of significant variables suggests that the data is overfitting and future mpg data may not be predicted accurately. 

#### Suspension Coil Summary
The manufacturing data show a mean of 1500 PSI, median of 1500 PSI, standard deviation of 8.73 and a variance of 76.2. Based on the current manufacturing data, the suspension coils meet the design specifications of no more than 100 pounds -per -inch variance. The statistics show that the data has a variance of 76.2, which is a variation of 76.2 PSI, below the 100 PSI threshhold. 

#### Suspension Coil T-Test
I took a random sample of 50 readings from the population data file of 150 observations. I performed a one sample t-test which returned a p-value of 0.89. My p-value was greater than my significance level of .05% and therefore my null hypothesis that there is no statistical difference between the observed sample and the population mean is rejected. I found that there is statistical difference with the random sample taken.

#### Designed Study
For further study and analysis on the MechaCar and its comparison to other cars on the market, I would study the fuel efficiency. Since the current analysis on mpg has shown that the vehicle length and ground clearance have a correlation to the fuel efficiency, I would take the study one step further and analyze the standard tire size being used in the prototype cars.

The question I would present is the fuel efficiency of the car negatively affected by the tire size on the MechaCar prototype? My null hypothesis is that there is a negative correlation between the tire size and the miles per gallon. The alternative hypothesis is that there is no statistical significant correlation between the miles per gallon and tire size. 

I would first perform tests using A/B testing with two different tire sizes and gather the miles per gallon data, the tire sizes used and the tread depths if needed for further analysis. I would group the data by tire size and perform a simple linear regression on each set of data to determine if there is a predictable trend. I would evaluate the p-value for each set. I would then use a multiple linear regression on each set of data to see if the tire size had as much effect on the miles per gallon compated to the other collected data.

### Tech Used
- RStudio
- JSONlite
- Tidyverse

### Sample code
![sample code](/image/code.png)