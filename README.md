# Tumor Detection with Transfer Learning from Gigapixel Pathology Images

This is the Github folder for Applied Deep Learning course final project

Author: Wei Han (wh2365), Yang Gao (yg2499) , Chengtian Xu (cx2168) 

YouTube Demo: [Presentation](https://www.youtube.com/watch?v=3qS0IxjzOok&feature=youtu.be), [Code Walkthrough](https://www.youtube.com/watch?v=7Ut5lu7wIjI&feature=youtu.be)

### Data

* Based on CAMELYON 16 challenge dataset
* Different Zoom Level provides both context and detail
* WSI (Whole Slide Image)
* Up to 8 levels of magnification

### Approach

* Data Preprocessing using OpenSlide
* Color Normalization & Feature Extraction

![alt text](https://github.com/gyoung2014/tumor_cancer_prediction/blob/master/README%20IMAGE/README_IMAGE1.png "Logo Title Text 1")

### Training & Testing Images

![alt text](https://github.com/gyoung2014/tumor_cancer_prediction/blob/master/README%20IMAGE/README_IMAGE3.png "Logo Title Text 1")


Training Slides #: [016, 101, 084, 094, 096]
* Extraction Level: 5 & 6
* Extraction of 120 Positive Patches + 170 Negative Patches

Testing Slides: #: [110]
* Extraction Level: 5 & 6
* Predict the patches of size (299 x 299 )
* Create heatmap ,each patch contains a value between 0 and 1,indicating the probability that the patch contains tumor

![alt text](https://github.com/gyoung2014/tumor_cancer_prediction/blob/master/README%20IMAGE/readme_image2.png "Logo Title Text 1")

### Evaluation Matrics

* Confusion Matrix
* Accuracy, F1 score, Precision, Recall

### References
[1] [Starter Code to Begin Final Project](https://github.com/random-forests/applied-dl/blob/master/project/starter-code.ipynb)<br>
[2] [Yun Liu et al., Detecting Cancer Metastases on Gigapixel Pathology Images](https://arxiv.org/abs/1703.02442)<br>
[3] [Assisting Pathologists in Detecting Cancer with Deep Learning by Google AI Blog](https://ai.googleblog.com/2017/03/assisting-pathologists-in-detecting.html)
