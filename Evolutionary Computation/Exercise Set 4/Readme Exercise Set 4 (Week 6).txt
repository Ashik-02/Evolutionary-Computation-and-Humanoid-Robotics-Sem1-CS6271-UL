Instructions
Material covered by this lab sheet

Low level GE questions
Comparing GE with GP
 We will also do some pen-and-paper exercises to be help you understand GE fully. Each question should have its own file, and name them QuestionX.ipynb , where X is the question number, or QuestionX.png in the event of a question you need to scan.

1. Given the grammar below, show what the following individual (already converted to decimal) would map to. Please show the mapping process step by step. You can assume that there is no wrapping, so if you get to the end of the genome, you can stop and assume that is your answer:

27, 176, 22, 53, 77, 74, 177, 215, 200, 183, 229, 111, 77, 124, 66, 94, 91, 232, 44, 53, 114, 71, 234, 98, 72, 106, 71, 231, 97, 203, 32, 15

<e>::= (<o><e><e>)|(<u><e>)|<v>

<o>::=+|-|/|*

<u>::=Sin|Cos|Tan

<v>::=x|y

2. Create a notebook that compares the performance of GP and GE using different experimental setups on a 4-bit parity problem. Make sure that you use the same population size and function set, but vary parameters such as mutation and crossover so that you have at least two different experimental setups for each.