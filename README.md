# cnn_scratch

Classic CNNS get over-representation because they are not sampled - just include all redundant pixels 
Start with MNIST then extend to colour images

Convolutional - how the shape o one function is modified by the shape of another function = Slide shape over image, the more it contributes to influencing the image, the closer to 1 the value is 

Steps for a convolution:
1. Multiply each image pixel by a weight and then by filter pixel (dot product)
2. Add them up
3. Divide by total number of pixels in the filter

In order to speed up calculations, a layer usually processes multiple images at once. Therefore, we pass a four-dimensional tensor with shape [n, h_in, w_in, c] as an input. Here n corresponds to the number of images processed in parallel — so-called batch size. The rest of the dimensions are quite standard — width, height, and the number of channels.

 The most important rule, in that case, is that the filter and the image must have the same number of channels. (For colour images)

 The main task of the pooling layer is to reduce the spatial size of our tensor. We do this to limit the number of parameters that we need to train — shortening the whole training process. 