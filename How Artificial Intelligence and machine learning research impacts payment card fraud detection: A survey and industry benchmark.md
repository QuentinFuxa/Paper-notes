# How Artificial Intelligence and machine learning research impacts payment card fraud detection: A survey and industry benchmark

This paper proposes a benchmark of published method, between 1990 and 2017, as if they were all implemented in an FMS in 2017.
fraud vectors have until recently slowly evolved
payments industry tacitly accepting that the cost of fraud as an acceptable write-off cost of business. The fraud
levels grew but were a disproportionately small portion of the bank profits.

FMS = Fraud Management System

Comprehensible classifiers are essential to guide them towards a particular type of investigation and towards creating 
prevention that is more effective.

A key metric is the number of alert in day, 𝐴𝑙𝑒𝑟𝑡𝐷: There is an operational cost for such a process.



The data held on each transaction including the CHD, the cardholder and merchant is sensitive. Lack of data available for researchers.
Even data available to an FMS is partial:
- A merchant : Only data of the transactions that have occured in their firm
- An issuer (customer's bank):  Only data on the transactions that have been undertaken on their issued card by the cardholder
- An acquirer (merchant’s bank): Only transactional information from the merchant along with information they keep on their merchants

three types of classifier: (1) Rules, (2) Supervised classifier, (3) Anomaly classifier

Metrics:
- confusion matrix
- 𝐹-𝑠𝑐𝑜𝑟𝑒
- Receiver Operating Characteristic: how well the classifier is able to be specific and sensitive simultaneously
- Matthews Correlation Coefficient

The practitioner metrics typically are
- 𝐴𝑙𝑒𝑟𝑡𝐷
- %fraud entity detected
- %amount saved following the first alerted transaction
- 𝐹𝑃𝑅
- TPR

Class imbalance
- Ratio of Genuine to Fraud (RGF) = P/N
- A/f = 𝐴𝑙𝑒𝑟𝑡𝐷∕𝑇𝑃′

They grouped papers by methodology/ Type of model:
- Expert system/Decision Tree
- Supervised neural networks
- Unsupervised neural networks
- Unsupervised neural networks and clustering
- Bayesian network
- Evolutionary computing
- Hideen Markov Model (HMM)
- Support vector machine (SVM)
- Eclectic

Lot of differences:
- variation in the dataset size
- fraud imbalance
- dimensionality
- complexity

Fraud is typically carried out repeatedly using the same CHD/payment card until it is blocked. It is therefore important that these sequence frauds that occur over a time period are detected as early as possible. There are only a few methods that describe this issue and these use statistics that are aggregated over time to improve their performance. It is suggested that more advanced time series modelling approaches may yield better real-world performance.


Future directions:
- data philanthropy by Mastercard
- possibility of using more complex data

Improving classifier performance:
- Does deep learning has any advantages in the fraud detection domain?
- Area of improvement: The temporal and sequential nature of transactions is important as humans develop habitual behaviours, where patterns of expenditure on certain goods, shops, brands, amounts can be observed over a period.

Conclusion:
- The top-ranking method uses human written rules, three methods are based on neural networks, two use decision tree/random forest and one uses a semi-supervised method based on cluster profiling. 
- While neural etworks dominate as a classifier, there is not sufficient evidence to make a firm conclusion.
- impact on the payment card industry has been minimal
- academic work in this area is difficult and marginalised in terms of funding
- methods provide limited improvements over the earlier works

