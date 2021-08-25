# Project sky trading

# About

The project has the objective of learning rl, the algorithm will be based on data from IQFeed, the main goal is to create an algorithm that the bot will buy a position and we sold it or open a position and the BOT sold it,
 all projects are closely related to the goal of creating an algorithm


# Getting Started 

Getting Started - Reinforcement learning (RL):

 Tic-tac-toe - version of popular entry reinforcement learning problem, Contains tools for statistical comparation of training epochs/chance of winning versus the bot. 
 Gokart - A car is on a one-dimensional track, positioned between two "mountains". The goal is to drive up the mountain on the right; however, the car's engine is not strong enough  to scale the mountain in a single pass. Therefore, the only way to succeed is to drive back and forth to build up momentum. Here, the reward is greater if you spend less energy to reach the goal
 Karty - Playing Cards is the project where we use python to solve game card problem to find a good results, 
is intended to be a card game between two players, the player with the most points wins


# Instalation 

# IQFeed Downloader

Python scripts created to use with DTN IQFeed Market Data application. Connect to IQFeed socket, download historical data or start a live flow of prices for desired ticker.


## How to use?

1. Clone the repository or download both files.
2. Log into any IQFeed application and have it running in the background - make sure you've bought the data plan that contains desired ticker. 
3. Run the script.


## Running the script

There are two ways of running the script and here are the examples:
- historical data access
```
python iqfeed_downloader historical 127.0.0.1 9100 20210201 20210220 1 TLRY GME
```
- live data access
```
python iqfeed_downloader live 127.0.0.1 5009 AMC
```

### Historical access

As in example you have the specify that you want to obtain the historical data, hence "historical", after you put the ip address and port, then start and end date followed by the list of tickers (stock names) you want to download.

If you run the IQFeed app on your PC then the socket address is **localhost** on port **9100**, else you have to use the proxy address.

Date has to be in **YYYYMMDD** format.

As return the script saves CSV file with name: **TICKER_STARTDATE_ENDDATE_INTERVAL.CSV**

### Live access

You only have to feed it three things: host address, host port and ticker name. In return it prints live tick data of desired stock until interrupted.

Default port of IQFeed live data socket is **5009**.


# Examples and running 
