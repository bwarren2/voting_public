---
title: "Ohio"
date: 2019-02-12T01:54:00-05:00
draft: false
---

The outliers of Ohio are mostly concentrated in the east and southeast parts of the state.

### Change in Republican Presidential vote percentage points, 2016-2012

{{<localplotly "OH/shift_map.html" 920 500>}}

(You can mouseover counties to get more information.)

What is notable about that part of the state?  That is where the coal seams are, and where coal mining has historically happened.

### That outlier area ~= coal country

<img src="/OH/ohiocoal_map.png" width="600" height="600" />

An initial guess might be that coal miners had exceptionally negative views of Hillary Clinton, and/or positive views of Donald Trump.  Why might that be?

### Miners might have especially disliked Clinton



<img src="/hillary1.gif" width="600" height="600" />

> "We are going to put a lot of coal miners and coal companies out of business.  Right Tim?" - Hillary Clinton

This clip makes a "miners dislike Clinton" intuition a little more substantial, trending toward plausible.  I think the attack ad you make out of this clip if you run the Trump campaign in Ohio is pretty obvious.

### Even non-mining counties can be heavily invested in coal prospering

But even if a county doesn't _produce_ coal, it might be invested in coal.  What is something you can build near coal mines to make money?  Coal-fired power plants.  For example, in Gallia (at the southern tip of that map):

> Two of Gallia County's largest employers are the Lightstone Generation Power Plant and OVEC Kyger Creek Power Plant.  The Lightstone Generation, Gavin Plant is a 2.6 Gigawatt coal-fired power station in Cheshire, OH.  It is the largest coal fired power facility in Ohio, and one of the largest in the nation.[^galliaplants]

(Via [here.](http://www.growgallia.com/Key-Industries.aspx) Footnote mine.)

[^galliaplants]: Kyger is also a coal plant.  For the record, those plants are _enormous_.  Almost all _nuclear_ power plants in the US are 2.4GW.  The standard huge wind turbine you may have seen is generally 1-2 MW, or .0015GW.

### The outlier area is rife with coal plants (and retirements)

In fact, coal plants or retirements afflict much of the area with a big percentage shift toward Trump.

<img src="/OH/retirements.png" width="600" height="400" />

(Via [Brookings.](https://www.brookings.edu/blog/the-avenue/2016/12/19/coal-plant-retirements-will-continue-despite-trumps-epa-pick/))

Whether your county's coal plant is retiring or not, a hostility toward coal represents a threat to a source of lucrative jobs in your community.  There is another piece, though: insofar as Clinton was favorable to Obama policies, the Obama administration's Mercury and Air Toxics Standards rule (which increased regulatory burden on coal plants) can also be read as hostile or deleterious to those sources of jobs.  In fact, in anecdotal interviews with miners, that was exactly what came up.

> "The 2012 requirements prompted a wave of closures of coal-fired power plants. Coal miners have pushed the Trump administration to reverse the standards, arguing that they discouraged power companies from burning the fossil fuel to generate electricity, causing sales to suffer."

(Via [Bloomberg](https://www.bloomberg.com/news/articles/2018-12-28/mercury-limits-on-coal-plants-no-longer-appropriate-epa-says))

Note also how Trump is attempting to make good on his promises to help miners.

***


### Heavy industry lives around Cleveland

In addition to digging coal out of the ground and burning it immediately for power, what else might you do with it?  Sell it and ship it elsewhere.  That would probably be easiest if you carted the coal north, to Cleveland and the Great Lakes, which is historically exactly what happened.  And if you have a confluence of shipping and energy, you might build a bunch of manufacturing there, like energy-intensive steel foundries.

<img src="/OH/iron_and_steel.jpg" width="600" height="400" />

(Via [EPA.](https://archive.epa.gov/sectors/web/html/map-6.html))

Not only is northeast Ohio the home of steel production, it is the main base of Ohio manufacturing generally.

<img src="/OH/ohio_manufacturing_map.png" width="600" height="600" />

(Via [the Ohio Manufacturing Association.](http://www.ohiomfg.com/OMA_Manufacturing_Counts_2018-19.pdf))

### Cleveland yielded the most new-net-votes for Trump

{{<localplotly "OH/net_r_votes_map.html" 600 600>}}

These are net votes, ie (GOP2016 - Dem2016) - (GOP2012 - Dem2012).  But these votes could come from two sources: new Republican voters, or Dems staying home.  For example, if the parties were tied at 100K in 2012 and in 2016 5 dem voters stayed home, the math would be (100K - (100K - 5)) - (100K -100K) = (100K - 100K + 5) - 0 = 5.  If 5 new GOP voters showed up, it would be instead be ((100K + 5) - 100K) - (100K -100K) = 5.  So which is it: new Republican votes or missing Dem votes?


### 2016 GOP votes - 2012 GOP votes

{{<localplotly "OH/rep_votes_map.html" 720 420>}}

Republicans had one county in the Cleveland area where they earned 11K votes, and 5 in the 5Kish vote range.

### 2016 Dem votes - 2012 Dem votes

{{<localplotly "OH/dem_votes_map.html" 720 420>}}

Democrats had *7* counties in the area where they lost huge numbers of votes.  All of those counties are bigger losses than the biggest county was a gain for Republicans (except one that is about 1,000 votes shy), and the biggest vote loss is Cuyahoga at ~37K votes.  That is close to the _total_ vote gain for those Republican counties _combined_.

### GOP Turnout change, 2016 GOP votes / 2012 GOP votes

{{<localplotly "OH/r_vote_gain_%25_2012.html" 720 420>}}

Republicans saw a consistent, large voter turnout increase throughout eastern Ohio, with many counties in excess of a 25% increase.  Mathematically, it's like 2012 GOP voters made groups of four people, and each group got someone who did not vote R in 2012 to vote Trump.  In Gallia county, (the county with the two large coal plants as their biggest employers,) the GOP vote increased *66%*.  R voters made groups of three and each group found _2_ people to vote Trump.  This is an effect.

### Dem Turnout change, 2016 Dem votes / 2012 Dem votes

{{<localplotly "OH/d_vote_gain_%25_2012.html" 720 420>}}

Democrats, by contrast, saw turnout shrink by at least a quarter in huge swaths of the state, especially in the coal belt where R turnout was so much higher.  We don't know individual votes to say if Dem voters switched or if many Dems stayed home and Republicans found previous non-voters to vote for Trump, but circumstantial evidence implies some vote-switching may have happened.  These are counties that had voted significantly for Obama, but swung hard for Trump.

### Multiyear Context

{{<localplotly "OH/grouping.html" 600 600>}}

In the aggregate, Republican voting was slightly up, but Democratic voting cratered in 2016 compared to 2012.  So many Democratic voters failed to turn out that Trump only had to do as well as Romney to win. He did better than Romney.  Circumstantially, it is plausible that Trump flipped Obama voters in coal country.  Overall, Clinton lost the state more than Trump won it because of her diminished vote counts in the Cleveland region (which dwarfed GOP gains there).

### Ohio Support Change vs Education and Whiteness, with Support Change from <80% White Counties in the US

{{<localplotly "OH/compare_scatter.html" 600 600>}}

Toggle these series ^ to see the datasets independently.  Red dots are coal counties, orange are coal-adjascent, other are neither.

Some things to note:

#### Almost all of the high-shift points are coal counties or coal-adjacent

Three of the four that aren't, Ashtabula, Adams, and Brown, as still in the swath of Ohio riddled with coal power plants.  Paulding is the first county decisively away from that phenomenon.

#### There is a strong HS-education-only relationship with the Trump shift

If you unselect "OH counties", showing only "<80% White US Counties", you will see a very strong relationship between change in Republican support % and % of county with only a HS degree.  If you reselect "OH counties", you will see that the rest of the original data also showed an education sensitivity.  The two datasets are showing the same thing (an education relationship) with different degrees of severity.  _Maybe the drumstick plot, which looked like a poorer relationship, is actually a collection of stronger relationships with varying sensitivity to education_.

#### Something is weird about Holmes county

As a fun note: why is Holmes county a huge outlier in this chart?  Honestly, my process involves a fair amount of seeing an outlier and looking at in on Wikipedia.  From the article for that county:

> The Amish community in Holmes County established in 1808, had a 17,654 adherents in 2010,[22] or 41.7% of the county's population.

(Via [Wikipedia](https://en.wikipedia.org/wiki/Holmes_County,_Ohio#Amish_community))

In other words, it looks like religious culture, whether is Mormon or Amish, still matters.

***

## [Let's look at another major state from our outlier map: Wisconsin.]({{< ref "wi" >}})

***

### Coda: the end of Clinton's statement

The next 25 seconds of Clinton's statement read very differently than the first 8.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <iframe src="https://www.youtube.com/embed/ksIXqxpQNt0?start=17&end=42" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border:0;" allowfullscreen title="Out of Business"></iframe>
</div>

> And we are going to make it clear that we don't want to forget those people.  Those people labored in those mines for generations, losing their health, often losing their lives to turn on our lights and power our factories.  Now we've got to move away from coal and all the other fossil fuels but I don't want to move away from the people who did the best they could to produce the energy that we relied on. - Hillary Clinton

For a broader take on Hillary's media problems, consider [this](https://www.vox.com/energy-and-environment/2017/9/15/16306158/hillary-clinton-hall-of-mirrors).  I won't claim it is definitive, but it is interesting.

<!-- https://www.bls.gov/eag/eag.oh.htm -->
<!-- https://www.brookings.edu/blog/the-avenue/2017/01/25/automation-guarantees-a-bleak-outlook-for-trumps-promises-to-coal-miners/ -->

<!-- https://fred.stlouisfed.org/series/MANEMP -->
<!-- https://www.google.com/imgres?imgurl=https%3A%2F%2Ffred.stlouisfed.org%2Fgraph%2Ffredgraph.png%3Fwidth%3D880%26height%3D440%26id%3DOHMFGN&imgrefurl=https%3A%2F%2Ffred.stlouisfed.org%2Fseries%2FOHMFGN&docid=IIILQo0Z5stBEM&tbnid=r3ST6gTOatRThM%3A&vet=10ahUKEwiYy9zhr_nhAhVPheAKHQZ2CvkQMwhDKAMwAw..i&w=880&h=460&bih=725&biw=1440&q=fred%20ohio%20manufacturing%20jobs%201980&ved=0ahUKEwiYy9zhr_nhAhVPheAKHQZ2CvkQMwhDKAMwAw&iact=mrc&uact=8 -->
