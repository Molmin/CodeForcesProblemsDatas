## Description

<div><p>For a square matrix of integers of size $n \times n$, let's define its <span class="tex-font-style-bf">beauty</span> as follows: for each pair of side-adjacent elements $x$ and $y$, write out the number $|x-y|$, and then find the number of different numbers among them.</p><p>For example, for the matrix $\begin{pmatrix} 1 &amp; 3\\ 4 &amp; 2 \end{pmatrix}$ the numbers we consider are $|1-3|=2$, $|1-4|=3$, $|3-2|=1$ and $|4-2|=2$; there are $3$ different numbers among them ($2$, $3$ and $1$), which means that its beauty is equal to $3$.</p><p>You are given an integer $n$. You have to find a matrix of size $n \times n$, where each integer from $1$ to $n^2$ occurs exactly once, such that its <span class="tex-font-style-bf">beauty</span> is the maximum possible among all such matrices.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 49$)&nbsp;– the number of test cases.</p><p>The first (and only) line of each test case contains a single integer $n$ ($2 \le n \le 50$).</p></div><div class="output-specification"><p>For each test case, print $n$ rows of $n$ integers&nbsp;— a matrix of integers of size $n \times n$, where each number from $1$ to $n^2$ occurs exactly once, such that its beauty is the maximum possible among all such matrices. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 49$)&nbsp;– the number of test cases.</p><p>The first (and only) line of each test case contains a single integer $n$ ($2 \le n \le 50$).</p>

## Output

<p>For each test case, print $n$ rows of $n$ integers&nbsp;— a matrix of integers of size $n \times n$, where each number from $1$ to $n^2$ occurs exactly once, such that its beauty is the maximum possible among all such matrices. If there are multiple answers, print any of them.</p>





```input1|2
2
2
3
```




```output1
1 3
4 2
1 3 4
9 2 7
5 8 6
```


