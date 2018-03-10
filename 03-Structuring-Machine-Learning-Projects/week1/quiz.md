# Bird recognition in the city of Peacetopia (case study)
## 1. Problem Statement

This example is adapted from a real production application, but with details disguised to protect confidentiality.

![City of Peacetipia](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/RjThWXtFEeeumw4MySoK5g_4b24d6550498b64919bb5255dd329704_mont-saint-michel-688405_1920.jpg?expiry=1520812800000&hmac=1DamngkE1UUSsiFwglZeaJaPK0XJIh3TvPRuJjM3Biw)

You are a famous researcher in the City of Peacetopia. The people of Peacetopia have a common characteristic: they are afraid of birds. To save them, you have to **build an algorithm that will detect any bird flying over Peacetopia** and alert the population.

The City Council gives you a dataset of 10,000,000 images of the sky above Peacetopia, taken from the city’s security cameras. They are labelled:

- y = 0: There is no bird on the image
- y = 1: There is a bird on the image

Your goal is to build an algorithm able to classify new images taken by security cameras from Peacetopia.

There are a lot of decisions to make:

- What is the evaluation metric?
- How do you structure your data into train/dev/test sets?

## Metric of success

The City Council tells you the following that they want an algorithm that

1. Has high accuracy
2. Runs quickly and takes only a short time to classify a new image.
3. Can fit in a small amount of memory, so that it can run in a small processor that the city will attach to many different security cameras.

**Note**: Having three evaluation metrics makes it harder for you to quickly choose between two different algorithms, and will slow down the speed with which your team can iterate. True/False?

- [ ] True
- [x] False

## 2. After further discussions, the city narrows down its criteria to:

- "We need an algorithm that can let us know a bird is flying over Peacetopia as accurately as possible."
- "We want the trained model to take no more than 10sec to classify a new image.”
- “We want the model to fit in 10MB of memory.”

If you had the three following models, which one would you choose?

- [ ] A

Test Accuracy | Runtime | Memory size
----- | ----- | -----
97% | 1 sec | 3MB

- [ ] B

Test Accuracy | Runtime | Memory size
----- | ----- | -----
99% | 13 sec | 9MB

- [ ] C

Test Accuracy | Runtime | Memory size
----- | ----- | -----
97% | 3 sec | 2MB

- [x] D

Test Accuracy | Runtime | Memory size
----- | ----- | -----
98% | 9 sec | 9MB

## 3. Based on the city’s requests, which of the following would you say is true?

- [x] Accuracy is an optimizing metric; running time and memory size are a satisficing metrics.

- [ ] Accuracy is a satisficing metric; running time and memory size are an optimizing metric.

- [ ] Accuracy, running time and memory size are all optimizing metrics because you want to do well on all three.

- [ ] Accuracy, running time and memory size are all satisficing metrics because you have to do sufficiently well on all three for your system to be acceptable.

4. Structuring your data

Before implementing your algorithm, you need to split your data into train/dev/test sets. Which of these do you think is the best choice?

- [ ] A

Train | Dev | Test
----- | ----- | -----
3,333,334 | 3,333,333 | 3,333,333

- [ ] B

Train | Dev | Test
----- | ----- | -----
6,000,000 | 3,000,000 | 1,000,000

- [x] C

Train | Dev | Test
----- | ----- | -----
9,500,000 | 250,000 | 250,000

- [ ] D

Train | Dev | Test
----- | ----- | -----
6,000,000 | 1,000,000 | 3,000,000

After setting up your train/dev/test sets, the City Council comes across another 1,000,000 images, called the “citizens’ data”. Apparently the citizens of Peacetopia are so scared of birds that they volunteered to take pictures of the sky and label them, thus contributing these additional 1,000,000 images. These images are different from the distribution of images the City Council had originally given you, but you think it could help your algorithm.

## 5. True/False?
You should not add the citizens’ data to the training set, because this will cause the training and dev/test set distributions to become different, thus hurting dev and test set performance. 

- [ ] True
- [x] False

## 6. One member of the City Council knows a little about machine learning, and thinks you should add the 1,000,000 citizens’ data images to the test set. You object because:

- [x] This would cause the dev and test set distributions to become different. This is a bad idea because you’re not aiming where you want to hit.

- [x] The 1,000,000 citizens’ data images do not have a consistent x-->y mapping as the rest of the data (similar to the New York City/Detroit housing prices example from lecture).

- [ ] A bigger test set will slow down the speed of iterating because of the computational expense of evaluating models on the test set.

- [ ] The test set no longer reflects the distribution of data (security cameras) you most care about.

## 7. You train a system, and its errors are as follows (error = 100%-Accuracy):

Training set error | 4.0%
----- | -----
Dev set error | 4.5%

This suggests that one good avenue for improving performance is to train a bigger network so as to drive down the 4.0% training error. Do you agree?


- [ ] Yes, because having 4.0% training error shows you have high bias.


- [ ] Yes, because this shows your bias is higher than your variance.


- [ ] No, because this shows your variance is higher than your bias.


- [x] No, because there is insufficient information to tell.

## 8. You ask a few people to label the dataset so as to find out what is human-level performance. You find the following levels of accuracy:

Bird watching expert #1 | 0.3% error
----- | -----
Bird watching expert #2 | 0.5% error
Normal person #1 (not a bird watching expert) | 1.0% error
Normal person #2 (not a bird watching expert) | 1.2% error

If your goal is to have “human-level performance” be a proxy (or estimate) for Bayes error, how would you define “human-level performance”?

- [ ] 0.0% (because it is impossible to do better than this)

- [x] 0.3% (accuracy of expert #1)

- [ ] 0.4% (average of 0.3 and 0.5)

- [ ] 0.75% (average of all four numbers above)

## 9. Which of the following statements do you agree with?

- [x] A learning algorithm’s performance can be better than human-level performance but it can never be better than Bayes error.

- [ ] A learning algorithm’s performance can never be better than human-level performance but it can be better than Bayes error.

- [ ] A learning algorithm’s performance can never be better than human-level performance nor better than Bayes error.

- [ ] A learning algorithm’s performance can be better than human-level performance and better than Bayes error.

## 10. You find that a team of ornithologists debating and discussing an image gets an even better 0.1% performance, so you define that as “human-level performance.” After working further on your algorithm, you end up with the following:

Human-level performance | 0.1%
---- | ----
Training set error | 2.0%
Dev set error | 2.1%

Based on the evidence you have, which two of the following four options seem the most promising to try? (Check two options.)

- [x] Try increasing regularization.

- [ ] Get a bigger training set to reduce variance.

- [ ] Try decreasing regularization.

- [x] Train a bigger model to try to do better on the training set.

