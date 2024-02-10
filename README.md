# Monochrome to Mosaic: Decoding Color with Encoding Power
Built and trained an autoencoder neural network in Keras with TensorFlow as backend. Autoencoder stores the input image representation in the latent space with very few dimensions compared to the input image.
The Decoder block of autoencoder consists of an output layer that gives the reconstructed image and some hidden layers, generally a combination of Convolutional Transpose Layers and Upsampling layers. In the Decoder block, the autoencoder learns the reconstruction of the original image from the previously learned latent space.
In this project, tweaked the Autoencoder Neural Network in such a manner that while training, we input Grayscale Images and set the output as their corresponding color images. In this way, the autoencoder layers would learn how to convert the latent space representation of grayscale images into colored images. For the Encoder, chose a pre-trained VGG16 model trained on ImageNet Dataset to classify 1000 classes. For the decoder part of the autoencoder, to upsample the latent representation up to the size of the original image used UpSampling Layers.
The project performed significantly well on converting grayscale images to colored rgb images. Some of the results can be seen below:

![image](https://github.com/Mudit-123/Monochrome-to-Mosaic/assets/78809022/13772afb-c9c1-4ddd-9d0a-31c14c2bdd07)
![test_dog_1](https://github.com/Mudit-123/Paint-it-/assets/78809022/aeba3c05-32b9-4d6e-a307-0f76cd79e887)
![test_flower_1](https://github.com/Mudit-123/Paint-it-/assets/78809022/5d1f2905-b480-4dd4-acfb-691ee6271168)
![test_car](https://github.com/Mudit-123/Paint-it-/assets/78809022/11f54839-b5f3-4d69-9dfc-253fd952156e)

