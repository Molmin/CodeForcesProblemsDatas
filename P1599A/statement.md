## Description

<div><p>You are given an array $A$ of length $N$ weights of masses $A_1$, $A_2$...$A_N$. No two weights have the same mass. You can put every weight on one side of the balance (left or right). You don't have to put weights in order $A_1$,...,$A_N$. There is also a string $S$ consisting of characters "L" and "R", meaning that after putting the $i-th$ weight (not $A_i$, but $i-th$ weight of your choice) left or right side of the balance should be heavier. Find the order of putting the weights on the balance such that rules of string $S$ are satisfied. </p></div><div class="input-specification"><p>The first line contains one integer $N$ ($1 \leq N \leq 2*10^5$) - the length of the array $A$ The second line contains $N$ distinct integers: $A_1$, $A_2$,...,$A_N$ ($1 \leq A_i \leq 10^9$) - the weights given The third line contains string $S$ of length $N$ consisting only of letters "L" and "R" - string determining which side of the balance should be heavier after putting the $i-th$ weight of your choice</p></div><div class="output-specification"><p>The output contains $N$ lines. In every line, you should print one integer and one letter - integer representing the weight you are putting on the balance in that move and the letter representing the side of the balance where you are putting the weight. If there is no solution, print $-1$.</p></div>

## Input

<p>The first line contains one integer $N$ ($1 \leq N \leq 2*10^5$) - the length of the array $A$ The second line contains $N$ distinct integers: $A_1$, $A_2$,...,$A_N$ ($1 \leq A_i \leq 10^9$) - the weights given The third line contains string $S$ of length $N$ consisting only of letters "L" and "R" - string determining which side of the balance should be heavier after putting the $i-th$ weight of your choice</p>

## Output

<p>The output contains $N$ lines. In every line, you should print one integer and one letter - integer representing the weight you are putting on the balance in that move and the letter representing the side of the balance where you are putting the weight. If there is no solution, print $-1$.</p>





```input1
5
3 8 2 13 7
LLRLL
```




```output1
3 L
2 R
8 R
13 L
7 L
```



## Note

<p>Explanation for the test case:  </p><p>after the 1st weight: 3 L (left side is heavier)</p><p>after the 2nd weight: 2 R (left side is heavier)</p><p>after the 3rd weight: 8 R (right side is heavier)</p><p>after the 4th weight: 13 L (left side is heavier)</p><p>after the 5th weight: 7 L (left side is heavier)</p><p>So, the rules given by string $S$ are fulfilled and our order of putting the weights is correct.</p>
