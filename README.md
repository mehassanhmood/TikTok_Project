# TikTokClaimDetective: Extracting Claims and Opinions using ML
The aim of the project is to use machine learning to extract claims or propositions within TikTok videos and comments and classify each data point as a claim or opinion. 
To approach this task i will be using the PACE frame-work that is an accronym for a 4 stage approach Plan, Analyze, Construct and Execute.
## Plan :
1. Goal: To determine whether a video contains a claim or whther it offers an opinion.
2. Strategies utilized :
   1. Data Source : Gathered with in from the organization (first party) and provided as a csv.
   2. KPIs : Would depend on the insights covered via statistical inferences and mavhine learning algorithms and their performnace.
   3. Tools : Python, statsmodel, scipy, scikit-learn and various others on need basis.
   4. Deliverables for Plan stage : Dataset scrubbed for EDA, visualizations, statistical model, regression analysis, and/or machine learning.
3. Deliverables :
   1. Findings:
      1. After looking at the dataset, the two variables that are most likely to help build a predictive model are claim_status and opinion_status. We can create a classification model to differentiate the two variables, as instructed from the employer.
      2. The mean is larger than the median, so the data is right-skewed. Therefore, it is recommended to consider applying a variable transformation, such as taking logarithms, prior to modeling.
   3. Python file : [Stage 1 Deliverable](Exploring_data_1.ipynb)
## Analyze :
In this stage we will be covering the following processes:
   1. ETL (as/if required).
   2. EDA (Exploratory Data Analysis) to uncover as much insights as possible.
   3. This stage also includes working with the stakeholders to create a subset of the insights discovered in the previous step. This subset will only include those insights that are to be pursued further.
