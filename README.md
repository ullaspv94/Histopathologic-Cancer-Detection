# Histopathologic-Cancer-Detection
A Kaggle competition, Implemented as an academic project https://www.kaggle.com/c/histopathologic-cancer-detection
The training images here are 1:1 (96x96) cropped lymphnode tissue samples either containing a tumour or not.
Model is built with keras in python and is trained to detect and classify the tissue sample as positive or neagtive cancer cells.
Training images are nearly 600k in total having nearly 60:40 distribution of positive and negative samples.
Many more images are generated with the use of ImageDataGenerator by rescaling etc.
The model is trained/built using CNN of 19 layers deep with 3 drop out layers after every 3 Conv2D layers and MaxPool layer.
Finally converging at Dense Layer that predicts whether it is a positive or negative result.
The activation function used here is ReLU and Softmax to finally classify the image sample.
The learning Rate here is 0.0001 using the Adam optimizer and 15 epochs.


The ROC AUC is 0.94 and the prediction Accuracy was at 0.94 and other evaluation metrics are as follows:
Precision for Label 0: 
0.9485046098493366
Precision for Label 1: 
0.9495497575617641
Recall for Label 0:
0.9666182873730044
Recall for Label 1:
0.9229129263913824
F Score for Label 0:
0.9574757869249394
F Score for Label 1:
0.9360418800500739
Support for Label 0:
13091
Support for Label 1:
8912


A code to see the image after the 4 activation layers has also been added and can be tried out to examine how CNN 'sees' an image.
