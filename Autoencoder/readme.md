# Autoencoder Summary

<img src="https://4.bp.blogspot.com/-oUcusrWxk2U/WkntSbY7EQI/AAAAAAAAXHM/SzJ7vLUDu4U0IV5QfxQj-6W78h6-JUfSwCLcBGAs/s1600/4110_2.PNG" width="500" height="300">

Autoencoder is useful in extracting latent representation of high dimensional data, and with latent space visualization, we can see how the original data is distributed with new learned features. Most importantly for my case, not with this dataset though, but with the images I'm currently working on at my company, this technique could be used to detect anomalies if together we implement clustering or other outlier techniques such as isolation forest or local outlier factor.

Before building autoencoder models, first let's take a look at how data points are distributed in high dimensional space. Use t-SNE(t-distributed Stochastic Neighbor Embedding) to help visualize high dimensional data.

![1](images/tsne.png)

We can see there are obvious clusters that separate digits apart from different ones, which indicates linear separability in high dimensional space. Next, let's see if autoencoders are able to do anything good to keep the clusters while compressing the data into only 2 dimensions.

First we compare model without hidden layers with those with single hidden layer of size 400 and 256 respectively.

No Hidden|400|256|
:---:|:---:|:---:|
![1](images/clusters_None.png)|![2](images/clusters_400.png)|![3](images/clusters_256.png)|
![4](images/digits_None.png)|![5](images/digits_400.png)|![6](images/digits_256.png)|