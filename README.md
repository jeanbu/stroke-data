# stroke-data
We are interested in finding the factors that make a patient more likely to suffer a stroke. We are going to study different variables to explore the relationship and differences among biological and environmental factors and stroke incidence.

Our data focuses on over 5000 patients. This project offers exciting possibilities for prediction analysis and hopefully actionable insights to reduce strokes.

### Data Cleaning
We have check for duplicates
We have identified missing BMI and smoking_status information
We have dummified the variables to manipulate the data in our models later on

### Exploratory Data Analysis
We could see in charts that both bmi and average glucose had a positive relationship with suffering a stroke.
By dividing the population in different subcategories (for example, underweight, obese, etc.) we were able to show a big difference in the stroke rate.
Age also showed a clear relationship with stroke, with virtually no patients younger than 30 suffering from it.
Hypothesis
We tested our null hypothesis to see wether or not the patient median age was different between those who suffered a stroke and those who didn't. We rejected the null hypothesis.

We also test our null hypothesis to see wether or not the patient mean BMI was different between those who suffered a stroke and those who didn't. We rejected the null hypothesis.

### ML models
We assigned all children under 10 as never smoked. The rest of the missing values were assigned by random forest.
We assigned the bmi missing values by random forest too, which resulted in a mean higher than the overall population mean.
We tuned two different models, logistic regression and random forest. Due to it's simplicity and good recall rate relative to f1-score, we prefer the logistic regression model.
