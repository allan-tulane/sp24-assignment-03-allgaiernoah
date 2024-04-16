# CMPS 2200 Assignment 3
## Answers

**Name:**__Noah Allgaier_______________________


Place all written answers from `assignment-03.md` here for easier grading.

1a)When N is dollars, the highest denomination(2^k) that's <= N. The repeat this process over and over, each time subtracting the denomination from N until N is 0. 

1b)Choosing the highest possible denomination that is <= N will give us the best solution. This is because if you have a denomination where d > 2^k, then more coins will have been used compared to choosing 2^k. By using this greedy choice over and over, we make the optimal solution. This solution is contructed by soltuions of its subproblems, so the optimal substructure properties holds true. 

1c)The work is O(log N) and the span is O(1).

2a)The counterexample is N=6 and the denominations {1, 4}. 4 would be chosen first, using 2 coins. However, it would be best to use 3 coins of denomination 1. 

2b)This is true because if we consider all possible denominations at each step, we choose the one that minimizes the total number of coins used. 

2c)Using a bottom-up approach, the work is O(Nk) and the span is O(Nk) where k is the number of denominations.

