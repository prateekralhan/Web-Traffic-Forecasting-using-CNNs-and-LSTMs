# Web Traffic 🕸💥 Forecasting using CNNs and LSTMs 

The web traffic is basically the number of sessions in a given time frame, and it varies a lot with respect to what time of the day it is, what day of the week it is, and so on, and how much web traffic of platform can withstand depends on the size of the servers that are supporting the platform.

#### If the traffic is more than what the servers can handle, the website might show this 404 error, which is something we don’t want to happen. It will make the visitors go away.

* One solution to this problem is to increase the number of servers. However, the downside of the solution is the cause can go up, which is again undesirable. So, what is the solution?
* You can dynamically a lot of servers based on the historical visitor’s volume data or based on the historical web traffic data. And that brings us to the data science problem, which is basically forecasting the web traffic or a number of sessions based on the historical data.

## Installation and Usage:
* Run the command ***pip install -r requirements.txt*** to install the necessary dependencies.
* Run the command ***jupyter notebook*** and follow along the commented Jupyter notebook.

## Dataset:
We will work with the web traffic dataset. It is a six-month series data which you can find [here.](https://www.kaggle.com/kajal1/web-traffic-forecast-dataset)

## Model Architectures : 
1. Basic LSTM Model :
 
![lstm_model](https://user-images.githubusercontent.com/29462447/134826086-fda426cf-99e1-4d78-a872-a2dbf4be81e4.png)


2. Basic CNN Model :

![cnn_model](https://user-images.githubusercontent.com/29462447/134826108-8891d98d-14a3-4bbb-a0c2-f1560d977a96.png)

###### ( Baseline model was taken as a simple moving average model. )

## Training/Validation Loss : 

| Basic LSTM Model      | Basic CNN Model|
| ----------- | ----------- |
| ![loss_lstm](https://user-images.githubusercontent.com/29462447/134826157-7ba86d3c-d2ee-42ef-9508-8d88b1c1790b.png)      | ![loss_cnn](https://user-images.githubusercontent.com/29462447/134826162-47b688f5-6c3c-44ac-a4b5-a42f047ec68f.png)       |

## Results: 

1. Basic LSTM Model :

![pred_lstm](https://user-images.githubusercontent.com/29462447/134826200-27252b04-3f2d-47ef-be86-523c01e19d49.png)

2. Basic CNN Model : 

![pred_cnn](https://user-images.githubusercontent.com/29462447/134826193-8f024fef-970e-46f9-96c4-7c2e6feb6417.png)

## Conclusions: 
* Going through the results, we conclude that both the models tend to have almost similar performance. Feel free to fine tune the hyperparameters ( different batch sizes, optimizers etc. ) or customize the DL architectures?
* Transfer Learning, SOTA models? 😯
* Facebook Prophet?😏
