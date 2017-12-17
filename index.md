---
layout: post
title:  "Consequences of AirBnB on cities"
date:   2017-12-16 11:36:50 +0100
---

# Airbnb data analysis
## Introduction
Airbnb is without a doute a dominant housing platform in Europe. There is a lot of controversy about it. Some find that it opens the market in a good way, allowing cheap housing in apartments for everybody, while helping people paying for their rent. Some seem to consider it as the harbinger of doom of the hotel industry, while bringing up the price of housing for the local population. We do not want to take position in this debate, but rather to shed light on some facts about the service.

There is a lot of variety on the usage of Airbnb across countries. To get some insight about the situation in Europe, we chose Amsterdam and Berlin. Two cities in the top 10 of the most visited cities in Europe by tourists, while being rather different, especially in size. They both acted to regulate Airbnb in 2016, in different ways. Berlin banned the service entirely, to decide later to allow it again under strict condition and restricted time for private people. Amsterdam on the other side made a deal directly with the company to limit the ability the rent an apartment to a limited number of days per year.

We will first investigate on the small coastal city of Amsterdam, and then on the gigantic international city of Berlin. For those two we will look first at the usage of Airbnb and how it evolved over time. The data comes from [Inside Airbnb](http://insideairbnb.com), a project to help explore the website. After this, we will look at some data that we found about the cities themselves. Several open data website were used, most notably [Berlin Open Data](https://daten.berlin.de/) and [the Netherlands data portal](https://data.overheid.nl/). The goal is then to see if there are correlation between data we know about the cities and different parameters

After these explorations, we try to see if correlation

## Amsterdam

### General
As announced previously, our first focus for this analysis will be Amsterdam. Amsterdam is a small city (220 km^2, 850 000 inhabitants), yet very touristic.
The city tried to limit the usage of AirBnb in 2017 by allowing private people to rent their entire home (as listed on the website) only 60 days per year (private rooms are not taken into account in this limitation).

The following map gives a very brief overview of the city, how are organised the neighbourhoods, it also shows the number of AirBnB rentals available in each of those neighbourhoods. 

{% include amsterdam_neighbourhoods_map.md %}

As we can see on this map, there are much more AirBnb available in the neighbourhoods close to the city center than in the one a little farther.

### Over the years

{% include amsterdam_price_years.md %}

While we were comparing the data from 2015 and 2017, we also noticed that the number of available AirBnB increased in each and every neighbourhood of the city

{% include amsterdam_top_neighbourhoods.md %}

## Berlin

{% include berlin_neighbourhoods_map.md %}

## Possible links between Airbnb and the city ecosystem
## Conclusion