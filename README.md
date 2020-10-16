# One shot learning
  

You only have to pass your image one time and thats it.Next time it will automatically recognize your face.
  

Here i am using a pretrained model vgg-face.mat that has been trained on millions of images on an angorithms called triplet Loss.
  

# About Triplet Loss
  
In Siamese networks, we take an input image of a person and find out the encodings of that image, then, we take the same network without performing any updates on weights or biases and input an image of a different person and again predict it’s encodings. Now, we compare these two encodings to check whether there is a similarity between the two images. These two encodings act as a latent feature representation of the images. Images with the same person have similar features/encodings. Using this, we compare and tell if the two images have the same person or not.
  
You might be wondering, how to actually train the network? you can train the network by taking an anchor image and comparing it with both a positive sample and a negative sample. The dissimilarity between the anchor image and positive image must low and the dissimilarity between the anchor image and the negative image must be high.

  
![alt text](https://github.com/sachin327/Face_Recognition_Using_vgg-face.mat/blob/main/triplet_loss_image.png)
  
# Loss Function
  
![alt text](https://github.com/sachin327/Face_Recognition_Using_vgg-face.mat/blob/main/triplet%20loss.svg)
  
![alt text](https://github.com/sachin327/Face_Recognition_Using_vgg-face.mat/blob/main/loss_triplet.svg)
