# Exploratory data analysis (EDA)

## Haberman Cancer Survival dataset

The [dataset](https://www.kaggle.com/gilsousa/habermans-survival-data-set) contains cases from a study that was conducted between 1958 and 1970 at the University of Chicago's Billings Hospital on the survival of patients who had undergone surgery for breast cancer.

#### 1. About the file
1. Title:  Haberman's Survival Data
2. Sources:
(a) Donor: Tjen-Sien Lim (limt@stat.wisc.edu)
(b) Date: March 4, 1999
3. Relevant Information:
The dataset contains cases from a study that was conducted between
1958 and 1970 at the University of Chicago's Billings Hospital on
the survival of patients who had undergone surgery for breast
cancer.
4. Number of Instances: 306
5. Number of Attributes: 4 (including the class attribute)
6. Attribute Information:
   Age of patient at time of operation (numerical),
   Patient's year of operation (year - 1900, numerical),
   Number of positive axillary nodes detected (numerical),
   Survival status (class attribute)
       1 = the patient survived 5 years or longer
       2 = the patient died within 5 year
7. Missing Attribute Values: None

## 1. High level statistics of the dataset 

***Observations:***

1. The age of the patients vary from 30 to 83 with the median of 52.
2. Although the maximum number of positive lymph nodes observed is 52, nearly 75% of the patients have less than 4 positive  axillary lymph nodes and nearly 25% of the patients have no positive  axillary lymph nodes
3. The target column is imbalanced with 74% of values are 1

## 2. Objective

To predict whether the patient who had undergone surgery for breast cancer will survive after 5 years or not based upon the patient's age, year of treatment and the number of positive axillary nodes detected.

## 3. Univaraite analysis 

***Observations***
1. The number of positive  axillary lymph nodes of the survivors is highly densed from 0 to 5 
2. Almost 80% of the patients have less than or equal to 5 positive  axillary lymph nodes. 
3. The patients treated after 1966 have the slighlty higher chance to surive that the rest. The patients treated before 1959 have the slighlty lower chance to surive that the rest.
4. If number of axillary node is less,than survival of patients is more.

## 4. Bi-variate analysis 

**Observations**
1. Comparing with other 2 plots Age of patient at time of operation(Age) and Number of positive axillary nodes detected(Nodes) are the most useful features to identify Survival status.
2. There is no clear seperation between survival status
3. combinations of features are not useful in classfication
4. if number of axillary node is less,than survival of patients is more.

## 5. Conclusion

1. The given dataset is imbalenced as it does not contains euqal number of data-points for class 1 and class 2.
2. The given dataset is not linearly seprable form each class. There are too many overlapping in the data-points and hence it is very diffucult to classify using given features. 
3. we can not build simple model for classification using only if else condition. We need to have some more complex technique to handle this datase or more data faatures to build a efficient model
4. By plotting all pdf, cdf, box-plot, pair plots, scatter plot etc. we get only one conclusion if number of axillary node is less,than survival of patients is more.
