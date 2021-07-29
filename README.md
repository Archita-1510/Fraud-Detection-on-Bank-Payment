# Fraud-Detection-on-Bank-Payment

Team Members
1. Archita Mukhopadhyay
2. Anushi Sharma
3. Rashmi Chindalia
4. Palak Goyal

Domain: Crime, Banking

Objective: To predict whether a transaction can be flagged fraud or not

Data set: https://www.kaggle.com/ealaxi/banksim1

Details: BankSim is an agent-based simulator of bank payments based on a sample of aggregated transactional data provided by a bank in Spain. The main purpose of BankSim is the generation of synthetic data that can be used for fraud detection research. Statistical and a Social Network Analysis (SNA) of relations between merchants and customers were used. BankSim was ran for 180 steps (approx. six months), several times and calibrated the parameters in order to obtain a distribution that get close enough to be reliable for testing. Then several log files were collected and the most accurate ones were selected. Thieves were injected that aim to steal an average of three cards per step and perform about two fraudulent transactions per day. 594643 records were produced in total where 587443 are normal payments and 7200 fraudulent transactions. Since this is a randomised simulation the values are of course not identical to original data. (Real data can not be used as that is violation of customer privacy) 

We plan on answering the following:
1. Does gender have anything to do with being a target for fraud?
2. Does age matter in this case?
3. Is there any particular category (or categories) of purchase where we have a significantly high percentage of fraud?
4. Customer to merchant relation matters?
5. When should the bank reach out to the customer to see the transaction was done by them or was it a fraud?

Further, using all the information that we have been provided with, we would like to predict whether a transaction can be flagged fraud or not

to get a statistical answer as to which variables matter in the prediction of fraud, we use simple correlation coefficient and chi square test of independence

after working throught the eda, modelling came under question
in this case, our first step was to use logistic regression, even though there is a high imbalance in the data set, that can be manipulated using different cut off points for logistic regression (which is 0.5 by default)
after that we try balancing the data set by using under sampling, over sampling and smote and then using different models to judge which works the best
further we use precision, recall, accuracy to judge which model is best suited for the purpose


