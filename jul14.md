## July 14 Response

### A. 

The first filter applied reduced all of the features in the image. The lines and colors were all diminished resulting in a dark image. 

<img width="469" alt="first filter" src="https://user-images.githubusercontent.com/60228365/87466423-39bb1a00-c5e4-11ea-92f2-7a2bd00c8fbf.png">
First filter 

The second filter enhanced the vertical lines. The vertical lines on the staircase (as well as other locations in the image) were all enhanced. 

<img width="484" alt="second filter" src="https://user-images.githubusercontent.com/60228365/87466440-40e22800-c5e4-11ea-8cb3-f862db706a5c.png">
Second filter

The third filter enhanced all of the horizontal lines. The horizontal lines on the staircase towards the top of the image were enhanced greatly. 


<img width="475" alt="thirdfilter" src="https://user-images.githubusercontent.com/60228365/87466454-45a6dc00-c5e4-11ea-8266-fb2abcbdc8ad.png">
Third filter

As you apply the filter to your original array, you are multiplying each pixel's neighbor by it's weight, the current pixel by its weight, and adding them together. This process is done for every pixel in the image, resulting in a transformed image. Depending on which filter you choose, you are either enhancing or diminishing a certain part of the image (vertical/horizontal lines, for example). This is a useful tool, as when an individual is interested in looking at a specific computer vision, he/she may not want to see every single feature of that image. By using a filter, the individual can focus on only couple aspects of the image (that they are interested in). 



### B.

The pooling image became slighly blurry and grainy. This is the image I expected, however, because pooling works by extracting all of the extraneous information from the image (keeping all of the important features of that image). All of the main features of the image were preserved. The results decreased in size. The scales on both the x-axix and y-axis decreaesd from 500 (non-pooling) to 250 (pooling). The pooling used was max pooling, and this is evident because of the last couple lines of code: 
    pixels.append(i_transformed[x+1, y+1])
    pixels.sort(reverse=True)
    newImage[int(x/2),int(y/2)] = pixels[0]
   
 

<img width="496" alt="pooling" src="https://user-images.githubusercontent.com/60228365/87466458-48093600-c5e4-11ea-9233-9b4bb9288ed0.png">
Pooling


### C. 

It seems that by adding the Conv2D and MaxPooling2D layers, the accuracy of the neural network improved. Without any convolutions the accuracy was 0.9744. However, after the convolutions were added with 32 neurons, the accuracy increased to 0.9916. When the convolutions were changed from 32 to 16, the accuracy decreased very slightly. It decreased from 0.9916 to 0.989. This is plausible because the number of layers decreased so accruacy decreased as well. Without convolutions, the run time for each epoch was an average of 3 seconds. With the convolutions (32) the average run time for each epoch was 42 seconds. With the convolutions (16) the run time for each epoch was approximatley 30 seconds. Adding 1 more convolution layer increased the accuracy from 0.989 to 0.974 with 28 seconds per epoch (accuracy decreased, probably due to overfitting).   
<img width="564" alt="Screen Shot 2020-07-14 at 2 42 45 PM" src="https://user-images.githubusercontent.com/60228365/87466469-4b9cbd00-c5e4-11ea-8c14-1df29eb98f2e.png">
Box of 12 images




