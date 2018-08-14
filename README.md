# GSoC 2018 
## Implement a 1D plug flow reactor model with surface chemistry
All the files of GSoC 2018 are included in this folder.
## The objectives of my project
1. Derive the governing differential equations and algebraic constraints (DAE) for the 1D plug flow reactor with surface chemistry
2. Implement the reactor model through python for isothermal model, adiabatic model and etc.
## My project progress
1. Derive the DAE system and the initial conditions, simplified them into each specific condition (e.g. isothermal/adiabatic reactor). The details are illustrated in [my report](https://github.com/yuj056/yuj056.github.io/blob/master/Week1/yuj056_github_io.pdf)
2. Find the proper solver to solve the DAE system. Here we tried nested CVODE+IDA, nested CVODE+CVODE and single IDA solver, after testing with the results from [Richard S. Larson et al. 1996, SAND96-8211](https://github.com/yuj056/yuj056.github.io/blob/master/_posts/Sandia.pdf), the single IDA solver yields the best agreement.
