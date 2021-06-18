# Autoregressive-Model-in-Natural-Gas-Price

This time I would like to do a simulation of Autoregressive model in Natural Gas Price using Python. 

1. Import the dataset and convert into panda dataframe

![pic1](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%201.png)




2. Replace the missing values with mean values

![pic2](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%202.png)




3. import Autoregressive library, we provide train model and fit the model

![pic3](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%203.png)




4. Considering how many lag variables in our model

![pic4](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%204.png)




5. Getting coefficient for lag values. By getting the values of the coefficient, we could predict the future values. 
![pic5](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%205.png)




6. Otherwise we could use predict functions. It will later show you the last 7 of predicted values. Later we could also directly called the predicted values, in this case we called the first predicted values.

![pic6](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%206.png)




7. We run the mse function, the result is bigger than the mse value we got from naive model (0.013473258789010692 > 0.004342142857142858). It indicates that the time series model has random walk problem.


![pic7](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%207.png)




8. Next, we would like to run walk forward validation. First, define df and how many values we would like to set as train test


![pic8](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%208.png)




9. Run the syntax to obtain the predicted values


![pic9](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%209.png)





10. Obtain the mse values and plot the graphs. As we can see the mse values decreased rather than mse values that has been run in AR model (0.005255871278210083 <  0.013473258789010692). However it still bigger than mse in naive model (0.005255871278210083 > 0.004342142857142858).


![pic 10](https://github.com/altheanabila/Autoregressive-Model-in-Natural-Gas-Price/blob/main/pic%2010.png)



