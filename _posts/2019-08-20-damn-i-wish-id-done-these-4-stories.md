---
title: Damn, I Wish I'd Done These 4 Stories
tags: [Data Science, Data Journalism,  Inspiration]
style: fill
color: light
description: Inspired by FiveThirtyEight's "jealously lists."
---

<br>

Every so often, FiveThirtyEight (one of my favorite sites) used to put together [lists of stories](https://fivethirtyeight.com/tag/envy/) carried by other news outlets that they wish they had published. They themselves borrowed this idea from Bloomberg News, which puts out an annual ["Jealously List"](https://www.bloomberg.com/features/2018-jealousy-list/). This led me to reflect on some of the coolest data journalism projects that I've come across and that have inspired me. Here are 4 pieces that I'm super jealous of.


#### [Nike Says Its $250 Running Shoes Will Make You Run Much Faster. What if That’s Actually True? (The Upshot)](https://www.nytimes.com/interactive/2018/07/18/upshot/nike-vaporfly-shoe-strava.html) 

In 2017, Nike released the [Zoom Vaporfly 4% running shoe](https://news.nike.com/footwear/nike-zoom-vaporfly-4), claiming that the $250 pair would shave 4% off of race times for competitors. The data journalism team at the New York Times set out to test this claim for themselves. To do so, they compiled data from public race reports and personal profiles from [Strava](https://www.strava.com/), a social network for athletes. 

The authors employed four approaches to measuring the Vaporfly's effect. The first was a statistical model controlling for runners' ages, genders and race histories. The second compared groups of runners who completed the same two races, examining the performance of those who switched their shoes to Vaporflies versus those who did not. The next approach examined runners who competed in multiple races and changed the shoes they used over time. Finally, authors probed the effectiveness of the Vaporflys by measuring the likelihood of a runner achieving a personal best time while wearing them. Using all four of these metholologies, the results show that Vaporflys really do make runners faster. As the authors put it: 

> Wherever we look for evidence that shoes matter in a marathon or half marathon, we find Vaporflys at or near the top of that list. More than that, the shoes tend to be outliers among all popular shoes, suggesting that there is something happening in races with Vaporflys that is not happening in races with nearly any other kind of popular shoe.

This project has it all: a fascinating dataset (which the authors assembled themselves through web scraping). Beautiful and intuitive visualizations. And a convincing answer to a fascination question of how effective these Nike shoes really are. 


#### [Are Juiced Balls The New Steroids? (FiveThirtyEight)](https://fivethirtyeight.com/features/are-juiced-balls-the-new-steroids/) 

In recent years, there's been a puzzling spike in the number of home runs being hit in Major League Baseball. The team of baseball writers at FiveThirtyEight has been leading the investigative charge in getting to the bottom of this mystery. Their conclusion: "juiced baseballs" (or baseballs engineered to travel farther) are likely responsible for the recent home run surge. Examining other potential explanations-hitters changing their offensive approaches or learning to hit fastballs better, or teams putting a premium on pitchers with higher velocity-didn't seem to offer conclusive evidence. All answers seems to be pointing to the baseball itself. But other than testing a batch of baseballs in a laboratory setting, how might data help shed light on this puzzle. Ben Lindbergh and Rob Arthur (the authors of the piece) realized that the MLB has "a built-in control group: the minor leagues." Exploring home run rates in the majors versus the minors could elucidate whether the home run spike may be stemming from player development trends. Yet while home run rates in the minors had mirrored the major-league rate for the past two decades, in recent years the two rates have diverged, showing a notable spike in the majors but not the minors. Clearly something different is going on in the majors. 

To further test this intriguing finding, the authors exploit a natural experiment by zeroing in on players who have played in both the major and minor leagues in recent seasons. Looking at just this smaller group of players who've played using these different baseballs, they find that players in Triple-A hit balls out of the park at a rate of 3 percent, but when playing with major league balls these same players' home run rates rise to 3.8 percent. The authors further drill down to keep conditions even more consistent by looking at head-to-head matchups between pitchers and batters who have played against one another at both the major- and minor league levels. This comparison also reveals an appreciable difference: "matchups between exactly the same hitters and pitchers are yielding many more homers in MLB than Triple-A." This is strong evidence that differences in baseballs are to blame. 

I'm a sucker for deep dives into fascinating pockets of baseball analytics. And I keep coming back to this article for inspiration for ways to uncover natural experiments. 


#### [The National Parks Have Never Been More Popular (FiveThirtyEight)](https://fivethirtyeight.com/features/the-national-parks-have-never-been-more-popular/) 

I love this piece by Andrew Flowers because it combines two of my favorite things: the great outdoors and data. Flowers doesn't make use of any fancy statistical techniques, but rather sets out to explore historical data from the National Park Service and chart how popular the national parks have been over time. To no one's surprise, some of the classics are found at the top of the list, with the Great Smokies at the top (with about 10 million average annual visitors, nearly double the second place Grand Canyon's 4.5 million visitors). Other icon parks like Yosemite and Yellowstone also make the top 5. But what makes me super jealous of this piece is one graph in particular, where Flowers plots the national parks' change in annual rankings over time. I'm obsessed with his ["bump chart"](https://www.kenflerlage.com/2017/01/my-thoughts-on-bump-charts-and-when-to.html) and have found myself returning to this article constantly as I've tried to build similar charts in my own projects. 


#### [We Read 150 Privacy Policies. They Were an Incomprehensible Disaster. (The Upshot)](https://www.nytimes.com/interactive/2019/06/12/opinion/facebook-google-privacy-policies.html) 

Kevin Litman-Navarro put together this neat piece analyzing the texts of privacy policies from various companies. There are two things I really love about this article. First is how it makes use of a pretty unique dataset and charts different privacy policies in a way that makes for easy comparison across companies. The second is the author's use of ["scrollytelling"](https://pudding.cool/process/how-to-implement-scrollytelling/) and interactive charts using D3. Reading through this piece, it really jumps out at you which companies employ particularly inscrutable privacy policies. Airbnb stands out at one of the denser ones (requiring nearly 40 minutes to read through) while also scoring high on complexity (which is based on factors like sentence length and vocabulary from a test developed by the education company Metametrics). On the other hand, the BBC sticks to a privacy policy that is far more readable than the others. After reading through this piece, I was left with a clear sense of which companies are aggressively trying to stake out in legal jargon expansive claims to collecting and selling your personal data, and which companies are more responsible stewards of personal data. The larger takeaway is a distrubing one. As Litman-Navarro puts it:

> a significant chunk of the data collection economy is based on consenting to complicated documents that many Americans can’t understand.