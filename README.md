# Melanoma-Detection-Assignment
Upgrad's Melanoma detection code for skin cancer.

# Setup the CUDA and CUDANN alongwith the tensorflow required for GPU usage.
## For windows we have to install the CUDA toolkit from the NVIDIA site.
## Transfer the libs, include and bins from CUDANN to the CUDA folders.
## Here we used 11.2 CUDA and 8.2 CUDANN, and tensorflow 2.8.0.
## 

# Steps are very simple post the installation of the components:
## Get the paths of the train and test data in the python
## Get the images from the folder directly frm the dataset.
## Scale the images to H * W: 180 * 180 image size.
## Create the RGB model layers to build the base layer.
## Convert the pixel value of 255 to 1, rescaling.
## Then make the convolution layers.
## Add the pooling under them.
## Flatten them into one vector.
## Then try putting the dense layers with the activation function.
## **The dropouts are optional in case we wanna plug in to help the fitting.

## Once the sequential layer is ready and we can view the summary as how many trainable and non trainable parameters will be there, move to fitting.
## Choose an optimizer and the loss function which will be used to train the model.
## Once we are done, we have both train ds and validation ds which we can use to check the progress of our model.

# Try checking the data augmentation and imbalance in check which may work in favor of the predictions.
## At the very end try to test the model on the test images and try producing a csv.
