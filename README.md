# 2016 Voting Analysis

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/bwarren2/voting_public/master)

Lots of people have lots of feels about the 2016 US Presidential election, but most of the graphics I have seen are lacking.  This is my attempt to do better.



## The notebooks

Load data with the `Data.ipynb` notebook before using the other notebooks.

`viz.ipynb` is the major notebook for complex scatterplots.

`Outliers.ipynb` is for the colored outliers plots.

`Cross State Analysis.ipynb` is what it sounds like.

`Basic Analysis.ipynb` is for the basic state maps.


## Running them

Install reqs with

`pip install requirements.txt`

Change the name of `Pipfile1` to `Pipfile` and use `pipenv run jupyter notebook`.  (This is a hack to get around netlify's incorrect default settings interpretation.)
