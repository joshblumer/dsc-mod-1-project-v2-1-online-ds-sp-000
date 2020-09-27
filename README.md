# Module 1 Final Project

Film Industry Data Analysis

## Introduction

   * An exploratory data analysis of the film industry through databases provided by The Flatiron School and found at [kaggle.com](https://www.kaggle.com). My goal in this analysis is to extract meaningful insights from the data and manipulate them into actionable recommendations using statistical methods and visualizations.

## Technologies
* The Jupyter Notebook "student.ipynb" found in this repo was created using Python 3.7.6


### Necessary libraries to reproduce and run this project are:

 * Pandas
 * NumPy
 * MatPlotLib
 * Seaborn

## Methodology

After exploring and analyzing the given data sets I chose to focus on an approach that measured films box office success by calculating film profit (subtracting film budget from film gross) and film profit quotient (dividing film budget from film gross). Once I obtained film profit and profit quotient I compared them to several other variables such as genre, rating, and release month that a studio chooses when producing a film. My hypothesis is that by filtering variables through profit correlation a studio will maximize the return on investment of its films.

## Table of Contents

* [Evaluating Gross and Profit Against Budget](#budget)
* [Gross and Profit by Release Month](#month)
* [Profit and Profit Quotient by Rating, Genre, and Runtime](#rgr)
* [Studios by Gross](#studio)

<a name="budget"></a>
### Evaluating Gross and Profit Against Budget

![wholeset](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Whole%20Set.png)
![top500p](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Top500P.png)
![top500pq](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Top500PQ.png)

#### The primary benchmark of this analysis is comparing multiple variables to the levels of correlation between a film budget and its gross, profit, and profit quotient. There is a moderately strong correlation (0.75) between the entire data sets budget and gross meaning that if a studio has the capital to invest into a particular film the gross will usually increase as the budget increases. The entire data sets profit has a slightly weaker correlation (0.61) with the budget, but it is still positive so generally as a studio invests more they will also profit more. A surprising insight extrapolated from the data is that the top 500 highest grossing films in the set had weaker correlations between budget/gross (0.67) and budget/profit (0.51). This means that even though these films were the highest grossing, they had a weaker return on investment than the set as a whole. As expected the top 500 films by profit quotient had a very strong correlation with budget/gross (0.92) and budget/profit (0.91) meaning that as these films budgets increase their gross and profit increases in nearly direct proportion. After filtering these films with a high profit quotient their variables can be further analyzed for trends that a studio can follow to maximize their ROI.

<a name="month"></a>
### Gross and Profit by Release Month
![month1](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Month1.png)
![month2](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Month2.png)

#### The entire data set and Top 500 films gross and profit the most in the summer months of May, June, and July, and then again over the holiday season in November and December. Profit quotient is more evenly distributed by month than gross or profit among the entire data set implying that the increases in profit are closely proportionate to an increase in budget. Profit quotient for the Top 500 films resembles the entire set with the exceptions of a sharp increase in August and a decrease in June, July, November, and December, which implies again that the large increases in profit during those months is correlated to an increased budget as well.

<a name="rgr"></a>
### Profit and Profit Quotient by Rating, Genre, and Runtime 
![rating](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Rating.png)

#### Profit is nearly equally distributed among ratings but R rated films have an average 25% higher profit quotient.

![genre](https://github.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/blob/master/Images/Genre.png)

#### Drama, adventure, and horror share the top profits among genres. Horror has a very strong lead in profit quotients.

![runtime](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Runtime.png)

#### There is no correlation between profit or profit quotient and movie runtimes.

<a name="studio"></a>
### Studios by Gross
![studio](https://raw.githubusercontent.com/joshblumer/dsc-mod-1-project-v2-1-online-ds-sp-000/master/Images/Studio.png)

#### Buena Vista, a subsidiary of Disney, total grosses more than double the next entry, Warner Brothers, but only grosses slightly more than the next few entries per film. Finding the top performing studios is a valuable insight for choosing who to collaborate with, where to look when acquiring talent, and whose films to further analyze.

## Conclusion

My aggregate finding and recommendation after filtering and comparing several variables through top performing films gross, profit, and profit quotient is that films in the drama, adventure, and  especially horror genres that are rated R and released towards the end of the summer will sustain a profit quotient 25%+ higher than films of other genres and ratings released at other times throughout the calendar year. This translates to a much higher return on investment which will position the production company to use their increased profits to fund the production of additional films. 



