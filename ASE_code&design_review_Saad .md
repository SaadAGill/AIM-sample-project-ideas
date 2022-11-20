# Facial Recognition

## Abstract

In recent times, facial recognition technology has advanced by leaps and bounds. You can identify the gender, ethnicity and expressions of  . My goal is to correctly identify and pair a human's expression.

## Detailed Description

We use a series of pictures as the input to perform forward propogation. Moreover, back propogation algorithm will be used to update the value of parameters until the input images can be classified correctly as much as possible.

### Datasets
![alt text](2.png)

The size of the file is 1.95 GB. It contains 70,000 files, the format of which is PNG. The resolution of the files is 128x128. The link of the dataset is shared below.

[Get Here](https://drive.google.com/drive/folders/1tg-Ur7d4vk1T8Bn0pPpUSQPxlPGBlGfv)

### Arcitecture Proposal
![alt text](1.png)

The method is to give an original value to the conventional kernels which have 3x3 size.

We will use the kernels to cover different human expressions in the selected pictures. At the moment each of the Kernels is mapping with the 9 pixels of the picture. 

The next step would be the convolution of the picture by the Kernels. 

After convoluting several times, pooling and activating would take place. 

Next, we'll get the picture which will be opened up to form the input of the fully-connected layers.

Furthermore, we use the fully-connected neural networks to classify the image.

The accuracy rate may be low in the beginning so we will have to use the gradient decline algorithm to train the model that is to update the weight parameters each time we select the batch of the pictures.

Lastly, we'll get a well trained classification model.



## References

Agrawal, P., Girshick, R., & Malik, J. (2014). Analyzing the performance of multilayer neural networks for object recognition. In ECCV (pp. 329–344)

Chellappa, R. (2016). The changing fortunes of pattern recognition andcomputer vision. Image and Vision Computing, 55, 3–5.

Liu, Li, et al. “Deep Learning for Generic Object Detection: A Survey.” International Journal of Computer Vision, vol. 128, no. 2, Feb. 2020, pp. 261–318. Springer Link, https://doi.org/10.1007/s11263-019-01247-4.

