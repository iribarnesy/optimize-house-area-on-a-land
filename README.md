# Optimization problem : solved with DE or PSO algorithms

Author : Sylvain Iribarne <iribarnesy@eisti.eu>

Date : 12 Dec, 2020

## Problem : Maximize the area of a house on a land

A house is represented with a rectangle. A land is any polygon, convex or concave.

## Algorithms : Differential Evolution and Particle Swarm Optimization

The aim of this repository is to compare the two optimizers above. As you can see in the main notebook the DE algorithm is more robust and faster than PSO on this problem.
This difference is even greater since PSO is in vanilla implementation.

You can select different optimiation strategy by setting the hyperparameters in the builder. For example you can toggle the "ACCEPT_WHEN_INVALID_MOVE" parameter to dynamically set the bounding function.

## About the project

The aim of the project is to keep separate the logic between the problem and the optimization.
That's why you will see a Rectangle class and a builder for the optimizers.

**To solve your problem you just have to create *a minima* an evaluation function. You can also give a bounding and an initialization functions to the optimizer.**

The builder allow to manage dynamically the optimizers. It is necessary to define an optimizer into a class, with a "fit" function. Then, add a build function into the optimizer to put the creation logic.


## Notebooks
- [Main](https://github.com/iribarnesy/optim/blob/master/Main.ipynb) : The study about the performance of the optimizers
- [Rectangle](https://github.com/iribarnesy/optim/blob/master/Rectangle.ipynb) : Class and functions related to the problem definition
- [OptimizerBuilder](https://github.com/iribarnesy/optim/blob/master/OptimizerBuilder.ipynb) : Builder for the optimizers
- [PSO](https://github.com/iribarnesy/optim/blob/master/PSO.ipynb) : Class for the PSO optimizer
- [DE](https://github.com/iribarnesy/optim/blob/master/DE.ipynb) : Class for the DE optimizer

## Installation

All the code is contained into notebooks to make easier to get and read. Let me know if you want a requirements.txt file to download the necessary python packages.
