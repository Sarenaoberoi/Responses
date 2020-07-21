### 1)

#### A) Problem Statement: 
Diabetes is a very prevalent disease around the world, with over 30.3 million diabetic individuals in the United States alone. A disease known as diabetic retionopathy, although uncommon, has a number of negative consequences including color blindness, blurry vision, and a loss of vision altogether. This disease is characterized by the damage it causes to the back of the eye (also known as the the fundus). By taking images of the fundus, scientists are able to learn whether or not an individual has diabetic retinopathy. By creating a convolutional network, scientists can feed in training and testing images to teach a network how to accuractly predict whether an individual has diabetic retinopathy based on photographs of the fundus. Although this disease is rare, it still has a number of debilitating consequences. By training this convolutional neural network and using other machine learning methods, scientistis have the ability to accuratley diagnose patients with diabetic retinopathy and treat them before it is too late. 

#### B) DATA AND METHODS:


#### C)
I will create a poster that includes a portion for the introduction of the disease as well as another portion for the introduction of a convolutional neural network (and what it is used for in this study), conclusion of the study (how accurate the network was), and another portion for some of the code I used and how the network was created and performed. 


#### D: 
##### 1) 
The optimizer used for this exercise was the RMSprop optimizer. This optimizer was paired with a high learning rate (lr = 0.001) in order to help the model perform better. The RMSprop optimizer works by doing two things: help keeps a moving average of the square gradients and divdies the gradients by the root of the average from the first step. The RMSprop optimizier is similar to Adagrad which is another adaptive learning rate algorithim. Adagradm adds element-wise scaling of the gradient based on the historical sum of squares in each dimension. So, it keeps a running sum of squared gradients and adapts the learning rate by dividing it by that sum. 

#### 2) 
The loss function used for the cats and dogs dataset was the binary cross-entropy loss function. This is the most common lost function used for binary datasets. This loss function works by returning high values for bad predicitons and low values for good predictions. As each prediction is made, the loss function usually goes down because the predictions are getting better and better with each guess. *PENALIZING BAD PREDICTIONS*

#### 3) 
There is a metric= argument in our model.compile() function is very important in judging the performance of a specific model. *WHAT IS THIS**


#### 4) 
