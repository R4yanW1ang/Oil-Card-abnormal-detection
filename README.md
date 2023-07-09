# Oil-Card-abnormal-detection
A Machine Learning project aiming at detecting abnormal gas card usage behavior (cash-out) using K-means &amp; Isolation Forest.
Oil card cash-out is an illegal behavior in which the driver acquires money from the deposit of oil cards. In most cases, the man in charge of oiling will get a 10% to 15% commission. This project used the desensitized data from an oil company to come up with an algorithm that automatically detects cards that could be potentially involved in cash-out. 
These are the steps of the projects:
1. ETL in Hive database for data extraction and pre-processing
2. Data exploratory analysis & Data Engineering (SQL)
3. Feature Engineering: add concerned variables that could be related to abnormal oiling behaviors (SQL)
4. Apply feature scaling by using PCA to convert the data frame to lower dimensions
5. Fit the data with Kmeans++ & Isolation Forest model, set the default cash-out ratio to 1:2000
6. Use grid search for hyperparameter tuning
7. Use the overlapping output from the two models as the final result
8. Save the model for future use
9. Set up the code scheduling to run the model once a month
