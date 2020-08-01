# Responses 

## 1) 
CNN: 
sentence = ["four tech titans face grilling over their dominance", "gop congressman who frequently refuses to wear a mask tests positive", "kendall jenner opens the doors to her bohemian la home", "Some kids are scared theyll get sick at school", "obamas reflect on how they used elite education and access to help empower their communities"]

[[2.2702990e-05] - 
 [3.1110308e-01]
 [8.0594087e-14]
 [1.1602519e-01]
 [5.6418092e-09]]
 
 
 FOX NEWS:
 sentences = ["karl rove previews joe biden's top vp contenders", "Preliminary study investigates how coronavirus particles may travel in classrooms, indoor areas", "NYC man fatally shot inside Staten Island deli in front of customer", "Man shocked to find late mother's lost wedding ring in the garden after 34 years", "Taller people face higher risk of catching COVID-19, survey says"]

[[8.3203786e-06]
 [1.7339656e-01]
 [7.3055789e-18]
 [1.7867841e-01]
 [3.8097411e-10]]
 

 FRANCE24:
 sentences = ["‘The birds have landed': French-made Rafale jets arrive in India amid China tensions", "Trump retweets viral video of doctor saying US government is run by 'reptilians'", "Postcard provides clue to exact spot of Van Gogh’s last painting, says researcher", "Five US states report one-day records for Covid-19 deaths", "French cinemas look to stay afloat amid Covid-19 drought of Hollywood blockbusters"]

[[2.7390050e-05]
 [1.9859433e-01]
 [1.4524075e-11]
 [6.7119390e-02]
 [3.0054558e-08]]
 
 The Babylon Bee:
 sentence = ["Dr. Fauci Recommends Encasing Your Entire Body In Bubble Wrap To Protect Against Coronavirus", "Nation Approves Plan To Push Hollywood Into Pacific Ocean", "Congress Members To Wear Barcodes So Lobbyists Can Scan Prices, Self-Checkout", "Man Who Gets Coronavirus Relieved He Can Finally Touch His Face All He Wants", "Founding Fathers Strapped Down In Graves To Prevent Further Spinning", "Aliens Report No Intelligent Life On Earth After Landing In Portland", "Millennial Drops Support For Socialism After Learning How Hard It Is To Get Avocado Toast In Venezuela"]

[[9.9886167e-01]
 [9.9995244e-01]
 [9.9997568e-01]
 [9.9946576e-01]
 [9.9953842e-01]
 [8.1983793e-01]
 [3.2602070e-20]] 
 
 
I began by choosing some of the most commmon new sources today such as CNN, Fox news, and FRANCE24. Many of the articles I chose were not sarcastic and the model was able to predict these correclty. However, there were a couple headlines that did have very sarcastic titles that the model was not able to catch. I then chose a news source that is known to have satirical headlines: The Babylon Bee. I was very surprised by how well the model was able to distinguish these sources! As you can see above, all of the headlines I chose under The Babylon Bee were very sarcastic and the model predicted 6 our of the 7 articles correclty (as sarcastic). I was shocked to see that one of the most sarcastic headlines ("Millennial Drops Support For Socialism After Learning How Hard It Is To Get Avocado Toast In Venezuela") was deemed non-sarcastic by the model. However, for the most part the model did a good job of distinguishing between sarcastic and non-sarcastic headlines.  
 
 
 ## 2) 
 
This model works in a very interesting way, in that it begins without knowing a single word, but learns new words each time the model is run. The model is trained in batches of 100 characters, and with each run it becomes familiar with more and more words. The model is made up of three different layers: an input layer, an RNN layer, and and output layer. The loss function used is the sparse_categorical_crossentropy function and the optimizer used is Adam. The generate_text function is built on the basis of the RNN using informaiton it has learned from one character, to come up with a meaningful prediction for the next character. I think that the model did imporove from the first run to the second run. It seemed that there were a lot of words spelled wrong in the first run, and although there were words spelled incorrectly in the second run as well, I think that the second run did make (slightly) more sense. In conclusion, the second run was able to replicate the first run pretty well in terms of coherance, with slight improvement.     
 
 #### First time running generate_text() command:
 
 ROMEO: Norboly us,
We time on the contrast upon my knees redeyman.

BIANCA:
Farewell; my lord
Hastings on the spotes from the father with a banishmy, come
Is all these plause west.

NORTHUMBERLAND:
These pleasurthere from by you,--
That we banis high spides; if that the
dukes he is Old Twomach you sway, once have
do better stwear, and so your spirits cold feigned
May compain with trurions, welcome.

SICINIUS:
I say it is, I
know now? a, shall I reis and knows not fears;
It was the need slaves a subject storm;
And if thou that envious Capulet,
Sister!---

SICon,
While earth too.

MIRAPDWAR:

JOHN OF GAUNT:
That is his very heart; and how he art thou
shalt doth.

Messenger:
The people and weepand minteers in prisoner.

DUCHESS OF YORK:
What, art chattest there?

MENENIUS:
Better; if, come.

POLIXENES:
Have you note off from these you are?

QUEEN MARGARET:
Bloody protector far to dine with beholding
Upon the sword of that her brook the world, whose hose be Dized,
A happiness, sire, a man can of 

#### SECOND TIME RUNNING:

ROMEO: You will brought when he hath
A be o' the gods, much grows there want these the king?

DUKE VINCENTIO:
Well, would your ignory?

WARWICK:
The end o' judgm'd it, and your honours
Embrach with a numb' bunisle you:
'Tis fled the men of choose well talk outward.
Mummile up my body: be you
with him! be good and friends, then plasubed my letters; although I be given it would weep,
The next watharing tedood of you. We'll buly
But conduct his cares your hands.

POLIXENES:
Here's not yours, from arch, or when myself with
Any showers gave: boldly naked, nor look upon: he slew her?
Dool the day o' the season were knot with crowns death.

GLOUCESTER:
The geerest loving-sake drunk.

RICHARD:
Who had not send to speak there is on calo.

CORIOLANUS:
You to disgraced there.

ESCALUS:
To shrip the day, wheress of all the great sorrow.

BENVOLIO:
Look, the gods,--meam not out of his son,
Enturious lord, you're tell's the wooft;
O, thence thou art deceiving a lay my water!

CAPULET:
Come, crades! my mast


## 3) 

The first setence I picked was "me gusta tu casa." (I like your house). This setence was translated perfectly!

<img width="668" alt="Screen Shot 2020-07-31 at 10 43 20 PM" src="https://user-images.githubusercontent.com/60228365/89092387-6fe7f000-d37f-11ea-99b1-3c3617501d93.png">

The second setence I picked was "¿Cómo esta el clima hoy?" (How's the weather today?). This setence was almost perfect but left out "today".

<img width="679" alt="Screen Shot 2020-07-31 at 10 43 36 PM" src="https://user-images.githubusercontent.com/60228365/89092389-71b1b380-d37f-11ea-9713-b8d6e6de87f6.png">

The last sentence I picked was "¿pusiste el pollo sobre la mesa para la cena?" (Did you put the chicken on the table for dinner). This translation made me laugh because it was completley incorrect. The model translated the setence to "do cats lock the cup".

<img width="662" alt="Screen Shot 2020-07-31 at 10 43 47 PM" src="https://user-images.githubusercontent.com/60228365/89092390-737b7700-d37f-11ea-8737-85d417c83a01.png">

I was surprised by the accuracy of the model. It seemed that it was able to correctly translate simple setences, but once the sentences became slightly more complex, the model really struggled to produce the correct translation. This idea can be seen clearly with the last sentence I used. 
