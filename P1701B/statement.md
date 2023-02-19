## Description

<div><p>Recall that a permutation of length $n$ is an array where each element from $1$ to $n$ occurs exactly once.</p><p>For a fixed positive integer $d$, let's define the cost of the permutation $p$ of length $n$ as the number of indices $i$ $(1 \le i &lt; n)$ such that $p_i \cdot d = p_{i + 1}$.</p><p>For example, if $d = 3$ and $p = [5, 2, 6, 7, 1, 3, 4]$, then the cost of such a permutation is $2$, because $p_2 \cdot 3 = p_3$ and $p_5 \cdot 3 = p_6$.</p><p>Your task is the following one: for a given value $n$, find the permutation of length $n$ and the value $d$ with maximum possible cost (over all ways to choose the permutation and $d$). If there are multiple answers, then print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The single line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the value $d$ in the first line, and $n$ integers in the second line&nbsp;— the permutation itself. If there are multiple answers, then print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The single line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the value $d$ in the first line, and $n$ integers in the second line&nbsp;— the permutation itself. If there are multiple answers, then print any of them.</p>





```input1|2
2
2
3
```




```output1
2
1 2
3
2 1 3
```


