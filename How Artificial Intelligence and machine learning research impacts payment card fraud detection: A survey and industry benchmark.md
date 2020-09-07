# How Artificial Intelligence and machine learning research impacts payment card fraud detection: A survey and industry benchmark

This paper proposes a benchmark of published method.

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


