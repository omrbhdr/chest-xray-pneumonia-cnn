# chest-xray-pneumonia-cnn
About Dataset
Context
http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5



Figure S6. Illustrative Examples of Chest X-Rays in Patients with Pneumonia, Related to Figure 6
The normal chest X-ray (left panel) depicts clear lungs without any areas of abnormal opacification in the image. Bacterial pneumonia (middle) typically exhibits a focal lobar consolidation, in this case in the right upper lobe (white arrows), whereas viral pneumonia (right) manifests with a more diffuse ‘‘interstitial’’ pattern in both lungs.
http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5

Content
The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).

Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care.

For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.

Acknowledgements
Data: https://data.mendeley.com/datasets/rscbjbr9sj/2

License: CC BY 4.0

Citation: http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5
...........................................................................................
......libs......
import os
import numpy as np
import matplotlib.pyplot as plt
from matplotlib.pyplot import imshow
import  pandas as pd
import cv2
from PIL import Image
from tensorflow import keras
from keras import layers as tfl
from keras import layers, models, optimizers
from keras.preprocessing.image import ImageDataGenerator
from tensorflow.keras import Sequential
from tensorflow.keras.layers import Conv2D,MaxPool2D,Dropout,Flatten,Dense,BatchNormalization
..............................................................................................
![image](https://github.com/omrbhdr/chest-xray-pneumonia-cnn/assets/12261537/5c844fc4-0317-40b4-973c-3b9453e3958c)
![image](https://github.com/omrbhdr/chest-xray-pneumonia-cnn/assets/12261537/23ffa158-087f-40a7-8ed1-84e673215e64)
![image](https://github.com/omrbhdr/chest-xray-pneumonia-cnn/assets/12261537/a57504f9-8328-4a45-99a5-325b88422913)

