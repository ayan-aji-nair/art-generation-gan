# Art Generation GANs


## Model Architecture
The architecture used in this DCGAN implementation is drawn directly from the research paper and the PyTorch DCGAN tutorial. 
![alt text](https://pytorch.org/tutorials/_images/dcgan_generator.png)




## Datasets
The Ancient Chinese Art dataset can be found here: https://github.com/ychen93/Chinese-Painting-Dataset/blob/master/data.zip
The Van Gogh dataset can be found here: https://www.kaggle.com/ipythonx/van-gogh-paintings 

The Chinese Art data contains two sets of the same images; one for MacOSX and another folder for windows. The MacOSX folder is not necessary - deleting this folder and re-zipping the file allows for the model to run quickly.


