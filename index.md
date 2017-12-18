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

In 2017, the city tried to limit the usage of AirBnb by allowing private people to rent their entire home (as listed on the website) only 60 days per year (private rooms are not taken into account in this limitation).

The following map gives a very brief overview of the city, how are organised the neighbourhoods, it also shows the number of AirBnB rentals available in each of those neighbourhoods. 

{% include am_neighbourhoods_map.md %}

As we can see on this map, there are much more AirBnb available in the neighbourhoods close to the city center than in the one a little farther.

A study was made by the city of Amsterdam regarding the satisfaction of its dwellers with respect to several criteria. The graph below show corellations in-between those, and also compared to the amount of Airbnb. We note that the first column, depending on the amount of Airbnb, is less corelated to the satisfaction values than themselves. This correlation can also be explained by proximity to city center, in other word, people seem more interested by the location of the Airbnb and its distance to the city center than the neighbourhood itself.

{% include am_satisfaction_corr.md %}



-- *TODO_GRAPH* compare satisfaction with living env to airbnb

### Over the years

The first number we want to highlight when talking about Airbnb in Amsterdam is the enormous increase in the amount of housing available through Airbnb between 2015 and 2017. Indeed, we found only 7k unique housing for 2015 and more than 15k for 2017, this is more than a times two factor !

While comparing the data from 2015 and 2017, we also noticed that the average price on Airbnb went up quite uniformaly. The raise is higher than normal inflation. Maybe this is due to the restricting agreement. Owners might need to pull up a higher price in order to make profit.

{% include am_price_years.md %}

An interesting plot to compare this price increase to is the following one. In this plot we see the distribution of prices per in Amsterdam in 2015 and 2016

{% include am_price_boxplot.md %}

From this graph, we clearly see that the housing price in Amsterdam raised a lot between 2015 et 2016.

As mentioned before, Amsterdam took steps in 2017 to regulate the market. We can clearly see this in effect when ploting the amount of days available per apartment. There is a shift towards shorter availability periods below 60 days. We can still surprisingly see that a lot of appartment where available for more than 60 days. It is probably due to the fact that availability doesn’t mean that the apartment was actually rented.

*TODO_graph* {% include am_availability_days_histogram.md %}

The law didn’t really impact creation of new Airbnb. We could even think that it actually created a need for more apartment, since they can be rented less time. The neighborhoods with the higher increase in Airbnb amount are shown below. They are mainly concentrated around the center.

-- *TODO graph* {% include am_top_neighbourhoods.md %}

-- *TODO graph* compare number of housing to number of Airbnb

The following two graphs show, before and after the regulation, the proportion of 

{% include am_airbnb_rate_2015.md %}
{% include am_airbnb_rate_2017.md %}

-- *TODO* corelation airbnb and land stock price

## Berlin

### General
** story about law

** overview of city

Berlin is the capital of the Germany, it's also its largest city with more than 3.5 millions inhabitants (and aproximately 900km^2).
As we did for Amsterdam, the following map gives an overview of the city and its districts (with the number of Airbnb on each one).

{% include be_neighbourhoods_map.md %}

We can notice a stronger density or Airbnb in the city center but it not as noticeable as in Amsterdam, this is mainly due to the fact that Berlin is much wider and do not have a single center.

In 2016 there was (according to our data), aproximatly 15k unique Airbnb availables. In 2017 this number reached 20k, this is an increase factor of roughly 33% in single year ! 

### Over the years

** evolution of price 

Contrary to Amsterdam, where the price of airbnb increased a lot, the price in Berlin actualy decreased (not as much as the price increase in Amsterdam, but still enough to be visible on the following graph).

{% include be_price_years.md %}


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