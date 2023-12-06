## The implementation of deep learning to develop an adequate tool for identifying the bumblebee species in Ireland

In this project, we trained, tested and evaluated ten pre-trained CNN models to build a tool using Keras and Pytorch libraries that can potentially predict the classes of unlabelled bumblebee images taken in Ireland as adequate as possible.

- **InceptionV3**
- **ResNet101**
- **VGG19**
- **MobileNetV3_Large**
- **EfficientNetV2_Large**

- **SuqeezeNet1_1**
- **DenseNet121**
- **ShuffleNetV2**
- **GoogleNet**
- **MNASNet1_0**

At the very beginning, images of 21 different bumblebee species were collected online, such as flickr, inaturalist and irecord. Totally 4200 images were gathered, 200 images for each species. Then the whole dataset was randomly splitted into three parts, train dataset, validate dataset and test dataset at the ratio of 72%, 18%, 10%.

Before training, data annotation was implemented using CVAT, an open-source annotating tool, to extarct the region of interest of the train and validate datasets.

Following that, few data augmentation methods were applied to the processed train dataset to generate more variety of data to increase generalisation and reduce overfitting, i.e. padding, random geometric augmentations etc.

The performance of the models were presented visually based on their accuracy score, classification report (i.e. precision, recall and f1-score), confusion matrix.

Finally, the models were evaluated based on test dataset that is "raw (without annotation)" using Local Interpretable Model-agnostic Explanations (LIME) to show the trust level of the models generated.



### Reference

- <p>https://www.flickr.com/photos/63075200@N07/collections/72157631518510934/</p>
- <p>https://www.flickr.com/</p>
- <p>https://www.inaturalist.org/observations</p>
- <p>https://irecord.org.uk/</p>
- <p>https://github.com/opencv/cvat</p>
- <p>https://keras.io/</p>
- <p>https://pytorch.org/</p>
- <p>https://github.com/marcotcr/lime</p>
- <p></p>
