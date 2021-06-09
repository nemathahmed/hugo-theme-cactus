---
title: AI Learns to Multiply in 20 Seconds
date: 2020-06-19 09:00:00
tags:
    - Deep Learning

category: Technology 
keywords:
    - Deep Learning
    - AI
mathjax: true
---

### AI Learns to Multiply in 20 Seconds

#### How quickly and accurately can AI learn multiplication?

> Today, Artificial Intelligence is accomplishing tasks that were once assumed to
> be past human aptitudes. Right from detecting Retinopathic eye to
life-threatening tumors, AI is soon becoming capable of all complex tasks out
there.

> Today we run downhill and see how AI performs at one of the most simple tasks
> for modern computers: Multiplication.

![](https://cdn-images-1.medium.com/max/1800/1*EpLVXD5q6qgcwHr5WEbTBw.png)


In this post, we will try to teach a machine learning model to multiply and see
how it performs. The post will be more inclined towards the beginner side of ML
with minimum code(14 lines to be precise).

Disclaimer: In real life, you would never want an ML algorithm to perform
multiplication for you. The post just walks you through an experiment to try and
build a machine learning model that does arithmetic. Let’s get started.

Our goal here is to develop a model that takes an integer number as an input and
gives out an output which is the input multiplied with some number, let’s take
this number to be 5. So, if you give in 10 as input, you must expect 50 as the
output. Do perceive that we are not going to tell the model that the task we are
looking for is a simple multiplication; it has to figure it out on its own.

![](https://cdn-images-1.medium.com/max/1200/1*At95dUAtP7GegmerbTEX1A.png)
<span class="figcaption_hack">Image by Author</span>

### First things first

The first job for us will be to create an example dataset by looking at which
the model can learn that the task we are looking for is multiplication by 5. We
will use 10k randomly generated data points between 1 and 300. So we have 10k
input data points [20,120…..5,15] and 10k output data points [100,600…..25,75]
i.e., input points multiplied by 5. The code for the same in Python is given
below.

    import random
    X=[]
    Y=[]
    for i in range(10000):
        n = random.randint(0,300)
        X.append(n)
        Y.append(n*5)

    #X is the input array and Y is the output array

Bingo! We have the dataset ready. Now, let us design a Neural Network that can
learn our task. An essential textbook ANN design looks something like the
figure(Fig.1) below with many hidden layers and many neurons in them, but that’s
for complex tasks such as digit classification. For our simple multiplication
task, a simple neural network with just one hidden layer and with one hidden
neuron might just work.

![](https://cdn-images-1.medium.com/max/1200/1*6kJCmu7qwE8G_EUqzMjuGQ.png)


### Architecture time

Let’s write the code for the architecture in Fig 2. and see if the model can
learn multiplication by 5. We use Keras, a high-level ML library, on top of
Tensorflow. We understand that the architecture that we are trying to build is a
straightforward sequential network. We add a Dense layer with one neuron, which
will be our hidden layer, and we then add one more layer with one neuron, which
will hold our output answer. We use ‘relu’ optimization function for all
neurons.

We use Mean Squared Error to see the error between the model predictions and the
ground truths at each step and optimize our loss using ‘Adam’ optimizer. The
‘metrics’ parameter, when enabled, shows the stats of your model while training.
Architecture is set, and now the model is all ready to learn. We finally use the
model.fit() function where the model tries to understand the relation between
input and output.

We pass on the input(X), output(Y), the batch size: number of data points to
look before resetting the model weights & biases, validation split: the fraction
of dataset used for validation and epochs: number of times model goes through
the entire set.

    from keras.models import Sequential #using Keras Library
    model=Sequential()
    model.add(Dense(1,activation='relu',input_shape=(1,)))
    model.add(Dense(1,activation='relu'))
    model.compile(loss='MSE', optimizer='adam', metrics=['accuracy'])
    model.fit(X, Y, batch_size=50,
                  validation_split=0.1, epochs=100, verbose=1,shuffle=1)

Let’s look at some stats that were printed while the model was being trained.

    #From 10k samples, since validation_split=0.1, we trrain on 0.9*10k i.e. 9k samples.

    After First iteration
    Epoch 1/100
    9000/9000 [==============================] - 1s 148us/step - loss: 625973.1757 - acc: 0.0038 - val_loss: 577468.6391 - val_acc: 0.0020

    After 74th iteration
    Epoch 74/100
    9000/9000 [==============================] - 0s 24us/step - loss: 0.0723 - acc: 0.9583 - val_loss: 0.0595 - val_acc: 1.0000

Look at the accuracy difference between the 1st and 74th steps. The accuracy was
0.0038 or 0.38% at the start concluding that the model had no idea what the
relation between inputs and outputs was at the beginning. The loss is also huge
at the start. As the training continues, the model starts making sense of data,
and the accuracy improves, and the loss(error) is reduced.

After the 74th step, the model had an accuracy of 0.9583 or 95.83% i.e., it was
able to tell with 95.83% surety that the task was multiplication by 5. We can
see that validation loss also improved from 0.20% to 100% within 74 iterations.
After 100 iterations, both the training accuracy(acc) and validation
accuracy(val_acc) reach 100%, stating that our model successfully discovered
that the relationship was multiplication by 5.

*The training process takes around 20 seconds to complete 100 iterations on an
NVidia 940 MX 4 GB GPU coupled with 16 GB RAM. That’s speedy learning indeed.*

### The Results

Finally, it’s time to test our model. Let’s take any five numbers in a
test_array and use the model built above to get the predictions. Ideally, the
output should be test_array elements multiplied by 5.

    test_array=np.array([4,27,100,121,9])
    print(model.predict([test_array]))

*Drum rolls! Time for the final predictions.*

    [[19.9995174407959], [134.9995880126953], [499.9997253417969], [604.9998168945312], [44.99952697753906]]

We see that our model is almost there. The actual values are
[20,135,500,605,45], and if the predictions are rounded off to two decimal
places, we see that the predictions are the same as the expected results.

![](https://cdn-images-1.medium.com/max/1200/1*n6hTDmetNQ1uvCdi69WAWQ.png)


So there you have it, a simple AI that has now learned multiplication by 5.
There are still some things; however, to be considered: try giving negative
values and check the output, what do you get? I would like to leave it to you to
try, experiment, and come up with techniques to make the algorithm more
accurate. Also, try making changes to the architectures, such as adding more
layers and neurons, and look at the difference in metrics. Do let me know in the
comments if you have any queries.

*****

I hope you liked the post and fancied building an AI that is programmed to
perform quite a simple task of multiplication. See you next time.
