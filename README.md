# Cardiovascular-Risk-Prediction
The dataset is from an ongoing cardiovascular studyon residents of the town of Framingham,Massachusetts. The classification goal is to predictwhether the patient has a 10-year risk offuture coronary heart disease (CHD). The dataset providesthe patients’ information. It includesover 4,000 records and 15 attributes.VariablesEach attribute is a potential risk factor. There are both demographic, behavioral, and medical riskfactors.

# Data DescriptionDemographic:
* Sex: male or female("M" or "F")
* Age: Age of the patient;(Continuous - Although therecorded ages have been truncated towhole numbers, the concept of age is continuous)Behavioral
* is_smoking: whether or not the patient is a currentsmoker ("YES" or "NO")
* Cigs Per Day: the number of cigarettes that theperson smoked on average in one day.(can beconsidered continuous as one can have any number ofcigarettes, even half a cigarette.)Medical( history)
* BP Meds: whether or not the patient was on bloodpressure medication (Nominal)
* Prevalent Stroke: whether or not the patient hadpreviously had a stroke (Nominal)
* Prevalent Hyp: whether or not the patient was hypertensive(Nominal)
* Diabetes: whether or not the patient had diabetes(Nominal)Medical(current)
* Tot Chol: total cholesterol level (Continuous)
* Sys BP: systolic blood pressure (Continuous)
* Dia BP: diastolic blood pressure (Continuous)
* BMI: Body Mass Index (Continuous)
* Heart Rate: heart rate (Continuous - In medicalresearch, variables such as heart rate though infact discrete, yet are considered continuous becauseof large number of possible values.)
* Glucose: glucose level (Continuous)Predict variable (desired target)
10-year risk of coronary heart disease CHD(binary:“1”, means “Yes”, “0” means “No”) -DV

# Steps involved:
The full code for this article can be found here. It is implemented in Python and different classification algorithms are used. Below is a brief description of the general approach that I employed:
* Data cleaning and pre-processing: 
Here I checked and dealt with missing and duplicate variables from the data set as these can grossly affect the performance of different machine learning algorithms (many algorithms do not tolerate missing data).
* Exploratory Data Analysis: 
Here I wanted to gain important statistical insights from the data and the things that I checked for were the distributions of the different attributes, correlations of the attributes with each other and the target variable and I calculated important odds and proportions for the categorical attributes.
* Encoding of categorical columns:
We used One Hot Encoding to produce binary integers of 0 and 1 to encode our categorical features because categorical features that are in string format cannot be understood by the machine and needs to be converted to numerical format.
* Feature Selection:
Since having irrelevant features in a data set can decrease the accuracy of the models applied, I used the Boruta Feature Selection technique to select the most important features which were later used to build different models.
* Model development and comparison:
I used four classification models, i.e., Logistic Regression, K-Nearest Neighbors, Decision Trees and Support Vector Machine, After which I compared the performance of the models using their accuracy and F1 scores. I then settled with the best performing model.
* Fitting different models:
For modelling we tried various classification algorithms like
1. Logistic Regression
2. K-nearest neighbors
3. Decision tree
4. SVM Classifier

# Conclusion
That's it! We reached the end of our exercise. Starting with loading the data so far we have done EDA , null values treatment, encoding of categorical columns, feature selection and then model building. In all of these models our accuracy revolves in the range of 70 to 96%. So the accuracy of our best model is 96% which can be said to be good for this large dataset. As we see there are some cardiovascular diseases more depends on age, sex, patient with hypertensive , and there are some features which effects least to our model like, Diabates, previous Strock history, Blood pressure history.

# References
https://www.nature.com/articles/s41598-020-62133-5
https://www.thelancet.com/journals/langlo/article/PIIS2214-109X(19)30365-1/fulltext
