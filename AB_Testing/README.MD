 # :iphone: :video_game: :joystick: Finding the best version for Mobile Game using A/B Testing

[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen)](https://www.python.org) 
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
[![](https://img.shields.io/badge/SciPy-654FF0?style=for-the-badge&logo=SciPy&logoColor=white)](https://www.scipy.org)
[![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org) 
[![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org) 
[![](https://img.shields.io/badge/conda-342B029.svg?&style=for-the-badge&logo=anaconda&logoColor=white)](https://www.anaconda.com)

## Introduction 
This is a DataCamp Case Study. Cookie Cats is a hugely popular mobile puzzle game developed by Tactile Entertainment. It's a classic "connect three"-style puzzle game where the player must connect tiles of the same color to clear the board and win the level. It also features singing cats. We're not kidding! Check out this short demo:



As players progress through the levels of the game, they will occasionally encounter gates that force them to wait a non-trivial amount of time or make an in-app purchase to progress. In addition to driving in-app purchases, these gates serve the important purpose of giving players an enforced break from playing the game, hopefully resulting in that the player's enjoyment of the game being increased and prolonged.



But where should the gates be placed? Initially the first gate was placed at level 30, but in this notebook we're going to analyze an AB-test where we moved the first gate in Cookie Cats from level 30 to level 40. In particular, we will look at the impact on player retention. But before we get to that, a key step before undertaking any analysis is understanding the data. 

## A/B testing using Bootstrapping Method

Bootstrapping method was use to create a sample of size 1000 having difference in mean of both the groups and then proportion of values greater than zero was calculated.
The results shows that 98% values favours gate30 for both one day and seven day retention.

## A/B testing using Permutation Test 

In a permutation test, the null hypothesis is the assumption that there is no difference between two groups being compared. The goal of a permutation test is to determine if the difference between the two groups is statistically significant or if it could have arisen by chance. To do this, the data is shuffled and the difference between the groups is calculated multiple times to create a null distribution of differences. The p-value is then calculated as the proportion of times that the difference between the permuted groups is greater than or equal to the original difference. If the p-value is less than a pre-determined significance level, such as 0.05, then the null hypothesis is rejected, and it is concluded that there is a significant difference between the two groups. If the p-value is greater than the significance level, then the null hypothesis is not rejected, and it is concluded that there is not enough evidence to say that 
there is a significant difference between the two groups.

* For one day retention, the results were statistically different which again favour gate 30. 
* For seven day retention, results were not statistically different. Hence, proportion test was implemented to cross check result and results were practical as well as statistically different. Also confidence interval was calculated. 

## Results
With reference to statistical test done, Gate should be placed at level 30. 
More details are available [here.](https://github.com/iqrabismii/Statistics-/blob/main/AB_Testing/ABtesting.ipynb) 
