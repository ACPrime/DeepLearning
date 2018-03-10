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

- [x] True
- [ ] False