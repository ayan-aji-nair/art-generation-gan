# Art Generation GANs
Experimenting with DCGANs for generating various kinds of art. 

## Model Architecture
The architecture used in this DCGAN implementation is drawn directly from the [DCGAN research paper](https://arxiv.org/abs/1511.06434) and the [PyTorch DCGAN tutorial](https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html). 
![alt text](https://pytorch.org/tutorials/_images/dcgan_generator.png)

The input to the generator is a 100-dimensional random latent feature vector, which goes through a series of convolutional transpose layers to generate a 64x64 colored image. For 128x128 image generation, one extra convolutional transpose layer is added. 

The discriminator takes a colored 64x64 image as input and outputs a probability that corresponds to the authenticity of the inputted image. Similar to the generator, one additional convolutional layer is added to the discriminator to allow it to classify 128x128 images. 

All hyperparameters, like latent feature vector size, learning rates, batch sizes, and feature map sizes were drawn directly from the DCGAN paper. 


## Datasets
[Find the Ancient Chinese Art dataset here](https://github.com/ychen93/Chinese-Painting-Dataset/blob/master/data.zip)

[Find the Van Gogh Paintings dataset here](https://www.kaggle.com/ipythonx/van-gogh-paintings)

Note about the Ancient Chinese Art dataset - the zip file for this dataset contains two copies of the same data, with one copy formatted for MacOSX. 


