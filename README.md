# Credit Card Default Prediction

**Classification Prediction with Imbalanced Target**

**Summary**

The goal of this project was to design predictive binary classification models to predict whether credit card account holders will default on their payments in the next month.  The models address the imbalance in the target variable.  Gradient Boosting and neural network models are highlighted.  The paper and presentation walk through the data understanding and preparation, different models tested, methodology, evaluation and anticipated follow-up steps to the project.  

**Tools**
* Scikit-learn 
* Keras
* Seaborn
* Matplotlib
* Numpy
* Pandas
* Scipy

**Data**

http://archive.ics.uci.edu/ml 

**Models / Methods / Metrics**
* Gradient Boosting Classification 
* Artificial Neural Network
* Random Forest
* Principal Component Analysis
* Log-Transformation and Scaling
* Recall, Log-Loss and Binary Crossentropy Loss

**Results**

The Gradient Boosting Classification model had the best Recall and Log Loss Error scores.  62.43% of the actual default accounts were labeled as true positives.  The Log Loss Error was .4545.  The Artificial Neural Network had a Recall score of .6989 and a binary crossentropy loss of .5958.  These scores resulted from addressing the imbalanced target variable.

## Project Preview

### Exploratory Data Analysis

The EDA shows there are distinctions between the default records and the non-default records.

![ECD](/images/credit card/ECD.PNG)

![PAY1](/images/credit card/Pay1.PNG)

![MEAN](/images/credit card/mean.PNG)

### Principal Component Analysis

PCA was implemented because of multicollinearity between groups of input variables.

![PCA](/images/credit card/PCA.PNG)

### Modeling

The imbalanced target variable was addressed by using predicted probabilities for positive outcome based on best classification threshold, and for the Artificial Neural Network, by weighting the binary target classes.


### Evaluation

**Gradient Boosting Classification, Logistic Regression and Random Forest Models:**

![RESULTS1](/images/credit card/Results1.PNG)

**Artificial Neural Networks:**

![ANNRESULTS](/images/credit card/ResultsANN.PNG)


**Notebooks**

1_EDA_Prep
This notebook includes the EDA, data preparation, and PCA.

2_Test_Subsets_of_Features
This notebook tests for best subsets of features with a logistic regression model.

3_Log_Regress_Model
This notebook includes the Logistic Regression Model’s model evaluation and selection and metric evaluation.

4_LASSO_Log_Reg_Model
This notebook includes the LASSO Logistic Regression Model’s model evaluation and selection and metric evaluation.

5_GBC_Model
This notebook includes the Gradient Boosting Classification Model’s model evaluation and selection and metric evaluation.

6_RandomForest_Model
This notebook includes the Random Forest Model’s model evaluation and selection and metric evaluation.

7_Neural_Network_Models
This notebook includes the Neural Network Models’ model evaluation and selection and metric evaluation.
