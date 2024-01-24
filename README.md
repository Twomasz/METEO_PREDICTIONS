# Engineering Thesis Project

This project is the source code of my engineering thesis with the title:  
__*Comparsion of mathematical weather forecasting models with machine learning models*__.

## Structure
The project consists 3 main parts divided into separate directories:

### Data

In __data/__ you can find only preprocessed data what is used to train models.
The original data is publicly available on [IMGW Institute official page](https://danepubliczne.imgw.pl/).
For the project, 22 different weather parameters for Cracow in 2017-22 were extracted from the original data.

### Preprocessing
Notebook files in which data was preprocessed are located in __preprocessing/__.
There is, for example, data assimilation, complementing weather data from different
weather stations, or aggregating data from an hourly time step to every 6 hours.

### Modeling
At the very end, the 3 learned models and their evaluation of their results are in __modeling/__ folder. 
The first model is a recurrent neural network based on LSTM units, which was trained for data with an hourly time step.
The second model has the same structure as the first but was trained for data with a six-hour time step.
The last one is an experimental model, as it includes a convolution filter as the first layer of the network, and the 
next layers are 2 bidirectional layers of LSTM units.
