## Description

<div><p>You are given an array consisting of all integers from $[l, r]$ inclusive. For example, if $l = 2$ and $r = 5$, the array would be $[2, 3, 4, 5]$. What's the minimum number of elements you can delete to make the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND</a> of the array non-zero?</p><p>A <span class="tex-font-style-it">bitwise AND</span> is a binary operation that takes two equal-length binary representations and performs the <span class="tex-font-style-it">AND</span> operation on each pair of the corresponding bits.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 2 \cdot 10^5$)&nbsp;— the description of the array.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 2 \cdot 10^5$)&nbsp;— the description of the array.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the answer to the problem.</p>





```input1
5
1 2
2 8
4 5
1 5
100000 200000
```




```output1
1
3
0
2
31072
```



## Note

<p>In the first test case, the array is $[1, 2]$. Currently, the <span class="tex-font-style-it">bitwise AND</span> is $0$, as $1\ \&amp; \ 2 = 0$. However, after deleting $1$ (or $2$), the array becomes $[2]$ (or $[1]$), and the <span class="tex-font-style-it">bitwise AND</span> becomes $2$ (or $1$). This can be proven to be the optimal, so the answer is $1$.</p><p>In the second test case, the array is $[2, 3, 4, 5, 6, 7, 8]$. Currently, the <span class="tex-font-style-it">bitwise AND</span> is $0$. However, after deleting $4$, $5$, and $8$, the array becomes $[2, 3, 6, 7]$, and the <span class="tex-font-style-it">bitwise AND</span> becomes $2$. This can be proven to be the optimal, so the answer is $3$. Note that there may be other ways to delete $3$ elements.</p>
