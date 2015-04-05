# Calculate-Pi-using-Monte-Carlo
approximate the value of a function using random sampling to define constraints on the value and then makes a sort of "best guess."

In computing, a Monte Carlo algorithm is a randomized algorithm whose running time is deterministic, but whose output may be incorrect with a certain (typically small) probability.

The related class of Las Vegas algorithms are also randomized, but in a different way: they take an amount of time that varies randomly, but always produce the correct answer. A Monte Carlo algorithm can be converted into a Las Vegas algorithm whenever there exists a procedure to verify that the output produced by the algorithm is indeed correct. If so, then the resulting Las Vegas algorithm is merely to repeatedly run the Monte Carlo algorithm until one of the runs produces an output that can be verified to be correct.

The name refers to the grand casino in the Principality of Monaco at Monte Carlo, which is well-known around the world as an icon of gambling.

#####One-sided vs two-sided error
Whereas the answer returned by a deterministic algorithm is always expected to be correct, this is not the case for Monte Carlo algorithms. For decision problems, these algorithms are generally classified as either false-biased or true-biased. A false-biased Monte Carlo algorithm is always correct when it returns false; a true-biased algorithm is always correct when it returns true. While this describes algorithms with one-sided errors, others might have no bias; these are said to have two-sided errors. The answer they provide (either true or false) will be incorrect, or correct, with some bounded probability.

For instance, the Solovay–Strassen primality test is used to determine whether a given number is a prime number. It always answers true for prime number inputs; for composite inputs, it answers false with probability at least ½ and true with probability at most ½. Thus, false answers from the algorithm are certain to be correct, whereas the true answers remain uncertain; this is said to be a ½-correct false-biased algorithm.

####Example: Calculating Pi
A simple Monte Carlo Simulation can be used to calculate the value for π. If you had a circle and a square where the length of a side of the square was the same as the diameter of the circle, the ratio of the area of the circle to the area of the square would be π/4.
So, if you put this circle inside the square and select many random points inside the square, the number of points inside the circle divided by the number of points inside the square and the circle would be approximately π/4.
Write a function to run a simulation like this, with a variable number of random points to select. 
Also, show the results of a few different sample sizes.
For software where the number π is not built-in, we give π to a couple of digits: 3.141592653589793238462643383280
