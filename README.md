# Credit_Risk_Analysis

## Purpose of Analysis
Credit risk is an unherently unbalanced classification problem, as good loans easily outnumber risky loans. We are tasked to using a credit card credit dataset from LendingClub, a peer-to-peer lending services company, to use machine learning to predict credit risk. Management believes that this will provide a quicker and more reliable loan experience as well as lead to a more accurate identification of candidates for laons, which will in turn, lead to lower default rates. We are to build an evaluate several machine learning models or algorithms to predict credit risk.

## Results

##### Naive Random Oversampling 
![Screenshot 2022-11-26 230911](https://user-images.githubusercontent.com/107603065/204123617-8f8f619f-0fa7-4f4e-8ad9-14cffce4ab76.png)

- Balanced Accuracy = 0.6515938052705158
- Precision: high-risk = 0.01 & low-risk = 1.00
- Recall: high-risk = 0.62 & low-risk = 0.68

##### SMOTE Oversampling
![Screenshot 2022-11-26 231620](https://user-images.githubusercontent.com/107603065/204123806-fbf1ca1f-2faa-45d0-a768-8f03c592111c.png)

- Balanced Accuracy = 0.6241876870888075
- Precision: high-risk = 0.01 & low-risk = 1.00 
- Recall: high-risk = 0.59 & low-risk = 0.66 

##### Undersampling
![Screenshot 2022-11-26 231737](https://user-images.githubusercontent.com/107603065/204123841-e37ea2b6-38b4-4141-ba32-5cbedbb0dbec.png)

- Balanced Accuracy = 0.6241876870888075
- Precision: high-risk = 0.01 & low-risk = 1.00
- Recall: high-risk = 0.60 & low-risk = 0.43

##### Combination (Over & Under) Sampling
![Screenshot 2022-11-26 231924](https://user-images.githubusercontent.com/107603065/204123898-609a8180-8903-4f7c-9001-4de6d5fbc52f.png)

- Balanced Accuracy = 0.5160196365189295
- Precision: high-risk = 0.01 & low-risk = 1.00
- Recall: high-risk = 0.70 & low-risk = 0.58


##### Balanced Random Forest Classifier
![Screenshot 2022-11-26 232025](https://user-images.githubusercontent.com/107603065/204123918-9995489a-c06a-4673-8804-13bf968c86f7.png)

- Balanced Accuracy = 0.7885466545953005
- Precision: high-risk = 0.03 & low-risk = 1.00
- Recall: high-risk = 0.70 & low-risk = 0.87

##### Easy Ensemble AdaBoost Classifier
![Screenshot 2022-11-26 232116](https://user-images.githubusercontent.com/107603065/204123936-1a117878-8b37-41fd-be93-e3cd89b35ad8.png)

- Balanced Accuracy = 0.9316600714093861
- Precision: high-risk = 0.09 & low-risk = 1.00
- Recall: high-risk = 0.92 & low-risk = 0.94

## Summary

The performance of a linear regression model is measured based on the difference between its predicted and actual values. One way of validating model's performance is its *accuracy score* in which is calculated as the percentage of predictions that are correct within the model. Another method would be measuring *precision*, also known as positve predictive value. It is a measure of how reliable positive classification is. Another way top assess a model's performance is called *sensitivity* also known as recall. It is a measure of how amny values were correctly true? The appropriate method to use would depend on the scenario. The values evaluated on their performance are between 0 and 1, with values closer to 1 being the more reliable model. Based upon this information, the Easy Ensemble AdaBoost Classifier would be the best model to conduct this evaluation with a 93% accuracy score, recall score at 0.92 and 0.94 respectively. 
