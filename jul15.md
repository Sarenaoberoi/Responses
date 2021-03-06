## A

1) The ImageDataGenerator command is used to pass directories to the generator and autolabel the images based on the directory name. It takes an argument called rescale, which works to rescale/noramlize the images. It can do this by dividing the pixels by 255 to make the pixel range from 0 to 1. The images are flown out of the directory using the flow_images_out_of_directory command. You must make sure to specify the directory that contains the data you want. For example, the train_dir directory contains all of the training images of horses and humans. The target_size has the size of the image. More often than not, the images you choose may not all be the exact same size. Target_size will resize the images. If you have 2 different classes you would use class mode = binary. If you have more than 2 classes you would say class mode = categorical. All of these same steps would be applied to the validation dataset (except reference the validation directory). The ImageDataGenerator works by passing in directories to the generator, while the flow_images_out_of_directory works to flow images out of the directory.


2) There were 3 convolution layers in the model (16, 32, and 64). There are some pixels that don't have neighbors to the right, left, up, or down. These pixels are removed. For example, if you begin with 28 by 28, they reduce to 26 by 26. Follwoing this, pooling reduces the dimensionalty by half so 26 by 26 become 13 by 13. In the horses and humans example the pooling halved the dimensionality from 298 by 298 to 149 by 149. This 149 by 149 reduced by half for the pixels that didn't have neighbors (147 by 147) and then reduced and then halved again. The activation function chosen is the sigmoid function. This function works by setting one class to  0 and the other to 1. For example, if an image of a horse was presented, the function would set horse to 1 and human to 0. 

## B

1) This graph allows you compare the different variables by creating a graph for each variable agaisnt another. The graph at the top left shows the variable 'MPG' compared with the same variable 'MPG'. The graph is a normal distribution meaning that these two variables have a high correlation. You can compare the different variables by observing how close the bell curves is to a normal distribution for each variable comparison.

2) It seemed that the amount of loss fluctuated in the last 5 epochs. The lowest amount of loss was in epoch number 996. The plot also shows this. Most of the points are close to the line, but if you look at the top right you can see that there are two points that stray far from the line. 
<img width="306" alt="Screen Shot 2020-07-17 at 10 14 51 PM" src="https://user-images.githubusercontent.com/60228365/87844028-eae0df00-c886-11ea-84bf-50922a9bed57.png">

<img width="556" alt="Screen Shot 2020-07-17 at 9 12 26 PM" src="https://user-images.githubusercontent.com/60228365/87844666-5463ec00-c88d-11ea-8ca0-f392c3dba7e3.png">
## C

1) After looking at the graph with the tiny, small, medium, and large training and testing sets, I noticed that the tiny one performed the best. This can be concluded as the tiny traning and the tiny validiation lines are closer to each other than any other pair is. This means that both the training and validation were going in the same direction and performed similarily. 

<img width="453" alt="Screen Shot 2020-07-18 at 12 25 15 AM" src="https://user-images.githubusercontent.com/60228365/87844664-5037ce80-c88d-11ea-80c2-f8d503bf836e.png">


