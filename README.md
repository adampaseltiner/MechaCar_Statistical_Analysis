# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![Image1](https://user-images.githubusercontent.com/82347825/128112434-8df09bd5-28b3-411b-8666-668f514fc665.png)

- Based on the multiple linear regression model, the most significant variables which show a non-random effect on the mpg of a MechaCar are the intercept (mpg), vehicle length, and ground clearance.

![Image2](https://user-images.githubusercontent.com/82347825/128114941-f64f0913-4e47-407f-a3ec-b69525bcbf6f.png)

- The slope of the linear model should not be considered zero, since the p-value of 5.35e-11 is much lower than an the level of significance of 0.05%.
- The linear model predicts the mpg of MechaCar prototypes rather effectively since the r-squared value of 0.7149 means the predictions are 71% accurate when using this model.

## Summary Statistics on Suspension Coils
![Image3](https://user-images.githubusercontent.com/82347825/128256843-324f5042-ae53-4204-bbb1-f7fff2c15088.png)

![Image4](https://user-images.githubusercontent.com/82347825/128255765-d2f51ad2-82ff-4bec-a523-9d5948510ed6.png)

*The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.*

- The overall variance of the production lot is 62.29 PSI, which is well within the 100 PSI variance requirement. However, when looking at the lots individually we see that Lot 1 and Lot 2 fall well under the 100 PSI requirement while Lot 3 is showing a variance of 170.29 which greatly exceeds the allowed variation.

## T-Tests on Suspension Coils

### Cumulative t-test
![ttestALL](https://user-images.githubusercontent.com/82347825/128257918-096d95b0-139c-47cd-8c66-85a49e96ee7b.png)
- The t-test for suspension coil PSI across all lots shows they are not statistically different from the population mean, with a p-value of 0.06028.

### Lot 1 t-test
![ttest1](https://user-images.githubusercontent.com/82347825/128257737-83553534-fd14-4538-b28b-699403868c18.png)
- The t-test for suspension coil PSI in lot 1 shows they are not statistically different from the population mean, with a p-value of 1.

### Lot 2 t-test
![ttest2](https://user-images.githubusercontent.com/82347825/128257742-9f9fbfce-ea3d-41eb-8c8b-dfb25b998a66.png)
- The t-test for suspension coil PSI in lot 2 shows they are not statistically different from the population mean, with a p-value of 0.6072.

### Lot 3 t-test
![ttest3](https://user-images.githubusercontent.com/82347825/128257750-c48d7c74-e6fe-4082-8024-81fb6bcfda4b.png)
- The t-test for suspension coil PSI in lot 3 shows they are slightly statistically different from the population mean, with a p-value of 0.04168 indicating we can reject the null hypothesis.

## Study Design: MechaCar vs Competition

### Metrics to Test
We can perform additional statistical studies to reveal how the MechaCar compares to its competition. For example, one significant metric that consumers consider when buying a car is horsepower. 

### Null and Alternative Hypotheses
- Null hypothesis: MechaCar has a similar engine horsepower to competitor vehicles in the same class.
- Alternative hypothesis: Mechacar horsepower is significantly above/below average compared to competitor vehicles in the same class.

### Statistical Test
To verify our hypothesis we can use linear regression models and t-tests to verify a significance level of 0.05%. Results could also be plotted with ggplot2 to show data spread with a boxplot.

### Data for Statistical Test
We would need to gather the data on horsepower for competitor vehicles to the MechaCar. 
