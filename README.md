# INFO-H410-Group16

Group 16's Project of INFO-H410 "Techniques of Artificial Intelligence" 2025-2026

This group's choosen problem is a binary classification.
To try and use all features to predict correctly a label, we use 3 machine learning methods :

* Bayesian Networks,

* Decision Tree,

* Neural Network.

This is done onto a specific dataset, which correspond to a subset of the <a href="https://www.cdc.gov/brfss/annual_data/annual_2014.html">"CDC Diabetes Health Indicators"</a> dataset.
This subset was found on <a href= "https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators">"UC Irvine Machine Learning Repository"</a> and was downloaded on <a href="https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset/data">"Kaggle"</a>.

The target classification is binary : 0 means non-diabetic, and 1 means pre-diabetic or diabetic.
This subset is balanced and contains 70,692 survey responses about 21 variables. Informations about those variables were given on the up-mention websites, and a notebook with all variables categories can be found on the CDC webpage.

* There are 14 binary features:
  * HighChol:0 if patient does not have high cholesterol, 1 if they do.
  * HighBP: 0 if patient does not have high blood pressure, 1 if they do.
  * Smoker: 1 if the patient has smoked at least 100 cigarettes in their entire life, 0 if they have not.
  * Stroke: 0 if they have never had a stroke, 1 if they have.
  * HeartDiseaseorAttack: 0 if they have never had coronary heart disease or myocardial infarction, 1 if they have.
  * PhysActivity: 1 if they’ve done physical activity in the last 30 days, not including their job; 0 otherwise.
  * Fruits: 1 if they consume fruits at least once a day; 0 otherwise.
  * Veggies: 1 if they consume vegetables at least once a day; 0 otherwise.
  * HvyAlcoholConsump: 1 if they’re a man- consuming more than 14 drinks per week, or a woman consuming more than 7 drinks per week; 0 otherwise.
  * AnyHealthcare: 1 if they have any healthcare coverage; 0 otherwise.
  * NoDocbcCost: 1 if, within the last year, they have needed to see a doctor but could not due to cost; 0 otherwise.
  * DiffWalk: 1 if they have serious difficulty walking or climbing stairs; 0 otherwise.
  * Sex: 0 for female, 1 for male.
* There are 3 quantitative features:
  * BMI: weight in kg divided by the square of the height in meters, rounded to the nearest integer.
  * MentHlth: number of days over the last 30 days that their mental health was bad.
  * PhysHlth: number of days over the last 30 days that their physical health was bad. 
* There are 4 ordinal variables:
  * GenHlth: patient rates their health in general as 1 = excellent, 2 = very good, 3 = good, 4 = fair or 5 = poor
  * Age: 1 = [18, 24], 2 = [25, 29], 3 = [30, 34], 4 = [35, 39], 5 = [40, 44], 6 = [45, 49], 7 = [50, 54], 8 =[55, 59], 9 = [60, 64], 10 = [65, 69], 11 = [70, 74], 12 = [75, 79], 13 = [80, 99],
  * Education: Highest level of education achieved, encoded as 1 = Never attended school or only kindergarten, 2 = Grades 1 through 8, 3 = Grades 9 through 11, 4 = Grade 12 or GED, 5 = College 1 year to 3 years, 6 = College 4 years or more,
  * Income: 1 = [0, 10000), 2 = [10000, 15000), 3 = [15000, 20000), 4 = [20000, 25000), 5 = [25000, 35000), 6 = [35000, 50000), 7 = [50000, 75000), 8 = 75000+. 
