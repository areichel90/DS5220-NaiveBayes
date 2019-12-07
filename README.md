# Exploring Naive Bayes Under Adverse Conditions
### Spring '19 DS5220 Group Project
### Authors: Andrew Reichel, Smruthi Ramesh, Ross Marino, Adam Ribaudo

## Project Description

The Naive Bayes classification method is a generative model known to perform well even when its underlying assumption of conditional independence between predictors given a particular class is broken. That being the case, conditions exist where the underlying data breaks this assumption to such an extent that class assignments change and predictions are no longer useful. This project explores these and other thresholds that outline when Naive Bayes performs worse than other models that make fewer or different assumptions about the data. 

The following adverse data conditions were explored as part of this project:
* Dependence between variables (breaking the assumption of conditional independence)
* High number of predictors and low number of observations (as found in biomedical data)
* Non-gaussian distributions (as found in manufacturing data) 
* Missing values (as found in survey data)
* High class imbalance (as found in text classification data)
* Combinations of the above conditions

## Summary of Findings

This project was inspired by the frequent reference to Naive Bayes’ “surprising” abilities. Our analysis attempted to unpack what makes Naive Bayes’ predictive capabilities so surprising. What we learned is that there are several features that make Naive Bayes robust to certain data quality issues. For instance, its presumption of conditional independence between predictors means that useful predictions can be made even when specific combinations of predictor values are not present in the data. When the data is corrected for class imbalance, Naive Bayes also has surprisingly good recall compared to discriminative classifiers.

That being said, it also became clear that Naive Bayes had certain limitations that in many cases made other models more preferred. Data with a high degree of predictor dependence proved to be especially problematic. While our section on Dependence Between Variables showed that dependence is not always problematic, a researcher would not be able to determine this without having access to the true underlying model generating the data.

In addition, Naive Bayes uses the distribution of predictors to make predictions, so as we imputed missing values or oversampled for classes with a low number of observations, we artificially lowered the variance of the predictors. This gave us a tighter decision boundary which would not generalize well to new data.

Ultimately, we judge that Naive Bayes is a simple, efficient model that provides useful predictions in many cases despite underlying data quality issues. For these reasons, our recommendation would be to use it as a starting baseline before evaluating more complicated models.
	
## References

- Zhang, Harry. (2004). The Optimality of Naive Bayes. Proceedings of the Seventeenth International Florida Artificial Intelligence Research Society Conference, FLAIRS 2004. 2. 

- Rennie et al. (2003). Tackling the Poor Assumptions of Naive Bayes Text Classifiers. Proceedings of the Twentieth International Conference on Machine Learning (ICML-2003), Washington DC, 2003.

- Kotzias et. al,. (2015) From Group to Individual Labels using Deep Features. KDD ‘15. Proceedings of the 21th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining.



