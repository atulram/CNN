**Name** :  Atul Ram

**Batch number** :  Batch 1

**Registered email** :  atul.13977@gmail.com

----------------

### 1. Convolution

Convolution is a mathematical operation which is used in variety of fields like signal processing, image processing, etc. At its core convolution simply means multiplying two functions/signals/matrices to produce third function/signal/matrix. It can be represented as  __g(x,y) = h(x,y) * f(x,y)__ where __*__ is the convolution operator. In convolutional neural network we convolute the input matrix at any layer with the kernel to get the output matrix or the next layer. Below image will make it clear.

![convolution](https://i.imgur.com/HsbwnM7.png)

### 2. Filters/Kernels

Filters/Kernels generally are the small sized matrices with which the input image is convolved to get a modified image. In image processing, kernels are used to sharpen, blur or perform similar tasks on the input image. In CNN, kernel/filter refers to the weight matrix which is convolved with the entire input image generating matrices which when activated gives the next layer. Gradually when the network learns, these kernels become capable of filtering features such as an edge or curve. Below example shows a kernel.

![kernel](https://i.imgur.com/R4FclEN.jpg)

### 3. Epochs

Machine learning models learn from the data set which we provide.When our model goes through all the data points in our data set, processes and learns from them, we call it as one epoch.For large datasets, processing all the images in one go becomes computationally difficult,so we divide our data sets into random batches.Once all the batches are fed forward and the errors back propagated, one epoch is completed.If epoch is set to 100, the model processes all the data points in the dataset 100 times to complete training.

### 4. 1X1 convolution

When an input tensor is convoluted with a 1X1 kernel,its height and width remains the same but its depth or the number of channels changes.Hence a 1X1 kernel can be used:

- To increase or decrease the depth of input tensor.When depth isn't changed its used to add a non linearity to the model

- To reduce the number of channels thereby reducing number of parameters and prevent overfitting

Below image gives the idea of dimension reduction using 1X1 kernel

![1x1conv](https://i.imgur.com/HmLcwkm.png)

### 5. Activation Function

Activation Function is an essential part of a neural network and serves 3 purposes

- The output of the convolution between input and kernel is passed to an activation function which decides what information should be sent forward to the next layer or in other words it decides the activation of the next layer.
- It introduces non-linearity so that our model learns complex functions
- Since it is differentiable,it helps the model to learn from backpropagation of errors

sigmoid,RELU,softmax, etc are the examples of activation functions.

![activationFunctions](https://i.imgur.com/r61z1Cx.png)