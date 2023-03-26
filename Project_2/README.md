# Sea Monsters Project 2
Group leader: Sharaf Tariq    
Group members: Audrey Himes, Alexa Owen

DS 4002

## Contents
This repository includes the contents of Project 2 for DS 4002. 

### Installing and Building Code


Packages:
```
import glob
import zipfile
import matplotlib.pyplot as plt
import numpy as np
import PIL
import tensorflow as tf

from tensorflow import keras
from tensorflow.keras import layers
from tensorflow.keras.models import Sequential
```

### Usage of the Code
Load data into a Jupyter Notebook and execute the code chunk-by-chunk.

### Data Dictionary

| Element/Variable Display Name | Description | Number of Images |             
|------------------------------|------------|----------|
| Images to Predict | JPG images to predict the species based on the leaf | 8 |
| Test | 24 folders containing JPG images of diseased and healthy leaves for each plant species to test the model | 110 |
| Train | 24 folders containing JPG images of diseased and healthy leaves for each plant species to train the model | 4274 |
| Validate | 24 folders containing JPG images of diseased and healthy leaves for each plant species used to validate results | 110 |


#### [Dataset](https://www.kaggle.com/datasets/csafrit2/plant-leaves-for-image-classification)

### Figures

| Figure | Summary |
|--------|---------|
| cloud_LOW.png | An image of a word cloud for the most prevalent words in the LOW dataset (ratings of 1-3). The most common words are "movie", "story", and "film". |
| cloud_MED.png | An image of a word cloud for the most prevalent words in the MEDIUM dataset (ratings of 4-7). The most common words are "movie", "story", and "film". |
| cloud_HIGH.png | An image of a word cloud for the most prevalent words in the LOW dataset (ratings of 8-10). The most common words are "movie", "story", and "film". |
| plot_explore.png | A bar graph displaying the number of reviews for each rating (1-10). The bar graph is color-coded to show the different rating groups. LOW is green, MEDIUM is blue, HIGH is red. Although there is a significantly larger number of reviews with a rating of 1, the groups are fairly evenly balanced. |
| cloud_LOW_clean.png | An image of a word cloud for the most prevalent words in the LOW dataset (ratings of 1-3). The most common words are "bad", "time", and "acting". |
| cloud_MED_clean.png | An image of a word cloud for the most prevalent words in the MEDIUM dataset (ratings of 4-7). The most common words are "time", "characters", and "watch". |
| cloud_HIGH_clean.png | An image of a word cloud for the most prevalent words in the HIGH dataset (ratings of 8-10). The most common words are "watch", "time", and "people". |
| plot_afinn_TOTAL.png | A stacked bar graph displaying counts of the afinn method scores for words within reviews in the LOW, MEDIUM, and HIGH groups. Words with no sentiment (a score of 0) are excluded from the figure. |
| plot_nrc_TOTAL.png | A stacked bar graph displaying counts of the nrc method sentiments for words within reviews in the LOW, MEDIUM, and HIGH groups. Negative sentiments are on the left and positive sentiments are on the right. |
| plot_bing_TOTAL.png | A stacked bar graph displaying counts of the bing method of sorting for words within reviews in the LOW, MEDIUM, and HIGH groups. Words are plainly categorized as either positive or negative. |

### References
[1] R. Kestenbaum, “The Pandemic Has Forever Changed The Active Outdoor Business,” Forbes, para. 1 & 2, Aug. 18, 2021. [Online]. Available: https://www.forbes.com. [Accessed Mar. 16, 2023].

[2] F. Chollet, “Image classification from scratch,” keras.io, para. 1, Nov. 10, 2022. [Online]. Available: https://keras.io/examples/vision/image_classification_from_scratch. [Accessed Mar. 14, 2023].

[3] TenserFlow, “Image classification,” tensorflow.org, para. 1, Dec, 15, 2022. [Online]. Available: https://www.tensorflow.org/tutorials/images/classification. [Accessed Mar. 14, 2023]. 

[4] B. G. Regmi, “Image Classification with tf.keras (Introductory Tutorial),” Medium, para. 1, Jan. 11, 2021. [Online]. Available: https://medium.com/analytics-vidhya/image-classification-with-tf-keras-introductory-tutorial-7e0ebb73d044. [Accessed Mar. 15, 2023].

[5] “Plant Leaves for Image Classification,” Kaggle, September, 2022. [Online]. Available: https://www.kaggle.com/datasets/csafrit2/plant-leaves-for-image-classification. [Accessed Mar. 14, 2023].

[6] National Parks Board, “Alstonia scholaris (L.) R. Br.,” Government of Singapore, Mar. 10, 2023. [Online]. Available: https://www.nparks.gov.sg/florafaunaweb/flora/2/7/2705. [Accessed Mar. 16, 2023].

[7] Center for International Forestry Research, “Energy From Forests: Pongamia pinnata,” CIFOR-ICRAF, 2023. [Online]. Available: https://www.cifor.org/feature/energy-from-forests/millettia-pongamia-pinnata/. [Accessed Mar. 16, 2023].  

[MI1](https://github.com/ahimes9/DS4002_GroupWork/blob/main/Project_2/Project%202%20MI1.pdf), [MI2](https://github.com/ahimes9/DS4002_GroupWork/blob/main/Project_2/Project%202%20MI2.pdf)
