### The Good, the Bad, & the Ugly of New York Health

    * Toni Anderson 
    * Alex Schackmuth 
    * Mieae Yun

## Intro:

Utilizing the New York Community Health Survey, this project examines the relationship between self-perceptions of health and certain behaviors and conditions.  Since we know with a great deal of certainty how behaviors such as smoking and drinking affect one’s health, this project is not designed to examine the actual health of the survey respondents.  We believe that the respondent’s perception of their own health offers a unique insight into the overall wellness of the respondents. 

## Questions and Findings:

* 1.) How do various demographic factors affect the self-reported general health of the respondent?
![](demo.PNG)
Age is a strong predictor of self-reported health.  Those in poor health are almost 120% more likely to be older than those in good health. Conversely those in excellent health are 20% more likely to be younger than those in good health. 

* 2.) How do various socio-economic factors affect the self-reported general health of the respondent?
![](se.PNG)
Education is also a strong predictor of self-reported health.  Those in poor health are almost 40% less likely to have a higher education than those in good health. Conversely those in excellent health are almost 50% more likely to have a higher education than those in good health.  

* 3.) How do various lifestyle and behavioral factors affect the self-reported general health of the respondent?
![](lifestyle.PNG)
While there is a direct positive relationship between healthy habits like exercise and eating fruits and veggies, apparently smoking and drinking also share a positive relationship with health.  This is due to the fact that a sizable amount of people that report themselves as in excellent health either smoke or drink.  While these behaviors do negatively affect health over time, one’s self-perception of health is somewhat subjective in the present. Therefore, at least in the present, people in excellent health are 20%  more likely to be smokers and drinkers.

* For specific descriptive plots see files in decriptive plots folder
## Data:

Per the Community Health Survey (CHS) website, the survey is conducted annually via telephone by the DOHMH,  Division of Epidemiology, Bureau of Epidemiology Services.  CHS data is cross-sectional and this analysis will utilize the 2013 data.  The survey sample consists of nearly 10,000 randomly selected adult New York City residents.  This data is used by local government to make policy decisions and increase understanding.
Our analysis will assess the relationship of self-reported general health in relation to certain demographic factors, lifestyle factors, and whether or not the respondent has health insurance.  The analysis begins with a descriptive visual analysis of the data then utilizes multinomial logistic regression modeling to inference these relationships at the population level.  The first of the three models will assess demographic and environmental factors, the second model (controlling for demographic and environmental factors)  will explore the effects of certain lifestyle behaviors on general health, and the third will test the relationship between perceived health and health insurance while controlling for demographic and behavioral factors.

## Data Cleanup:

The dataset was truncated to remove unneeded variables and data was prepared for analysis. See data_cleaner.ipynb

## Analysis:

The questions were answered using multinomial logistic regression. Relative percents were created by exponentiating the logits from the model then subtracting 1 from each value, then multipling by 100. See mnlm.ipynb




