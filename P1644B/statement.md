## Description

<div><p>Let's call a permutation $p$ of length $n$ <span class="tex-font-style-bf">anti-Fibonacci</span> if the condition $p_{i-2} + p_{i-1} \ne p_i$ holds for all $i$ ($3 \le i \le n$). Recall that the permutation is the array of length $n$ which contains each integer from $1$ to $n$ exactly once.</p><p>Your task is for a given number $n$ print $n$ <span class="tex-font-style-bf">distinct</span> anti-Fibonacci permutations of length $n$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 48$)&nbsp;— the number of test cases. </p><p>The single line of each test case contains a single integer $n$ ($3 \le n \le 50$).</p></div><div class="output-specification"><p>For each test case, print $n$ lines. Each line should contain an anti-Fibonacci permutation of length $n$. In each test case, you cannot print any permutation more than once.</p><p>If there are multiple answers, print any of them. It can be shown that it is always possible to find $n$ different anti-Fibonacci permutations of size $n$ under the constraints of the problem.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 48$)&nbsp;— the number of test cases. </p><p>The single line of each test case contains a single integer $n$ ($3 \le n \le 50$).</p>

## Output

<p>For each test case, print $n$ lines. Each line should contain an anti-Fibonacci permutation of length $n$. In each test case, you cannot print any permutation more than once.</p><p>If there are multiple answers, print any of them. It can be shown that it is always possible to find $n$ different anti-Fibonacci permutations of size $n$ under the constraints of the problem.</p>





```input1
2
4
3
```




```output1
4 1 3 2
1 2 4 3
3 4 1 2
2 4 1 3
3 2 1
1 3 2
3 1 2
```


