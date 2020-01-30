
# Kaggle-DonorsChoose-NLP-LightGBM

## Competition

DonorsChoose.org receives hundreds of thousands of project proposals each year for classroom projects in need of funding. Right now, many volunteers is needed to manually screen each submission before it's approved to be posted on the DonorsChoose.org website.
The goal of the competition is to predict whether a DonorsChoose.org project proposal submitted by a teacher will be approved, using the text of project descriptions as well as additional metadata about the project, teacher, and school. DonorsChoose.org can then use this information to identify projects most likely to need further review before approval.
Our goal here is to generate the numerical, categorical and rich text features that can be mined from the essay and resource request data. The hypothesis is that certain features mined such can be strong predictors of the binary outcome of whether an application will be accepted or not.

## Process Overview

![1574100207862](https://github.com/guptapiyush340/Kaggle-DonorsChoose-NLP-LightGBM/blob/master/1.png)

### Data Understanding

We have 3 datasets namely, Train (the training set), Test (the testing set), and Resources (items requested along with each application or proposal).

![1574100207862](https://github.com/guptapiyush340/Kaggle-DonorsChoose-NLP-LightGBM/blob/master/2.png)

### Feature Engineering and Text Analysis

Using all the features as it is rarely useful in data mining. To make this features more informative, we performed a range of feature engineering steps and performed text analysis on the essays and title of essays.

![1574100207862](![1574100207862](https://github.com/guptapiyush340/Kaggle-DonorsChoose-NLP-LightGBM/blob/master/3.png))

### Data Mining

**We experimented with multiple prediction algorithms**

1. Random Forest
2. SVM
3. [Boosting](https://github.com/guptapiyush340/Kaggle-DonorsChoose-NLP-LightGBM/blob/master/PredictiveDonorsCollated.ipynb)


![1574100207862](![1574100207862](https://github.com/guptapiyush340/Kaggle-DonorsChoose-NLP-LightGBM/blob/master/4.png))


### Prediction Performance

Based on the important features, we then implemented stacked model of LightGBM and CatBoost. Their comparative performance with Kaggle Leadership board is reported in the graph below.

![1574100207862](![1574100207862](https://github.com/guptapiyush340/Kaggle-DonorsChoose-NLP-LightGBM/blob/master/5.png))
