![aml-poster_48112829](https://user-images.githubusercontent.com/60228365/89741329-579e6200-da5e-11ea-8824-170ee8a5517c.png)

I learned a lot of interesting information about diabetic retinopathy and its current diagnosis and treatment while researching this project. Diabetic Retinopathy is characterized by the damage it causes to the retina. We all have small blood vessels located in the retina that are critical for keeping our eyes healthy and functioning. DR will often constrict these blood vessels, making it difficult for healthy blood to flow into the eye. Once the symptoms of diabetic retinopathy have presented themselves, the blood vessels will often become weak and die off, restricting the eye from getting the necessary blood. This will create symptoms such as blurriness, dark spots, or a loss of vision altogether. 

While doing this project I noticed that the current diagnosis was most effective in developed countries where doctors were very prevalent. However, when it came to third world countries, there were not enough resources and doctors to help diagnose and treat individuals. Because of this, doctors in Aravind Hospital located in India, attempted to create a technology-based model that allows individuals to retrieve a diagnosis without the need of a physical appointment. 

I retrieved the data used for my model from Kaggle. The full dataset consisted of a total of 88,702 images of the fundus taken of individuals living in small villages around India. Before splitting the images, I resized all of them to 1500 by 1000 pixels. I then split the images up into training and testing sets, with the training set amounting to a total of 35,126 images (I used 300 of these), and the testing set with 53,576 images (and I used 200 of these). The training images were all labeled with number from 0-4: 0 being no DR to 4 being proliferative DR. As you can see from this graph of the distributions of severity levels, most individuals did not have DR. with the next highest diagnosis being moderate DR or a level of 2. The next image snippet of how the data was organized in the testing and training files.  

![Messages Image(777973500)](https://user-images.githubusercontent.com/60228365/89743594-abb34180-da72-11ea-92de-e1db49d5584f.png)


![Messages Image(1530116381)](https://user-images.githubusercontent.com/60228365/89743596-ad7d0500-da72-11ea-8bbc-06ee4868cecc.png)

#### CNN:

After trying out a couple different combinations, I got my best results with a CNN made up of 3 convolutions of 16, 32, and 64 neurons in each of the layers, 1 flatten layer, and 2 dense layers. I used Adam as my optimizer, and Sparse_categorical_crossentropy as my loss function, since the data was categorical.

![Messages Image(3319245899)](https://user-images.githubusercontent.com/60228365/89743619-d7cec280-da72-11ea-8f18-9eebc4ad7255.png)

#### Results:

My best epoch resulted in an validation accuracy of of 73% and a loss of 0.84, and a training accuracy of 90% and a loss of 0.26 as you can see by the accuracy and loss plots shown. The accuracy graph defiantly showed some overfitting and needs some improvement, which will be addressed in future research. 

![Messages Image(1288454116)](https://user-images.githubusercontent.com/60228365/89741265-c929e080-da5d-11ea-8944-eae27895ba5a.jpeg)
![Messages Image(2272593950)](https://user-images.githubusercontent.com/60228365/89741266-caf3a400-da5d-11ea-8e48-8d8f02b4ed99.jpeg)

I used the model to predict the severity of a  healthy looking eye (as shown below) and the model was able to accurately predict the image with a label of 0. The model worked by giving a probability to each of the 5 labels, making the label with the highest probability the true label. So in this case, 0 had the highest probability of 0.35, making it the correct label. The model was able to easily predict 0’s for individuals that did not have dr, but had a harder time picking other less commonly seen numbers from the data set like 4 or proliferative dr. This is evident because the training dataset had an abundance of images with the label 0 but a very small number of 4’s, making it better at distinguishing 0’s.  

![Messages Image(3854663916)](https://user-images.githubusercontent.com/60228365/89743661-4e6bc000-da73-11ea-8d8d-76c86523240f.png)


#### The Future

The final model created by the data science team included image processing code that extracted some of the main features from each image. The scientists also applied gaussian blur and image augmentation in order to get a more comprehensive view of the fundus, including rotated and cropped pictures. This in-depth view of the varying images improved the performance of the model altogether.

As I explained above, I noticed that a lot of the data included images of individuals with no DR (0), which made the model good at 

![Messages Image(3045620765)](https://user-images.githubusercontent.com/60228365/89743687-84a93f80-da73-11ea-8569-411a45458392.png)

![Messages Image(2322208606)](https://user-images.githubusercontent.com/60228365/89743685-7fe48b80-da73-11ea-8bc5-336042bde561.png)



