# CNN-Dog_Image_Project
[//]: # (Image References)

[image1]: ./result/me.png "me"
[image2]: ./result/bullterrier.jpeg "melike"
[image3]: ./result/trump.png "trump"
[image4]: ./result/greyhound.jpeg "trumplike"

# Overview
The second project for Udacity Deep Learning Nanodegree program. In this project, I will explore state-of-the-art CNN models for classification, build a pipeline to process real-world, user-supplied dog images. Given an image of a dog, my model will identify an estimate of the canine’s breed. If supplied an image of a human, just for fun, my code will identify the resembling dog breed.

# Data
The training data for this project is located [here](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip). This dataset contains 133 different breeds of dogs and is already split into train, test, and validation sets. Place the training, testing, and validation datasets in the `dogImages` folder.

# Environment
Python: 3.6

PyTorch: 0.4.0

GPU: NVIDIA GeForce GTX 970M

Windows: 8.1

# Result
With the pretained Resnet50, I used transfer learning on new dog image data, the models has 75% accuracy on test data for dog breed with only 5 epochs of training (took less than 10 mins). The final user app uses the pretrained VGG16 as a dog detector, then uses the tuned Restnet50 as dog breed classifier, for huamans, I used OpenCV's implementation of Haar feature-based cascade classifiers to detect human faces in images.

I tried the app with photo of myself, it shows I look like a Bull terrier, and trump looks like Greyhound.
![me][image1]

here is a image of a bull terrier:
![melike][image2]

For trump:
![trump][image3]
![trumplike][image4]

# Deliverable
Check the *dog_app.ipynb* for model with detail in code.

Check *myphotos* for the photos I tried with my app.
