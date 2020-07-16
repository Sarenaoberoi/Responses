the imageDatagenerator - pass directories to generator and it autolabels the images based on the directory name 

rescale goes inside ImageDataGenerator(to rescale and normalize)

create a generator by flowing them out of the directory using the flow_images_out_of_firectory-- specify the directory that contains the data you want so for example train_dir which has the training images of horses and humans
target_size = the size of the iamge, you don't know that they will always be the same so it's a good idea to resize them
class-model = binary (2 classes - horses and humans) - if you have more you can do categoical 

DO SAME thing for validation dataset 


CODE PART:
how do they resize?
filter on CONV2D- how do image sizes decrease

which activation function selected for output? - the sigmoid is the activation function and works by setting a class to either 0 or 1

using target_size we resized the images to 150, 150

we used 3 different convolution layers all using differnet number of neurons- why was using 3 good? 

the model summary showed that the output shape changed because some of pixels don't work for edges so they are taken out so it goes from being 28 to 26, 26, and then pooling reduced the dimensionalty by half so 26 and 26 become 13 and in the examplel the pooling halved it it went from 298 to 149 and then reduced two because of the pixels that didn't have neughbors and then pooling halved it again 


it shows you linear regression or logistic regression or something like that and you can use it to compare the different graphs bc the top one is a normal distribution and you want the closest to a nomeal or gaussian distritubiton as possible 


the loss decreased and the validation increased fro themost part 

in the last 5 you an see that the loss kind of fluctuated throughout the last 5 but towards the end the total loss decreased !!!! idk 

