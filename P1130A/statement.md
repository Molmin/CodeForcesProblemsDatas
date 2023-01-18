## Description

<div><p>You are given an array of $n$ integers: $a_1, a_2, \ldots, a_n$. Your task is to find some <span class="tex-font-style-bf">non-zero integer</span> $d$ ($-10^3 \leq d \leq 10^3$) such that, after each number in the array is divided by $d$, the number of positive numbers that are presented in the array is greater than or equal to half of the array size (i.e., at least $\lceil\frac{n}{2}\rceil$). Note that those positive numbers do not need to be an integer (e.g., a $2.5$ counts as a positive number). If there are multiple values of $d$ that satisfy the condition, you may print any of them. In case that there is no such $d$, print a single integer $0$.</p><p>Recall that $\lceil x \rceil$ represents the smallest integer that is not less than $x$ and that zero ($0$) is neither positive nor negative.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the number of elements in the array.</p><p>The second line contains $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($-10^3 \le a_i \le 10^3$).</p></div><div class="output-specification"><p>Print one integer $d$ ($-10^3 \leq d \leq 10^3$ and $d \neq 0$) that satisfies the given condition. If there are multiple values of $d$ that satisfy the condition, you may print any of them. In case that there is no such $d$, print a single integer $0$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the number of elements in the array.</p><p>The second line contains $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($-10^3 \le a_i \le 10^3$).</p>

## Output

<p>Print one integer $d$ ($-10^3 \leq d \leq 10^3$ and $d \neq 0$) that satisfies the given condition. If there are multiple values of $d$ that satisfy the condition, you may print any of them. In case that there is no such $d$, print a single integer $0$.</p>





```input1
5
10 0 -7 2 6
```




```input2
7
0 0 1 -1 0 0 2

```




```output1
4
```




```output2
0
```



## Note

<p>In the first sample, $n = 5$, so we need at least $\lceil\frac{5}{2}\rceil = 3$ positive numbers after division. If $d = 4$, the array after division is $[2.5, 0, -1.75, 0.5, 1.5]$, in which there are $3$ positive numbers (namely: $2.5$, $0.5$, and $1.5$).</p><p>In the second sample, there is no valid $d$, so $0$ should be printed.</p>
