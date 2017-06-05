# CNN_digit_recognizer
How I got 99% accuracy on the digits recognition dataset on Kaggle using a modified version of Jason Brownlee's CNN.

I used the dataset from Kaggle: https://www.kaggle.com/c/digit-recognizer/data.

After reading a bunch of tutorials and other materials, I adjusted Jason Brownlee's CNN to get an accuracy of 99%. I highly recommend his blog, as it is loaded with the good stuff; not only that the dude knows what he's talking about but he explains complicated notions with ease so that anybody can follow. http://machinelearningmastery.com

I am a novice in ML and programming in general; until a year ago, python was just a big snake to me. If I make mistakes or end up at the wrong conclusion, please feel free to correct me as I want to learn as much as I can.

I did all the tutorials on Kaggle, the Analytics Vidhya model (with Keras and Tensorflow), worked throught the TensorFlow tutorial, even tried a bit of VGG16 on the dataset. My first good results came with multi-layer perceptron in Keras, where I did some pre-processing on the data as numpy arrays and used the following model:
- conv, conv, maxpool, conv, conv, maxpool, conv, maxpool, flatten, dense, dropout, dense(with 10 classes, 0-9, and softmax activation)
- the activation was relu for the conv and the first dense; i used Adam as the optimizer for this model. This model gave me 97% accuracy.

I tried some image data augmentation with Keras, different combination of algorithms but I got worst results and I moved to another CNN.
(I might have been doing something wrong).

This is the final CNN that I've tried and it gave me a 99% accuracy; as I stated above I used Jason Brownlee's model as it provided what i was looking for: less hidden layers and more depth.

Once I have more knowledge, I might come back and try to get the last 1 %.
