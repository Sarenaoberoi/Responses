### Responses- July 28
Why is using one-hot encoding an inefficient towards vectorizing a corpus of words?  How are word embeddings different? 

As talked about in the tensorflow exercise and Lawrence Maroney's video, one-hot encoding is an interesting (but somewhat inefficient) way to encode words. With one-hot encoding, one goal is to keep a uniform length, so each word will have 0's up until the word (and a 1 for the word). For example, if the sentence was "I love apples", one-hot encoding would look something like this:

         i --- love---- apples
i        1      0         0 

love     0       1         0

apples   0       0          1


2.Compile and train the model from the tensorflow exercise.  Plot the training and validation loss as well as accuracy.  Post your plots and describe them

D.Text Classification with an RNN


1.Again compile and train the model from the tensorflow exercise.  Plot the training and validation loss as well as accuracy.  Stack two or more LSTM layers in your model.  Post your plots and describe them.
