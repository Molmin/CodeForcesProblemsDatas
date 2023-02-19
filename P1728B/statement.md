## Description

<div><p>Let's define the value of the permutation $p$ of $n$ integers $1$, $2$, ..., $n$ (a permutation is an array where each element from $1$ to $n$ occurs exactly once) as follows:</p><ul> <li> initially, an integer variable $x$ is equal to $0$; </li><li> if $x &lt; p_1$, then add $p_1$ to $x$ (set $x = x + p_1$), otherwise assign $0$ to $x$; </li><li> if $x &lt; p_2$, then add $p_2$ to $x$ (set $x = x + p_2$), otherwise assign $0$ to $x$; </li><li> ... </li><li> if $x &lt; p_n$, then add $p_n$ to $x$ (set $x = x + p_n$), otherwise assign $0$ to $x$; </li><li> the value of the permutation is $x$ at the end of this process. </li></ul><p>For example, for $p = [4, 5, 1, 2, 3, 6]$, the value of $x$ changes as follows: $0, 4, 9, 0, 2, 5, 11$, so the value of the permutation is $11$.</p><p>You are given an integer $n$. Find a permutation $p$ of size $n$ with the maximum possible value among all permutations of size $n$. If there are several such permutations, you can print any of them.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 97$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains one integer $n$ ($4 \le n \le 100$).</p></div><div class="output-specification"><p>For each test case, print $n$ integers&nbsp;— the permutation $p$ of size $n$ with the maximum possible value among all permutations of size $n$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 97$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains one integer $n$ ($4 \le n \le 100$).</p>

## Output

<p>For each test case, print $n$ integers&nbsp;— the permutation $p$ of size $n$ with the maximum possible value among all permutations of size $n$.</p>





```input1|2,4
3
4
5
6
```




```output1
2 1 3 4
1 2 3 4 5
4 5 1 2 3 6
```


