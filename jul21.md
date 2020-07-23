## Responses

### A. Premade Estimators 
#### 1. 
The labels were split from the training set using this line of code:
train_y = train.pop('Species')
test_y = test.pop('Species')

The name of the labels dataset was 'species' and it told you the names of the 3 different species: Setosa, Versicolor, and Virginica.

#### 2.
- tf.estimator.DNNclassifier
- tf.estimator.DNNLinearCombinedClassifier
- tf.estimator.LinearClassifier
- tf.estimator.BaselineEstimator
- tf.estimator.BoostedTreesEstimator
- tf.estimator.BinaryClassHead

#### 3.
The purpose of the input functions is to provide a place to include training, testing, and prediction data. Within this fuction you can also add code that works to convert the input data into a dataset or dataframe. The feature columns are put in so that the model knows the list of features it should use. The feature colomuns tells you how to use the data that was inputted. 

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







### Build a Linear Model

##### 1. 
Using the dftrain dataset, upload an image where you used the seaborn library to produce a sns.pairplot().  Also include a histogram of age using the training set and compare it to the seaborn plot for that same feature (variable).  What interpretation can you provide of the data based on this plot?

After looking at the graph for age, it seems that the median age was late 20's. This graph of age can also be seen on the top left of the sns plots as well. 

##### 2. 
A categorial column is when a column only containing numercial data

##### 3. 








