## Description

<div><p>You have $n$ rectangular wooden blocks, which are numbered from $1$ to $n$. The $i$-th block is $1$ unit high and $\lceil \frac{i}{2} \rceil$ units long.</p><p>Here, $\lceil \frac{x}{2} \rceil$ denotes the result of division of $x$ by $2$, rounded <span class="tex-font-style-bf">up</span>. For example, $\lceil \frac{4}{2} \rceil = 2$ and $\lceil \frac{5}{2} \rceil = \lceil 2.5 \rceil = 3$.</p><p>For example, if $n=5$, then the blocks have the following sizes: $1 \times 1$, $1 \times 1$, $1 \times 2$, $1 \times 2$, $1 \times 3$.</p><center> <img class="tex-graphics" src="file://MVfK6xiM.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The available blocks for $n=5$</span> </center><p>Find the maximum possible side length of a square you can create using these blocks, <span class="tex-font-style-bf">without rotating any of them</span>. Note that you don't have to use all of the blocks.</p><center> <img class="tex-graphics" src="file://RN9TugEy.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">One of the ways to create $3 \times 3$ square using blocks $1$ through $5$</span> </center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^9$)&nbsp;— the number of blocks.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the maximum possible side length of a square you can create.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^9$)&nbsp;— the number of blocks.</p>

## Output

<p>For each test case, print one integer&nbsp;— the maximum possible side length of a square you can create.</p>





```input1|2,4
3
2
5
197654321
```




```output1
1
3
98827161
```



## Note

<p>In the first test case, you can create a $1 \times 1$ square using only one of the blocks.</p><p>In the second test case, one of the possible ways to create a $3 \times 3$ square is shown in the statement. It is impossible to create a $4 \times 4$ or larger square, so the answer is $3$.</p>
