# Computational-Statistics
2 task to solve 

TASK 1 
Consider an investment linked to a living person which provides an income for as long as that person is alive. The investment is as follows:
Consider a population with say 100000 individuals of age between 30 and 49. We assume that they are equally spread in ages, 5000 of them in each age. Also consider the lifetable with the probabilities of death within a year provided in the attached pdf.
The investment is the following.  Some people from the population (we do not know how many), provide 1 Euro per year for the next 4 years at time point 0,1,2,3,4. At the time point 5 all those people that are still alive share the money gathered. The investment is as simple as that. The idea is that one believes that he is going to be alive till the end then he will take back more money, taking the money of those that died.
 
For example, say that 5 people participate. One of them dies at year 3 (between time 3 and 4) and one at year 4. So, in total the fund has collected 22 euros and those euros are shared by the three alive at the end people, each one taking 7.33 euros (while they have paid 5 euros).
 
Assume that all people participate from the same time points and for 5 years they cannot withdraw their money/participation unless they die.
 
Implement this investment and examine:
•	What is the expected amount that each age can win/loose? Do you suggest this investment to all people?
•	Is the number of persons that are going to invest crucial for the amounts gained at the end. Run different scenario (you choose) to give an answer.
•	The company that receives the money invests them with an interest rate which is an exponential distribution with mean 2 per year. For example, if the money at point 0 are 5 Euros since 5 people participated, then at the end of the year with a rate of 2% (the mean rate) the amount is 5.1 Euros. Here the 5 people (nobody has dies) contribute 5 more and at the end of the second year, since the interest for the second year was 1.5% (random n umber generated from an exponential) they are 10,2515 and so on. So at the end of the 5years period the amount is that paid by the investors  with the interest rate per year. How much does this alter your calculations?
 
Please write a detailed report to your boss about this investment. You need to be thorough having also probabilistic considerations, a simple average does not suffice to describe things. Provide two files, one with the detailed report and one with the R code to replicate your analysis.


TASK 2 
Computational Statistics
PROJECT 2
A researcher wants to work with a distribution with density function given by
f(x; θ) = θ
2
θ + 1
(1 + x) exp(−θx), x, θ > 0
You can find in file project2.txt 150 observation that he believes that come from this
distribution
1. Estimate parameter θ using Maximum Likelihood method. You shall describe all
steps in full detail and write your own code for this.
2. Estimate the standard error using parametric bootstrap. This implies that you need
to find a way to simulate from this distribution.
3. An alternative model for the data could be one with pdf
f(x) = π
θ
2
θ + 1
(1 + x) exp(−θx) + (1 − π)λ exp(−xλ), x, λ, θ > 0
Estimate parameters π, θ, λ using ML method and in particular an EM algorithm.
Give all the steps of the algorithm in full detail. Then implement this algorithm in
R
