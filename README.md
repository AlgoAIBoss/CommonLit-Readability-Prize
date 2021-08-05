# AutoInland-Vehicle-Insurance-Claim-Challenge

## Introduction

| Title | Text |
| ------ | ------ |
| Intro | In 2021 during three months, Nigerian car insurance company held a competition in African data science competition platform called `Zindi`. In this competition the organizer wanted to know _wheter or not a client will submit a vehicle insurance claim in the next 3 months_. In this competition 600+ competitors participated. |
| Data | The dataset consisted of Train == 12000, Test == 1200, Sample_Submition, Nigerian_State_LGA_Name. |
| Metrics | F1_score for evaluating our algorithm.|
| ML Task | Binary Classification task.|


## Problems

1. The dataset was unbalanced.
2. It had missing values in some columns.
3. `Age` column had outliers.
4. Despite distinct IDs duplicated rows existed.
5. State and LGA column names were incorrect.
6. Some duplicated rows had different target.


## Solved

1. Used RandomOverSampler algorithm to oversample the minority class.
2. I tried to impute NaNs with Iterative-Imputer and KNN-Imputer.
3. I used absolute value of Age to fix negative values.
4. When I deleted duplicated values I got lower F1_score in public LB so I did not fix it. But in private LB I found out I should have deleted it.
5. Interestingly I used Nigerian_State_LGA_Name dataset to correct Names in LGA and State.
6. I again did not fix duplicated rows with different targets.


## Unsolved

1. Did not pay attention to scaling, transforming, feature selection, which led to overfitting.
2. rather than following ML rules I followed what public LB told me about duplicated rows.
3. I did not use Stacking or boosting from ensembles efficiently.


## Algorithms Used

1. CatBoost for  binary Classification.
2. Iterative-Imputer with ExtraTrees for Imputing Missing Values by Label-Encoding the categorical dtype.
3. RandomOverSampler for Over-Sampling minority class.
4. Others.




<br/>

<h3> 🛠 &nbsp;Tech Tools</h3>

- :space_invader:
  ![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
  
- ⚙️ &nbsp;
  ![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)
  ![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)
- 💻 &nbsp;
  ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
  


<br/>

