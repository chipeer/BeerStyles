Beer Ranking Study
================

## The Scenario

Lets say you are an entrepreneur with a passion for beer. Before opening
a brewery you want to know what types of beer are loved the most. You
plan to launch your brewery with a couple of flagship beers and you
believe if you appeal to most drinkers you will have a better chance of
taking off. Our data set we are working with has over 1.5 Million
reviews from Beer Advocate. Lets take a deep dive and answer these
questions. \* What are the top 5 beers? \* What style of beer is the
most popular? Shoutout to The Devastator for scraping this dataset from
Beer Advocate. License [CC BY-NC-SA
4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

## What are the top 5 beers?

Right now I want to take the time to make a prediction about what top 5
beers. I believe the top 5 will all be the same style of beer. That
would help us right away in deciding what type of beer we should make
first. We will only use beers that have at least 5 ratings.

### What did we find?

We found that people really like giving out 5 stars to beer, 468 beers
rated 5 stars. Really not what I was expecting. However, I think it will
give us good data for what style of beer people like the most out of the
5 star average beers.

    ## # A tibble: 468 × 4
    ## # Groups:   avg_score [1]
    ##    beer_name                                             brewe…¹ beer_…² avg_s…³
    ##    <chr>                                                 <chr>   <chr>     <dbl>
    ##  1 "\"Best Of Both Worlds\" Stout"                       Triang… Americ…       5
    ##  2 "10th Anniversary Bock-style Red Fox"                 Ezo Be… Bock          5
    ##  3 "10th Anniversary Strong Belgian"                     Beach … Belgia…       5
    ##  4 "120 Shilling Ale"                                    Lake P… Scotch…       5
    ##  5 "1906 Reserva Especial Can"                           Hijos … Americ…       5
    ##  6 "1908.0"                                              Witch'… Smoked…       5
    ##  7 "2005 Grand Cru"                                      BJ's R… Belgia…       5
    ##  8 "2009 Arquebus, Ch. Boswell Barrel Finish With Brett" Cambri… Americ…       5
    ##  9 "3-R Belgian"                                         Bear R… Americ…       5
    ## 10 "3 Threads"                                           McKenz… Saison…       5
    ## # … with 458 more rows, and abbreviated variable names ¹​brewery_name,
    ## #   ²​beer_style, ³​avg_score

## What style of beer is the most popular?

I am excited to find the answer to this. I believe IPA will be our
winner. I took beer rated 5 stars and the beer style had over 10 beers
on the list. Assume if it doesn’t have “American” as the first word of
the beer style that it is American.
![](Beer-Advocate-Case-Study_files/figure-gfm/style-1.png)<!-- -->
