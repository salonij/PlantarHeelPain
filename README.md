# PlantarHeelPain
Abstract: 

The Tendinopathy Team Cohort is conducting 3T_the 10000 Tendons study that aims to build a model that can predict the outcome for plantar heel pain tendinopathy. They are using traditional methods like Linear Regression to build the model. So, we are working on other methods to see if we can build a better predictive model. To better inform decisions, we need a deeper understanding of the complex factors and their interactions that influence health at patient’s level and more effective diagnostic methods.   Machine learning has been successful in building effective diagnosis systems. This study aims to distinguish plantar heel pain with other foot problem groups by performing classification based on machine learning classification algorithm such as Random Forest. The model building process was guided by common sense reasoning and by knowledge discovered during Exploratory data analysis and definitive conclusions were drawn. Findings not only reveal that Random Forest algorithm works better with regards to performance, but it also uncovers new knowledge that is hidden in data which helps in building a more robust feature set and strengthen the classification model.

About Data:

The dataset that we are using in this paper are the answers to the baseline questionnaires in the trial of plantar heel pain tendinopathy and related condition group. There are total 542 patients that are in one of the three condition groups: 1) People with PHP;2) Other foot problem;3) Healthy control. Due to Data Privacy Policy of the 3T_the 10000 Tendons study , we can't share the dataset but we are sharing list of features and their description in the dataset for better understanding.

Features in dataset and their description:

pid -	Patient ID
grp	- Condition Groups (1=People with plantar heel pain; 2=Other foot problem; 3=Healthy control)
g	- Gender
age	- Age
bmi	- Body mass index
TimeOnFeet - How much time do you spend on your feet in your daily life? (in Hours)
SportsCondition -	Do you do any sports or exercise regularly? (0=No;1=Yes)
ControlPrelnj	- Have you ever had any foot problem(s)? (0 = Yes-right foot;1 = Yes-left foot,2 = Yes-both feet;3=No;4=Do not know)
MorningPain	- Do you have pain in your foot when you first stand up in the morning? (0=Yes-always;1=Yes-occasionally;2=No)
MornPD	- How long does the morning pain last? (Number)
SeverityPain	- How severe is your foot pain during the first step in the morning? (Scale:0 to 100)
PreviousInjury	- Do you have any previous injury or problem in your feet? (0=Yes-right foot;1=Yes-left foot;2=Yes-both feet;3=No)
OtherTendinopathy	- Have you ever had or do you currently have symptom(s) in any tendon(s) other than plantar heel pain? (0=Yes-currently,1=Yes-previously;2=No)
BackP	- Do you have current or previous back pain? (0=Yes – Current; 1=Yes – Recurrent; 2=Yes – Previous; 3=No)
BackPainDistance	- How far does it go down ? (0=To the thigh; 1=To the knee; 2=Below the knee but not into the foot; 3=To the foot; 4=NoPain)
BackpainL	- Was(is) the back pain associated with leg pain? (0=Yes; 1=No)
Work	- Do you work? (0=Yes, full time; 1=Yes, part time; 2=No)
Occupation	- Occupation 
OccupationClass	- 0=Blue Collar; 1=White Collar; 2=Professional; 3=Self-employment; 4=Unemployment; 5=Housewife; 6=Retired; 7=Athlete 
FHSQPain	- Pain subscale of FHSQ (Foot Health Status Questionnaire) (Scale: 0 to 100)
FHSQFunction	- Function subscale of FHSQ (Foot Health Status Questionnaire) (Scale:0 to 100)
FHSQGeneralFootHealth	- General foot health subscale of FHSQ (Foot Health Status Questionnaire) (Scale:0 to 100) 
FHSQFootwear	- Footwear subscale of FHSQ (Foot Health Status Questionnaire) (Scale: 0 to 100)
gpa	- GPAQ = Global physical activity questionnaire 
pcs	- PCS = Pain Catastrophization Scale
fpa	- Physical activity subscale of FABQ (Fear- Avoidance Beliefs Questionnaire) (Scale: 0 to 24)
fw	- Work subscale of FABQ ( Fear- Avoidance Beliefs Questionnaire) (Scale: 0 to 42)
csi	- CSI = Central Sensitization of Inventory (Scale: 0 to 100) 
eq5d5li	- EQ5D5L= Generic Health Status Questionnaire  in 5 dimension (Scale: -0.208 to 1.0)
eq5d5lv	- EQ5D5L= Generic Health Status in VAS scale (Scale: 0 to 100)
DomLeg	- Which is your dominant leg? (0=Right, 1=Left, 2=Not sure)
RunningDistance	- Running Distance
RunFre	- How many days have you been running in a week generally? (0=1 - 2 times in a week; 1=3 - 4 times in a week; 2=5 - 6 times a week; 3=Other)
LevelOfSports	- At what level are you participating in your sports discipline ? (0=Fun/fitness; 1=Occasional amateur competition; 2=Competitive amateur; 3=Semi-professional; 4=Professional-youth/academy;5=Professional-senior competition; 6=Other)
YearofSports	- How many years have you been participating in your sporting discipline ?
EffectedSide	- In which foot(s) do you have plantar heel pain?(OR In which leg(s) do you have foot/ankle problem(s)? (0=Right; 1=Left; 2=Both)
PHPDuration_Right	- How long have you had Plantar heel pain for right foot ? (0=0-1 month; 1=1-3 months; 2=3-6 months; 3=6-9 months; 4=9-12 months; 5=1-2 years; 6=2-3 years; 7=>3 years)
PHPDuration_Left	- How long have you had plantar heel pain for left foot? (0=0-1 month; 1=1-3 months; 2=3-6 months; 3=6-9 months; 4=9-12 months; 5=1-2 years; 6=2-3 years; 7=>3 years)
Onset	- Please describe the onset of your pain? (0=Sudden, 1=Gradual, 2=Other)
PainSitting	- How is your pain after taking some steps following sitting or lying for a while? (0=Get worse, 1=Get better, 2=No effect)
PainWalking	- How is your pain after walking? (0=Get worse, 1=Get better, 2=No effect)
PainStanding	- How is your pain during standing? (0=Get worse, 1=Get better, 2=No effect)
WorkPart	- Have you had to change your work participation/activity as a result of your foot problem? (0=No 1=Yes)
ExtWorkPart	- To what extent did you change your work? (0=Now I can do only light duties, 1=I reduced my work hours, 2=I left my job, 3=I changed my job role, 4=Other)
OtherInjury	- Do you have any current injury or problems other than Plantar Heel pain in your feet? (OnlyPHP) (0=Yes, right foot, 1=Yes, left foot, 2=Yes, both feet, 3=No)
ConditionPrediction	- Do you think your condition will... (0=Get better, 1=Stay the same, 2=Get worse, 3=Do not know)
ConConf	-How confident are you with this recovery prediction?(%)
TimePrediction	- Please rate your confidence in your recovery time prediction? (%)
Menopause	- What is your menopausal status? (0=Not applicable, 1=Pre-menopausal, 2=Currently menopause, 3=Post menopause)
HormoneThe	- Do you take hormone replacement therapy? (0=Not applicable, 1=Yes, 2=No)
SleepDuration	- How many hours sleep do you get in a typical night?
SleepDifficulty	- Do you have any difficulties when you are sleeping? (0=No 1=Yes)
ReasonSleeDiff	- What is the main reason of your sleep difficulties? (0=Foot pain, 1=Other pain, 2=Depression, 3=Anxiety, 4=Other)
FeelingRested	- Do you feel rested after sleeping? (0=Yes, 1=Partially, 2=No)
Smoking	- Do you smoke? (0=Yes - active smoker, 1=Yes - Social smoker, 2=No - passive smoker, 3=No - ex smoker, 4=No - never smoked)
Ethinicty	- What is your ethnic origin? (0=White - British, 1=White - Irish, 2=White - any other White Background, 3=Arab, 4=Asian, 5=Black or Black British - Caribbean, 6=Black or Black British - African, 7=Black - any other Black background, 8=Chinese, 9=Mixed - White and Black African, 10=Mixed - Any other mixed background, 11=Prefer not to say, 12=Other)
Education	- What is the highest level of education you have completed? (0=Did not attend school, 1=Primary school, 2=Secondary school, 3=High school/collage, 4=Undergraduate degree, 5=Masters Level, 6=Doctor of Philosophy/PhD)
PASS	- Taking into account the many ways your foot pain affects your daily life, if you were to remain for the next few months as you are now, would you consider your current state to be satisfactory?  (0=No 1=Yes)
SANE	- How would you rate your foot today as a percentage of normal? (Scale: 0 to 100)
Footwear - What kind of shoes do you typically wear in a daily life? (1=Flip-flop,2=Sandals,3=Leather dress shoes, 4=High Heeled, 5=Slip on Shoes, 6=Sneaker, 7=Trainers, 8=Orthopedic Footwear, 9=other)
Comorbities	- Do you currently take any medicine prescribed by your doctor for any of the following conditions?(1=Diabetes,2=Osteoartritis,3=Blood Pressure, 4=Heart Disease, 5=Lung Disease, 6=Hormon Replacement, 7=High Cholesterol, 8=Rhemotoid Artritis, 9=Back Pain, 10=Depression, 11=Other,12=None)
NumofComorbity	- Number of Comorbidities 
Depression	- 0=non-selected,1=Selected
eHealth	- Scale: 8 to 40

Aim:

The main objective of using this questionnaire data is to build a classification model to learn the relationship between a set of features and the target class. In our case, we have patient’s self-reported physical factors, psychosocial factors, health-related quality of life, condition-specific factors and activity level as features and our target class is the group in which the patient belongs (plantar heel pain, other foot problem and control group).  Medical information has redundancy, multi-attribution, incompleteness and a close relationship with time. The problem of using the massive volumes of data effectively becomes a major problem for the health sector. Data mining provides the methodology and technology to convert these data mounds into useful decision-making information. Exploratory data analysis is done first to compare causes and symptoms of patients in the three condition groups (plantar heel pain, other foot problem and control group) and to choose subset of features that helps to distinguish the three condition groups better. In this paper, Random forest algorithm is used to build a classification model. Since, the patients involved in the trial are arbitrary, we are excluding the demographic data while building the model to avoid biasness. AUC-ROC curve is used to check the ability of model to distinguish between classes. It is one of the most important evaluation metrics for checking any classification model’s performance. Feature selection using Random Forest, is used to filter redundant features and to help clinicians identify the minimal questionnaires that can effectively distinguish the condition groups. This research will be of interest to anyone working in medical diagnosis using ML technology. 

Findings:

Using Random forest classifier, we can distinguish the plantar heel pain group from other foot problem group with 97% accuracy. However, while performing exploratory data analysis, we found that some of the features like Reason for Sleep Difficulty, Comorbidities, Onset of morning pain had some categories with zero probabilities causing imbalances in the sample. So, when we get more data, we would expect some of these imbalances to resolve and then we would revisit this thing, as we don’t know at the moment how well it’s going to work as we don’t have much data. So, if clinicians want to continue with this recruitment methodology and produce some data that is going to be useful for machine learning, then they got to concern themselves about the lack of balance in the data. 



 





