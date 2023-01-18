## Description

<div><p>We are definitely not going to bother you with another generic story when Alice finds about an array or when Alice and Bob play some stupid game. This time you'll get a simple, plain text.</p><p>First, let us define several things. We define function $F$ on the array $A$ such that $F(i, 1) = A[i]$ and $F(i, m) = A[F(i, m - 1)]$ for $m &gt; 1$. In other words, value $F(i, m)$ represents composition $A[...A[i]]$ applied $m$ times.</p><p>You are given an array of length $N$ with non-negative integers. You are expected to give an answer on $Q$ queries. Each query consists of two numbers – $m$ and $y$. For each query determine how many $x$ exist such that $F(x,m) = y$.</p></div><div class="input-specification"><p>The first line contains one integer $N$ $(1 \leq N \leq 2 \cdot 10^5)$ – the size of the array $A$. The next line contains $N$ non-negative integers – the array $A$ itself $(1 \leq A_i \leq N)$. The next line contains one integer $Q$ $(1 \leq Q \leq 10^5)$ – the number of queries. Each of the next $Q$ lines contain two integers $m$ and $y$ $(1 \leq m \leq 10^{18}, 1\leq y \leq N)$.</p></div><div class="output-specification"><p>Output exactly $Q$ lines with a single integer in each that represent the solution. Output the solutions in the order the queries were asked in.</p></div>

## Input

<p>The first line contains one integer $N$ $(1 \leq N \leq 2 \cdot 10^5)$ – the size of the array $A$. The next line contains $N$ non-negative integers – the array $A$ itself $(1 \leq A_i \leq N)$. The next line contains one integer $Q$ $(1 \leq Q \leq 10^5)$ – the number of queries. Each of the next $Q$ lines contain two integers $m$ and $y$ $(1 \leq m \leq 10^{18}, 1\leq y \leq N)$.</p>

## Output

<p>Output exactly $Q$ lines with a single integer in each that represent the solution. Output the solutions in the order the queries were asked in.</p>





```input1
10
2 3 1 5 6 4 2 10 7 7
5
10 1
5 7
10 6
1 1
10 8
```




```output1
3
0
1
1
0
```



## Note

<p>For the first query we can notice that $F(3, 10) = 1,\ F(9, 10) = 1$ and $F(10, 10) = 1$.</p><p>For the second query no $x$ satisfies condition $F(x, 5) = 7$.</p><p>For the third query $F(5, 10) = 6$ holds.</p><p>For the fourth query $F(3, 1) = 1.$</p><p>For the fifth query no $x$ satisfies condition $F(x, 10) = 8$.</p>
