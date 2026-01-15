## Fraud Detection 

Fraudulent behavior can be seen across many different fields such as e-commerce, healthcare, payment and banking systems. Fraud is a billion-dollar business and it is increasing every year. The PwC global economic crime survey of 2018 [1] found that half (49 percent) of the 7,200 companies they surveyed had experienced fraud of some kind.

Even if fraud seems to be scary for businesses it can be detected using intelligent systems such as rules engines or machine learning. 
Most people here in Kaggle are familier with machine learning but for rule engines here is a quick information. 
A rules engine is a software system that executes one or more business rules in a runtime production environment. 
These rules are generally written by domain experts for transferring the knowledge of the problem to the rules engine and from there to production. 
Two rules examples for fraud detection would be limiting the number of transactions in a time period (velocity rules), denying the transactions which come from previously known fraudulent IP's and/or domains.


Fraud data will be imbalanced like you see in the plot below and from the count of instances. 
To balance the dataset one can perform oversample or undersample techniques. 
Oversampling is increasing the number of the minority class by generating instances from the minority class . 
Undersampling is reducing the number of instances in the majority class by selecting random points from it to where it is equal with the minority class. 
Both operations have some risks: Oversample will create copies or similar data points which sometimes would not be helpful for the case of fraud detection because fraudulent transactions may vary. 
Undersampling means that we lost data points thus information. We will perform an oversampled technique called SMOTE (Synthetic Minority Over-sampling Technique).
SMOTE will create new data points from minority class using the neighbour instances so generated samples are not exact copies but they are similar to instances we have.
