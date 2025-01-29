## Domain Generalization of X-ray Diagnosis through Identification of Irrelevant Patterns

X-ray images are often taken, preserved, and transported through adverse circumstances in less-developed countries. As a result, many X-ray images contain noises. In this paper, we propose an extra class that contains potential unwanted patterns during the training phase. Firstly, we observe images and crop the unnecessary portion of images that may influence the training. Then, we develop a class containing those cropped irrelevant patterns. Finally, we train vision transformer (ViT), ResNet, and WideResNet models considering three classes: 1) Opacity (Diseased), 2) None (Healthy), and 3) Irrelevant Pattern. Our proposed approach improves generalization and provides higher accuracy than the traditional counterpart. We apply the proposed method to CIFAR-10 and CIFAR-100 datasets to verify its effectiveness. We received near state-of-the-art (SoTA) performances on CIFAR-10 and CIFAR-100 datasets while using the proposed method with the ViT-L/16 model. After the verification, we apply the proposed method to the chest X-ray (CXR) dataset. We statistically receive better performance with the proposed method compared to the counterpart for all of the investigated combinations. We prove the effectiveness of our model through the class activation map and deep feature factorization results. According to our investigation, the proposed method faces lower degradation due to the model ablation. We share the scripts of the proposed method at the following GitHub Repository: github.com/dipuk0506/X-ray\_pattern


## Irrelevant Information Class Dataset
### CIFAR data.
We develop irrelevant information class images through the following Kaggle Notebook:
https://www.kaggle.com/code/dipuk0506/background-image-data

The irrelevant class images for CXR data are generated through the following notebook. The output of the notebook contains data with sides.
https://www.kaggle.com/code/dipuk0506/dicom-files-to-rgb-512x512/notebook
