## Responses

### A. Premade Estimators 
#### 1. 
The labels were split from the training set using this line of code:
train_y = train.pop('Species')
test_y = test.pop('Species')

The name of the labels dataset was 'species' and it contained the names of the 3 different species: Setosa, Versicolor, and Virginica.

#### 2.
- tf.estimator.DNNclassifier
- tf.estimator.DNNLinearCombinedClassifier
- tf.estimator.LinearClassifier
- tf.estimator.BaselineEstimator
- tf.estimator.BoostedTreesEstimator
- tf.estimator.BinaryClassHead

#### 3.
The purpose of the input functions is to provide a place to include training, testing, and prediction data. Within this fuction you can also add code that works to convert the input data into a dataset or dataframe. The feature columns are included so that the model knows the list of features it should use. The feature colomuns specifies how the data inputted will be read into the model for training. 
#### 4. 
Describe the command classifier.train() in detail.  What is the classifier and how did you define it?  Which nested function (and how have you defined it) are you applying to the training and test detests?

The command classifier.train() works to train the model. We defined classifier in a couple cells above:
classifier = tf.estimator.DNNClassifier(
    feature_columns=my_feature_columns,
    # Two hidden layers of 30 and 10 nodes respectively.
    hidden_units=[30, 10],
    # The model must choose between 3 classes.
    n_classes=3)

It takes the input_fn we defined above as well as the data from training set. 


#### 5.
tf.estimator.LinearClassifier:


Prediction is "Setosa" (99.1%), expected "Setosa"
Prediction is "Versicolor" (97.2%), expected "Versicolor"
Prediction is "Virginica" (95.9%), expected "Virginica" 

tf.estimator.DNNLinearCombinedClassifier:


Prediction is "Setosa" (92.1%), expected "Setosa"
Prediction is "Versicolor" (69.3%), expected "Versicolor"
Prediction is "Virginica" (74.2%), expected "Virginica"

tf.estimator.DNNClassifier:


Prediction is "Setosa" (91.1%), expected "Setosa"
Prediction is "Versicolor" (48.2%), expected "Versicolor"
Prediction is "Virginica" (71.7%), expected "Virginica"

The LinearClassifier performed the best, the DNNLinearCombinedClassifier performed the second best, and the DNNClassifier performed the worst. 





### Build a Linear Model

##### 1. 

<img width="581" alt="Screen Shot 2020-07-21 at 2 39 30 PM" src="https://user-images.githubusercontent.com/60228365/88241684-d884ed80-cc58-11ea-98dc-45ef5c0cf8de.png">


<img width="1272" alt="Screen Shot 2020-07-21 at 2 45 20 PM" src="https://user-images.githubusercontent.com/60228365/88241688-dc187480-cc58-11ea-93f0-49649a0968ab.png">


After looking at the graph for age, it seems that the median age was late 20's. This graph of age can also be seen on the top left of the sns plots.  



##### 2. 
A categorial column a column containing only numercial, discrete values. A dense feature is slightly more complicated, in that it works to extract important features from an image. It is possible to break an image up into multiple dense features, with each dense feature including meaningful information from the image. By using dense features, users are able to get an in depth view of every feature in an image.     

##### 3. 

<img width="456" alt="Screen Shot 2020-07-24 at 11 00 37 PM" src="https://user-images.githubusercontent.com/60228365/88447475-9cd95780-ce01-11ea-8c13-d7ec42dc5cf4.png">


<img width="428" alt="Screen Shot 2020-07-24 at 11 01 00 PM" src="https://user-images.githubusercontent.com/60228365/88447476-9f3bb180-ce01-11ea-893e-b035f493023f.png">


Some of the basic feature columns included in the model were sex, n_siblings_spouces, parch, class, age, fare, ect. When we only trained the regular feature columns we obtained an accuracy of 75%, however, after including derived feature columns (combining two or more of the base feature columns such as age x sex) we obtained a higher accuracy of 77.6%. This shows that adding these cross featured columns improved the accuracy of the model. The addition of crossed features allow the model to predict more specific features and are able to capture more combintations of features. The predicted probabilities plot shows that the lowest probability of survival (slightly greater than 0.0) had the highest frequency. The graph also seems to be skewed to the right, meaning that only a small number of individuals had a high chance of survival. The ROC curve compares the false positive rate to the true positive rate. It seems that in the beginning, the true positive rate increased while the false positive rate remained static. Then, as the rate increased past 0.8 the line began to plateau. 



