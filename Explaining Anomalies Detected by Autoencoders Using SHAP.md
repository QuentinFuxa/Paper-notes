# Explaining Anomalies Detected by Autoencoders Using SHAP

This paper from University of the Negev researchers highlights a solution to explain Autoencoder error.



They used SHapley Additive exPlanations (SHAP) with an autoencoder.

SHapley Additive exPlanations (SHAP) is a a game theory-based framework which  has the capacity of explaining various supervised learning models.

One way of explaining is using an interpretable approximation of the original model
Other solutions:
- LIME: Model agnostic method
- DeepLIFT: back propagating the contributions of all neurons in the network
  to the input features.

SHAP values interpret the impact of having a certain value for a given feature in comparison to the prediction we'd make if that feature took some baseline value.
Shapley Value is a solution concept of fairly distributing both gains and costs to several actors working in coalition.
- Contribution Margin=Sales Revenue − Variable Costs
- Shapely value = average expected [marginal contribution](https://www.investopedia.com/terms/c/contributionmargin.asp) of one player after all possible combinations have been considered.


In the reconstruction error of the autoencoder, they:
1- Extract the topMfeatures list. 
2- Assign the weights of the model associated to the input to 0 -> Not interested in knowing the effect of the feature on its reconstruction. 
3- For each feature of the topMfeatures list, they extract the shapvalues associated.  Among these shapvalues, they extract the shapvalues contributing, and the shapvalues offsetting the the anomaly.



The example they took is to try to detect drug abuse, using a prescription database. They are able, for a given predicted value (drug amount), to explain values contributing and offsetting, with the amount of contribution too.


On the interquartile range anomalies, experts labeled out of the 114 anomalies 32 as "uninteresting", and the rest as "should be inspected".


To reduce False Positive rate, they checked if there is a feature intersection *i.e.* if there is an intersection between one feature
that contributed to the anomaly which is also a feature.
