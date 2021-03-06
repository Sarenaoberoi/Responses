### Responses- July 28

1) As talked about in the tensorflow exercise and Lawrence Maroney's video, one-hot encoding is an interesting (but somewhat inefficient) way to encode words. With one-hot encoding, one goal is to keep a uniform length in regards to the longest sentence, so each word will have 0's up until the word (and a 1 for the word). For example, if the sentence was "I love apples", one-hot encoding would look something like this (I created this table on word so I apologize if the formatting is a little weird):

<img width="576" alt="Screen Shot 2020-07-29 at 11 24 37 AM" src="https://user-images.githubusercontent.com/60228365/88819577-300de680-d18e-11ea-9088-01c294201f4f.png">


As we can see from the picture above, the majority of spaces are 0 (a sparse vector). Because of this, one-hot encoding is pretty inefficient. In order to create a more dense vector, known as word embeddings, we could assign a different number to each word. For example, for the sentence "the chocolate is in the cabinet", the to 1, chocolate to 2, is to 3, in to 4, and cabinet to 5 (This makes word embeddings much more efficient than one-hot encoding):

[1, 2, 3, 4, 1, 5]

 

2.

<img width="755" alt="Screen Shot 2020-07-29 at 6 43 08 AM" src="https://user-images.githubusercontent.com/60228365/88818783-16b86a80-d18d-11ea-812f-78b829d8aa9a.png">


<img width="770" alt="Screen Shot 2020-07-29 at 6 43 30 AM" src="https://user-images.githubusercontent.com/60228365/88818791-191ac480-d18d-11ea-9c82-755e0c61440d.png">

The first plot (loss graph) shows that the training loss went down for the most part, while the validation loss went down from 2 to 4 and again from 4 to 6, but then spiked up from 6 to 10. This is a very clear sign of overfitting. The model worked well on the training data, but once the validation data was introduced the model overfitted greatly. The second plot (accuracy graph) shows that the training accuracy went up for the most part, while the validation accuracy fluctuated greatly. The accuracy went up from 2 to 3 and from 5 to 6, but spiked down from 3 to 5. As I said before, this is a clear sign of overfitting.  



D.Text Classification with an RNN


1.

<img width="452" alt="Screen Shot 2020-07-29 at 7 54 59 AM" src="https://user-images.githubusercontent.com/60228365/88818801-1c15b500-d18d-11ea-9b35-045ad637d277.png">


<img width="450" alt="Screen Shot 2020-07-29 at 7 55 08 AM" src="https://user-images.githubusercontent.com/60228365/88818808-1e780f00-d18d-11ea-94d6-2d40b3098bb8.png">


<img width="438" alt="Screen Shot 2020-07-29 at 8 10 24 AM" src="https://user-images.githubusercontent.com/60228365/88818815-20da6900-d18d-11ea-9e7a-caf4e7f225dc.png">


<img width="431" alt="Screen Shot 2020-07-29 at 8 10 39 AM" src="https://user-images.githubusercontent.com/60228365/88818817-22a42c80-d18d-11ea-8807-6000043a293d.png">


The first plot (accuracy graph) showed that both the validation and training accuracy both began to plateau at the 3rd epoch (the training accuracy increased slightly but very slightly). This is also a big sign of overitting. The second plot (loss graph) shows a very similar story in that the training loss decreased from epoch 0 to epoch 6, but the validation loss decreased drastically from 0 to 1, but then began to plateau and slightly increase from 4 to 6. This can also be a sign of overfitting. The bottom two graphs have LSTM layers included. I think that these graphs look very similar to the original accuracy and loss models without LSTM layers, meaning that the graphs still show overfittness, even with the additon of the LSTM layers.    
