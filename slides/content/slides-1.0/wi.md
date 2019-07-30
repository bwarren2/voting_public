---
title: "Wisconsin"
date: 2019-02-11T14:05:03-04:00
draft: False
---

Your first intuitions in Wisconsin might be to check what was happening in Ohio to see if things are the same.  On a couple of counts, they are.

### Education vs Shift, OH + WI

{{<localplotly "WI/wi_oh.html" 600 600>}}

There is a very strong relationship between non-college rate and Republican shift by county, in Wisconsin as in Ohio.  Taken together, these two series have an r-squared of 0.65 and a p value of 6.09 * 10^-38, which are very decisive "this is not random" metrics.

### Education vs Shift vs Whiteness, OH + WI

{{<localplotly "WI/compare_scatter.html" 600 600>}}

And this is the same stronger-than-nationally trend we saw in the Ohio case.

But mining doesn't appear to be a factor because Wisconsin mining employment is de minimis in a state of 5.8 million people.

### GOP Turnout Didn't Flip Wisconsin, Dem Turnout Did

{{<localplotly "WI/turnout_bars.html" 600 600>}}

So where did the Dem votes change?

### Change in Dem Votes, Percentage

{{<localplotly "WI/d_vote_gain_%_2012.html" 825 425>}}

Just like Ohio, Dem turnout plunged across the board from 2012.  The best Dem showing was a 6% gain in Ozaukee, with two other counties (Dane and Waukesha) being near zero and most places being a 20% drop or more.  Milwaukee is especially troubling, because Milwaukee alone holds about 16% of the voting-aged population.

### Change in Dem Votes, Total

{{<localplotly "WI/dem_votes_map.html" 825 425>}}

### Where is the manufacturing?

<img src="/WI/WI_manufacturing.png" width="600" height="600" />

(Via [Brookings](https://www.brookings.edu/interactives/interactive-locating-american-manufacturing/))

The two big shortfall areas for Dems in terms of voters were the Appleton/Oshkosh area, (that blotch in the middle of the state,) and Milwaukee in the southeast.  Manufacturing concentrates in population centers, so this is not super surprising, but combined with the noncollege rate vs shortfall in turnout the data may suggest that declining labor prospects influenced votes.

## What Kinds Of Counties Mattered?

<img src="/WI/WI_vote_changes.png" width="600" height="600" />

(Via [Wiscontext](https://www.wiscontext.org/how-and-where-trump-won-wisconsin-2016))

Dem support fell apart across the state, and Milwaukee was the biggest single-county contributor, but the next-largest tier of counties by population caused a larger vote loss by far.

<img src="/WI/wi_map_wiscontext.png" width="600" height="600" />

(Via [Wiscontext](https://www.wiscontext.org/how-and-where-trump-won-wisconsin-2016))

## What Happened There?

Interestingly, there was extensive 3rd party voting in the Other Metro counties, which made the biggest difference in Clinton's outcomes.  (Clinton needed to lose roughly 200K votes compared to the Obama 2012 total, and half of that came from the Other Metro category.)  There are several possible stories here, considering that Libertarian (and Republican governor) Gary Johnson took 100K of the 3rd party vote and Jill Stein took only 31K:

 1. Did 2012 Democrats pull the lever for the Libertarian in 2016?
 + Did those voters stay home while some Republicans protest-voted and new voters came in to replace the 2012 Republicans in voting for Trump?
 + Did Obama flip some moderate Republicans, who were not similarly inspired by Hillary and couldn't bring themselves to vote for Trump?

I don't have great data to substantiate which of these is which yet[^data-needed], but if #3 was true we would expect to see similar numbers of votes in the Obama elections and 2016 election, but with a big skew toward Democrats in the Obama elections.

Turns out this is what we see:

{{<localplotly "WI/multiyear.html" 825 425>}}

It looks like Wisconsin is functionally tied in non-Obama years, but that in 2008 Obama may have flipped moderate Republicans and had some residual enthusiasm in 2012.  This lends circumstantial credence to #3, an Obama flip-effect wearing off.

[^data-needed]: Methodologically, here is how you exclude #2: get the file of who voted in the 2012 and 2016 elections.  Compare the sets of people who voted in each election.  If there is no surge of new voters in 2016 comparable to the Dem loss + new 3rd party voting, then it wasn't one flow of voters out of the D column and a different flow of previously-new voters into the 3rd party column.  Instead, there had to be some individuals switching parties themselves.  This analysis may sound creepy to you[^creepy], but political campaigns are almost definitely already doing it.

[^creepy]: There are also much creepier things you can do, which we will get to in the piece on Florida.

***

## Low Enthusiasm

There is one highly plausible explanation for lower Dem enthusiasm in 2016 compared to 2012.  This is the map of candidate vists to Wisconsin in 2012.  Note the darker blue pins in Madison, Milwaukee, and Green Bay, which represent visits by Obama during the 2012 campaign.

### Candidate Visits to WI in 2012 (Dark Blue is Obama)

<img src="/WI/2012_visits.png" width="600" height="600" />

(Via [FairVote](https://www.fairvote.org/fairvote-maps-the-2012-presidential-campaign))

  This map, produced in 2013, also happens to show the visits by Hillary Clinton as the candidate in 2016, because there weren't any.

<img src="/WI/2016_visits.png" width="600" height="200" />

(Via [FairVote](https://docs.google.com/spreadsheets/d/14Lxw0vc4YBUwQ8cZouyewZvOGg6PyzS2mArWNe3iJcY/edit#gid=0))

If having the candidate visit your state energizes voters and increases turnout, (which is probably true given how much time candidates spend on those events,) having fewer campaign visits in 2016 probably hurt Dem turnout overall compared to 2012.  It has been rumored that the campaign consciously chose to not visit Wisconsin because they thought increased exposure of the candidate _decreased_ support, but that is again a "Dems losing the state, not Reps winning it" scenario.

***

## Voter Suppression

Sadly, there is one last big factor to consider in Wisconsin specifically: voter suppression.

<img src="/states/voting_restrictions.png" width="600" height="400" />

(Via [Brennan Center](https://www.brennancenter.org/new-voting-restrictions-america))

This map shows which states had new restrictions on voting, like voter-ID laws, in place since 2010.  Note that Wisconsin is included, with laws effective 2014, and there is reason to believe the Wisconsin laws were targeted at likely Democratic voters[^north-carolina-villainy]:

> A trial over Wisconsin's voting laws kicked off Monday with a former aide to a Republican state senator testifying that GOP senators were "giddy" over the prospect the state's 2011 voter ID law could keep some people from voting.

>...

> "She got up out of her chair and hit her fist or her finger on the table and said, 'Hey, we've got to think about what this would mean for the neighborhoods around Milwaukee and the college campuses,'" Allbaugh said.

(Via [Journal-Sentinel Online](http://archive.jsonline.com/news/statepolitics/challenge-to-wisconsin-voter-id-law-begins-in-federal-court-b99726100z1-379657961.html/))

Some of the restrictions were struck down[^rules-struck-down], but they still had an impact.

### How much voter suppression happened in Wisconsin?

Different sources give different estimates based on their own work.  Some [initial hysteria](https://www.snopes.com/fact-check/300000-wisconsin-voters-turned-away-due-to-voter-id-laws/) estimated 300K votes suppressed, while other sources claimed it was 200K:

<img src="/WI/200K.png" width="600" height="600" />

However, via [The Elections Research Center at University of Madison-Wisconsin](https://elections.wiscweb.wisc.edu/wp-content/uploads/sites/483/2018/02/Voter-ID-Study-Release.pdf):

> "16,801 people in the two counties deterred from voting, and could be as high as 23,252"

But we can construct a comparison to sanity-check.

### Was voter suppression a big factor?  Compare with Minnesota

Trump's margin was 22,748 votes, so the high value from that study would flip the state.  However, we can compare Wisconsin to its neighbor Minnesota, which had no new voting restrictions, and see a very similar decline in Dem votes (and surge in 3rd party votes):

### Wisconsin and Minnesota Year-To-Year Vote Changes

{{<localplotly "WI/WI_MN_turnout_bars.html" 600 600>}}

Observe the same story as Wisconsin: nearly identical 2012 and 2016 Republican votes, and a big drop-off in Democratic votes.  These states are neighbors, and demographically pretty similar; they probably experienced declining Democratic voting for similar reasons, and only one state had restrictions.  These restrictions probably did not produce the majority of the Democratic vote decline.

### Percent Change in Democratic Vote From 2012 to 2016

{{<localplotly "WI/both_distributions.html" 600 600>}}

The X axis here is % change in turnout.  The bars and lines show inferred distributions, the ticks are specific data points.

Observe that the D percent changes top out near zero, while the R percent changes have a couple decreased turnouts but generally positive turnout.  (The mostly-neutral turnout D turnout changes are in core-demographic areas like big cities.)

***

### Conclusions

 1. Wisconsin saw big declines in Dem votes with no meaningful change in GOP votes from 2012 to 2016.  It's not reasonable to attribute the flip of the state to Republican voters, because their vote total was not what changed.  It looks like whatever new votes Trump might have gained may have been counterbalanced by people voting 3rd party for Gary Johnson.
 + Where D votes declined in largish metro areas, there was a surge of 3rd party voting.  Those might be Republicans Obama won over leaving the party, or unenthusiastic Dems not showing up and conservatives voting 3rd party.
 + Clinton made no visits to Wisconsin, unlike Obama in 2012 (and every major candidate from 1972 on).  It is reasonable to assume this resulted in less activation of her base.
 + Voter suppression occurred in Wisconsin, but was likely smaller than several reports would have you believe.  Depending on the methodology and error bars, it is possible that voter suppression was what flipped the state, but 1) it is not a given that is true, 2) declining Democratic votes compared to 2012 are the much larger factor.
 + Democratic turnout declined in almost every location, with the best counties merely running in place.  Running a candidate who can maintain turnout in core areas without turning out Democrats in non-core areas costs votes.

***
<center>
# [A few more states, then the end]({{< ref "others" >}})
</center>
***

### Coda 1: More on Minnesota

{{<localplotly "MN/d_vote_gain_%_2012.html" 825 425>}}

Just like in Wisconsin and Ohio, Minnesota was a sea of red produced by declining Democratic votes in 2016 compared to 2012, with no major uptick to counterbalance the shift.

***

### Coda 2: More on voter suppression

There is no evidence that the kind of fraud voter-ID laws prevent is at all important, according to [several](https://www.washingtonpost.com/news/wonk/wp/2014/08/06/a-comprehensive-investigation-of-voter-impersonation-finds-31-credible-incidents-out-of-one-billion-ballots-cast/?utm_term=.31bc91481045) [studies](https://www.vox.com/policy-and-politics/2016/10/31/13478134/voter-fraud-id-2016-trump).  However, there _is_ evidence of a concerted effort to use voter-ID laws to disenfranchise voters that don't vote with Republicans.[^north-carolina-villainy]  For more reading, consider [here](https://www.brennancenter.org/publication/truth-about-voter-fraud).

<img src="/misc/disenfranchisement.png" width="600" height="200" />

(Via [Politico](https://www.politico.com/story/2012/06/pa-pol-voter-id-helps-gop-win-state-077811).)

Further, the fraud that voter ID laws would stop doesn't make much sense.  Why show up _in person_ where you can get caught just to cast a single vote, when you can instead [use other people's absentee ballots](https://www.cnn.com/2019/02/27/politics/north-carolina-political-fraud-indictment/index.html)?  Clearly you can get many more fraudulent votes per hour that way.  The trick is that this question doesn't have an answer; showing up in person without an ID is a dumb way to commit fraud, which is probably why there are so few cases of it.  (And of the 30 cases in 1 billion votes there are, many are relatives voting in the spirit of the correct voter.)

It is pure villainy to seek election by denying your opponents votes, and as far as my research shows:

1. Voter-ID laws are a generally-Republican practice.
1. There is no reasonable basis in evidence for using them to stop actual fraud.
1. There is very real evidence of using them to disenfranchise other Americans who don't agree with you.

Don't just judge an idea on how it sounds.  Inspect how it operates in the real world.

And maybe consider talking to the politicians that have supported these policies.  If they have evidence, learn about it, and if not explain why their policy is odious.  In Wisconsin,

 * [these are the politicians who introduced the voter-ID bill](https://docs.legis.wisconsin.gov/2011/proposals/ab7),
 * [this is the list of Wikipedia entries for those people](https://en.wikipedia.org/wiki/100th_Wisconsin_Legislature).

> "[Grothman](https://en.wikipedia.org/wiki/Glenn_Grothman) said, 'What I'm concerned about here is winning, and that's what really matters here. ... We better get this done quickly while we have the opportunity,'" Allbaugh said.

> "I've characterized it as giddy and that's part of what bothered me so much," Allbaugh testified.

> Allbaugh named two other senators — Leah Vukmir and Randy Hopper — as being gleeful over passing the bill.

(Via the [Milwaukee-Wisconsin Journal-Sentinel](http://archive.jsonline.com/news/statepolitics/challenge-to-wisconsin-voter-id-law-begins-in-federal-court-b99726100z1-379657961.html/).)


### Appendix 1

### Wisconsin Mining is Immaterial

<iframe src="https://fred.stlouisfed.org/graph/graph-landing.php?g=nNmN&width=670&height=475" scrolling="no" frameborder="0"style="overflow:hidden; width:670px; height:525px;" allowTransparency="true"></iframe>

### Wisconsin Manufacturing has shrunk like OH has

<iframe src="https://fred.stlouisfed.org/graph/graph-landing.php?g=nNmP&width=670&height=475" scrolling="no" frameborder="0"style="overflow:hidden; width:670px; height:525px;" allowTransparency="true"></iframe>


[^surgical]: Via [Washington Post](https://www.washingtonpost.com/news/wonk/wp/2016/07/29/the-smoking-gun-proving-north-carolina-republicans-tried-to-disenfranchise-black-voters/?utm_term=.0025c58efae6).

[^rules-struck-down]: Via [Journal-Sentinel](https://www.jsonline.com/story/news/politics/2016/07/30/judge-strikes-down-wisconsin-voter-id-early-voting-laws/87803408/)

[^north-carolina-villainy]: Laws specifically engineered to exclude certain voters are a very real thing, as demonstrated in a court ruling on North Carolina restrictions that "target African Americans with almost surgical precision"[^surgical].  The *public* reasoning behind some of the restrictions was that they would differentially exclude African Americans.  African Americans tend to vote Democratic by huge margins (close to 90-10), so Republicans proposing those laws were seeking an advantage by disenfranchising non-supporters.

