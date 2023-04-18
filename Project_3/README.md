# Sea Monsters Project 3
Group leader: Alexa Owen    
Group members: Audrey Himes, Sharaf Tariq

DS 4002

## Contents
This repository includes the contents of Project 3 for DS 4002. 

### Installing and Building Code

Open code in Jupyter Notebook

Packages:
```
from IPython.display import display

import numpy as np
import pandas as pd

import matplotlib.pyplot as plt
from datetime import datetime
from datetime import timedelta
from pandas.plotting import register_matplotlib_converters

register_matplotlib_converters()

from statsmodels.tsa.seasonal import seasonal_decompose
from statsmodels.tsa.arima_model import ARIMA
from statsmodels.tsa.statespace.sarimax import SARIMAX
from statsmodels.tsa.stattools import adfuller
from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
from time import time
import seaborn as sns

import warnings
warnings.filterwarnings('ignore')

from tabulate import tabulate
```
After importing all packages:

```
df = pd.read_csv('/Users/"USERNAME"/Downloads/GlobalLandTemperatures_GlobalTemperatures.csv') #input own username of computer user
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


#### [Dataset]([https://www.kaggle.com/datasets/csafrit2/plant-leaves-for-image-classification](https://data.world/data-society/global-climate-change-data))

### Figures

| Figure | Summary |
|--------|---------|
| Model A Figure 1.png | A line graph showing the training (blue line) and validation (orange line) accuracy for the model that does not account for overfitting. |
| Model A Figure 2.png | A line graph showing the training (blue line) and validation (orange line) loss for the model that does not account for overfitting. |
| Model B Figure 1.png | A line graph showing the training (blue line) and validation (orange line) accuracy for the model that does account for overfitting. |
| Model B Figure 2.png | A line graph showing the training (blue line) and validation (orange line) loss for the model that does account for overfitting. |


### References
[1] R. Kestenbaum, “The Pandemic Has Forever Changed The Active Outdoor Business,” Forbes, para. 1 & 2, Aug. 18, 2021. [Online]. Available: https://www.forbes.com. [Accessed Mar. 16, 2023].

[2] F. Chollet, “Image classification from scratch,” keras.io, para. 1, Nov. 10, 2022. [Online]. Available: https://keras.io/examples/vision/image_classification_from_scratch. [Accessed Mar. 14, 2023].

[3] TenserFlow, “Image classification,” tensorflow.org, para. 1, Dec, 15, 2022. [Online]. Available: https://www.tensorflow.org/tutorials/images/classification. [Accessed Mar. 14, 2023]. 

[4] B. G. Regmi, “Image Classification with tf.keras (Introductory Tutorial),” Medium, para. 1, Jan. 11, 2021. [Online]. Available: https://medium.com/analytics-vidhya/image-classification-with-tf-keras-introductory-tutorial-7e0ebb73d044. [Accessed Mar. 15, 2023].

[5] “Plant Leaves for Image Classification,” Kaggle, September, 2022. [Online]. Available: https://www.kaggle.com/datasets/csafrit2/plant-leaves-for-image-classification. [Accessed Mar. 14, 2023].

[6] National Parks Board, “Alstonia scholaris (L.) R. Br.,” Government of Singapore, Mar. 10, 2023. [Online]. Available: https://www.nparks.gov.sg/florafaunaweb/flora/2/7/2705. [Accessed Mar. 16, 2023].

[7] Center for International Forestry Research, “Energy From Forests: Pongamia pinnata,” CIFOR-ICRAF, 2023. [Online]. Available: https://www.cifor.org/feature/energy-from-forests/millettia-pongamia-pinnata/. [Accessed Mar. 16, 2023].  

[MI1](https://github.com/ahimes9/DS4002_GroupWork/blob/main/Project_2/Project%202%20MI1.pdf), [MI2](https://github.com/ahimes9/DS4002_GroupWork/blob/main/Project_2/Project%202%20MI2.pdf)
