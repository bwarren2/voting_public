---
title: "Education vs Race vs Republican Shift"
date: 2019-02-13T01:56:00-05:00
draft: false
author: "Ben"
---

# Education

{{<localplotly "education_vs_shift.html" 600 600>}}

(These charts are interactive.  Mouseover to get values of nearby points, or click the legend to show/hide series.)

We can start to investigate the drivers of 2012->2016 Republican voting shift by examining the characteristics of each county.  Here we see what fraction of a county has a high school degree or less vs the 2016 shift toward Trump.

We can see [on the map]({{< ref "basic_maps" >}}) that the low outliers are Utah and Idaho.  This makes sense; McMullin was a spoiler candidate for Republicans in those states and especially popular among Mormons, who disliked Trump.

{{<localplotly "education_vs_shift_wo_id_ut.html" 600 600>}}

When we remove Idaho and Utah, the relationship becomes a bit clearer, but is still a drumstick instead of the line that would indicate a clean relationship.  What if we consider the oft-cited influence of race in the election?

# Racial Composition

{{<localplotly "race_vs_shift_wo_id_ut.html" 600 600>}}


# Comparing Three Variables At Once

{{<localplotly "race_vs_ed_vs_shift.html" 750 700>}}

Here, color is average income in that county.  Red is more, gray is less.  This is interactive; click and drag to rotate, mouseover for detail.

## Methods


This is a plotly 3D scatterplot of the two previous variables and the calculated Republican shift.  Putting them on the same plot at the same time makes it possible to easily see how the two variables are interacting.  Interestingly, color here is per-capita income.  Trump fared poorly in the higher-income counties.

## Results

Some observations immediately jump off of the page:

### A plane describes most of the points outside of the high-white, high-high-school-only area

If you had to draw a flat surface to approximate most of the plot, it would have a positive slope in the education dimension (more high-school-only-educated people means more Republican shift) and very little slope in the % white dimension (having fewer minority people doesn't change things much).

### Something weird is happening in the high-white, high-high-school-only area

Especially in the 93%+ white area, there are many points above the plane formed by the rest of the plot.  What exactly that area _is_ is in the next few slides.

### Education explains noise in the race chart

 * The "noise" we saw when looking at "% of county that is white" vs shift below 93%ish white is actually explained in the education dimension.  If you pick a region below that threshold, like the 40-60% range, you can see that as "% of county that is only high-school educated" increases, we get more shift, and that shows up as merely a cloud of points when you only look at % white vs shift

So where are the

# [places in that anomalous area?]({{< ref "colored-outliers" >}})
