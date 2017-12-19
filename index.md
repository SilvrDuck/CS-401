---
layout: post
title:  "Consequences of AirBnB on cities"
date:   2017-12-16 11:36:50 +0100
---

## Introduction
Airbnb is without a doute a dominant housing platform in Europe. There is a lot of controversy about it. Some find that it opens the market in a good way, allowing cheap housing in apartments for everybody, while helping people paying for their rent. Some seem to consider it as the harbinger of doom of the hotel industry, while bringing up the price of housing for the local population. We do not want to take position in this debate, but rather to shed light on some facts about the service and its use.

There is a lot of variety on the usage of Airbnb across countries. To get some insight about the situation in Europe, we chose Amsterdam and Berlin. Two cities in the top 10 of the most visited cities in Europe by tourists, while being rather different, especially in size. They both acted to regulate Airbnb around 2016, in different ways. Berlin banned the service entirely, to decide later to allow it again under strict condition and restricted time for private people. Amsterdam on the other side made a deal directly with the company to restrict the ability the rent an apartment to a limited number of days per year.

We will first investigate on the small coastal capital city of Amsterdam, and then on the gigantic international city of Berlin. For those two we will look first at the usage of Airbnb and how it evolved over time. The data comes from [Inside Airbnb](http://insideairbnb.com), a project to help explore the website. We will enrich this analysis using several datasets from open data website of the cities themselves. We used [Berlin Open Data](https://daten.berlin.de/) and [the Netherlands data portal](https://data.overheid.nl/). The goal is then to see if there are correlations between facts about the cities and what we see from Airbnb.

After these explorations, we will try to understand better what might be general about the tourists behaviour when traveling. 

## Amsterdam

### General
As announced previously, our first focus in this analysis will be Amsterdam. Amsterdam is small --- 220 km<sup>2</sup>, 850.000 inhabitants --- yet very touristic.

In 2017, the city tried to limit the usage of AirBnb by allowing private people to rent their entire home only 60 days per year (private rooms are not taken into account in this limitation).

The following map gives a very brief overview of the city and how are the neighbourhoods organised. Click on a district to see the amount of Airbnb in the area as of 2015.

{% include am_neighbourhoods_map.md %}

As we can see on this map, there are much more AirBnb available in the neighbourhoods close to the city center than far away from the center.

A study was made by the city of Amsterdam regarding the satisfaction of its dwellers with respect to several criteria. The graph below show correlations in-between those, and also compared to the amount of Airbnb. We note that the first column, depending on the amount of Airbnb, is less correlated to the satisfaction values than they are in between. This correlation can also be explained by proximity to city center, in other word, people seem more interested by the location of the Airbnb and its distance to the city center than the neighbourhood itself.

{% include am_satisfaction_corr.md %}

### Over the years

The first number we want to highlight when talking about Airbnb in Amsterdam is the enormous increase in the amount of housing available through Airbnb between 2015 and 2017. Indeed, we found only 7k unique housing for 2015 and more than 15k for 2017, this is more than a times two factor !

#### Price evolution

While comparing the data from 2015 and 2017, we also noticed that the average price on Airbnb went up quite uniformly. Maybe this is due to the restricting agreement. Owners might need to pull up a higher price in order to make profit.

{% include am_price_years.md %}

Looking at this graph, we see that there are spikes of price every weekend, and that the price during the summer vacation is way less predictable.

We can put this realization in perspective with the plot price distribution in the city between 2015 and 2016.

{% include am_price_boxplot.md %}

From this graph, we clearly see that the housing price in Amsterdam raised a lot between 2015 et 2016. What is interesting though is that *Airbnb’s price went up by 118% on average, while plot price went up 130%*.

#### Attempts at regulation

As mentioned before, Amsterdam took steps in 2017 to regulate the market. We can clearly see this in effect when plotting the amount of days available per apartment. There is a shift towards shorter availability periods below 60 days. We can still surprisingly see that a lot of apartment where available for more than 60 days. It is probably due to the fact that availability doesn’t mean that the apartment was actually rented.

{% include am_availability_days_histogram.md %}

The law didn’t really impact creation of new Airbnb. We could even think that it actually created a need for more apartment, since they can be rented less time. The neighbourhoods with the higher increase in Airbnb amount are shown below. They are mainly concentrated around the center.

{% include am_top_neighbourhoods.md %}

The following graph show a normalised vision of this increase with respect to the number of housing per neighbourhood.

{% include am_increase_in_neighbourhoods.md %}

The situation in 2017 is hence the following.

{% include am_airbnb_rate_2017.md %}

The goal of the regulation was to lessen the harmful effect of Airbnb on the local population. We can only see that it might have made the matter worst by encouraging people speculating on multiple apartments.

## Berlin

### General

Berlin is the capital of the Germany, it's also its largest city with more than 3.5 millions inhabitants and approximately 900km<sup>2</sup>.
As we did for Amsterdam, the following map gives an overview of the city and its districts. Click to see the number of Airbnb on a given district.

{% include be_neighbourhoods_map.md %}

We can notice a stronger density or Airbnb in the city center but it not as noticeable as in Amsterdam, this is mainly due to the fact that Berlin is much wider and do not have a single center.

### Over the years

In 2016 there was, approximatly 15k unique Airbnb available. In 2017 this number reached 20k, this is an increase factor of roughly 33% in single year !

#### Prices

Contrary to Amsterdam, where the price of airbnb increased a lot, the price in Berlin actually decreased (not as much as the price increase in Amsterdam, but still enough to be visible on the following graph).

{% include be_price_years.md %}

We clearly see an intriguing drop around May 2016. This particularly interesting, since in 2016 the city of Berlin decided to ban entirely the service. This entered into effect the 1st of may 2016. This hence explained. The curve comes back to regular usage in September, when it was again allowed for owners of second home. As we can see, the 2017 curve is much more in line with what we would expect after analysing Amsterdam.

#### Ban and availability

The following graph shows some interesting figures about the number of days available of each apartment. In 2015, before the ban, a lot more apartment where available year round. The new Airbnb created are then probably more about renting one room some days of the year rather than buying a full apartment just for rentability’s sake.

{% include be_availability_days_histogram.md %}

#### Where did it change?

We have seen that the density of Airbnb in the city center is higher. We were also interested to see where the increase of Airbnb is mainly located. To our surprise, it was in suburban districts that the increase was the strongest, as this map tells. We show here the top 15 districts in term of increase.

{% include be_map_top_districts.md %}

We then looked at the other side of the coin and saw that some neighbourhoods had experienced a decrease in amount of Airbnb. All of them were as well located outside of the city and had lost a dozen of Airbnb. A notable exception is Marzahn-Süd which went from 257 Airbnbs in 2016 to only 13 in 2017.

{% include be_map_worst_districts.md %}

In the following plot, we tried to see if the average square meter price to rent an apartment had any influence on the price the owner would rent its apartment. To our surprise, it didn’t. Each dot represents one district of Berlin.

{% include be_square_meter_versus_price.md %}

The outlier is due to a very expensive Airbnb in Haselhorst, where there is not much Airbnb.

## Possible links between Airbnb and the city ecosystem



## Conclusion

To conclude, we have learn a little bit more about the distribution and evolution of Airbnb in those two cities. What we see is that political solutions to help local hospitality service rival against the American giant are hard to put into practice effectively. In both Berlin and Amsterdam, the before and after the law weren’t much different on a statistical level. Except that in Berlin, the market went down for a few month.
