# Semi-Supervised Learning with Deep Convolutional Generative Adversarial Networks
Architecture:

<img src="https://gluon.mxnet.io/_images/dcgan.png" width="500" height="300">

Generative adversarial network(GAN in short) is a very interesting topic in deep learning nowadays, and its wide range of applications have been explored and proved to present incredible performance. In this notebook, I'm using DCGAN to implement semi-supervised learning, which only uses rather small number of labeled data but is able to learn robust features and generalize well on unseen data. As for why semi-supervised learning? In the real world, especially now and in the future, as more and more data is getting collected, some or even most of them will come without labels, and that's when semi-supervised learning comes in to play.

First, let's see how number of epochs can affect the learning process.

|20 epochs|
|:---:|
|![](images/epoch_20.png)|
|100 epochs|
|:---:|
|![](images/epoch_100.png)|
