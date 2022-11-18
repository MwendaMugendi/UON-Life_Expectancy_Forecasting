# UON-Life_Expectancy_Forecasting

## The business question

### <span style="color:blue"> Life Expectancy forecasting helps in understanding what factors are most responsible for short and long lifespans in countries.</span>

**The goal:** Forecast life expenctancy for a country.

<ins>**How does this help UON ML 2022 Class?**<ins>
* Gauge the technical skills required to prepare data and build a Linear regression ML model. 
* Understand factors that influence life expectancy. 

## Solution

* **Assumptions:**
- The life expectancy can be described by the features in the dataset. 
 

* Using the data provided, Group F builds a life expectancy prediction model that is able to provide approximate expected life span based on the features provided. 

* A linear regression model is built to model life expectancy based on the features provided.
* Root Mean Squared Error is used as an evaluation metric. 

## Conclusion and Next Steps
### About the data
* This data is right tailed but seem to follow a normal distribution pattern. 
* The life expectancy steadily from late thirties to mis seventies before reducing in the rate of increase. 
* By far, life expectancy between 70 and 75 seems the most frequent in the dataset. 

- While we find Adult Mortality to be strongly negatively correlated with life expectancy, it seems to be an obvious reason because more adult deaths mean a lower life expectancy. 
- HIV/AIDs has the second strongest negative correlation with life expectancy while Schooling has the strongest positive correlation with life expectancy.  
- Interestingly, higher intakes alcohol, diphtheria and BMI result in a higher life expectancy. 
- Population has the highest percentage of missing values yet its influence on the target variable is not significant. 

* We use a statistical test to verify whether life expectancy has a normal distribution or not. A p- value smaller than 0.05 means the null hypothesis is rejected. As such, a p-value of 0.05 or greater means that the distribution is a normal distribution. 
* Life expectancy, therefore, does follow a normal distribution. 
* A Shapiro-Wilk test is also used to confirm if the data has been drawn from a normal distribution or not. The results are similar to observations made using the D’Agostino’s K^2 Test. 

- Mean is used as the statistical measure because it describes the average life expectancy of the population. 
- Developed countries are seen to have the highest life expectancy. 
- African countries seem to have the lowest life expectancies.
- In general, life expectancy increases across the years. 

## About the code
* An explorative approach is used for modeling. 
* Multivariate linear regression is implemented, and the final model as a Root Mean Squared Error of 4.13 against a baseline of 9.71.
* RMSE is the preferred evaluation metric method because it penalises large errors more. 