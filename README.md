> # SMS_Ham_Spam_Classification

Short Message Service or SMS considered to be the text messaging service component of Telephone or Internet. In our day-to-day life we do receive considerable amount of SMS either from Friends, Telecom or Bank companies regarding our daily transactions or from tons of other sources. Some of these SMS texts are genuine whereas some can lead to fraudulent incidents.
Main task of this case study is making a Machine Learning model which can predict the SMS as HAM or SPAM with the help of text body of SMS.
Dataset for this case study can be found at Kaggle. It consist of 5574 English text messages which are labeled as Ham or Spam.

> ## Exploratory Data Analysis : 

We will be processing the text so as to remove any punctuation along with deconcatenation so as to make a complete word for model prediction.
With the help of available, we can also perform feature engineering as follows;

### Text Length of SMS Text :

Length of the complete text or words in the text can be considered to be the important feature for our analysis. The analysis of this feature can be seen in 
jupyter notebook named * SMS Spam Collection - EDA.ipynb *

### Presence of Digit in Text body :

Presence of any numerical words can also considered to be much valuable feature for this classification. 
Spam texts tend to have numerical words as it can sometimes refer to a phone/mobile number or numbers in specific web link etc.


> ## Machine Learning Modeling :

Initial task of modeling is to convert the text into numerical form with the help of Text Vectorization with the help of Bao of Words, TF-IDF or Word vector techniques.
Also, for evaluating the model performance, we will be considering AUC as metric for model performance.

We will be selecting three models viz. 

- Naive Bayes model which assumes that the data independent of each of the other features.

- Linear Regression which assumes that the data is linearly separable.

- Random Forest assumes that data can be classified with the help of tree based classification technique.


Best Model to perform is Naive Bayes which gives us AUC score of more than 0.99.







> ## Deep Learning Models : 

As we can see Machine Learning modeling works better with given data, we can also try Deep Learning Models like LSTM and simple Dense models to check the performance on data.
For text data, we can simply use Word Vector techniques as well as Word Embedding Layer to embed each word as Numerical representation and accordingly passing the same into deep learned layers.

We trained data with ;

- Simple Deep Neural Network, where we used two layered dense network to train with BoW or TF-IDF word vectorized text features along with two numerical features

- Simple LSTM Model, where LSTM layer was added before Dense Layers so as to preserve the symantic relationship between words in sentences. This model is trained with Word2Vec vectorized text vector

- LSTM Model with Word Embedding, where we first embed each word of the sentence in SMS text with numerical digit and this embedding layer is trained with remaining Deep Learned model so as to get optimal performance.



> # Conclusion :

Both Naive Bayes from simple Machine Learning model and LSTM Model with Embedding layer perform well on given data despite being imbalanced data. In this classification of Text data, NLP playes very importat role in extracting the meaningful information from text. Also, extracting the useful features from the available text proves to be the important step in getting the optimal performance.
