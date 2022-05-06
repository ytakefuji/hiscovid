# hiscovid
hiscovid is a PyPI tool that calculates time transition scores for individual policies against COVID-19.

The goal of hiscovid is for policymakers to understand fatal mistakes by their decisions.
Policymakers must learn their mistakes for possible corrections in the future.

The time transition score is calculated by dividing the number of deaths in the time series 
due to COVID-19 by the population in millions.

Scores monotonically increase so that policymakers can only suppress them, but cannot improve them.
Mistakes by policymakers cannot be corrected and are fatal forever.

The lower the score, the better the policy.

In other words, the score is equivalent to the accumulation of mistakes made by policymakers.

The perfect policy outcome means there are no covid-19 deaths. There is no perfect policy in the world, but
mistakes by policymakers can be corrected for future better decisions.


hiscovid scrapes the latest data from the following site over the Internet:

https://covid.ourworldindata.org/data/owid-covid-data.csv

Mistakes can be observed in the calculated graph.

# How to install hiscovid
$ pip install hiscovid

# How to run hiscovid
$ hiscovid Japan 'South Korea'

<img src='https://github.com/ytakefuji/hiscovid/raw/main/result.png' height=480 width=640>

In the graph of South Korea, there are two points where the slope of the scoreline changed abruptly,
including mid-November 2021 and mid-February 2022.

In the graph of Japan, there is a single abruptly changed point around mid-January 2022.


$ hiscovid Taiwan 'New Zealand'

<img src='https://github.com/ytakefuji/hiscovid/raw/main/twnz.png' height=480 width=640>

There is one point in the Taiwan graph that changes abruptly around mid-May 2021.

There is one point in the New Zealand graph that changes abruptly around the beggining of March 2022.

$ hiscovid Taiwan 'United States' 'United Kingdom'

<img src='https://github.com/ytakefuji/hiscovid/raw/main/twusuk.png' height=480 width=640>

In the US graph, it is constantly bad, but a single point that changes abruptly around the mid-July 2021.

In the UK graph, there are two points where the slope of the scoreline changed abruptly,
including the beggning of April 2020 and mid-November 2021.

