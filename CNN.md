# CNN notes

## QML person said work with tensors was very popular in QML right now - maybe sme of that work applies here  

Tensor = generalisation of a matrix to higher dimensions

Image is a matrix of R**HXQ so a HXW image where each pixel is a value between 0 and 255.

However because three channels of colour we have 3 tensor of Height X width X Channels - This is used with the convolution filters or kernels to give a 3 tensor output representing spatial size and number of dimensions

A CNN is composed of 4 main procedures, compiled and repeated in any order : Convolution layers,
most often followed by an Activation Function, Pooling Layers and some Fully Connected layers at the end. We will note ` the current layer.

source: https://fr.mathworks.com/solutions/deep-learning/convolutional-neural-network.html For diagram of CNN

Page 5 of QCNN paper for instructions on what a CNN does


Usually, a network utilizes more than one filter per layer. When that is the case, the outputs of each filter’s convolution over the input image are concatenated along the last axis, forming a final 3D output.

Filters are your features going to the next layer - more features = more complex network with more parameters going to next network - this will be the channel dimension

When the feature is present in part of an image, the convolution operation between the filter and that part of the image results in a real number with a high value. If the feature is not present, the resulting value is low.

Each filter gives you a certain feature for it to look for

An added benefit of max pooling is that it forces the network to focus on a few neurons instead of all of them which has a regularizing effect on the network, making it less likely to overfit the training data and hopefully generalize well.


After this:
Check CNN is next module
Start building CNN frm scratch t understand

