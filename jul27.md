### Response: July 27

I predicted the population of 5 different images. 

<img width="501" alt="Screen Shot 2020-07-27 at 1 51 13 PM" src="https://user-images.githubusercontent.com/60228365/88575653-3aa37100-d012-11ea-9a40-901c0ef4ec73.png">

This first image showed a very forresty area. The model predicted a population of 32.315475 and the true population from the csv file was 38.8057289. I was slightly confused as why the population was so high in this very forresty area. I assume that there was a populated road near by.  


<img width="488" alt="Screen Shot 2020-07-27 at 1 52 07 PM" src="https://user-images.githubusercontent.com/60228365/88575667-3f682500-d012-11ea-87ac-ab3545db46fa.png">

This second image also showed a very forrestry area. The model predicted a population of 30.5362 and the true population from the csv file was 7.95019. I'm really not sure why the model predicted such a high population for this area. I think it could have been slightly confused by a more highly populated area near where the image was taken. 


<img width="500" alt="Screen Shot 2020-07-27 at 1 53 20 PM" src="https://user-images.githubusercontent.com/60228365/88575674-42fbac00-d012-11ea-9a0a-89603e300e3c.png">

This third image showed a couple houses. The model predicted a population of 33.708145 and the true pouplation from the csv file was 50.004032. This number makes the most sense because we would expect there to be more people in neighborhoods.

<img width="500" alt="Screen Shot 2020-07-27 at 1 54 47 PM" src="https://user-images.githubusercontent.com/60228365/88575686-45f69c80-d012-11ea-84c2-77f22e75069a.png">

This image showed a number of trees. The population predicted for this image was 31.238304 while the true population from the csv file was 9.50581. -Same reasoning as image number two.- 

<img width="484" alt="Screen Shot 2020-07-27 at 1 57 13 PM" src="https://user-images.githubusercontent.com/60228365/88575699-4858f680-d012-11ea-8200-8d005d118d1e.png">

This last image showed a couple hosues (similar to image number 3). The model predicted a poulation of 34.3583 while the true poulation from the csv file was 27.415765. I think that this population makes sense for the image –– There were roughly 2 or 2 and a half houses shown in the image, with a road as well.   

I think that this model works relatively well for the most part. Most of my model's predictions were pretty close to the real value (except for image 2). I think that I could've gotten more accurate predictions if I trained the model on more images. For predictions, I decreased both the training and testing images to 100. As we talked about in class, there were a couple problems with the data. One problem was that the raster population counts and the population counts from the orthoimages were not perfectly aligned which could have caused the accuracy to decrease.  
