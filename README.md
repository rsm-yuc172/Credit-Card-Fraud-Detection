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


Detailed Sequence: 
The machine learning pipeline began with a thorough data cleaning phase where outliers were identified and removed, and missing data points were imputed through various methods, ensuring robustness in the dataset. Then, we generate new features that could potentially indicate fraudulent behavior based on our domain knowledge on CNP fraud. Feature selection was crucial to refining the model, employing both filtering and wrapper methods to determine the top 20 most crucial features. This was followed by testing several models including Logistic Regression, Decision Trees, Random Forests, LightGBM, and Neural Networks. LightGBM was ultimately selected due to its high performance, particularly OOT validation, which is critical for assessing how the model will perform in real-world scenarios. The model was tuned with parameters like number of trees (n_estimators=30), maximum depth (default), number of leaves (num_leaves=4), and learning rate (0.1) to balance complexity and generalization capabilities.
The final outcomes included a detailed performance evaluation of the LightGBM model and financial analysis to determine the optimal fraud detection cutoff, balancing the detection of fraud and minimizing false positives. At a 4% cutoff, the model achieved a Fraud Detection Rate (FDR) of 62% in OOT data, equating to substantial annual savings estimated at around $40.5 million, considering both the detection benefits and costs associated with false positives. Further improvements could include exploring additional data sources, refining feature engineering, or experimenting with alternative machine learning models to enhance predictive accuracy and reduce false positives.
