# Landmark-Recognition-2019
Final project of Learning AI 2019

# The Project Context : 

Did you ever go through your vacation photos and ask yourself: What is the name of this temple I visited in China? Who created this monument I saw in France? This is where Landmark recognition can help : This technology aims at predicting landmark labels directly from image pixels.

# The files :

Data_preparation.ipynb - Download Pictures from the Dataset, Resize them, Store them Class by Class in three separate folders, 'Training Data', 'Validation Data', 'Test Data'.
The three set have been separated with a percentage : 75%,20%,5%. No Data Augmentation has been performed.

Model_Pretraining.ipynb - Pre-training of the four models on ImageNet dataset and then feed with LAndmark recognition examples to quickly 
identify the most appropriate one to train further.

VGG16_Optimizition.ipynb, Inception_Optimization.ipynb, Resnet_Optimization.ipynb, Densenet_Optimization.ipynb - Training of the four models,
Hyper-parameters tuning with RandomizedSearch, Dropout and Regularization to avoid overfitting.

Ensemble_Algorithm.ipynb - Get an ensemble of the four previous models and get a prediction score on the test set.
