## Description

<div><p>You are given one integer $n$ ($n &gt; 1$).</p><p>Recall that a permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2, 3, 1, 5, 4]$ is a permutation of length $5$, but $[1, 2, 2]$ is not a permutation ($2$ appears twice in the array) and $[1, 3, 4]$ is also not a permutation ($n = 3$ but there is $4$ in the array).</p><p>Your task is to find a permutation $p$ of length $n$ that there is no index $i$ ($1 \le i \le n$) such that $p_i = i$ (so, for all $i$ from $1$ to $n$ the condition $p_i \ne i$ should be satisfied).</p><p>You have to answer $t$ independent test cases.</p><p>If there are several answers, you can print any. It can be proven that the answer exists for each $n &gt; 1$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($2 \le n \le 100$) — the length of the permutation you have to find.</p></div><div class="output-specification"><p>For each test case, print $n$ distinct integers $p_1, p_2, \ldots, p_n$ — a permutation that there is no index $i$ ($1 \le i \le n$) such that $p_i = i$ (so, for all $i$ from $1$ to $n$ the condition $p_i \ne i$ should be satisfied).</p><p>If there are several answers, you can print any. It can be proven that the answer exists for each $n &gt; 1$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($2 \le n \le 100$) — the length of the permutation you have to find.</p>

## Output

<p>For each test case, print $n$ distinct integers $p_1, p_2, \ldots, p_n$ — a permutation that there is no index $i$ ($1 \le i \le n$) such that $p_i = i$ (so, for all $i$ from $1$ to $n$ the condition $p_i \ne i$ should be satisfied).</p><p>If there are several answers, you can print any. It can be proven that the answer exists for each $n &gt; 1$.</p>





```input1
2
2
5
```




```output1
2 1
2 1 5 3 4
```


