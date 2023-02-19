## Description

<div><p>The Winter holiday will be here soon. Mr. Chanek wants to decorate his house's wall with ornaments. The wall can be represented as a binary string $a$ of length $n$. His favorite nephew has another binary string $b$ of length $m$ ($m \leq n$).</p><p>Mr. Chanek's nephew loves the non-negative integer $k$. His nephew wants exactly $k$ occurrences of $b$ as substrings in $a$. </p><p>However, Mr. Chanek does not know the value of $k$. So, for each $k$ ($0 \leq k \leq n - m + 1$), find the minimum number of elements in $a$ that have to be changed such that there are exactly $k$ occurrences of $b$ in $a$.</p><p>A string $s$ occurs exactly $k$ times in $t$ if there are exactly $k$ different pairs $(p,q)$ such that we can obtain $s$ by deleting $p$ characters from the beginning and $q$ characters from the end of $t$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq m \leq n \leq 500$) — size of the binary string $a$ and $b$ respectively.</p><p>The second line contains a binary string $a$ of length $n$.</p><p>The third line contains a binary string $b$ of length $m$.</p></div><div class="output-specification"><p>Output $n - m + 2$ integers — the $(k+1)$-th integer denotes the minimal number of elements in $a$ that have to be changed so there are exactly $k$ occurrences of $b$ as a substring in $a$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq m \leq n \leq 500$) — size of the binary string $a$ and $b$ respectively.</p><p>The second line contains a binary string $a$ of length $n$.</p><p>The third line contains a binary string $b$ of length $m$.</p>

## Output

<p>Output $n - m + 2$ integers — the $(k+1)$-th integer denotes the minimal number of elements in $a$ that have to be changed so there are exactly $k$ occurrences of $b$ as a substring in $a$.</p>





```input1
9 3
100101011
101
```




```output1
1 1 0 1 6 -1 -1 -1
```



## Note

<p>For $k = 0$, to make the string $a$ have no occurrence of <span class="tex-font-style-tt">101</span>, you can do one character change as follows.</p><p><span class="tex-font-style-tt">10010<span class="tex-font-style-bf">1</span>011</span> $\rightarrow$ <span class="tex-font-style-tt">10010<span class="tex-font-style-bf">0</span>011</span></p><p>For $k = 1$, you can also change a single character.</p><p><span class="tex-font-style-tt">100<span class="tex-font-style-bf">1</span>01011</span> $\rightarrow$ <span class="tex-font-style-tt">100<span class="tex-font-style-bf">0</span>01011</span></p><p>For $k = 2$, no changes are needed.</p>
