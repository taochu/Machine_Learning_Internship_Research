# Convolutional VAE Summary

![1](https://cdn-images-1.medium.com/max/2000/1*TOJD69Y8dZsKFEW-21xUPg.png)

Taking advantage of convolutional neural network being widely used in extracting meaningful image features, convolutional variational autoencoder(ConvVAE) learns the probability representation of the original image data and aims to reconstruct or even generate new images by sampling from the learned probability distribution. However, tuning process of ConvVAE can be very cumbersome since it combines the hyperparameters of CNN and VAE. Followings are some of the hyperparameters I've tuned to see the effects they have in terms of reconstruction and latent variable modelling.

Parameters if not tuned:
`intermediate layers sizes = 1000,256`
`filters = [16,32]`
`KL divergence ratio = 0.000001`

- Different Filter Sizes

8,16|16,32|
:---:|:---:|
![1](images/clusters_8_16.png)|![2](images/clusters_16_32.png)|
![3](images/digits_8_16.png)|![4](images/digits_16_32.png)|

- Different Intermediate Layers Sizes

1000-256|1000-256-32|
:---:|:---:|
![1](images/clusters_8_16.png)|![2](images/clusters_8_16-256-32.png)|
![3](images/digits_8_16.png)|![4](images/digits_8_16-256-32.png)|


