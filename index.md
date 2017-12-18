---
layout: post
title:  "Consequences of AirBnB on cities"
date:   2017-12-16 11:36:50 +0100
---

## Introduction
Airbnb is without a doute a dominant housing platform in Europe. There is a lot of controversy about it. Some find that it opens the market in a good way, allowing cheap housing in apartments for everybody, while helping people paying for their rent. Some seem to consider it as the harbinger of doom of the hotel industry, while bringing up the price of housing for the local population. We do not want to take position in this debate, but rather to shed light on some facts about the service.

There is a lot of variety on the usage of Airbnb across countries. To get some insight about the situation in Europe, we chose Amsterdam and Berlin. Two cities in the top 10 of the most visited cities in Europe by tourists, while being rather different, especially in size. They both acted to regulate Airbnb around 2016, in different ways. Berlin banned the service entirely, to decide later to allow it again under strict condition and restricted time for private people. Amsterdam on the other side made a deal directly with the company to limit the ability the rent an apartment to a limited number of days per year.

We will first investigate on the small coastal city of Amsterdam, and then on the gigantic international city of Berlin. For those two we will look first at the usage of Airbnb and how it evolved over time. The data comes from [Inside Airbnb](http://insideairbnb.com), a project to help explore the website. We will enrich this analysis using several open data website about the cities themselves. We notably used [Berlin Open Data](https://daten.berlin.de/) and [the Netherlands data portal](https://data.overheid.nl/). The goal is then to see if there are correlations between data we know about the cities and different parameters.

After these explorations, we will try to understand better what might be general about the tourists behavior when traveling. 

## Amsterdam

### General
As announced previously, our first focus for this analysis will be Amsterdam. Amsterdam is small (220 km^2, 850 000 inhabitants), yet very touristic.

The city tried to limit the usage of AirBnb in 2017 by allowing private people to rent their entire home (as listed on the website) only 60 days per year (private rooms are not taken into account in this limitation).

The following map gives a very brief overview of the city, how are organised the neighbourhoods, it also shows the number of AirBnB rentals available in each of those neighbourhoods. 

{% include am_neighbourhoods_map.md %}

As we can see on this map, there are much more AirBnb available in the neighbourhoods close to the city center than in the one a little farther.

A study was made by the city of Amsterdam regarding the satisfaction of its dwellers with respect to several criteria. The graph below show corellations in-between those, and also compared to the amount of Airbnb. We note that the first column, depending on the amount of Airbnb, is less corelated to the satisfaction values than themselves. This correlation can also be explained by proximity to city center.

{% include am_satisfaction_corr.md %}

-- *TODO_GRAPH* compare satisfaction with living env to airbnb

### Over the years

While comparing the data from 2015 and 2017, we also noticed that the average price on Airbnb went up quite uniformaly. The raise is higher than normal inflation. Maybe this is due to the restricting agreement. Owners might need to pull up a higher price in order to make profit.

{% include am_price_years.md %}

As mentioned before, Amsterdam took steps in 2017 to regulate the market. We can clearly see this in effect when ploting the amount of days available per apartment. There is a shift towards shorter availability periods below 60 days. We can still surprisingly see that a lot of appartment where available for more than 60 days. It is probably due to the fact that availability doesn’t mean that the apartment was actually rented.

*TODO_graph* {% include am_availability_days_histogram.md %}

The law didn’t really impact creation of new Airbnb. We could even think that it actually created a need for more apartment, since they can be rented less time. The neighborhoods with the higher increase in Airbnb amount are shown below. They are mainly concentrated around the center.

-- *TODO graph* {% include am_top_neighbourhoods.md %}

-- *TODO graph* compare number of housing to number of Airbnb

-- *TODO* corelation airbnb and land stock price

## Berlin

### General
** story about law

** overview of city

{% include be_neighbourhoods_map.md %}

-- *TODO* where are airbnb

### Over the years

** evolution of price 

*TODO* {% include be_price_years.md %}

** availability per day

*TODO* {% include be_availability_days_histogram.md %}

** top neighborhood

*todo* {% include be_top_neighbourhoods.md %}

-- *TODO* compare tourist income with airbnb increase

-- *TODO* corelation airbnb and rental price

-- *Todo* compare overnight with airbnb growth

## Possible links between Airbnb and the city ecosystem

-- *TODO* compare what can be compared

## Conclusion