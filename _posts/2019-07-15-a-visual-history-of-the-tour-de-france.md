---
title: A Visual History of the Tour de France
tags: [Data Science, Web Scraping, Data Viz, Bikes]
style: fill
color: light
description: Charting the last century of Tour de France races.
---

<br>

On July 2, the largest annual sporting event in the world got underway for the 110th (?) time in history. The Tour de France is perhaps the most famous cycling race in the world because of its combination of grit and grace: each year the top cyclists in the world endure 21 punishing days of racing while winding their way through picturesque backdrops of the lavender fields of Provence and the peaks of the Pyrenees. I was curious how today's Tour differs from its earliest days, so I wrote a web-scraper in Python to compile information on each race going back to 1903, the first year the Tour took place. The official race website contains [historical stats](https://www.letour.fr/en/) on each year's race, including information on rankings at the end of each day of racing, the route, and race times and winners. Using this information, I wanted to chart the last century of Tour de France races to explore how it has evolved throughout history. 

<br>

#### *Le Tour* has criss-crossed every corner of France

One aspect of the Tour de France that makes it such a unique sporting event is how the race course changes from one year to the next. Some years, the race has even dipped into neighboring Italy or Spain. As a result, no two races in history are alike. The starting city of each year's race rotates every year, though since 1975 every race has concluded with a final leg along the Champs-Elysees in Paris.

The interactive [chord chart](https://en.wikipedia.org/wiki/Chord_diagram) below plots links between every city in which at least 5 Tour stages have taken place since 1903. Each node along the circle's edge denotes a city, and each line running between nodes represent a single stage throughout history. Lines sharing the same color as a city's node show stages that originated from that city, while lines with different colors show stages that finished in that city. For example, Paris (dark blue, 3 o'clock) has most often been the end of a stage, with stages starting from Caen (orange), Dunkerque (pink), Versailles (purple) and Dijon (brown). In total, ### stages have passed through Paris. XXX has hosted the most stages overall. 

<iframe src="/images/tdf/chord.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="700"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

<br>

#### *Le Tour* through the ages

How has the Tour de France evolved since 1903? One way in which the races of the 21st century differ from earlier routes is in length. Since 1999, the number of days of racing (or "stages") of the Tour has remained the same each year, remaining constant at 21 days. But in earlier eras the number of stages could vary widely from one year to the next. The 1937 race consisted of 32 stages, the most in history. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/00_num_stages_over_time.png" alt="num_stages_over_time" width="700"/>

Another way to look at the make-up of the race is through the lens of nationality. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/04_nationalities_of_riders.png" alt="nationalities_of_riders" width="700"/>

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/05_euro_riders.png" alt="euro_riders" width="700"/>

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/06_noneuro_riders.png" alt="noneuro_riders" width="700"/>

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/07_nationality_mixture_over_time.png" alt="nationality_mixture_over_time" width="700"/>

<br>

#### Who are the most successful riders in history?

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/13_lifetime_jersey_winners.png" alt="lifetime_jersey_winners" width="700"/>

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/01_cumulative_yellow_jerseys_over_time.png" alt="cumulative_yellow_jerseys_over_time" width="700"/>

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/02_rankings_2018.png" alt="rankings_2018" width="600"/>
