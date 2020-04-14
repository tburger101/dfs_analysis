# dfs_analysis
Analyzing DFS Results and Roster Construction from 2019

This project looks at real NFL tournament entries from Draftkings to try and determine how the top .25 percentile teams, 
which we will call winning lineups, are being constructed. Rather than trying to figure out which players will have the best games 
I will instead be focusing on the macro level of roster construction. We will explore this both with data analysis and a machine 
learning model which can be used to differentiation which entries are more likely to produce a winning tournament entry.

## Required Libraries
* sklearn
* numpy
* pandas
* matplotlib
* seaborn

## Data
The data being analyzed is located in data.zip folder.  
* flea_flicker_contest_history.csv- This file contains the raw data being analyzed.  It was created by combining data from 
Armchairanalysis.com and my own personal contest history from Draftkings.  Python scripts were run to output the final form
to be analyzed.
* data_description.csv- This files describes what each column represents

## Acknowledgements
https://www.armchairanalysis.com - Used to help create unique input data about the lineups
https://www.dezyre.com/recipes/plot-roc-curve-in-python - Used as basis for ROC Curve in jupyter notebook
https://machinelearningmastery.com/columntransformer-for-numerical-and-categorical-data - Used to create Column Transformer

## Summary of Findings
After reviewing the data there are couple of interesting points. It appears which QB you roster is the cornerstone of lineup
construction.  Rostering lower owned QBs and QBs in higher total games appear to be optimal.  Also, game stacking your QBs
with a 2 WRs from the same team and 1 Opp WRs is the far and away the optimal stack type.

A blog describing the findings also appears here: 
