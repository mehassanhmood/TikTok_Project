# TikTokClaimDetective: Extracting Claims and Opinions using ML
The aim of the project is to use machine learning to extract claims or propositions within TikTok videos and comments and classify each data point as a claim or opinion. 
To approach this task i will be using the PACE frame-work that is an accronym for a 4 stage approach Plan, Analyze, Construct and Execute.
## Plan :
1. Goal: To determine whether a video contains a claim or whther it offers an opinion.
2. Strategies utilized :
   1. Data Source : Gathered with in from the organization (first party) and provided as a csv.
   2. KPIs : Would depend on the insights covered via statistical inferences and mavhine learning algorithms and their performnace.
   3. Tools : Python, statsmodel, scipy, scikit-learn, Tableau and various others on need basis.
   4. Deliverables for Plan stage : Dataset scrubbed for EDA, visualizations, statistical model, regression analysis, and/or machine learning.
3. Deliverables :
   1. Findings:
      1. After looking at the dataset, the two variables that are most likely to help build a predictive model are claim_status and opinion_status. We can create a classification model to differentiate the two variables, as instructed from the employer.
      2. The mean is larger than the median, so the data is right-skewed. Therefore, it is recommended to consider applying a variable transformation, such as taking logarithms, prior to modeling.
   3. Python file : [Stage 1 Deliverable : Notebook](Exploring_data_1.ipynb)
## Analyze :
1. In this stage we will be covering the following processes:
   1. ETL (Extract, Transform, Load) as/if required.
   2. EDA (Exploratory Data Analysis) to uncover as much insights as possible.
   3. This stage also includes working with the stakeholders to create a subset of the insights discovered in the previous step. This subset will only include those insights that are to be pursued further.
2. Findings and Deliverables :
   1. Executive Summary : [Stage 2 Deliverabe: Summary File](EDA_ExecutiveSummary)
   2. Python File : [Stage 2 Deliverable : Notebook](2_EDA)
## Construct :
1. This stage includes the following processes :
   1. Deciding what insights to pursue.
   2. Statistical Analysis
   3. Regression Analysis
   4. Utilizing Machine Learning Algorithm.
2. Starting with Statistical Analysis our next step is to find out if there is any statistical difference betweem the mean of video views count of verified and un-verified accounds. We do this by finding the p-value and if this less than our threshold of 5% we will reject the null hypothesis.
   1. Eexecutive Summary : [Stage 3 Deliverables : Statistics Summary File](Stats_ExecutiveSummary)
   2. Python File : [Stage 3 Deliverables : Notebook](Stats_Analysis)
3. Earlier, we observed that if a user is verified, they are much more likely to post opinions. Since the end goal is to classify claims and opinions, it’s important to build a model that shows how to predict the behavior of the account type (verified) that tend to post more opinions. So, in this part of the project, we built a logistic regression model that predicts verified_status. 

