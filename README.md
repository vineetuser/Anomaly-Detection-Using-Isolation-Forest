1. Data Preparation:

2. Model Training: The IsolationForest model is initialized with a specified contamination parameter (indicating the expected proportion of anomalies) and a random state for    reproducibility.
   The model is then fitted on the feature data (df[['value']]), and predictions are made. The model returns 1 for normal points and -1 for anomalies.

3. Result Interpretation:
   Anomalies are identified by filtering the DataFrame where the prediction is -1.
