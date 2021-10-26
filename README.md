# MechaCar_Statistical_Analysis

## Deliverable 1: Linear Regression to Predict MPG


![deliverable1_linearRegression](https://user-images.githubusercontent.com/86584404/138804848-388ed1e9-53d7-4059-ac32-8c0f8f99967e.jpeg)

![deliverable1_Summary 1](https://user-images.githubusercontent.com/86584404/138804862-46cc92a2-1f2e-4b93-9869-e1cc01d0d26c.jpeg)


1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
The vehicle length and ground clearance variables provided non-random degrees of variance compared to the MPG values.

2. Is the slope of the linear model considered to be zero? Why or why not?
The p-value for this set is smaller than the assumed significance (p-value: 5.35e-11) which tells us that there is evidence to reject a null hypothosis, as well, inidicates that slope would not be zero. 

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
This model encompasses approximately 71% of MPG predictions which tells us that it is a good model for prototyping. 

## Deliverable 2: Create Visualizations for the Trip Analysis 
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![suspension_coil_AllLots](https://user-images.githubusercontent.com/86584404/138969707-e1508502-d0e6-47f2-bdde-6ac073c773d1.jpeg)

With a variance of 62.29, the current manufacturing design for all lots meets the current specifications (not to exceed 100 PSI). 

![suspension_coil_PerLot 1](https://user-images.githubusercontent.com/86584404/138969711-58472efb-cb78-4547-9efe-2223b94afbfe.jpeg)

With variances of 0.98 and 7.47 Lot 1 and Lot 2, respectively, would also meet design specifications. However, Lot 3 has a variance of 170.29 which would cause concern as it is disproportionate to the total lot summary as well as compared to Lot 1 and Lot 2. Per Lot 3's statistics, design specs would not be met and someone should proabably dig into that further. 

## Deliverable 3: 
### T-Tests on Suspension Coils

Objective: determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

![t testAllLots](https://user-images.githubusercontent.com/86584404/138968106-cb15b3b3-010a-47e0-84de-b6c62869ca51.jpeg)

With a mean of 1498 and a p-value of .06, the PSI across **all** manufacturing lots would be statistically similar to the population mean of 1,500. 

Obective: determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

Lot 1: 
![t testLot1](https://user-images.githubusercontent.com/86584404/138968723-1abc8ff7-23aa-4fff-b4b9-3f275df00b0c.jpeg)
With a mean of 1500 and a p-value of 1, the PSI across **manufacturing Lot 1** would be also be statistically similar to the population mean of 1,500. 


Lot 2:
![t testLot2](https://user-images.githubusercontent.com/86584404/138968739-6b12e95b-be15-4abc-b0a4-5932c040f5cf.jpeg)
Similar to Lot 1, and with a mean of 1500.02 and a p-value of .61, the PSI across **manufacturing Lot 2** would be also be statistically similar to the population mean of 1,500. 


Lot 3: 
![t testLot3](https://user-images.githubusercontent.com/86584404/138968764-0de835ab-f468-483b-8d5a-12179a1d8b04.jpeg)
With a mean of 1496 and a p-value of .04 (lower than the common significance of .05), the PSI across **manufacturing Lot 3** would be then be statistically different to the population mean of 1,500. 

## Deliverable 4:
### Study Design: MechaCar vs Competition

Objective: design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

Hypothetically speaking, this study would span across 10 years. We would be looking at the performance of German-engineered vehicles: BMW, Audi, Mercedes Benz

_What metric or metrics are you going to test?_

1. MPG (highway and in-town driving)
2. Horsepower
3. Oil Change Freqency 
4. Engine size

_What is the null hypothesis or alternative hypothesis?_

The faster one drives, the lower the MPG rating. 
The slower one drives, the higher the MPG rating.
With more oil changes comes better engine performance. 
The higher the horsepower, the lower the MPG rating. 
The lower the horsepower, the higher the MPG rating. 
Bigger engine sizes require more oil changes. 

_What statistical test would you use to test the hypothesis? And why?_

Because of the many variables, I would run a MLR (multiple linear regression) study. 

_What data is needed to run the statistical test?_

Per manufacturer MPG, Horsepower, Engine Size and Oil Change Frequency
