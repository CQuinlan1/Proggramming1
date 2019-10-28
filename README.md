# Programming1
This is my assignment for Programming in Data Analysis. I hope to discuss using Jupyter
 * the purpose of numpy.random 
 * explain the use of " Simple Random data" and "Permutations" functions,
 * decribe the uses of least 5 of the distribution function, 
 * and the use of seeds.
 
 
## Numpy
Numpy is a module for Python programming. Numpy allows you collect numericaldata and put them in arrays and do manipulations or calculations on this data. 
Under Numpy.random we have 5 branches. Simple random data, permutations, distribution and random generator.


#### Simple Random Data
*Simple Random Data* offers 10 different functions to choose from. We are offered a selection of possibilities for creating random values. We can set the parameters and include or exclude the highest limit and the data returned can be **integers, bytes or floating values**.
In specific functions the  returned random integers can be drawn from parameters low (inclusive) to high (exclusive).There is a  function  to find Random **integers** of type np.int between low and high, where both are inclusive.
Example to put in:

 We also find a range of functions like  Radom Sample, Random, Ranf  and Sample that return random **floats** in a half-open interval [0.0, 1.0). 


#### Permutations
The  Permutations function offers 2 methods : 
* Shuffle and 
* Permutation 
to modify the order of values.

example to do

#### Distribution Functions
Of the many distribution functions offered by Numpy. I will review the uses of the  following :
* Normal
* Randn
* Binomial
* Standard normal
* Multivariate normal

##### Normal Distribution
This works mainly relying on the mean and the standard deviation. This draws random samples from a normal Gaussian distribution. It takes its guide from the mean (“centre”) of the distribution. The function has its peak at the mean, and its “spread” increases with the standard deviation.
Normally distributed data is often referred to giving a ‘Bell Shape’ curve.
Everytime you run it, it will generate different values due to their randomness but  following the normal distribution.

We can  set the standard deviation to  different values, however unless specified it will return to the default of (Loc) 0 and (size) 1.


##### Randn
Shown as np.random.randn, this function is very similar to the normal distribution function above.It also produces random values from a normal distribution.However,it work as if the (Loc) mean is at 0 and (scale) standard deviation is always 1



##### Binonmial
Written as Numpy.random.binomial  This draws samples from a Binomial distribution. Samples are drawn from a binomial distribution with specified parameters, n trials and p probability of success where n an integer >= 0 and p is in the interval [0,1]. (n may be input as a float, but it is truncated to an integer in use)

Uses: If we think of the binomial distribution of an experiment repeated numerous times but with only 2 outcomes, success or failure. It can be applied to estimate the number of successes or failures in  an event where only 2 outcomes exist and each experiment is independent of each other.



##### Standard Normal


