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

| Element/Variable Display Name | Description | Data Type |             
|------------------------------|------------|----------|
| dt | Date of temperature recording | Character |
| LandAverageTemperature | Average land surface temperature in celsius | Integer |
| LandAverageTemperatureUncertainty | 95% confidence interval for LandAverageTemperature | Integer |
| LandMaxTemperature | Max land surface temperature in celsius | Integer |
| LandMaxTemperatureUncertainty | 95% confidence interval for LandMaxTemperature | Integer |


#### [Dataset]([https://www.kaggle.com/datasets/csafrit2/plant-leaves-for-image-classification](https://data.world/data-society/global-climate-change-data))

### Figures

| Figure | Summary |
|--------|---------|
| 1850.png | Four graphs showing temperature data from 1850-2015; first is a line graph of our data , second is a trend graph, third is a seasonal graph, and fourth is a remainder graph. |
| 1900.png | Four graphs showing temperature data from 1850-1899; first is a line graph of our data, second is a trend graph, third is a seasonal graph, and fourth is a remainder graph. |
| 1900_SARIMA.png | A line graph from our SARIMA model showing the actual trend and the predicted trend from 1850-1899. |
| 1900_acf.png | An Autocorrelation Function plot of our data from 1850-1899. |
| 1900_pacf.png | A Partial Autocorrelation Function plot of our data from 1850-1899. |
| 1950.png | Four graphs showing temperature data from 1900-1949; first is a line graph of our data, second is a trend graph, third is a seasonal graph, and fourth is a remainder graph. |
| 1950_SARIMA.png | A line graph from our SARIMA model showing the actual trend and the predicted trend from 1900-1949. |
| 1950_acf.png | An Autocorrelation Function plot of our data from 1900-1949. |
| 1950_pacf.png | A Partial Autocorrelation Function plot of our data from 1900-1949. |
| 2000.png | Four graphs showing temperature data from 1950-1999; first is a line graph of our data, second is a trend graph, third is a seasonal graph, and fourth is a remainder graph. |
| 2000_SARIMA.png | A line graph from our SARIMA model showing the actual trend and the predicted trend from 1950-1999. |
| 2000_acf.png | An Autocorrelation Function plot of our data from 1950-1999. |
| 2000_pacf.png | A Partial Autocorrelation Function plot of our data from 1950-1999. |
| 2015.png | Four graphs showing temperature data from 2000-2015; first is a line graph of our data, second is a trend graph, third is a seasonal graph, and fourth is a remainder graph. |
| 2015_SARIMA.png | A line graph from our SARIMA model showing the actual trend and the predicted trend from 2000-2015. |
| 2015_acf.png | An Autocorrelation Function plot of our data from 2000-2015. |
| 2015_pacf.png | A Partial Autocorrelation Function plot of our data from 2000-2015. |
| 268A21DB-B80E-4DAD-BD8B-C1A4C7E6C4A0.jpeg | Plot graph showing monthly trends of the average temperature of every January from 1850-2015 with a line of best fit. |
| 24ECC1F36-1A42-44E4-848C-6BC3CF790685.jpeg | Plot graph showing monthly trends of the average temperature of every July from 1850-2015 with a line of best fit. |
| 606D6DF8-0021-4C42-BEDA-BE0B542B0D21.jpeg | Plot graph showing monthly trends of the average temperature of every month from 1850-2015, seperated by month. |
| 65EB388F-20A6-4279-9E53-A7AA9CBFFC4B.jpeg | Line graph of the average temperatures from 1850-2015. |
| 98844BC2-540C-4A84-9BC0-164D21F39C30.jpeg | Line graph of the average temperatures from 2000-2015. |
| A463DC54-4A93-46A8-BB6F-9CC0BFD6CEEF.jpeg | Line graph of the average temperatures from 1900-1949. |
| A9DDA26C-B5A9-47DA-BC85-8FF077B002A0.jpeg | Line graph of the average temperatures from 1850-1899. |
| Screen Shot 2023-04-18 at 12.43.45 PM.png | Table showing the R-squared values of the data from the 50-year intervals |
| ts_acf.png | An Autocorrelation Function plot of our data from 1850-2015. |
| ts_pacf.png | A Partial Autocorrelation Function plot of our data from 1850-2015. |

### References:

[1] Data Society, “Global Climate Change Data,” data.world, 2016. [Online]. Available: https://data.world/data-society/global-climate-change-data/discuss/global-climate-change-data/gntggylf. [Accessed Apr. 13, 2023].

[2] Berkeley Earth, “About Berkeley Earth,” Berkeley Earth, 2012. [Online]. Available: https://berkeleyearth.org/about/. [Accessed Apr. 13, 2023]. 

[3] ArcGIS, “Seasonal-Trend decomposition using LOESS,” Esri, 2023. [Online]. Available: https://doc.arcgis.com/en/insights/latest/analyze/stl.htm.

[4] L. Monigatti, “Interpreting ACF and PACF Plots for Time Series Forecasting,” Medium, Aug. 2, 2022. [Online]. Available: https://towardsdatascience.com/interpreting-acf-and-pacf-plots-for-time-series-forecasting-af0d6db4061c.

[5] A. Bajaj, “Arima & Sarima: Real-world time series forecasting,” neptune.ai, 26-Jan-2023. [Online]. Available: https://neptune.ai/blog/arima-sarima-real-world-time-series-forecasting-guide. [Accessed: 11-Apr-2023]. 

[6] A. L. Duca, “How to model a time series through a SARIMA model,” Medium, Sept. 9, 2020. [Online]. Available: https://towardsdatascience.com/how-to-model-a-time-series-through-a-sarima-model-e7587f85929c.

[MI1](https://github.com/ahimes9/DS4002_GroupWork/blob/main/Project_3/Project%203%20MI1.pdf), [MI2](https://github.com/ahimes9/DS4002_GroupWork/blob/main/Project_3/Project%203%20MI2.pdf)
