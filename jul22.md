## III Responses
### A. Boosted Trees
#### 1.
A one-hot-encoded column is created when a categorical column is split into new columns with each column being given either a 0 or 1. The source values are disecrete, as each column is either labeled with a 0 or 1. For example, from the titanic dataset, when trying to distinguish betweeen class (one, two, or three), a one-hot-encoded column would provide us with an array: [0, 0, 1]. The first number represents the first class, the second number represents the second class, and the third number represents the third class. Since the '1' is on the third number, we know that we are referncing the third class. 

#### 2. 
Dense features are commonly used to specify the absence and presence of data. By labeling columns as 0, dense features allow the user to know that there is no data in that location. On the other hand, by labeling a column with 1, dense features let the user know that there is data in this area. In general, dense features allow users to get an in depth view of whatever dataset they are looking at (by describing where there is a presence and absence of data). The "tf.keras.layers.DenseFeatures(your_features)(your_object).numpy()" takes the dataframe, applies the DenseFeatures, and turns it into an array with 1's and 0's. The 1 means that there is data there (if there is a 1 for n_siblings_spouces it means that you have a sibling/spouce on board, while 0 means that you are alone).  

#### 3. 
The accuracy for the logistic regression was 0.765, while the accuracy for the boosted tree model was 0.818. The graph shows that the boosted tree model had a higher frequency (approximatley 80) with a probability of around 0.75 chance of survival, while the logitic regression had a lower frequency (approximatley 70) with a 0.75 probability of survival. The boosted model also showed a higher frequency of individuals with a 100% probability of survival, while the logistic regression showed a much lower frequency for 100% chance of survival. At first, the ROC graph shows that the true postive rate increased rapidly, while the false positive rate reamined static (at 0). However, the ROC graph shows that as the false positive rate increases, the true positive rate increased as well. The AUC value is 0.876615 (very high) indicating a very good predictive model (more area under the curve). 
<img width="445" alt="Screen Shot 2020-07-22 at 6 57 42 PM" src="https://user-images.githubusercontent.com/60228365/88238925-023a1680-cc51-11ea-9633-ae6657153d39.png">

<img width="427" alt="Screen Shot 2020-07-22 at 6 56 53 PM" src="https://user-images.githubusercontent.com/60228365/88238928-0403da00-cc51-11ea-8e77-678a55d8875e.png">

<img width="435" alt="Screen Shot 2020-07-22 at 6 35 55 PM" src="https://user-images.githubusercontent.com/60228365/88238942-082ff780-cc51-11ea-9fb6-cb529e7a303b.png">

### B. Boosted Trees continued (with model understanding)
<img width="762" alt="Screen Shot 2020-07-22 at 7 28 51 PM" src="https://user-images.githubusercontent.com/60228365/88239561-bee0a780-cc52-11ea-8c70-f158915fe6da.png">

<img width="727" alt="Screen Shot 2020-07-22 at 7 29 06 PM" src="https://user-images.githubusercontent.com/60228365/88239566-c1430180-cc52-11ea-8cea-1907557c2451.png">
The first horizontal graph shows the features that have the highet probability of death. For example, males had the highest chance of not surviving. On the other hand, higher fare gave individuals a (very) slightly higher chance of survival. The violin plot showed a very similar distribution as the horizontal graph, just in a different format.  


<img width="722" alt="Screen Shot 2020-07-22 at 7 32 37 PM" src="https://user-images.githubusercontent.com/60228365/88239570-c30cc500-cc52-11ea-82a0-3bc8c7b58679.png">



The gain feature importance plot shows that sex played a very big role in the survival rate (0.35). Fare, age, and class played big roles as well. The permuation feature plot shows that sex played a big role in survival rate as well, with class, deck, and n_siblings_spouses being the next most common survival features. 
