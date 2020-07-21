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

<img width="520" alt="Screen Shot 2020-07-21 at 8 35 54 AM" src="https://user-images.githubusercontent.com/60228365/88055658-59df6180-cb2d-11ea-984b-04b29e0417a3.png">



<img width="491" alt="Screen Shot 2020-07-21 at 8 36 08 AM" src="https://user-images.githubusercontent.com/60228365/88055663-5cda5200-cb2d-11ea-8833-ea1327e64ba0.png">



#### 5)

![CATJPEG](https://user-images.githubusercontent.com/60228365/88055715-6c599b00-cb2d-11ea-9489-ec107d8ea239.jpg)



<img width="656" alt="Screen Shot 2020-07-20 at 5 00 44 PM" src="https://user-images.githubusercontent.com/60228365/88055736-74b1d600-cb2d-11ea-9f69-cb3658a9e636.png">


![CAT2!](https://user-images.githubusercontent.com/60228365/88055755-7d0a1100-cb2d-11ea-8ece-4467882cf85a.jpg)


<img width="621" alt="Screen Shot 2020-07-20 at 5 02 01 PM" src="https://user-images.githubusercontent.com/60228365/88055762-809d9800-cb2d-11ea-8399-f8abc5f38d77.png">




![CAT3](https://user-images.githubusercontent.com/60228365/88055781-872c0f80-cb2d-11ea-9c4e-d8f07adb1659.jpg)



<img width="604" alt="Screen Shot 2020-07-20 at 5 03 51 PM" src="https://user-images.githubusercontent.com/60228365/88055791-8c895a00-cb2d-11ea-9722-d4ecbbc08d3a.png">



![dogimage1](https://user-images.githubusercontent.com/60228365/88055813-94e19500-cb2d-11ea-9837-18a95073809b.jpg)



<img width="585" alt="Screen Shot 2020-07-20 at 5 05 49 PM" src="https://user-images.githubusercontent.com/60228365/88055818-97dc8580-cb2d-11ea-9c12-ca0367554528.png">



![DOGIMAGE2](https://user-images.githubusercontent.com/60228365/88055834-9e6afd00-cb2d-11ea-85d2-794c0266766a.jpg)



<img width="592" alt="Screen Shot 2020-07-20 at 5 06 39 PM" src="https://user-images.githubusercontent.com/60228365/88055842-a0cd5700-cb2d-11ea-9a10-aa1accd42971.png">


![FUNNYDOG](https://user-images.githubusercontent.com/60228365/88055855-a4f97480-cb2d-11ea-8e5a-013e98c16074.jpg)


<img width="622" alt="Screen Shot 2020-07-20 at 5 08 12 PM" src="https://user-images.githubusercontent.com/60228365/88055868-a9be2880-cb2d-11ea-891f-7236f7b08e1e.png">



![dogyay](https://user-images.githubusercontent.com/60228365/88055890-b0e53680-cb2d-11ea-82d0-58c3bd541a00.jpg)



<img width="554" alt="Screen Shot 2020-07-20 at 5 08 48 PM" src="https://user-images.githubusercontent.com/60228365/88055901-b478bd80-cb2d-11ea-9c19-90d7d0a129a4.png">

