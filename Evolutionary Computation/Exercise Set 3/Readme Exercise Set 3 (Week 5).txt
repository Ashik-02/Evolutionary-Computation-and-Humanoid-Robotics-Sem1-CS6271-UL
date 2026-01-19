Instructions
Material covered by this lab sheet

Low level GP questions
Symbolic Regression
For this lab sheet you can modify the Symbolic Regression and Multiple Run code from the class notebooks. We will also do some pen-and-paper exercises to help you understand GP fully. Each question should have its own file, and name them QuestionX.ipynb, where X is the question number, or QuestionX.png in the event of a question you need to scan.

1. Construct GP trees for each of the following expressions and perform crossover between them. You may choose the crossover point yourself, but the subtree exchanged should contain at least three nodes:

(* (+ (* 3 5) (sqrt (+ 3 1))) (+ 3 4))

(- ( * (+ 6 7) (- 9 8)) (sqrt (* (* 9 7) (/ 8 4))))

2. Modify the code from the class notebooks to solve this problem. Do several runs, use your best individual so far to plot a graph with its outputs, and plot the expected curve (from the dataset) in the same graph.

Tip: Note that you will need to use a bigger function set. Here are some protected functions that you may find useful
 

# Protected functions
def protectedDiv(left, right):
    try:
        return left / right
    except ZeroDivisionError:
        return 1


def psin(n):
    try:
        return numpy.sin(n)
    except Exception:
        return numpy.nan

def pcos(n):
    try:
        return numpy.cos(n)
    except Exception:
        return numpy.nan

def pow2(n):
    return operator.pow(n, 2)
3. Create a notebook that compares the performance of GP using different function sets on a 3-bit parity problem. Compare at least three different function sets, showing their performance and the average size of the individuals created.

 