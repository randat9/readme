# Project sky trading
 
 
## About

The project has the objective of learning Reinforcement Learning, the algorithm will be based on data from IQFeed, the main goal is to create an algorithm that the bot will open a position and we close it or open a position and the bot close it,
 all projects are closely related to the goal of creating an algorithm



## Getting Started 


##### Tools
* Jenkins
* Github

## Instalation 

### IQFeed Downloader

Python scripts created to use with DTN IQFeed Market Data application. Connect to IQFeed socket, download historical data or start a live flow of prices for desired ticker.


#### How to use?

1. Clone the repository `git clone https://github.com/skygate/sky-trading` or download both files.
2. Log into any IQFeed application and have it running in the background - make sure you've bought the data plan that contains desired ticker. 

![](https://user-images.githubusercontent.com/26166097/131078951-463583e1-2c28-4e0f-a3e4-60264fbecc0f.png | width = 250)


#### Running the script

There are two ways of running the script and here are the examples:
- historical data access
```
python iqfeed_downloader historical 127.0.0.1 9100 20210201 20210220 1 TLRY GME
```
As in example you have the specify that you want to obtain the historical data, hence "historical", after you put the ip address and port, then start and end date followed by the list of tickers (stock names) you want to download.

If you run the IQFeed app on your PC then the socket address is **localhost** on port **9100**, else you have to use the proxy address.

Date has to be in **YYYYMMDD** format.

As return the script saves CSV file with name: **TICKER_STARTDATE_ENDDATE_INTERVAL.CSV**

- live data access
```
python iqfeed_downloader live 127.0.0.1 5009 AMC
```
You only have to feed it three things: host address, host port and ticker name. In return it prints live tick data of desired stock until interrupted.

Default port of IQFeed live data socket is **5009**.



######Getting Started - Reinforcement learning (RL):

if you want start learn please [read](https://en.wikipedia.org/wiki/Reinforcement_learning), this will help you understand material from RL 

The first programs you can write

 [Tic-tac-toe](https://towardsdatascience.com/reinforcement-learning-implement-tictactoe-189582bea542) - version of popular entry reinforcement learning problem, Contains tools for statistical comparation of training epochs/chance of winning versus the bot. 
 
 [Gokart](https://gym.openai.com/envs/MountainCar-v0/#id1) - A car is on a one-dimensional track, positioned between two "mountains". The goal is to drive up the mountain on the right; however, the car's engine is not strong enough  to scale the mountain in a single pass. Therefore, the only way to succeed is to drive back and forth to build up momentum. Here, the reward is greater if you spend less energy to reach the goal no i tu tez colab
 
 Karty - Playing Cards is the project where we use python to solve game card problem to find a good results, 
is intended to be a card game between two players, the player with the most points wins [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h1RjOziH5jb5OuE33Pj00O53FxZ8KCxF?authuser=1#scrollTo=U5Sq79GmiQoZ]




## Examples and running 

A model of the whole project
![image](https://user-images.githubusercontent.com/26166097/131041029-c1fb79bd-cca1-4b10-9d2e-1abc435007cc.png)
