###Project 3

The first step in doing this project was importing the 10,000 images into pycharms. I split my images up into two groups: testing images (accraims) with 9,000 images and testing images (testing) with 1,000 images. After bringing the images in, I made sure to check the length of the images and labels to make sure they were lining up. Following this, I divided the training images and testing images by 255.0 to normalize the images. I began by creating a DNN model and then moved to the CNN model. For the DNN model, I included 1 flatten layer, and 3 dense layers (64, 64, and 1). Then I added in 3 convolutions (16, 32, and 64). Each of these convolutions had the activation= ‘relu’. 

For the model.compile function I used RMSprop as my optimizer (with a learning rate of 0.001). The loss function I used was the mse, and the metrics were ‘mse’ and ‘mae’. The optimizer RMSprop works by providing an average of the square of gradients, and then divides the gradient by the square root of the average (from the first step). The MSE loss function is good for providing a mean squared error between the values we have and what we are trying to predict. I ran model.fit with all 9,000 images, so I had 90 steps_per_epoch and a batch_size of 100. I began by running 3 epochs and go an mae of 29.5612. However, after running with 6 epochs, I got an mae of 25.0337 and an mse of 964.7205.    

<img width="826" alt="Screen Shot 2020-07-26 at 5 53 15 PM" src="https://user-images.githubusercontent.com/60228365/88493950-c4572e00-cf81-11ea-982c-03fd934dec44.png">

The first epoch began with a loss of 2,358, and ended with a loss of 964.72 at epoch number 6. The mae began at 38.85 at epoch number one, and ended at 25.0337 at epoch number 6. Each epoch took about 15 minutes to run. 


<img width="828" alt="Screen Shot 2020-07-26 at 5 53 39 PM" src="https://user-images.githubusercontent.com/60228365/88493954-c620f180-cf81-11ea-9dc3-87790d767e0c.png">

model.evaluate took about 28 seconds to run and had a loss of 1501 and an mae of 33.9754. I noticed that this mae is slightly higher than the results from model.fit. 

<img width="615" alt="Screen Shot 2020-07-26 at 6 44 18 PM" src="https://user-images.githubusercontent.com/60228365/88493955-c91be200-cf81-11ea-9c6a-1a91eeb0b2b0.png">

This graph above shows the loss per epoch for the convolutional neural network. the graph clearly shows that the decreased per epoch and ended with the lowest loss (epoch 6). 

<img width="612" alt="Screen Shot 2020-07-26 at 6 46 05 PM" src="https://user-images.githubusercontent.com/60228365/88493956-cb7e3c00-cf81-11ea-9c7f-4daff2685db1.png">

The graph above shows the mean absolute error. As before, the graph shows that the mae decreases with each epoch (with epoch 6 having the lowest mae). 

