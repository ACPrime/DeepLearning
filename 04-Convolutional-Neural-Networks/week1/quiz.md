# The basics of ConvNets
Quiz, 10 questions
## 1. Question 1
What do you think applying this filter to a grayscale image will do?

![](https://latex.codecogs.com/gif.latex?%5Cbegin%7Bbmatrix%7D%200%26%201%20%26%20-1%20%26%200%5C%5C%201%26%203%20%26%20-3%20%26%20-1%5C%5C%201%26%203%20%26%20-3%20%26%20-1%5C%5C%200%26%201%20%26%20-1%20%26%200%20%5Cend%7Bbmatrix%7D)

- [ ] Detect 45 degree edges

- [x] Detect vertical edges

- [ ] Detect horizontal edges

- [ ] Detect image contrast

> Because the left part is positive, and the right part is negative.

## 2. Question 2
Suppose your input is a 300 by 300 color (RGB) image, and you are **not** using a convolutional network. If the first hidden layer has 100 neurons, each one fully connected to the input, how many parameters does this hidden layer have (including the bias parameters)?

- [ ] 9,000,001

- [ ] 9,000,100

- [ ] 27,000,001

- [x] 27,000,100

## 3. Question 3
Suppose your input is a 300 by 300 color (RGB) image, and you use a convolutional layer with 100 filters that are each 5x5. How many parameters does this hidden layer have (including the bias parameters)?

- [ ] 2501

- [ ] 2600

- [ ] 7500

- [x] 7600

## 4. Question 4
You have an input volume that is 63x63x16, and convolve it with 32 filters that are each 7x7, using a stride of 2 and no padding. What is the output volume?

- [x] 29x29x32

- [ ] 16x16x32

- [ ] 29x29x16

- [ ] 16x16x16
> n = 63, f = 7, s = 2, p = 0, 32 filters.
## 5. Question 5
You have an input volume that is 15x15x8, and pad it using “pad=2.” What is the dimension of the resulting volume (after padding)?

- [ ] 17x17x10

- [x] 19x19x8

- [ ] 19x19x12

- [ ] 17x17x8

## 6. Question 6
You have an input volume that is 63x63x16, and convolve it with 32 filters that are each 7x7, and stride of 1. You want to use a “same” convolution. What is the padding?

- [ ] 1

- [ ] 2

- [x] 3

- [ ] 7

## 7. Question 7
You have an input volume that is 32x32x16, and apply max pooling with a stride of 2 and a filter size of 2. What is the output volume?

- [ ] 15x15x16

- [ ] 16x16x8

- [x] 16x16x16

- [ ] 32x32x8

## 8. Question 8
Because pooling layers do not have parameters, they do not affect the backpropagation (derivatives) calculation.

- [x] True

- [ ] False

> Go to [this page](https://www.slideshare.net/kuwajima/cnnbp) for further information.

## 9. Question 9
In lecture we talked about “parameter sharing” as a benefit of using convolutional networks. Which of the following statements about parameter sharing in ConvNets are true? (**Check all that apply.**)

- [x] It reduces the total number of parameters, thus reducing overfitting.

- [x] It allows a feature detector to be used in multiple locations throughout the whole input image/input volume.

- [ ] It allows parameters learned for one task to be shared even for a different task (transfer learning).

- [ ] It allows gradient descent to set many of the parameters to zero, thus making the connections sparse.

## 10. Question 10
In lecture we talked about “sparsity of connections” as a benefit of using convolutional layers. What does this mean?

- [ ] Regularization causes gradient descent to set many of the parameters to zero.

- [ ] Each filter is connected to every channel in the previous layer.

- [x] Each activation in the next layer depends on only a small number of activations from the previous layer.

- [ ] Each layer in a convolutional network is connected only to two other layers



