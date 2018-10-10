
# EIP-2 Assignment 1
------------

![image-20181005193104038](https://www.richardvanhooijdonk.com/wp-content/uploads/2018/04/shutterstock_705165757-min.jpg)


Name : Purushotham Pushpavanth


Batch # 7


##### Convolution:

It is important to learn convolution so that you will be able to behaviour of certain types of outputs just by looking at the input signals. It also explains how truncating/windowing a signal affects the resolution of key features in the frequency domain in signal processing.

Convolution is multiplying 2 singals in frequency domain i.e. the Fourier representation for the product is the convolution of the Fourier representations of the individual signals. 

Convolution can also be discribed as the affect of impulse response of the LTI(Linear Time Invariant) system on the input signals. 
```math
y[n] = \sum_{k=-\infty}^{\infty} h[k] x[n-k]
```
        
      
      
#####  Filters/Kernels

Kernels also known as convolutional matrix which is used in convolution to attain certain output. There are various kinds of kernels based on use cases like blurring, sharpening, embossing, edge detection etc. In image processing a Kernel is a 2-dimensional matrix of numbers whose size and its values can vary depending on use case.
Below is the kernel for gaussian blurring.

```math
\frac{1}{16}
\begin{bmatrix}
1 & 2 & 1 \\
2 & 4 & 2 \\
1 & 2 & 1
\end{bmatrix}
```
    


##### Epoch

Epoch is a hyper parameter which is defined as passing of an entire dataset both forward and backward through the neural network only once completing all batches. To optimise the learning using Gradient Descent method in deep learning with limited dataset is an iterative process. So, updating the weights with one epoch is not enough. As the number of epochs increases, more number of times the weight are changed in the neural network and the curve goes from underfitting to optimal to overfitting curve
```math
1 Epoch = (1 Forward pass + 1 Backward pass) * \frac{total number of samples}{batch size}
```


##### Feature Map

Feature map also known as activation map, is the output activations for a given filter irrespective of the layer. It is called so because it is a mapping of a certain kind of feature found in the image indicating occurrence of feature if activation is high.


##### Feature Engineering
Any field or attribute participating in the training Machine learning model is called feature. The is a process of extracting features by using the knowledge of domain the data is derived from.
Processes involed in feature engineering include brainstorming, deciding, creating features and checking performance of each with the model and improving if needed.

##### 1x1 convolution
1x1 convolution filters can be used to change the dimensionality in the filter space. If `F1>F` then we are increasing dimensionality, if `F1<F` we are decreasing dimensionality, in the filter dimension where `F` is the number of convolutional filters. 1x1 convolutions are used to compute reductions before the expensive 3x3 and 5x5 convolutions




