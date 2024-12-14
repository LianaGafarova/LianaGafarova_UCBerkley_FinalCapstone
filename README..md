### Leveraging Applicant Information to Enhance Credit Decisioning for Fintech Companies with FICO Score


**Liana Gafarova**

#### Executive summary
Credit scoring is a critical tool in financial decision-making, helping lenders make informed decisions while enabling consumers to access credit responsibly. 

Developed in 1989 by Fair Isaac Corporation (FICO), FICO Score is one of the first standardized credit scoring model, which became the industry benchmark due to its innovative approach to evaluating creditworthiness.

Several years ago a few fintech companies broke the news claiming that they are not using FICO score for their underwriting due to FICO Score inferiority. I decided to build a loan default prediction model based on Lending Club data (one of the biggest B2B lending fintech companies) and compare performance to the FICO score.


#### Rationale
As consultants, we try to improve clients' lending practices by showcasing the value of combining several tools while building strategies for underwriting and credit management. 

#### Research Question
The main objectives of this research are to:
* Determine the key factors that influence a consumer's credit risk level based on the Lending Club data (custom score)
* Compare the custom Lending Club model to the Broad based FICO Score (consortium model)

#### Data Sources
Lending club loan data from Kaggle (https://www.kaggle.com/datasets/wordsforthewise/lending-club/data?select=accepted_2007_to_2018Q4.csv.gz).

#### Methodology
Classification techniques were employed to determine the consumer credit risk level (Logistic Regression, SVC, KNN, Decision Tree)

#### Results
One of the objectives of the project was to develop a model to predict consumer credit risk based on the observed characteristics of Lending Club applicants. 
As the result of the analysis we developed several models (KNN, Logistic regression, Decision Tree and SVM) to identify factors which affect consumers' risk level. We used accuracy, precision, recall, F1 metrics and ROC-AUC curve to identify the best model.

Logistic regression outperformed the other models in terms of performance metrics and runtime. 

As we analyzed coefficients of the logistic regression build on Lending Club data, the following groups of consumers tend to have higher credit risk:
* Consumers assigned high risk grade (by credit bureau)
* Consumers with higher installment lines
* Consumers who Rent
* Consumers who were a part of debt settlement program
* Consumers who have more accounts
* Consumers who apply for longer term loan
* Consumers with higher utilization on revolving trades
* Consumer with higher number of inquiries in the last 6 months
* Consumers with lower payments

Comparison of the Lending Club custom model with the FICO score (broad based consortium model) demonstrated similar performance, with FICO score slightly outperforming the custom Lending club model both in rank ordering and performance metrics.

Based on the results outlined above, it is recommended to use the custom built model with the FICO scores for credit decisioning, especially for swap-in opportunities.


#### Next steps
One of the logical extensions of the analysis would be a dual score strategy, which utilizes both scores as separate tools in credit assessment.

#### Outline of project

- Jupyter Notebook: https://github.com/LianaGafarova/LianaGafarova_Capstone_1stSubmission/blob/main/Part%201_Capstone.ipynb


##### Contact and Further Information
E-mail: lianamks@gmail.com
