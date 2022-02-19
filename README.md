# Carduovascular-Risk-Prediction
The dataset is from an ongoing cardiovascular studyon residents of the town of Framingham,Massachusetts. The classification goal is to predictwhether the patient has a 10-year risk offuture coronary heart disease (CHD). The dataset providesthe patients’ information. It includesover 4,000 records and 15 attributes.VariablesEach attribute is a potential risk factor. There are both demographic, behavioral, and medical riskfactors.

Data DescriptionDemographic:
Sex: male or female("M" or "F")
Age: Age of the patient;(Continuous - Although therecorded ages have been truncated towhole numbers, the concept of age is continuous)Behavioral
is_smoking: whether or not the patient is a currentsmoker ("YES" or "NO")
Cigs Per Day: the number of cigarettes that theperson smoked on average in one day.(can beconsidered continuous as one can have any number ofcigarettes, even half a cigarette.)Medical( history)
BP Meds: whether or not the patient was on bloodpressure medication (Nominal)
Prevalent Stroke: whether or not the patient hadpreviously had a stroke (Nominal)
Prevalent Hyp: whether or not the patient was hypertensive(Nominal)
Diabetes: whether or not the patient had diabetes(Nominal)Medical(current)
Tot Chol: total cholesterol level (Continuous)
Sys BP: systolic blood pressure (Continuous)
Dia BP: diastolic blood pressure (Continuous)
BMI: Body Mass Index (Continuous)
Heart Rate: heart rate (Continuous - In medicalresearch, variables such as heart rate though infact discrete, yet are considered continuous becauseof large number of possible values.)
Glucose: glucose level (Continuous)Predict variable (desired target)
10-year risk of coronary heart disease CHD(binary:“1”, means “Yes”, “0” means “No”) -DV
