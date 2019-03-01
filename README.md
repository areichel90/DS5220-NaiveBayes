# DS5220-NaiveBayes
Spring '19 DS5220 Group Project

Project Proposal - Naive People Figuring out Naive Bayes
Authors: ...

Description of Problems
Summary:
How robust is Naive Bayes to data quality issues that we see in real life?
Individual Problems
How independent do the features actually need to be to produce decent results?
Domain: Real Estate
How does Naive Bayes perform at varying combinations of number of predictors compared to number of observations?
Domain: Biomedical (high number of predictors)
As part of this, measure computational performance as compared to other methods
How does naive Bayes perform when presuming varying distributions and applying it to data generated using varying distributions? Use histogram of data vs. Normal? 
Domain: Manufacturing defects (non-normal distribution of defects)
How robust is Naive Bayes to missing data?
Domain: Survey data
How robust is Naive Bayes to class imbalance?
Domain: Web conversions
Final Problem: Performance under worst case scenario for the above problems: missing data, class imbalance, wrong distribution, collinear data
Summary of Data
We’ll produce simulated data that demonstrates each of the problems described above. 
Missing values
High number of predictors and low number of observations
Underlying Models
Low to high polynomial functions
Interactions
Distributions of predictors
Varying degrees of Multicollinearity
Combination of continuous and categorical predictors 
Methods
Simulate data sets for each question
EG For collinearity we will create multiple data sets that have a range of collinearity between the predictors being generated
For each question we will have a data sets with a range of faultiness which corresponds to the question
Vary the amount of covariance between predictors
Baseline-- QDA or Logistic regression
Zero Rule - Majority class (generally better than random classifier)
Random classifier 
Cross Validation of models
Preliminary Results
Generate some simulated data, run it once
	
References
Git hub url: https://github.com/areichel90/DS5220-NaiveBayes.git


