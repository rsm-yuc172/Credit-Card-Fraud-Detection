# Credit-Card-Fraud-Detection
![image](https://github.com/user-attachments/assets/fd5df4ae-8bdb-4a89-bc5e-8873fcc1079d)  
In this report, we aimed to capture credit card fraud transactions by implementing data-driven machine learning techniques. The data of 97,852 credit card transaction data encompasses 95,805 non-fraudulent transactions and 2,047 fraudulent transactions. 

ML Pipeline:

Training Data: card transactions.csv
1. Data Exploration: EDA.ipynb
2. Data Cleaning: Data_Cleaning.ipynb
3. Data Engineering: feature_selection.ipynb
4. model selection/model tuning: modeling.ipynb

To briefly summarize the project, by implementing the LightGBM model, the overall average accuracy is 0.74 for training data, 0.74 for testing data, and 0.53 for out-of-time data. From this approach, we selected FDR@4% as our cutoff, which will be capable of capturing 62% of the fraud transaction that accounts for approximately $40.5 million dollars of savings per year.
