# Summary

An algorithm that combine the output of a neural network and a text analytics analysis to trade stocks.
This work is part of our course <b>"Algorithmic trading with Python"</b> at <b>Hult University</b> with <b>Professor Micheal Rolleigh</b>.

Our team had around 4 days to dedicate to this project, during this time we had to:
Get to know each other
Come up with a trading strategy
Find a way a to implement it in Python
Backtest it and compared to a benchmark strategy

# Conclusions
We decided to implement an LSTM model and combine its recommendation with the sentiment analysis on the tweets. In particular we decided to follow the recommendation provided by the LTSM only when the sentiment analysis was recommending the same (either buy or sell). If the 2 models did not agree with each other we would just close all the current positions and take any other position until they agreed with each other again.

At the end, our model has an outstanding performance on the traning data (due to overfitting) and in the testing data (compared to benchmark strategy of buying and holding the assets). However, combining the LSTM model with the sentiment analysis allowed us to achieve a better performance than either of the models taken alone.


# Team 2
> <i>
> <br>Nicola Bini
> <br>Felipe Domingues
> <br>Tri Dung Dinh
> <br>Manuel Echazarra
> </i>

# Stocks traded
![Screenshot 2021-06-17 at 3 53 46 PM](https://user-images.githubusercontent.com/63654846/122463914-35ca1180-cf84-11eb-8cbb-beadf05ba7e9.png)

# LSTM model
![Screenshot 2021-06-17 at 3 54 34 PM](https://user-images.githubusercontent.com/63654846/122464136-7e81ca80-cf84-11eb-89c8-a18c905ba689.png)

# Performance of the LSTM model on training data
![Screenshot 2021-06-17 at 3 58 18 PM](https://user-images.githubusercontent.com/63654846/122464559-fbad3f80-cf84-11eb-8319-f7e34f5fc5a9.png)

# Performance of the LSTM model on testing data
![Screenshot 2021-06-17 at 3 58 18 PM](https://user-images.githubusercontent.com/63654846/122464528-f3550480-cf84-11eb-9e8b-8328f3bdd0aa.png)

