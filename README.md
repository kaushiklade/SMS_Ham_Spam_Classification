# SMS_Ham_Spam_Classification

Short Message Service or SMS considered to be the text messaging service component of Telephone or Internet. In our day-to-day life we do receive considerable amount of SMS either from Friends, Telecom or Bank companies regarding our daily transactions or from tons of other sources. Some of these SMS texts are genuine whereas some can lead to fraudulent incidents.
Main task of this case study is making a Machine Learning model which can predict the SMS as HAM or SPAM with the help of text body of SMS.
Dataset for this case study can be found at Kaggle. It consist of 5574 English text messages which are labeled as Ham or Spam.

## Exploratory Data Analysis : 

We will be processing the text so as to remove any punctuation along with deconcatenation so as to make a complete word for model prediction.
With the help of available, we can also perform feature engineering as follows;

### Text Length of SMS Text :

Length of the complete text or words in the text can be considered to be the important feature for our analysis. The analysis of this feature can be seen in 
jupyter notebook named * SMS Spam Collection - EDA.ipynb *

### Presence of Digit in Text body :

Presence of any numerical words can also considered to be much valuable feature for this classification. 
Spam texts tend to have numerical words as it can sometimes refer to a phone/mobile number or numbers in specific web link etc.


## Machine Learning Modeling :

Initial task of modeling is to convert the text into numerical form with the help of Text Vectorization with the help of Bao of Words, TF-IDF or Word vector techniques.
Also, for evaluating the model performance, we will be considering AUC as metric for model performance.

We will be selecting three models viz. 
Naive Bayes model which assumes that the data independent of each of the other features
Linear Regression which assumes that the data is linearly separable, 
Random Forest assumes that data can be classified with the help of tree based classification technique.

