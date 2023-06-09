# Abstract:
  Parkinson’s disease (PD) is a neurodegenerative disorder that affects millions of people worldwide. There are three main symptoms - tremors (shaking), slowness of movement and rigidity (muscle stiffness). This study presents two different approaches to detecting and classifying PD using two datasets. One is a Convolutional Neural Network (CNN) based model for analysing the drawing patterns of spiral sketches. Then the CNN model is compared with two other medical image datasets such as lung cancer and brain tumour. Another one is Machine Learning based models such as XGBoost, Logistic Regression, DecisionTree Classifer, and SVC for analysing the speech recordings of the
patients. The overall classification accuracy resulting from the CNN model is 97.26% and the testing accuracy is 0.79, 0.82, 0.90 and 0.92 for XGBoost, Logistic Regression, DecisionTree Classifer, and SVC models respectively. Also, I have used KNN and RandomForest Classifier for the classification of the speech dataset.

## CNN Model: 
The model architecture used in the implementation is a CNN model with the following features:
  1. Four convolutional layers with 128, 64, 32, and 32 filters each are present in the model.
  2. There are filters with different filter sizes in the convolutional layers.
  3. Each convolutional layer is followed by a MaxPool2D layer. 
  4. The convolutional block is followed by one fully linked layer.
  5. The last layer includes 2 channels for 2 classifications with softmax function.

Using Adam optimiser, the model is trained at a learning rate of 3.15e-5. Epochs have been set to 50.

![](Info/CNN_Model.png)

## Accuracy and Loss for Parkinson's Disease:
Validation Loss: 0.07
Validation Accuracy: 0.97

![](Info/PD_Accuracy.png)
![](Info/PD_Loss.png)

## Comparing the CNN Model on Other Medical Dataset

### Brain Tumor:
Validation Loss: 0.27
Validation Accuracy: 0.93

![](Info/Brain_Tumor_Accuracy.png)
![](Info/Brain_Tumor_Loss.png)

### Lung Cancer:
Validation Loss: 0.14
Validation Accuracy: 0.95

![](Info/Lung_Cancer_Accuracy.png)
![](Info/Lung_Cancer_Loss.png)
