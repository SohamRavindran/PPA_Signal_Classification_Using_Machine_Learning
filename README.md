# PPA_signal_classification_Using_CNN

In this project we were provided with images of PPA signals of various patients with different cardiovasclar diseases.We used different Ml techniques to build a model of predict the the health condition of patient using the image of his PPA signals. PPA stands for Peripheral Pulse Analyser.These signals are obtained by placing 2 sensors at the wrist of a patient.

Since the data given to us was completely raw and uncatagorized we had to first sort and clean the data. This was the most tiresome and time consuming part in this project. After doing research we found that there are 10 types of patterns present in these signals. These patterns help us decide on the health condition of a patient.

So first we used K_means clustering to categorize them into 10 classes. We also used the help of MobileNetV2 for feature extraction.
Once we made 10 classes of the image dataset, we split it into train, validation, and test sets in a 60:20:20 ratio.
Once that was done the dataset had to be augmented in order for the model to give better results as there were a large number of classes to differentiate from.
Next, we trained 2 models on this data, a CNN model and a pre-trained RestNet50 model to compare their outputs.
We trained these for 10 epochs.
After building and training the models and comparing their MAp scores, the ResNet50 gave a better output in prediction. The accuracy of the ResNet model was 93.7%.
These models were trained on a total of 2771 images.

This project at that time was a part of a Masters project in colaboration with Homi Baba Atomic Research Center.
