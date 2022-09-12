# Image recommendation algorithm for new users

Task: 
There is a telegram bot with an meme-image recommendation system based on watched memes. We need to make a recommendation for new users we havn't data.

Solution:
I use clusterization alhgorithm KMeans to separate objects into classes. 

![изображение](https://user-images.githubusercontent.com/74490203/189728826-e32f8b16-0f42-4812-aff0-dd347c5f33e0.png)

Elbow method shows that optimal number of clusters = 3.
Then we need to see like/dislike ratio in each cluster.

![изображение](https://user-images.githubusercontent.com/74490203/189729435-f0c5f6c0-a36f-4d8e-8e92-cdfb5d5d2244.png)

The highest quality cluster is 1. So, we need to recodend top-10 images in that cluster.

Testing of the algorithm showed a better recommendation of images, in contrast to the "take the most liked pictures" method.
