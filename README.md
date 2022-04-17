# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Coefficients:
                   Estimate Std. Error t value Pr(>|t|)    
(Intercept)      -1.040e+02  1.585e+01  -6.559 5.08e-08 ***
vehicle_length    6.267e+00  6.553e-01   9.563 2.60e-12 ***
vehicle_weight    1.245e-03  6.890e-04   1.807   0.0776 .  
spoiler_angle     6.877e-02  6.653e-02   1.034   0.3069    
ground_clearance  3.546e+00  5.412e-01   6.551 5.21e-08 ***
AWD              -3.411e+00  2.535e+00  -1.346   0.1852    
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 8.774 on 44 degrees of freedom
Multiple R-squared:  0.7149,	Adjusted R-squared:  0.6825 
F-statistic: 22.07 on 5 and 44 DF,  p-value: 5.35e-11

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Is the slope of the linear model considered to be zero? Why or why not?

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

## Summary Statistics on Suspension Coils

![image](https://user-images.githubusercontent.com/96349827/163726930-f887d70c-f730-43aa-9692-03e02970de91.png)

![image](https://user-images.githubusercontent.com/96349827/163726921-fe4b7abd-78fb-48c2-b970-ad1963f97f8e.png)

The summary variance at Lot1 and Lot2 are lower than 100, so they fit specification. However, the summary variance at Lot3 is 170, and SD is 17. Lot3 have some vehicles are out of specification.

## T-Tests on Suspension Coils

ALL

> results

	One Sample t-test

data:  sc$PSI
t = -1.8931, df = 149, p-value = 0.06028
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1497.507 1500.053
sample estimates:
mean of x 
  1498.78 
  
Lot 1

> results1

	One Sample t-test

data:  lot1$PSI
t = 0, df = 49, p-value = 1
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1499.719 1500.281
sample estimates:
mean of x 
     1500 
     
Lot 2
 
> results2

	One Sample t-test

data:  lot2$PSI
t = 0.51745, df = 49, p-value = 0.6072
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1499.423 1500.977
sample estimates:
mean of x 
   1500.2 
   
Lot 3

> results3

	One Sample t-test

data:  lot3$PSI
t = -2.0916, df = 49, p-value = 0.04168
alternative hypothesis: true mean is not equal to 1500
95 percent confidence interval:
 1492.431 1499.849
sample estimates:
mean of x 
  1496.14
  
## Study Design: MechaCar vs Competition

What metric or metrics are you going to test?

We will test the mean City MPG for MechaCar vs the comptition

What is the null hypothesis or alternative hypothesis?

Null: Mechacar has a better city MPG compared to the competition

What statistical test would you use to test the hypothesis? And why?

We would need to t.test the Mean city MPG for MechaCAr vs the Mean city mpg for the competition

What data is needed to run the statistical test?

To run this study, a sufficient amount of data of each car's city MPG would be need to be collected. According to the Central Limit Theorem, a sample size larger than 30 is sufficient for the theorem to hold.
