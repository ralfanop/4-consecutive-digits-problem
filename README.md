# 4-consecutive-digits-problem

Author: Professor Malcolm Farrow, The University of Newcastle, Newcastle, England, United Kingdom

The following model assumes that all decimal digits are independently and identically distributed with a uniform distribution over the values {0,1,⋯,9}. That is, we will observe an ordered sequence ▁S_ =(D_1,D_2,⋯,D_J) of digits and, for d=0,1,⋯,9 and j=1,2,⋯,J, we have Pr⁡(D_j=d)=0.1.  Furthermore, D_j is independent of D_h unless h=j. Now, suppose that we will observe two such sequences, denoted ▁S_1 and ▁S_2, and that these are independently and identically distributed. Now, choose some positive integer, k≤J (for example, k=4). 

The problem is to find the probability, denoted P(J,k) , that there is at least one ordered sequence of k digits, |t=(t_1,t_2,⋯,t_k) which occurs at least once in each of |S_1 and |S_2.

We have not found a closed-form expression for this probability, or, so far, a practicable deterministic method for computing it. However, we can approximate P(J,k)  by Monte Carlo sampling and we have done such computations using code written in R [1]. 

Let the observed proportion of samples giving a match out of r trials be P ̂_r (J,k). The standard error, denoted s, of P ̂_r (J,k), as an estimator of P(J,k), is approximated using: 

s=r^(-1) 〖[P ̂_r (J,k)(1-P ̂_r (J,k))]〗^(1/2)

[1]  R Core Team 2022 R: A language and environment for statistical computing (Vienna: R Foundation for Statistical Computing) https://www.r-project.org/
R software version adopted:  3.6.3.nn.pkg

Monte Carlo test seed:       89   [matches3R.txt](https://github.com/ralfanop/4-consecutive-digits-problem/files/11359338/matches3R.txt)

Below, data sets of several Monte Carlo tests. From 10 000 000 up to 5 000 000 000 tests:

[R Console(8,4,ss=TRUE,seed=89,4000000000).txt.zip](https://github.com/ralfanop/4-consecutive-digits-problem/files/11359358/R.Console.8.4.ss.TRUE.seed.89.4000000000.txt.zip)
[R Console(8,4,ss=TRUE,seed=89,100000000).txt](https://github.com/ralfanop/4-consecutive-digits-problem/files/11359359/R.Console.8.4.ss.TRUE.seed.89.100000000.txt)
[R Console(8,4,ss=TRUE,seed=89,3000000000).txt](https://github.com/ralfanop/4-consecutive-digits-problem/files/11359360/R.Console.8.4.ss.TRUE.seed.89.3000000000.txt)
[R Console(8,4,ss=TRUE,seed=89,50000000).txt](https://github.com/ralfanop/4-consecutive-digits-problem/files/11359362/R.Console.8.4.ss.TRUE.seed.89.50000000.txt)
[R Console(8,4,ss=TRUE,seed=89,10000000).txt](https://github.com/ralfanop/4-consecutive-digits-problem/files/11359363/R.Console.8.4.ss.TRUE.seed.89.10000000.txt)
