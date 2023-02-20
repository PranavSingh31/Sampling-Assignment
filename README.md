# Sampling Assignment

We employed sampling strategies on a credit card fraud detection dataset in this Python code, then applied multiple ML models to the dataset to see which model-sampling strategy combo gave us the best accuracy.

The following five sampling techniques were employed:
1. Random Under Sampler (Sampling 1)
2. Random Over Sampler (Sampling 2)
3. TOMEK links (Sampling 3)
4. Near Miss (Sampling 4)
5. SMOTE (Sampling 5)

The following formula was used to calculate the sample size: 
![image](https://user-images.githubusercontent.com/76558062/220184739-cfdc6f01-6ed3-48c5-8486-7a21509d48eb.png)

Z-score taken as 1.96 for the 95% confidence interval, P taken as 0.5 for a balanced dataset, Margin of Error taken as 0.1 for a sample size of 1000.

For the sampled dataset, the following 5 models were used:
1. Logistic Regression (Model 1)
2. Extra Tree Classifier (Model 2)
3. Random Forest Classifier (Model 3)
4. Support Vector Classifier (SVC) (Model 4)
5. Decision Tree Classifier (Model 5)

The following results were obtained after running the code:
(The decimals represents Accuracy Score)
![image](https://user-images.githubusercontent.com/76558062/220185643-e7df0ec4-c456-40a1-8beb-ec339f3e9341.png)

Random Over Sampler, SMOTE and TOMEK links gave best result (that is 99.35%) when applied on Random Forest Classifier, Support Vector Classifier, Extra Tree Classifier.
