Instructions
Material covered by this lab sheet

Writing a fitness function
Solving a problem with a GA
For this exercise you will write your own fitness function and attempt to solve a problem using DEAP. The problem you will tackle is the 0-1 Knapsack Problem, as described on p39 of the course book. 

Simply put, in this problem we have a set of objects, each of which has an associated weight and value, along with a knapsack that can hold a certain amount of weight. Your task is to select the objects with the highest total value that isn't too heavy for the knapsack.

The following code creates 100 items with values ranging from 1 to 10 and weights ranging from 1 to 100. Make sure you include this with no changes so that you have the correctly specified problem.

 

NBR_ITEMS = 100
MAX_WEIGHT = 1000

# set the random seed. Make sure you do this BEFORE creating the knapsack
# creating the knapsack
RANDOM_SEED = 42
random.seed(RANDOM_SEED)

# Create the item dictionary: item name is an integer, and value is
# a (value, weight) 2-uple.

items = {}

# Create random items and store them in the items' dictionary.
for i in range(NBR_ITEMS):
     items[i] = (random.randint(1, 10), random.randint(1, 100)) 
Your tasks are as follows:

Write a GA to maximise the value without going over the weight limit, using a population of 500. You can vary any other parameters that you like;
Identify the best individual and fitness you can find (we've managed 281 so far). Also, identify the total weight of the objects for the best individual;
Plot a graph of mean best and mean average performance for at least two experimental set ups.
What to hand up:

Your code (it is okay to modify the OneMax code from last week)
Your two graphs and the best individual found (it is okay to have these embedded in the same notebook)
Organise everything in a notebook called Week04Lab.ipynb.
Warning!

This is not a trivial problem. You may have to employ a penalty function as described on P141 of the Course Book. This basically would penalise any individuals that violate the weight constraint. The interesting part of this assignment is constructing your fitness function. Feel free to talk to the teaching team if your individuals are failing to evolve.

Caution!

A quick Google search will reveal sample code to solve a similar problem, but most of that code uses multi objective fitness, which we will be covering in Week 4. You should be able to solve this problem without using a multiobjective fitness function.