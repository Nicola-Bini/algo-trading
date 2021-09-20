# Summary

An algorithm that combine the output of a neural network and a text analytics analysis to trade stocks.
This work is part of our course <b>"Algorithmic trading with Python"</b> at <b>Hult University</b> with <b>Professor Micheal Rolleigh</b>.

Our team had around 4 days to dedicate to this project, during this time we had to:

<ol>
  <li>Get to know each other</li>
  <li>Come up with a trading strategy</li>
  <li>Find a way to implement it in Python</li>
  <li>Backtest it and compare results with a benchmark strategy</li>
</ol>


# Findings
We decided to implement an LSTM model and combine its recommendation with the sentiment analysis on the tweets. In particular we decided to follow the recommendation provided by the LTSM only when the sentiment analysis was recommending the same (either buy or sell). If the 2 models did not agree with each other we would just close all the current positions and take any other position until they agreed with each other again.

At the end, our model had an outstanding performance on the traning data (due to overfitting) and a poor performance in the testing data (compared to benchmark strategy of buying and holding the assets). However, combining the LSTM model with the sentiment analysis allowed us to achieve a better performance than either of the models taken alone.


# Team
> <i>Felipe Domingues
> <br>Manuel Echazarra
> <br>Nicola Bini
> <br>Tri Dung Dinh
> </i>

# Stocks traded
![Screenshot 2021-06-17 at 3 53 46 PM](https://user-images.githubusercontent.com/63654846/122463914-35ca1180-cf84-11eb-8cbb-beadf05ba7e9.png)<br>

# LSTM model
![Screenshot 2021-06-17 at 3 54 34 PM](https://user-images.githubusercontent.com/63654846/122464136-7e81ca80-cf84-11eb-89c8-a18c905ba689.png)<br>

# Performance of the LSTM model on training data
![Screen Shot 2021-09-19 at 9 29 27 PM](https://user-images.githubusercontent.com/63654846/133949925-2f224a09-71d2-40a6-937b-4ecd61cfbecc.png)
)<br>

# Performance of the LSTM model on testing data
![Screenshot 2021-06-17 at 3 58 18 PM](https://user-images.githubusercontent.com/63654846/122464528-f3550480-cf84-11eb-9e8b-8328f3bdd0aa.png)<br>

# Performance of all the tested models on testing data
<img width="954" alt="Screenshot 2021-06-21 at 12 59 35 PM" src="https://user-images.githubusercontent.com/63654846/122800109-8bf2c980-d290-11eb-8fd9-c07e29b88dfd.png"><br>


# Presentation pictures

![35e8e755-f1d6-4658-963f-cfd78b286cf1](https://user-images.githubusercontent.com/63654846/122800672-366aec80-d291-11eb-98a3-815a34028722.jpg)
![210ba7ac-1c24-4402-baea-463737e1d4dd](https://user-images.githubusercontent.com/63654846/122800674-366aec80-d291-11eb-9db7-3c1997c014ed.jpg)
![da9632a0-3693-47b9-b3bb-78b522afb3fb](https://user-images.githubusercontent.com/63654846/122800675-366aec80-d291-11eb-9c62-904c515fc3fc.jpg)
![5c7709e1-dafe-41d0-ae42-b250d1a2a03e](https://user-images.githubusercontent.com/63654846/122800671-35d25600-d291-11eb-938c-c7f311278923.jpg)
