## Description

<div><p>Alan Turing is standing on a tape divided into cells that is infinite in both directions.</p><p>Cells are numbered with consecutive integers from left to right. Alan is initially standing in cell $0$. Every cell $x$ has cell $x - 1$ on the left and cell $x + 1$ on the right.</p><p>Each cell can either contain an integer or be empty. Initially all cells are empty.</p><p>Alan is given a permutation $a_1, a_2, \ldots, a_n$ of integers from $1$ to $n$ that was chosen <span class="tex-font-style-bf">uniformly at random</span> among all permutations of length $n$.</p><p>At time $1$, integer $a_1$ is written down into cell $0$ where Alan is located.</p><p>At each time $i$ from $2$ to $n$ inclusive, the following happens. First, Alan decides whether to stay in the same cell he's currently in, move to the neighboring cell on the left, or move to the neighboring cell on the right. After that, integer $a_i$ is written down into the cell where Alan is located. If that cell already contained some integer, the old integer is overwritten and irrelevant from that moment on.</p><p>Once $a_n$ is written down into some cell at time $n$, sequence $b$ of all integers contained in the cells from left to right is formed. Empty cells are ignored.</p><p>Turing's award is equal to the length of the longest increasing subsequence of sequence $b$.</p><p>Help Alan and determine the largest possible value of his award if he acts optimally.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>Each test case is given in two lines. The first line of each test case contains a single integer $n$ ($2 \le n \le 15\,000$)&nbsp;— the length of the permutation given to Alan.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of the permutation.</p><p>It is guaranteed that the permutation was chosen uniformly at random among all permutations of the corresponding length.</p><p>The sum of $n$ over all test cases does not exceed $15\,000$.</p></div><div class="output-specification"><p>For each test case output a single integer&nbsp;— the largest possible value of Turing's award.</p><p><span class="tex-font-style-bf">Hacks are not allowed for this problem.</span></p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>Each test case is given in two lines. The first line of each test case contains a single integer $n$ ($2 \le n \le 15\,000$)&nbsp;— the length of the permutation given to Alan.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of the permutation.</p><p>It is guaranteed that the permutation was chosen uniformly at random among all permutations of the corresponding length.</p><p>The sum of $n$ over all test cases does not exceed $15\,000$.</p>

## Output

<p>For each test case output a single integer&nbsp;— the largest possible value of Turing's award.</p><p><span class="tex-font-style-bf">Hacks are not allowed for this problem.</span></p>





```input1
4
2
1 2
4
4 1 2 3
7
3 6 5 7 4 1 2
7
5 2 3 7 6 1 4
```




```output1
2
3
4
4
```



## Note

<p><span class="tex-font-style-it">Longest increasing subsequence</span> of sequence $b$ is the longest increasing sequence that can be obtained from $b$ by deletion of several (possibly, zero or all) elements.</p><p>In the first test case, Alan can make a decision only at time $2$. If Alan stays in cell $0$, sequence $b$ will be equal to $[2]$. If Alan moves to the left, to cell $-1$, sequence $b$ will be equal to $[2, 1]$. If Alan moves to the right, to cell $1$, sequence $b$ will be equal to $[1, 2]$. Only in the last case the length of the longest increasing subsequence of $b$ is $2$, therefore, the answer is equal to $2$.</p><p>In the second test case, one of the optimal sequences of actions looks as follows: move to the left at times $2$ and $3$, and move to the right at time $4$. Then sequence $b$ will be equal to $[2, 3, 4]$, and the length of its longest increasing subsequence is $3$.</p><p>In the third test case, one of the best ways is to always move to the left. Then sequence $b$ will be equal to $[2, 1, 4, 7, 5, 6, 3]$, and the length of its longest increasing subsequence is $4$.</p><p>In the fourth test case, one of the best ways is to move to the right four times, then move to the left once, and stay in the same cell once. Sequence $b$ will be equal to $[5, 2, 3, 4, 6]$.</p>
