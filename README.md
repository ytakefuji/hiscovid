# hiscovid
[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/5655627/tree)

Takefuji Y. (2022) hiscovid for calculating time transition scores of policies against COVID-19 [Source Code]. https://doi.org/10.24433/CO.7364293.v1

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
$ hiscovid <country name(s)>

$ hiscovid Japan 'South Korea'

<img src='https://github.com/ytakefuji/hiscovid/raw/main/result.png' height=480 width=640>

$ hiscovid Japan Taiwan

<img src='https://github.com/ytakefuji/hiscovid/raw/main/twjp.png' height=480 width=640>


The vertical axis shows the overall result scores for policy, individual behavior, vaccination, 
and new COVID-19 variants. 
Score is the number of deaths due to COVID-19 per population in millions.

In the graph of South Korea, there are two points where the slope of the scoreline changed abruptly,
including mid-November 2021 and mid-February 2022.

In the graph of Japan, there is a single abruptly changed point around mid-January 2022.


$ hiscovid Taiwan 'New Zealand'

<img src='https://github.com/ytakefuji/hiscovid/raw/main/twnz.png' height=480 width=640>

There is one point in the Taiwan graph that changes abruptly around mid-May 2021.

There is one point in the New Zealand graph that changes abruptly around the mid-February 2022.

$ hiscovid Taiwan 'United States' 'United Kingdom'

<img src='https://github.com/ytakefuji/hiscovid/raw/main/twusuk.png' height=480 width=640>

In the US graph, the scoreline is constantly bad, but a single point that changes abruptly around the mid-August 2021.

In the UK graph, there are two points where the slope of the scoreline changed abruptly,
including the mid-March 2020 and the mid-October 2020.

