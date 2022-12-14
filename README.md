I have used genetic algorithms in both MATLAB and Python for this optimization.

# Problem Description

## System

Using genetic algorithms, find K1:4 and C1:4 so that the cost function gets minimized.

<img src="https://github.com/sarajahedazad/Optimal-Design-of-a-Suspension-System/blob/main/Suspension_System.JPG" width=30%>

try out the following conditions for MATLAB:
* Default settings
* Change population type to "bit string"
* Change population size to 500
* Change fitness scaling
* Use tournament for selection
* Use twopoint crossover
* Change CrossoverFraction to 0.3
* Change MaxStallGenerations to 10
* Change  to 0.001


## Constraints

![\Large 5000N/m<=X_1,X_2<=20000N/m](https://latex.codecogs.com/svg.latex?\Large&space;5000N/m<=K_1,K_2<=20000N/m) 

![\Large 90000N/m<=X_1,X_2<=150000N/m](https://latex.codecogs.com/svg.latex?\Large&space;90000N/m<=K_3,K_4<=150000N/m) 

![\Large 5000N/m<=X_1,X_2<=20000N/m](https://latex.codecogs.com/svg.latex?\Large&space;500N.s/m<=C_1,C_2,C_3,C_4<=2000N.s/m) 



## Initial Conditions
![\Large x_1(0)=0.03](https://latex.codecogs.com/svg.latex?\Large&space;x_1(0)=0.03) 

![\Large x_2(0)=0](https://latex.codecogs.com/svg.latex?\Large&space;x_2(0)=0) 

![\Large x_3(0)=0](https://latex.codecogs.com/svg.latex?\Large&space;x_3(0)=0) 

## Cost Function

The following should be minimized in the first 2 seconds.

![\Large](https://latex.codecogs.com/svg.latex?\Large&space;RMS(\ddot{X_1})+5RMS(\dot{X_2})) 


# Solution

First, we need to drive matrices of this system. You can find my solution [here](https://github.com/sarajahedazad/Optimal-Design-of-a-Suspension-System/blob/main/Using%20Lagrange%20multipliers%20to%20solve%20the%20problem.pdf).


## MATLAB
The codes written for this section are provided in the 

## Python

The library used for this part is [geneticalgorithm](https://pypi.org/project/geneticalgorithm/).
