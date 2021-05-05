# Mental-Health-Disorders-Diagnosis

**Proprietory Statement**
_Data from the RADARS® System Survey of Non-Medical Use of Prescription Drugs Program
are not public. These data are proprietary and are only to be used for the purposes of the
American Statistical Association’s DataFest._

**Link to presentation video:** https://drive.google.com/file/d/1ETTxWzelNi1-ePkUr26hBciJEE84ndNQ/view?usp=sharing

**Primary Questions:**
Overburdened by studies, many students conform to drug use and alcoholism. They are also often worst affected by
mental health. Substance abuse is known to trigger or intensify the feelings of loneliness, sadness and hopelessness
often associated with depression (Depression and Substance Abuse - Addiction Center, 2021). How many students
are affected by mental illness or substance abuse? Is there any relation between the two? How many students are
aware of their illness/abuse and choose to seek counselling?
The **general goal** of the project was to analyse the usage of the most common drugs/substances among students in
Canada and come up with a process that would assist universities in diagnosing students with mental health
disorders in an efficient manner if there is a relationship between the two.
**Methodology:**
We selected the Canadian dataset and narrowed our focus to only Canadian university students. This was done by
filtering (DEM_STDNT==1). Since there were a lot of drugs provided, we decided to only concentrate on
Cannabis and Alcohol which are very popular and widely available among university students. We started by doing
exploratory data analysis and found some interesting insights such as the relationship between recreational
Cannabis use and anxiety. From our EDA, we built a logistic regression model where the selection of predictors
were influenced by EDA. The process starts with students filling out a questionnaire form (shown below) which is
based on the predictors from our logistic regression model.
**Questionnaire:**
1. What is your gender?
2. How old are you?
3. Are you currently a healthcare professional (providing care to patients)?
4. Have you ever attempted to get a prescription from a physician for a medication that you did not need and
intended to misuse?
5. How often did you drink alcoholic beverages during the past 12 months?
6. Have you ever used Cannabis (non-medical, recreational, or illicit marijuana) and how often?
7. Have you ever used Cannabis (medical marijuana) and how often?
8. Have you ever had blackouts or flashbacks as a result of drug use?
9. Do you ever feel bad or guilty about your drug use?
10. Does your spouse (or parents) ever complain about your involvement with drugs?

The answers of our questionnaire form would act as the input of the model and that would be used to calculate the
accuracy through 5 or 10-fold cross validation. In our experiment, we obtained **70.73% accuracy** through 5-fold
cross validation which is excellent considering the time constraint. From these results, the university can take
actions and narrow down the diagnosis making the overall process much faster, promoting awareness through
workshops about mental health to targeted students, and facilitating the appropriate treatment to students.

There are a few concerns regarding accuracy especially because the mental health data refers to students being
informed about their disorders at any point in their life. There wasn’t enough data to deduce whether mental health
disorders promoted drug/alcohol consumption, or vice versa. Furthermore, the amount of analysis to deduce the
relationship among predictors was limited due to the time constraints and there is still room for deeper analyses in
this area. Next steps include, analysing new/stronger predictor variables and also designing a more efficient flow to
the diagnosis process after collaborating with key stakeholders such as the university and mental health specialists.
