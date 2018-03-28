# Special applications: Face recognition & Neural style transfer
Quiz, 10 questions

## 1. Question 1
Face verification requires comparing a new picture against one person’s face, whereas face recognition requires comparing a new picture against K person’s faces.

- [x] True

- [ ] False

## 2. Question 2
Why do we learn a function ![](https://latex.codecogs.com/gif.latex?d%28img1%2C%20img2%29) for face verification? **(Select all that apply.)**

- [x] This allows us to learn to recognize a new person given just a single image of that person.

- [x] We need to solve a one-shot learning problem.

- [ ] This allows us to learn to predict a person’s identity using a softmax output unit, where the number of classes equals the number of persons in the database plus 1 (for the final “not in database” class).

> Softmax output unit has been removed.

- [ ] Given how few images we have per person, we need to apply transfer learning.

> We don't need to use transfer learning.

## 3. Question 3
In order to train the parameters of a face recognition system, it would be reasonable to use a training set comprising 100,000 pictures of 100,000 different persons.

- [ ] True

- [x] False

> More than one pictures per person are needed.

## 4. Question 4
Which of the following is a correct definition of the triplet loss? Consider that ![](https://latex.codecogs.com/gif.latex?%5Calpha%20%3E%200). (We encourage you to figure out the answer from first principles, rather than just refer to the lecture.)

- [x] ![](https://latex.codecogs.com/gif.latex?max%28%7C%7Cf%28A%29-f%28P%29%7C%7C%5E2%20-%20%7C%7Cf%28A%29-f%28N%29%7C%7C%5E2%20&plus;%20%5Calpha%2C%200%29)

- [ ] ![](https://latex.codecogs.com/gif.latex?max%28%7C%7Cf%28A%29-f%28N%29%7C%7C%5E2%20-%20%7C%7Cf%28A%29-f%28P%29%7C%7C%5E2%20-%20%5Calpha%2C%200%29)

- [ ] ![](https://latex.codecogs.com/gif.latex?max%28%7C%7Cf%28A%29-f%28P%29%7C%7C%5E2%20-%20%7C%7Cf%28A%29-f%28N%29%7C%7C%5E2%20-%20%5Calpha%2C%200%29)

- [ ] ![](https://latex.codecogs.com/gif.latex?max%28%7C%7Cf%28A%29-f%28N%29%7C%7C%5E2%20-%20%7C%7Cf%28A%29-f%28P%29%7C%7C%5E2%20&plus;%20%5Calpha%2C%200%29)

## 5. Question 5
Consider the following Siamese network architecture:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/xryVS70VEee3NhLzohKsog_98c778df87f041af9903bd66d2d98bbd_Screen-Shot-2017-10-29-at-6.57.51-PM.png?expiry=1522368000000&hmac=De3Ip0e29LULvqMrf7NpKBeDm0sgsjxECvN_fUuV_DY)

The upper and lower neural networks have different input images, but have exactly the same parameters.

- [x] True

- [ ] False

> Wee need the same parameters to get ![](https://latex.codecogs.com/gif.latex?f%28x%5E%7B%28i%29%7D%29)

## 6. Question 6
You train a ConvNet on a dataset with 100 different classes. You wonder if you can find a hidden unit which responds strongly to pictures of cats. (I.e., a neuron so that, of all the input/training images that strongly activate that neuron, the majority are cat pictures.) You are more likely to find this unit in layer 4 of the network than in layer 1.

- [x] True

- [ ] False

## 7. Question 7
Neural style transfer is trained as a supervised learning task in which the goal is to input two images (![](https://latex.codecogs.com/gif.latex?x)), and train a network to output a new, synthesized image (![](https://latex.codecogs.com/gif.latex?y)).

- [ ] True

- [x] False

> Images have no labels.

## 8. Question 8
In the deeper layers of a ConvNet, each channel corresponds to a different feature detector. The style matrix ![](https://latex.codecogs.com/gif.latex?G%5E%7B%5Bl%5D%7D) measures the degree to which the activations of different feature detectors in layer ![](https://latex.codecogs.com/gif.latex?l) vary (or correlate) together with each other.

- [x] True

- [ ] False

## 9. Question 9
In neural style transfer, what is updated in each iteration of the optimization algorithm?

- [ ] The neural network parameters

- [x] The pixel values of the generated image ![](https://latex.codecogs.com/gif.latex?G)

- [ ] The regularization parameters

- [ ] The pixel values of the content image ![](https://latex.codecogs.com/gif.latex?C)

## 10. Question 10
You are working with 3D data. You are building a network layer whose input volume has size 32x32x32x16 (this volume has 16 channels), and applies convolutions with 32 filters of dimension 3x3x3 (no padding, stride 1). What is the resulting output volume?

- [x] 30x30x30x32

- [ ] Undefined: This convolution step is impossible and cannot be performed because the dimensions specified don’t match up.

- [ ] 30x30x30x16

> Please refer to [https://blog.csdn.net/koala_tree/article/details/78647528](https://blog.csdn.net/koala_tree/article/details/78647528) for further information.