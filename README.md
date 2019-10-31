

# Programming 1
This is my assignment for Programming in Data Analysis due November 11th 2019. I hope to discuss the purpose of numpy.random and use a Jupyter package to explain the use of " Simple Random data" and the "Permutations" functions, at least 5 of the distribution functions looking at their use and lastly the purpose and use of seeds in generating  pseudo random numbers.



## Numpy
Numpy is a module for Python programming. Numpy allows you collect numericaldata and put them in arrays and do manipulations or calculations on this data. 
Under Numpy .random we have 5 branches to generate random values. Simple random data, Permutations, Distribution and Random generator.


#### Simple Random Data
*Simple Random Data* offers 10 different functions to choose from. We are offered a selection of possibilities for creating random values. We can set the parameters and include or exclude the highest limit and the data returned can be **integers, bytes or floating values**.
The returned random integers from low (inclusive) to high (exclusive).There is a  function  to find Random **integers** of type np.int between low and high, inclusive also.
Example to put in:

 We also find a range of functions like  Radom Sample, Random, Ranf  and Sample that return random **floats** in a half-open interval [0.0, 1.0). 


#### Permutations
The  Permutations function offers 2 methods of creating random values: 
* Shuffle and 
* Permutation 
to modify the order of values.

example to do

#### Distribution Functions
Of the many distribution functions offered by Numpy. I will review the uses of the  following :
* Normal
* Multivariate Normal
* Chisquare
* Binomial
* Standard normal


##### 1.Normal Distribution
This works mainly relying on the mean and the standard deviation. This draws random samples from a normal Gaussian distribution. It takes its guide from the mean (“centre”) of the distribution. The function has its peak at the mean, and its “spread” increases with the standard deviation.
Normally distributed data is often referred to giving a ‘Bell Shape’ curve.
Everytime you run it, it will generate different values due to their randomness but  following the normal distribution.

We can  set the mean, and standard deviation to a different values, however unless specified it will return to the default of (Loc) 0 and (size) 1.


##### 2.Multivariate Normal 
We  can generate random values from   a multivariate normal function which  works with the mean and *covariance* of a one to higher dimensional  normal distribution.The mean is taken as the centre and the covariance as the spread.The covariance itself is how 2 variables react with each other, where the change in 1 variable equals a change in another. Uses of this would be in portfolio management where risk needs to be minimized then negative covariance may be sought between 2 products.




##### 3.Chisquare
Sample values can be created with the numpy function chisquare  drawing samples from a chi-square distribution.

It  creates independent random variables, each with standard normal distributions (mean 0, variance 1), which  are  *squared and summed* , the resulting distribution is chi-square  . This distribution is often used in hypothesis testing and confidence intervals.It is a way to test if observed values fit into values expected, asuming the null hypothesis is true.



##### 4.Binomial
shown as Numpy.random.binomial  This draws samples from a Binomial distribution. Samples are drawn from a binomial distribution with specified parameters, n trials and p probability of success where n an integer >= 0 and p, the probability, is in the interval [0,1]. (n may be inputed as a float, but it is truncated to an integer in use)

Uses: If we think of the the Bernoulli experiments which is a case of the binomial distribution, it invloves  an experiment being repeated numerous times but with only 2 outcomes, *success or failure*. It can be applied to estimate the number of successes or failures in  an event where only 2 outcomes exist and each experiment is independent of each other.

##### 5.Standard Normal
This  also draws values from a normal distribution , where our loc (mean) is 0 and  scale (standard deviation) is at 1. The input can be  set  to an integer or integer tuple. The output could be a float or an nd array.




#### Use of seeds generating pseudorandom numbers 
In Numpy we have 4 functions under Random Generator, where seed is one of those functions.
To understand the effect of the function seed firstly its worth considering the function random without calling the function seed previously and realising how the function random will continuesly return  values  that are completely random,  different float values are output each time.

Example:

However if we introduce the seed function and then activate  the random function , random numbers are generated, however the same random numbers are generated each time with this seed.

Example:


So our random output is not completely random but *pseudo random*, as with this seed we are getting a set output each time .
So we are are using the seed as a pseudo random generator, as it by reseeding with this same value we are recreating the same sequence of values each time.
We often see that the seed used may be  a number representing date/time (avoiding repeats) in  the pseudo random number generator (PRNG) .
The uses of this can be found in cryptography and encryption algorithm, where codes and passwords cannot be guessed.


##### Conclusion
The selection available of functions  for creating random values is extremely wide. I suggest that certain areas repeatly use the  most relevant to their area of speciality, and while the assignment is very worthwhile, it will be interesting to see the preferred methods by different sectors in industry.


##### References:
https://docs.scipy.org/doc/numpy-1.14.0/reference/routines.random.html

https://rstudio-pubs-static.s3.amazonaws.com/274412_16e565d38d49483497c662ac8ef7f2ea.html

https://blog.quantinsti.com/python-numpy-tutorial-installation-arrays-random-sampling/

https://seaborn.pydata.org/tutorial/distributions.html
