Instructions
Material covered by this lab sheet

Running experiments with DEAP
For each question, create a notebook called QuestionXX.ipynb, where XX is the question number. When you are asked a question, put the answer in the comments at the top of the notebook. Your notebooks must have all the code as well as the execution results to prove the answers you gave.

You should modify the GA OneMax notebook from the module repository for this lab sheet.

1. Using roulette wheel selection, what is the smallest population size and number of generations to find a perfect solution with an individual size of 50?  Give your answer regarding individuals processed: the population size multiplied by the number of generations required.

2. Redo Question 1 using tournament selection and answer the same question but for an individual size of 100.

3. Create your own fitness function that works similarly to OneMax, except that the maximum fitness is when 50% of the individual's genes are 1, with a linear decay on either side. That is, calculate the sum of an individual like OneMax does, let's call it i, and then use the following pseudocode:

if (i) <= Individual_Length/2 return (i)

else return Individual_Length-i;

Using tournament selection, what is the smallest number of individuals you need to process to solve this? Why is this problem so much easier than OneMax?

Tips: GA is a stochastic method, so when asked for the smallest number of individuals processed, do not try to find it out deterministically, because there is not a single answer. Instead, try different setups, changing the parameters individually, and notice how the results change. Give your answer with the best result you found, but also explain other setups you have tried.