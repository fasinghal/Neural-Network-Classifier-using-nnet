# Predicting-the-Employees-Salary--Nnet
CS6375 Machine Learning Final Project  

Predicting an Employee’s wage – A comparison between Logistic Regression and Neural Networks

Falak Singhal
The University of Texas at
Dallas, USA
fxs161530@utdallas.edu

Melvin James
The University of Texas at
Dallas, USA
mxj162130@utdallas.edu

Vidya Sri Mani
The University of Texas at
Dallas
vxm163230@utdallas.edu

Abstract
The aim of this project is to predict whether a given employee’s salary will be lesser than or greater that 50K. A given person’s salary depends on various factor’s such as his location, educational qualification, age., The project uses two models, namely Logistic Regression and Neural Networks to classify the data (Adult data set) and use them to predict the salary of a new employee. The report provides a comparative study of the results. This project is completed using R.

Keywords: Logistic Regression, Neural Networks, classification

Dataset description
This project uses the Adult dataset to train its models. “Adult” Dataset, also known as “Census Income” dataset. This data was extracted from the census bureau database found at http://www.census.gov/ftp/pub/DES/www/welcome.html.

Fitting the Model
Cross Validation : Cross validation, popularly known as rotation estimation is a model validation technique for assessing how the results of a statistical analysis will generalize to an independent data set. A part of the complete dataset is removed for testing. Cross validation refers to the idea of splitting data as training and testing data. The project uses 70% of the total number of observations for training purposes and the remaining 30% to test the data.

Logistic Regression : Logistic Regression is a classification algorithm for fitting the regression curve, y=f(x), where y is a categorical variable. This algorithm predicts y, given a set of predictors, x.
y = [exp(b0 + b1x)] / [1 + exp(b0 + b1x)]. Logistic regression fits b0 and b1, the regression coefficients. The glm() function is used to do generalized linear models. Logistic Regression can be used, when we wish to predict a discrete variable, in this case, if the employee’s wage is greater that 50K (represented as 1) or less than 50K (which we represent as 0), given a set of independent variables. R provides support to fit a logistic regression model. The glm() function is used for the fitting process.

Neural Network
Neural Networks are used to identify non-linear patterns. Non-linear pattherns are those where oneto-one relationship between input and output is not present.Predicting an Employee’s wage – A comparison between Logistic Regression and Neural Networks
Neural networks work on the principle of identifying patterns between combinations of the input and the given output. Prediction using Neural network in R requires the nnet Package.

ROC and AUC Analysis of fitted Models
The ROC Curve or Receiver Operating Characteristics curve is used estimate the performance of the Logistic Regression Model. It summarizes the model’s performance by determining the tradeoff between true positives and false positive rate. The ROC curve summarizes the predictive capability

Accuracy of the two models
Logistic Regression ~ 85 %
Neural Network ~ 88 %
