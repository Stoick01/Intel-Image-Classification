# Intel Image Classifier

This model was developed to classify images for the Intel challenge on [Kaggle](https://www.kaggle.com/puneet6060/intel-image-classification).

## Dataset overview

Dataset contains 25k images of size 150x150 under 6 categories [buildings, forest, glacier, mountain, sea, street].

![Example](/assets/classes_example.png)


## Solution

All original dimension of images are used, the model is vgg11 without pretraining (While pretrained model like resnet would achieve much better results, I wanted to see how vgg11 without pretraining behaves). Optimization is done using Adam optimizer with the following parameters: lr=0.000003, betas=(0.8, 0.999).

![Example](/assets/vgg.jpg)

## Results

Without pretraining such a big model has hard time generalizing. The following are the best results achieved with this approach.

Loss:
![Example](/assets/loss.png)

Accuracy:
![Example](/assets/acc.png)

Here we can also see how the model predicted some images.

![Example](/assets/examples.png)
