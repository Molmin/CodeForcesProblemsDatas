## Description

<div><p>You're given an array $a$ of length $n$. You can perform the following operation on it as many times as you want:</p><ul> <li> Pick two integers $i$ and $j$ $(1 \le i,j \le n)$ such that <span class="tex-font-style-bf">$a_i+a_j$ is odd</span>, then swap $a_i$ and $a_j$. </li></ul><p>What is lexicographically the smallest array you can obtain?</p><p>An array $x$ is <a href="https://en.wikipedia.org/wiki/Lexicographical_order">lexicographically smaller</a> than an array $y$ if there exists an index $i$ such that $x_i&lt;y_i$, and $x_j=y_j$ for all $1 \le j &lt; i$. Less formally, at the first index $i$ in which they differ, $x_i&lt;y_i$</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of elements in the array $a$.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p></div><div class="output-specification"><p>The only line contains $n$ space-separated integers, the lexicographically smallest array you can obtain.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of elements in the array $a$.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p>

## Output

<p>The only line contains $n$ space-separated integers, the lexicographically smallest array you can obtain.</p>





```input1
3
4 1 7
```




```input2
2
1 1
```




```output1
1 4 7
```




```output2
1 1
```



## Note

<p>In the first example, we can swap $1$ and $4$ since $1+4=5$, which is odd.</p>
