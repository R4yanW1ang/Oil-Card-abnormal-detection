# Oil-Card-abnormal-detection

Oil card cash-out is an illegal behavior in which the driver acquires money from the deposit of oil cards. In most of these cases, the man in charge of oiling will get 10% to 15% commission. This project used the desentisized data from a oil company to come up with an algorithm that automatically detect cards that could be potentially involved in cash-out. 
These are the steps of the projects:
1. Data exploratory analysis & Data Engineering (SQL)
2. Adding columns concern with abnormal oiling behaviors using aggregation (SQL)
3. Apply feature scaling, then use PCA to convert the dataframe to two-dimensional
4. Fit the data with Kmeans++ & Isolation Forest model, set the default cash-out ratio to 1:2000
5. Use the overlapping output from the two model as the final result
6. Save the model for future use
