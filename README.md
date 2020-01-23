# DS6306_Case_Study_01

https://youtu.be/4s90tmhPOvw

SMU DS 6306 Doing Data Science Case Study 1 by Jules Stacy

Conclusions:
1.   How many breweries are present in each state?
DC	1
ND	1
SD	1
WV	1
AR	2
DE	2
MS	2
NV	2
AL	3
KS	3
NH	3
NJ	3
TN	3
HI	4
KY	4
NM	4
SC	4
UT	4
WY	4
IA	5
ID	5
LA	5
NE	5
RI	5
OK	6
AK	7
GA	7
MD	7
CT	8
ME	9
MO	9
MT	9
VT	10
AZ	11
MN	12
FL	15
OH	15
NY	16
VA	16
IL	18
NC	19
WI	20
IN	22
MA	23
WA	23
PA	25
TX	28
OR	29
MI	32
CA	39
CO	47



3.   Address the missing values in each column.
Dealing with missing (or NA) values:
Analyses dealing solely with ABV can include beers with missing IBU values and vice versa. 
Analyses dealing with both ABV and IBU will not include any beers that have NA values for either of these variables.

4.   Compute the median alcohol content and international bitterness unit for each state. Plot a bar chart to compare.
The median alcohol content tends to fall around 0.05 and IBU varies greatly from state to state. 
For a graph of values, please see case_study_01.html (Figures 2 and 3)

5.   Which state has the maximum alcoholic (ABV) beer? Which state has the most bitter (IBU) beer?
Colorado has the beer with the highest ABV at 0.128.
Oregon has the most bitter beer with an IBU of 138.

6.   Comment on the summary statistics and distribution of the ABV variable.
The mean ABV for the dataset is 0.05987305
The median ABV for the dataset is 0.056
The standard deviation among ABV for the dataset is 0.01352549
The variance among ABV for the dataset is 0.0001829388

The quartile ranges are:
Min.      1st Qu.   3rd Qu.     Max.
0.00100   0.05000   0.06800     0.12800 

Based on these values, we can expect 95% of beers to fall between 0.03282208 and 0.08692402 ABV.

The distribution is approximately normal with right skew, with the mean centered at 0.0599. 
There appear to be additional popular ABV targets at approximately 0.06, 0.08, and 0.095, as evidenced by the spikes in the distribution at those numbers.

7.   Is there an apparent relationship between the bitterness of the beer and its alcoholic content? Draw a scatter plot.  Make your best judgment of a relationship and EXPLAIN your answer.
Visually, it appears that the data are related. 
According to analytical software there is a best-fit line with an equation of y= 0.0003506x + 0.0450713 and a correlation coefficient of 0.6690977. 
This means that 67% of the data is explained by the fitted line, and therefore ABV and IBU are moderately related.

8.  Budweiser would also like to investigate the difference with respect to IBU and ABV between IPAs (India Pale Ales) and other types of Ale (any beer with “Ale” in its name other than IPA).  You decide to use KNN classification to investigate this relationship.  Provide statistical evidence one way or the other. You can of course assume your audience is comfortable with percentages … KNN is very easy to understand conceptually.
Visually there is a clear difference, with Ale tending to have a lower IBU and ABV than IPA's.
Hyperparameter K's were chosen as 19 for a train-and-test, and as 8 for a leave-one-out analysis.
Using train-and-test, the computer was able to correctly classify beers 82-83% of the time.
Using leave-one-out, the computer was able to correctly classifiy beers approx. 86% of the time.

9. Knock their socks off!  Find one other useful inference from the data that you feel Budweiser may be able to find value in.  You must convince them why it is important and back up your conviction with appropriate statistical evidence. 
An analysis of common words used in beer names was run. "Ale" was the top choice. Most beers were named for their type.
Words related to aged beer were popular. Years were popular.

An analysis of variance was run on ABV and IBU. It was found that Wisconsin had consistently low ABV and IBU beer.
There could be a market for stronger beers in Wisconsin, but likely not for more bitter beers.
