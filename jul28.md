### Responses- July 28
Why is using one-hot encoding an inefficient towards vectorizing a corpus of words?  How are word embeddings different? 

As talked about in the tensorflow exercise and Lawrence Maroney's video, one-hot encoding is an interesting (but somewhat inefficient) way to encode words. With one-hot encoding, one goal is to keep a uniform length in regards to the longest sentence, so each word will have 0's up until the word (and a 1 for the word). For example, if the sentence was "I love apples", one-hot encoding would look something like this:

ADD PIC 

As we can see from the picture above, the majority of spaces are 0 (a sparse vector). Because of this, one-hot encoding is pretty inefficient. In order to create a more dense vector, known as word embeddings, we could assign a different number to each word. For example, for the sentence "the chocolate is in the cabinet", the to 1, chocolate to 2, is to 3, in to 4, and cabinet to 5:

[1, 2, 3, 4, 1, 5]

This method is much more efficient. 


2.Compile and train the model from the tensorflow exercise.  Plot the training and validation loss as well as accuracy.  Post your plots and describe them

<img width="755" alt="Screen Shot 2020-07-29 at 6 43 08 AM" src="https://user-images.githubusercontent.com/60228365/88818783-16b86a80-d18d-11ea-812f-78b829d8aa9a.png">


<img width="770" alt="Screen Shot 2020-07-29 at 6 43 30 AM" src="https://user-images.githubusercontent.com/60228365/88818791-191ac480-d18d-11ea-9c82-755e0c61440d.png">




D.Text Classification with an RNN


1.Again compile and train the model from the tensorflow exercise.  Plot the training and validation loss as well as accuracy.  Stack two or more LSTM layers in your model.  Post your plots and describe them.

<img width="452" alt="Screen Shot 2020-07-29 at 7 54 59 AM" src="https://user-images.githubusercontent.com/60228365/88818801-1c15b500-d18d-11ea-9b35-045ad637d277.png">


<img width="450" alt="Screen Shot 2020-07-29 at 7 55 08 AM" src="https://user-images.githubusercontent.com/60228365/88818808-1e780f00-d18d-11ea-94d6-2d40b3098bb8.png">


<img width="438" alt="Screen Shot 2020-07-29 at 8 10 24 AM" src="https://user-images.githubusercontent.com/60228365/88818815-20da6900-d18d-11ea-9e7a-caf4e7f225dc.png">


<img width="431" alt="Screen Shot 2020-07-29 at 8 10 39 AM" src="https://user-images.githubusercontent.com/60228365/88818817-22a42c80-d18d-11ea-8807-6000043a293d.png">

