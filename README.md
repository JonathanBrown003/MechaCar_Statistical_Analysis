# MechaCar_Statistical_Analysis
Using statistics and R to analyze automotive data in a manufacturing environment. 

Please review the RScript Challenge Code ![here.](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/f77d8ef4614efbd80107cfd92ea22c6424474cae/MechaCarChallenge.R)

## Project Summary
The goal of this project is to analyze production data for a new automotive prototype in the works. Performance is analyzed over a number of statistical tests to provide insight to the manufacturing team. Variables such as miles per gallon, vehicle length, weight, ground clearance, and all-wheel-drive capability were some of the variables analyzed. 

## Linear Regression to Predict MPG
Please see below for a summary of the data as returned in R:

![](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/faab47efc1a186d33618fa94fe62dab96ae9a05a/Resources/Deliv1_Output.PNG)

1) Variance of a non-random variable is generally 0. Taking this into consideration, vehicle_length and ground_clearance variables can be said to provide a non-random amount of variance to the miles per gallon values in this dataset.

2) The slope of the linear model cannot be considered to be zero because of the low value of the p-value above. The null hypothesis must be rejected as a result of this p-value. 

3) All else equal, and taking into account the R-squared value of 0.7149 - this model can be said to be 71% accurate in predicting variability as the R-Squared value is the dependent variable variation that a linear model explains. At 71% accurate, this model is relatively effective at predicting miles per gallon of prototypes. 

## Summary Statistics on Suspension Coils
Please see below for a summary of the data as returned in R:

### Lot Summary: 
![](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/ca02a18262be1542f3b78701c94d9560054ae8e8/Resources/Deliv2_Lot_Summary.PNG)

### Total Summary
![](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/ca02a18262be1542f3b78701c94d9560054ae8e8/Resources/Deliv2_Total_Summary.PNG)

1) The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. As you can see above in the Lot Summary, lots 1 & 2 do not exceed this threshold though lot 3 does exceed the threshold of 100 PSI. In total, as seen above in the Total Summary, the totality of all lots has a variance of 62.29 which is well within an acceptable range. A wise solution would be to inspect Lot 3 for defects. 

## T-Tests on Suspension Coils

### Lot 1 T-Test
![](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/05abe13f10eb1f306b94021b04a1aed7d915363a/Resources/Deliv3_Lot1_Ttest.PNG)

### Lot 2 T-Test
![](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/05abe13f10eb1f306b94021b04a1aed7d915363a/Resources/Deliv3_Lot2_Ttest.PNG)

### Lot 3 T-Test
![](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/05abe13f10eb1f306b94021b04a1aed7d915363a/Resources/Deliv3_Lot3_Ttest.PNG)

### Cumulative Data T-Test
![](https://github.com/JonathanBrown003/MechaCar_Statistical_Analysis/blob/05abe13f10eb1f306b94021b04a1aed7d915363a/Resources/Deliv3_One_Sample_Ttest.PNG)

1) Lot 3 has a P-Value of 0.04168 which is low enough to reject the null hypothesis. The other 2 lots and the Cumulative T-Test have P-Values high enough to not reject the null hypothesis. Lot 3 needs more evaluation for defects for the purposes of rejecting the coils. This T-Test for Lot 3 along with the high variance as reported in the Summary Statistics heading above point to manufacturing defects specifically with Lot 3.   

## Study Design: MechaCar vs Competition

