# Deep convolutional models

Quiz, 10 questions

## 1. Question 1
Which of the following do you typically see as you move to deeper layers in a ConvNet?

- [ ] ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D) and ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D) increases, while ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D) decreases

- [ ] ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D) and ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D) decreases, while ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D) also decreases

- [ ] ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D) and ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D) increases, while ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D) also increases

- [x] ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D) and ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D) decrease, while ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D) increases

## 2. Question 2
Which of the following do you typically see in a ConvNet? (**Check all that apply.**)

- [x] Multiple CONV layers followed by a POOL layer

- [ ] Multiple POOL layers followed by a CONV layer

- [x] FC layers in the last few layers

- [ ] FC layers in the first few layers

## 3. Question 3
In order to be able to build very deep networks, we usually only use pooling layers to downsize the height/width of the activation volumes while convolutions are used with “valid” padding. Otherwise, we would downsize the input of the model too quickly.

- [x] True

- [ ] False

> 小傻瓜

## 4. Question 4
Training a deeper network (for example, adding additional layers to the network) allows the network to fit more complex functions and thus almost always results in lower training error. For this question, assume we’re referring to “plain” networks.

- [ ] True

- [x] False

## 5. Question 5
The following equation captures the computation in a ResNet block. What goes into the two blanks(*?*) above?

![](https://latex.codecogs.com/gif.latex?a%5E%7B%5Bl&plus;2%5D%7D%3Dg%28W%5E%7B%5Bl&plus;2%5D%7Dg%28W%5E%7B%5Bl&plus;1%5D%7Da%5E%7Bl%7D&plus;b%5E%7B%5Bl&plus;1%5D%7D%29&plus;b%5E%7B%5Bl&plus;2%5D%7D&plus;%3F%29&plus;%3F)

- [ ] 0 and ![](https://latex.codecogs.com/gif.latex?z%5E%7B%5Bl&plus;1%5D%7D), respectively

- [x] ![](https://latex.codecogs.com/gif.latex?a%5E%7B%5Bl%5D%7D) and 0, respectively

- [ ] ![](https://latex.codecogs.com/gif.latex?z%5E%7B%5Bl%5D%7D) and ![](https://latex.codecogs.com/gif.latex?a%5E%7B%5Bl%5D%7D), respectively

- [ ] 0 and ![](https://latex.codecogs.com/gif.latex?a%5E%7B%5Bl%5D%7D), respectively

> ![](https://latex.codecogs.com/gif.latex?a%5E%7B%5Bl&plus;2%5D%7D%3Dg%28z%5E%7B%5Bl&plus;2%5D%7D&plus;a%5E%7B%5Bl%5D%7D%29%3Dg%28W%5E%7B%5Bl&plus;2%5D%7DZ%5E%7B%5Bl&plus;1%5D%7D&plus;b%5E%7B%5Bl&plus;2%5D%7D&plus;a%5E%7B%5Bl%5D%7D%29%3Dg%28W%5E%7B%5Bl&plus;2%5D%7Dg%28W%5E%7B%5Bl&plus;1%5D%7Da%5E%7B%5Bl%5D%7D&plus;b%5E%7B%5Bl&plus;1%5D%7D%29&plus;b%5E%7B%5Bl&plus;2%5D%7D&plus;a%5E%7B%5Bl%5D%7D%29)

## 6. Question 6
Which ones of the following statements on Residual Networks are true? (**Check all that apply.**)

- [ ] Using a skip-connection helps the gradient to backpropagate and thus helps you to train deeper networks

- [x] The skip-connections compute a complex non-linear function of the input to pass to a deeper layer in the network.

- [ ] A ResNet with L layers would have on the order of ![](https://latex.codecogs.com/gif.latex?L%5E%7B2%7D) skip connections in total.

- [x] The skip-connection makes it easy for the network to learn an identity mapping between the input and the output within the ResNet block.

## 7. Question 7
Suppose you have an input volume of dimension 64x64x16. How many parameters would a single 1x1 convolutional filter have (including the bias)?

- [ ] 2

- [ ] 17

- [x] 4097

- [ ] 1

> 64x64x1 + 1 = 4097

## 8. Question 8
Suppose you have an input volume of dimension ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D%5Ctimes%20n_%7BW%7D%5Ctimes%20n_%7BC%7D). Which of the following statements you agree with? (Assume that “1x1 convolutional layer” below always uses a stride of 1 and no padding.)

- [ ] You can use a 1x1 convolutional layer to reduce ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D) but not ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D), ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D).

- [x] You can use a pooling layer to reduce ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D), ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D), but not ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D).

- [x] You can use a 1x1 convolutional layer to reduce ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D), ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D), and ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D).

- [ ] You can use a pooling layer to reduce ![](https://latex.codecogs.com/gif.latex?n_%7BH%7D), ![](https://latex.codecogs.com/gif.latex?n_%7BW%7D), and ![](https://latex.codecogs.com/gif.latex?n_%7BC%7D).

## 9. Question 9
Which ones of the following statements on Inception Networks are true? (**Check all that apply.**)

- [ ] Inception networks incorporates a variety of network architectures (similar to dropout, which randomly chooses a network architecture on each step) and thus has a similar regularizing effect as dropout.

- [x] Inception blocks usually use 1x1 convolutions to reduce the input data volume’s size before applying 3x3 and 5x5 convolutions.

- [x] A single inception block allows the network to use a combination of 1x1, 3x3, 5x5 convolutions and pooling.

- [x] Making an inception network deeper (by stacking more inception blocks together) should not hurt training set performance.

## 10. Question 10
Which of the following are common reasons for using open-source implementations of ConvNets (both the model and/or weights)? **Check all that apply.**

- [ ] A model trained for one computer vision task can usually be used to perform data augmentation even for a different computer vision task.

- [x] Parameters trained for one computer vision task are often useful as pretraining for other computer vision tasks.

- [x] The same techniques for winning computer vision competitions, such as using multiple crops at test time, are widely used in practical deployments (or production system deployments) of ConvNets.

- [x] It is a convenient way to get working an implementation of a complex ConvNet architecture.

> Please refer to [http://blog.csdn.net/koala_tree/article/details/78531398](http://blog.csdn.net/koala_tree/article/details/78531398) and [http://blog.csdn.net/nichengwuxiao/article/details/78709725](http://blog.csdn.net/nichengwuxiao/article/details/78709725) for further information.