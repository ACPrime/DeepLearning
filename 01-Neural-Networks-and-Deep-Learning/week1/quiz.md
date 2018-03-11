# Introduction to deep learning
Quiz, 10 questions

## 1. Question 1

What does the analogy “AI is the new electricity” refer to?

- [ ] AI is powering personal devices in our homes and offices, similar to electricity.

- [x] Similar to electricity starting about 100 years ago, AI is transforming multiple industries.

> Yes. AI is transforming many 􀃒elds from the car industry to agriculture to
supply-chain...

- [ ] Through the “smart grid”, AI is delivering a new wave of electricity.

- [ ] AI runs on computers and is thus powered by electricity, but it is letting computers do things not possible before.

## 2. Question 2
Which of these are reasons for Deep Learning recently taking off? (Check the three options that apply.)

- [ ] Neural Networks are a brand new field.

- [x] We have access to a lot more computational power.

> Yes! The development of hardware, perhaps especially GPU computing, has
signi􀃒cantly improved deep learning algorithms' performance.

- [x] Deep learning has resulted in significant improvements in important applications such as online advertising, speech recognition, and image recognition.

- [x] We have access to a lot more data.

> Yes! The digitalization of our society has played a huge role in this.


## 3. Question 3
Recall this diagram of iterating over different ML ideas. Which of the statements below are true? (Check all that apply.)

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/FalVl3ygEeegaQ4NYTdESg_7a0184575b8bdc47f8c3f29601302cb8_Screen-Shot-2017-08-08-at-6.13.59-PM.png?expiry=1520899200000&hmac=rGPZjU8bArk__0uIndV6GfEVX48u2MrwOTDfDp-x9Hs)

- [x] Being able to try out ideas quickly allows deep learning engineers to iterate more quickly.

> Yes, as discussed in Lecture 4.

- [x] Faster computation can help speed up how long a team takes to iterate to a good idea.

> Yes, as discussed in Lecture 4.

- [ ] It is faster to train on a big dataset than a small dataset.

- [x] Recent progress in deep learning algorithms has allowed us to train good models faster (even without changing the CPU/GPU hardware).

## 4. Question 4

When an experienced deep learning engineer works on a new problem, they can usually use insight from previous problems to train a good model on the first try, without needing to iterate multiple times through different models. True/False?

- [ ] True

- [x] False

> Yes. Finding the characteristics of a model is key to have good
performance. Although experience can help, it requires multiple iterations
to build a good model.

## 5. Question 5

Which one of these plots represents a ReLU activation function?

- [x] Figure 1:
![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/rDlJVXGkEeeOXQ7jdzu9Bg_ebe829e5a35b0a8d44b8fe85c7b28f9a_figure-1.png?expiry=1520899200000&hmac=kLDugmkl0uUQfbzJ5Elapcc8E-X5kdkJuvdI4rZmKHM)

- [x] Figure 2:
![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/fwrRT3GkEee1BBJ2zgI9PA_c3a9e3d21c9e6cad5bb938ba596f94e3_Figure-2.png?expiry=1520899200000&hmac=9cAUt-N3sCDBD6J3zsrqJjG0lcc6OKTlujz9UG8vC2o)

- [ ] Figure 3:
![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sBkbVnGkEee1BBJ2zgI9PA_2e3410579d847b4df4c2cf2691d63d3e_figure3.png?expiry=1520899200000&hmac=Jo0Ld1dG9nV2IB3V4Oty1cDaMb1FGZw89Gs_PuiCRGI)

> Correct! This is the ReLU activation function, the most used in neural
networks.

- [x] Figure 4:
![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/0GhwpHGkEeewexKhHrUb5g_2e64af1a0d0520a05f4b366bd77328ff_figure4.png?expiry=1520899200000&hmac=Xg0A2lTicabQRwK8qIcasMFTDQWMNqgbMkvUjyr2DD0)

## 6. Question 6
Images for cat recognition is an example of “structured” data, because it is represented as a structured array in a computer. True/False?

- [ ] True

- [x] False

> Yes. Images for cat recognition is an example of “unstructured” data.

## 7. Question 7
A demographic dataset with statistics on different cities' population, GDP per capita, economic growth is an example of “unstructured” data because it contains data coming from different sources. True/False?

- [ ] True

- [x] False

> A demographic dataset with statistics on di􀃗erent cities' population, GDP
per capita, economic growth is an example of “structured” data by
opposition to image, audio or text datasets.

## 8. Question 8
Why is an RNN (Recurrent Neural Network) used for machine translation, say translating English to French? (Check all that apply.)

- [x] It can be trained as a supervised learning problem.

- [ ] It is strictly more powerful than a Convolutional Neural Network (CNN).

- [x] It is applicable when the input/output is a sequence (e.g., a sequence of words).

> Yes. An RNN can map from a sequence of english words to a sequence of
french words.

- [ ] RNNs represent the recurrent process of Idea->Code->Experiment->Idea->....

## 9. Question 9
In this diagram which we hand-drew in lecture, what do the horizontal axis (x-axis) and vertical axis (y-axis) represent?

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/JP--G3ooEeeJIwrF5BVsIg_b60d752c05bec0881d8ca08cfc2646d2_Screen-Shot-2017-08-05-at-2.30.09-PM.png?expiry=1520899200000&hmac=Q9lDvTV0q4jd23gib-xr_JsEYovfwfBUK7NV2u7VS9c)

- [ ] A
    - x-axis is the performance of the algorithm
    - y-axis (vertical axis) is the amount of data.

- [ ] B
    - x-axis is the input to the algorithm
    - y-axis is outputs.

- [ ] C
    - x-axis is the amount of data
    - y-axis is the size of the model you train.

- [x] D
    - x-axis is the amount of data
    - y-axis (vertical axis) is the performance of the algorithm.

## 10. Question 10
Assuming the trends described in the previous question's figure are accurate (and hoping you got the axis labels right), which of the following are true? (Check all that apply.)

- [ ] Decreasing the training set size generally does not hurt an algorithm’s performance, and it may help significantly.

- [x] Increasing the size of a neural network generally does not hurt an algorithm’s performance, and it may help significantly.

- [x] Increasing the training set size generally does not hurt an algorithm’s performance, and it may help significantly.

- [ ] Decreasing the size of a neural network generally does not hurt an algorithm’s performance, and it may help significantly.