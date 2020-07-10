1) The TF hub is an area of the cloud that contains information and data for a number of commonly datasets and machine learning models. These models can be used for a number of reasons, including fitting training and fitting models, as well as creating neural networks and predicting new values from the datasets. The TF hub was able to bring in all of the movie review data, including 50,000 movie reviews. 

2) The optimizer and loss function work together in order to find the best possible guess with the lowest loss. The neural network will come up with a predictive guess and the loss function will calculate how much loss/accuracy is in that guess. These results then go back to the optimizer which comes up with another guess depending on the previous one. This cycle repeats over and over again- the loss continues to go down with each guess and the accuracy increases. The text classificaiton movie reviews had an accuracy of 86.19% which is a relatively good accuracy. 

3) The first graph plotted the training loss over the number of epochs (loss on y-axis and ephochs on x-axis). The graph showed that the average loss decreased as the number of epohs increased. This is what you will typically see, as the loss and optimizer function work together in order to decrease the loss with each guess. 

<img width="423" alt="Screen Shot 2020-07-09 at 2 00 14 PM" src="https://user-images.githubusercontent.com/60228365/87074833-71dde980-c1ed-11ea-9a36-02fe53714009.png">


The second graph showed the training and validation accuracy with the epochs on the x-axis and the accuracy on the y-axis. The graph shows that the accuracy increased as the ephochs increased. This means that accuracy increased (and the loss decreased) with each epoch. When the line peaks, this means that the accruacy is no longer increasing, and the model is beginning to become overfit. 

