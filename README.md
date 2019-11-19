# Landmark-Recognition-2019
Final project of Learning AI 2019

# The Project Context : 

Did you ever go through your vacation photos and ask yourself: What is the name of this temple I visited in China? Who created this monument I saw in France? Landmark recognition can help! This technology can predict landmark labels directly from image pixels, to help people better understand and organize their photo collections.

Today, a great obstacle to landmark recognition research is the lack of large annotated datasets. In this competition, we present the largest worldwide dataset to date, to foster progress in this problem. This competition challenges Kagglers to build models that recognize the correct landmark (if any) in a dataset of challenging test images.

Many Kagglers are familiar with image classification challenges like the ImageNet Large Scale Visual Recognition Challenge (ILSVRC), which aims to recognize 1K general object categories. Landmark recognition is a little different from that: it contains a much larger number of classes (there are more than 200K classes in this challenge), and the number of training examples per class may not be very large. Landmark recognition is challenging in its own way.

# The files :

Data_preparation.ipynb - Download Pictures from the Dataset, Resize them, Store them Class by Class in three separate folders, 'Training Data', 'Validation Data', 'Test Data'.
The three set have been separated with a percentage : 75%,20%,5%. No Data Augmentation has been performed.

Model_Pretraining.ipynb - Pre-training of the four models on ImageNet dataset and then feed with LAndmark recognition examples to quickly 
identify the most appropriate one to train further.

VGG16_Optimizition.ipynb, Inception_Optimization.ipynb, Resnet_Optimization.ipynb, Densenet_Optimization.ipynb - Training of the four models,
Hyper-parameters tuning with RandomizedSearch, Dropout and Regularization to avoid overfitting.

Ensemble_Algorithm.ipynb - Get an ensemble of the four previous models and get a prediction score on the test set.
