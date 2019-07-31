---
title: "Where are the outliers?"
date: 2019-02-13T01:55:00-05:00
draft: false
author: "Ben"
---

If we glance at the race/education/Trump shift chart, it looks like there is a linear relationship in education except for (roughly) these red points:

{{<localplotly "simple-3d-scatter-colored.html" 800 800>}}

(Remember that you can rotate 3D plots by clicking and dragging.  I just eyeballed this slice, it was not scientific.  It should be close enough for the broad-strokes analysis we'll do though.)

We can filter out all of the gray points and think of them as explained by the education effect.  If we only plot these red points, where are they?

{{<localplotly "outlier_all.html" 800 500>}}

If we remove a bunch of states to zoom in on the midwest, we get this:

{{<localplotly "outlier_zoom.html" 800 500>}}

(Remember, you can toggle some of the buckets of data as invisible by clicking them in the legend.)

Some things to note:

* If you only show the counties with a shift of 15% or more, there are a ton in Ohio and Iowa, a few in Missouri and some elsewhere.
* There is basically a continuous blotch from the southern part of Illinois to the border with Canada
* Almost all of Iowa is in this "unexplained by education" set

Recall from our basic analysis, the figure below is how things changed across all counties.

![R Shift](/maps/republican_shift.png)

We are looking at many fewer counties in this new "outlier" group.  We already have a likely candidate (HS-educated people) to explain the change elsewhere, in all the places present in the chart below not present in the chart above.  Progress!


## Next Steps

But which voters drove change in those areas?  It can vary state-by-state, so let's dig in.  We'll compare county voting changes to attributes of those counties, and build a narrative around the overall dynamic there.

# [What happened in Ohio?]({{< ref "ohio" >}})


