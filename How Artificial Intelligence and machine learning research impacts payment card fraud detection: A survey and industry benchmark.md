# How Artificial Intelligence and machine learning research impacts payment card fraud detection: A survey and industry benchmark

https://www.researchgate.net/publication/328665645_How_Artificial_Intelligence_and_machine_learning_research_impacts_payment_card_fraud_detection_A_survey_and_industry_benchmark

This paper proposes a benchmark of published method, between 1990 and 2017, as if they were all implemented in an FMS (Fraud Management System) in 2017.

- Card Expenditure Volume and fraud both grow exponentially. However, in 2017, for the first time fraud grew more rapidly than CEV. Fraud vectors have until recently slowly evolved. Payments industry has tacitly accepted that the cost of fraud as an acceptable write-off cost of business. The fraud levels grew but were a disproportionately small portion of the bank profits.

**Major challenges in real-world fraud detection**
- Transparent decisions: Problem of ML is its opacity. Industry considers that it is only the timely understanding of new fraud vectors that will allow improved prevention methods to be put in place
- Cost of fraud detection to the payments industry: Most FMS produce a large volume of 𝐴𝑙𝑒𝑟𝑡𝐷 that must be matched against available and costly human review resource and so the issue of prioritization requires attention. a commercial decision must be made between these costs and the impact and savings by detecting fraud
- Lack of large-scale and sensitive real-world datasets: Researchers have reported that the exchange of ideas in fraud detection and specifically in payment card fraud detection is severely limited due to security and privacy concerns. 75% of the datasets are considered "small".
The data held on each transaction including the CHD, the cardholder and merchant is sensitive. 
Even data available to an FMS is partial:
  - A merchant: Only data of the transactions that have occurred in their firm
  - An issuer (customer's bank):  Only data on the transactions that have been undertaken on their issued card by the cardholder
  - An acquirer (merchant’s bank): Only transactional information from the merchant along with information they keep on their merchants
- Concept drift and disruptive industry technologies: The detection of fraud is nonstationary as fraud vectors change over time. An efficient FMS should be able to learn new fraud vectors

**Metrics**

Metrics:
- confusion matrix
- 𝐹-𝑠𝑐𝑜𝑟𝑒
- Receiver Operating Characteristic: how well the classifier is able to be specific and sensitive simultaneously
- Matthews Correlation Coefficient

A key metric is the number of alert in day, 𝐴𝑙𝑒𝑟𝑡𝐷: There is an operational cost for checking new alerts.
The practitioner metrics typically are
- 𝐴𝑙𝑒𝑟𝑡𝐷
- %fraud entity detected
- %amount saved following the first alerted transaction
- 𝐹𝑃𝑅
- TPR

Class imbalance
- Ratio of Genuine to Fraud (RGF) = P/N
- A/f = 𝐴𝑙𝑒𝑟𝑡𝐷∕𝑇𝑃′

Results are recalculated according to the an average ‘‘large issuer in 2017’’ standards


**Models**
Results are recalculated and tabulated in a consistent format using 𝐴𝑙𝑒𝑟𝑡𝐷 in Eq.6

three types of classifier: (1) Rules, (2) Supervised classifier, (3) Anomaly classifier

They grouped papers by methodology/ Type of model:
- Expert system (rule based models): Methods widely adopted throughout the payment industry. Easy to understand. However it does not adapt to new payment and criminal methods.
-Decision Tree: Easy to understand. DT method typically being sensitive to noise in the data. surveyed methods create a large number of rules each with many antecedents which makes their interpretation difficult.
- Supervised neural networks: Gave rather good results
- Unsupervised neural networks and clustering: Lack of data: perfect results + many clustering approaches are considered computationally intensive
- Bayesian network: Bayesian network methods provide no practical improvement in performance.
- Evolutionary computing: Rather good results, but high RPR 
- Hidden Markov Model (HMM): HMM methods generally lower in performance than other simpler methods
- Support vector machine (SVM): First SVM: 14
- Eclectic: They cover a range of differing classification techniques and many propose hybrid/ensemble methods making use of multiple classifiers.

Lot of differences between dataset:
- variation in the dataset size
- fraud imbalance
- dimensionality
- complexity

**Future directions:**
- data philanthropy by Mastercard
- possibility of using more complex data
- Area of improvement: The temporal and sequential nature of transactions is important as humans develop habitual behaviors, where patterns of expenditure on certain goods, shops, brands, amounts can be observed over a period. Fraud is typically carried out repeatedly using the same CHD/payment card until it is blocked. It is therefore important that these sequence frauds that occur over a time period are detected as early as possible. There are only a few methods that describe this issue and these use statistics that are aggregated over time to improve their performance. It is suggested that more advanced time series modelling approaches may yield better real-world performance.


**Conclusion:**
- The top-ranking method uses human written rules, three methods are based on neural networks, two use decision tree/random forest and one uses a semi-supervised method based on cluster profiling. 
- While neural networks dominate as a classifier, there is not sufficient evidence to make a firm conclusion.
- impact on the payment card industry has been minimal
- academic work in this area is difficult and marginalized in terms of funding
- methods provide limited improvements over the earlier works
