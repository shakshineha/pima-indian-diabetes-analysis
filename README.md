# pima-indian-diabetes-analysis
This repository consists a basic analysis of a diabetes dataset.

Link from where the dataset is taken https://www.kaggle.com/uciml/pima-indians-diabetes-database/version/1

Columns of the table

Pregnancies------- Number of times pregnant
Glucose-------Plasma glucose concentration a 2 hours in an oral glucose tolerance test Blood Pressure-----Diastolic blood pressure (mm Hg)
Skin Thickness-----Triceps skin fold thickness (mm)
Insulin------------2-Hour serum insulin (mu U/ml)
BMI----------------Body mass index (weight in kg/(height in m)^2)
Diabetes Pedigree Function -Diabetes pedigree function
Age---------------Age (years)
Outcome Class----- variable (0 or 1)


Steps that have been performed in the analysis:

Step 1: Import all the files necesaary 
Step 2: Get the dataset and print its data and get to know mundane facts about it
**By mundane facts we mean here that the facts like shape of dataset, columns, some of its rows etc**
Step 3:Grouping the number of elements based on outcomes to get a general idea
Step 4:Grouping the number of elements based on age to get a general idea
Step 5:Grouping the number of elements based on number of pregnancies to get a general idea
Step 6:Get a graph to generalize all the columns visually
**First set of graphs represent data when Outcome=0
Second set of graphs represent data when Outcome=1**
Step 7:When we calculate we will find that there is no missing value, hence we need not go any further in this direction
Step 8:When analyzing the histogram we can identify that there are some outliers in some columns. We will further analyse those outliers and determine what we can do about them.

**Blood pressure 
By observing the data we can see that there are 0 values for blood pressure. And it is evident that the readings of the data set seems wrong because a living person cannot have diastolic blood pressure of zero. By observing the data we can see 35 counts where the value is 0.

**Plasma glucose levels
Even after fasting glucose level would not be as low as zero. Therefor zero is an invalid reading. By observing the data we can see 5 counts where the value is 0.

**Skin Fold Thickness
For normal people skin fold thickness can’t be less than 10 mm better yet zero. Total count where value is 0 : 227.

**BMI
Should not be 0 or close to zero unless the person is really underweight which could be life threatening.

**Insulin
In a rare situation a person can have zero insulin but by observing the data, we can find that there is a total of 374 counts which is not at all common.

The cases we see above are invalid as the value of Insulin or BMI or Glucose Level can never be zero.
Skin Thickness can also not be zero but since it is not the most important character while analysis and establishing the fact that wether a person has diabetes or not we can ignore it as well,

Step 9: Remove all the values where BP, BMI or Glucose Level is zero
Step 10: Make a graph again to get a idea and see how the values have improved
Step 11: After this various graphs in between the different properties can be made so as to get a relation between them

