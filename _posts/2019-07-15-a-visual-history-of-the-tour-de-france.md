---
title: A Visual History of the Tour de France
tags: [Data Science, Web Scraping, Data Viz, Bikes]
style: fill
color: light
description: An article exploring the last century of Tour de France races.
---

<br>

On July 2, 2019, the largest annual sports competition in the world, the Tour de France, got underway for the 105th time in history. The Tour is the most famous cycling race in the world perhaps due to its combination of grit and grace: each year the top cyclists in the world endure 21 punishing days of racing while winding their way through picturesque backdrops of the lavender fields of Provence and the peaks of the Pyrenees. I was curious about how today's Tour differs from its earliest days, so I wrote a web-scraper in Python to compile information on each race going back to 1903, the first year the Tour took place. The official race website contains [historical statistics](https://www.letour.fr/en/history) on each year's race, including information on daily race standings, details about the route, race times and winners. Using this information, I wanted to chart the last century of Tour de France races to explore how it has evolved throughout history. 

#### The Tour has criss-crossed every corner of France

One aspect of the Tour de France that makes it such a unique sporting event is how the race course changes from one year to the next. Some years, the race has even dipped into neighboring Italy or Spain. As a result, no two races in history are alike. The starting city of each year's race rotates every year, though since 1975 every race has concluded with a final leg along the Champs-Elysees in Paris.

The interactive [chord chart](https://en.wikipedia.org/wiki/Chord_diagram) below plots links between every city in which at least 5 Tour stages have taken place since 1903. Each node along the circle's edge denotes a city, and each line running between nodes represents a single stage throughout history. Lines sharing the same color as a city's node show stages that originated from that city, while lines with different colors show stages that finished in that city. For example, Paris (dark blue, 3 o'clock) has most often been the end of a stage, with stages starting from Caen (orange), Dunkerque (pink), Versailles (purple) and Dijon (brown). In total, 63 stages have passed through Paris, while Bordeaux has hosted the most stages overall at 78. 
<iframe src="/images/tdf/chord.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>  

#### *Le Tour* through the ages

How has the Tour de France evolved since 1903? One way in which the races of the 21st century differ from earlier routes is in length. Since 1999, the number of days of racing (or "stages") of the Tour has remained constant at 21. But in earlier eras the number of stages could vary widely from one year to the next. The 1937 race consisted of 32 stages, the most in history. The chart below also shows two breaks in racing that correspond with World War I and World War II. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/00_num_stages_over_time.png" alt="num_stages_over_time" width="700"/>

Another way to explore how the Tour has changed is in the composition of riders themselves. For instance, you can look at the make-up of the race through the lens of nationality. Unsurprisingly, French riders are far and away the most well represented among the racers throughout history. What's more surprising is the extent to which the number of French competitors dwarfs all other countries: the number of riders from France overall (about 5,400) nearly equals the next three countries combined (Belgium, Italy and Spain). For reference, races in recent years have included between 180 and 200 competitors. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/04_nationalities_of_riders.png" alt="nationalities_of_riders" width="700"/>

*Le Tour* remains a sporting event dominated by Europeans. France, Belgium, Italy, Spain and the Netherlands have each had over 900 riders compete in the Tour. Thirty European countries have participated in all, though many have sent just a handful of riders. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/05_euro_riders.png" alt="euro_riders" width="700"/>

When we look at all non-European countries, Colombia, the United States and Australia stand out as having the best representation in the Tour. The chart below shows that other than Colombia and the United States, very few other countries from the Americas (dark and light red) have competed in the Tour. Yet competitors from Asia (dark blue) and Africa (light blue) are even rarer.   

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/06_noneuro_riders.png" alt="noneuro_riders" width="700"/>

The chart below looks at how the composition of racers' nationalities has fluctuated over time. What's striking is how French-heavy earlier Tours once were, and even today France is still the best-represented country. In the earliest years of the Tour, France and Belgium made up nearly 100% of riders. It wasn't until the pre-WWII period that the share of countries other than France and Belgium approached 50%. Interestingly, German riders first began to compete in the Tour in the late-1930s, but in the aftermath of WWII don't seem to return to the competition until the late 1950s. Recent decades have seen a notable spike in the participation of more countries. The United States, for instance, didn't begin to send significant numbers of riders until the 1980s. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/07_nationality_mixture_over_time.png" alt="nationality_mixture_over_time" width="700"/>

<br>

#### Who are the most successful riders in history?

There are a number of ways of looking at the best-performing racers in the history of the Tour. The most straightforward way to quantify this is to look at those with the most jersey wins in history. Race officials award four different types of colored cycling jerseys for various award categories. The yellow jersey (or *Le maillot jaune*) is awarded to the rider with the fastest cumulative time in the race overall. The tradition of awarding jerseys didn't start until 1919, when the Belgian Firmin Lambot was presented with the first yellow jersey in history. The green jersey, given to the winner of the most sprint stages, weren't given out until 1933. (Certain segments of each Tour will reward racers points for finishing sprint courses with faster times.) Race officials also reward riders who perform the best in mountainous stages with the polka-dot jersey, a tradition that started in 1953. More recently, the white jersey is also given out the best young rider in each year's race. This practice was adopted in 1977. 

The chart below shows lifetime jersey counts for yellow, green and polka-dot jersey winners. Many of the sport's most legendary riders appear on the graph. There are also a handful of riders throughout history who have won multiple jerseys in the same year. Two riders have won both the yellow and polka-dot in the same year (Richard Virenque in 2003 and Chris Froome in 2015), while Andy Schleck won the yellow and white jerseys in 2010. Nairo Quintana became the first man to simultaneously win the polka-dot and white jerseys. No rider has yet won both the yellow and green jerseys in the same year. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/13_lifetime_jersey_winners.png" alt="lifetime_jersey_winners" width="700"/>

While most people would probably point to lifetime yellow jersey wins as the best metric to compare the best performers in the history of the Tour, another way to look at this might be cumulative jersey wins. At the end of each day of racing, the rider with the fastest overall time at that point is awarded a yellow jersey. Using this information, I added up the number of yellow jerseys awarded to a rider after every stage he ever raced and looked at the top performers. The chart below shows that by this measure Eddy Merckx has been the best racer ever, having racked up 110 yellow jersey wins. In other words, after every stage that Merckx has ever raced in in the Tour, he's been in first place overall 110 times in his career. Lines with steeper slopes show riders that accumulated yellow jerseys in a shorter span of time. Vertical lines represent riders that won multiple yellow jerseys in a just single year. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/01_cumulative_yellow_jerseys_over_time.png" alt="cumulative_yellow_jerseys_over_time" width="700"/>

It's also possible to use this stage-level information to look at how a single year's race unfolded. For example, the chart below shows how daily standings for all riders changed after each day of racing in the 2018 Tour de France. The x-axis shows each stage in the 2018 race, while the y-axis shows ranking. Each individual line represents one rider. At the end of the first day of racing, Fernando Rendon was in first place. After being over taken by Peter Sagan on the second day, Rendon dropped all the way to the 100s before dropping out from the race altoghether by stage 11. By contrast, Geraint Thomas from Great Britain steadily climbed up the rankings during the first few stages. After taking hold of the yellow jersey by stage 11, he never relinquished first place for the rest of the race. Many stages seem to show very little overall changes in rankings, which likely correspond to flat stages (which make gaining or losing time relative to other racers rather difficult). By contrast, stages that seem to line up with dramatic swings in the standings seem to be the more mountainous stages, where large leads in the race are often won or lost. 

<img src="https://raw.githubusercontent.com/yontartu/tour-de-france/master/img/02_rankings_2018.png" alt="rankings_2018" width="600"/>

One thing you may have noticed about the above charts showing top jersey winners is the conspicuous omission of Lance Armstrong, who was known as the most dominant cyclist in the history of the sport before admitting to using performance enhancing drugs. It appears as though race officials have completely scrubbed his name from the records, as well as other known dopers. 

Code snippets showing how I built some of these charts can be found [here](https://yontartu.github.io/projects/2-tour-de-france).