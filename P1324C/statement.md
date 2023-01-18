## Description

<div><p>There is a frog staying to the left of the string $s = s_1 s_2 \ldots s_n$ consisting of $n$ characters (to be more precise, the frog initially stays at the cell $0$). Each character of $s$ is either '<span class="tex-font-style-tt">L</span>' or '<span class="tex-font-style-tt">R</span>'. It means that if the frog is staying at the $i$-th cell and the $i$-th character is '<span class="tex-font-style-tt">L</span>', the frog can jump only to the left. If the frog is staying at the $i$-th cell and the $i$-th character is '<span class="tex-font-style-tt">R</span>', the frog can jump only to the right. <span class="tex-font-style-bf">The frog can jump only to the right from the cell $0$</span>.</p><p><span class="tex-font-style-bf">Note that the frog can jump into the same cell twice and can perform as many jumps as it needs</span>.</p><p>The frog wants to reach the $n+1$-th cell. The frog chooses some <span class="tex-font-style-bf">positive integer</span> value $d$ <span class="tex-font-style-bf">before the first jump</span> (and cannot change it later) and jumps by no more than $d$ cells at once. I.e. if the $i$-th character is '<span class="tex-font-style-tt">L</span>' then the frog can jump to any cell in a range $[max(0, i - d); i - 1]$, and if the $i$-th character is '<span class="tex-font-style-tt">R</span>' then the frog can jump to any cell in a range $[i + 1; min(n + 1; i + d)]$.</p><p>The frog doesn't want to jump far, so your task is to find the minimum possible value of $d$ such that the frog can reach the cell $n+1$ from the cell $0$ if it can jump by no more than $d$ cells at once. <span class="tex-font-style-bf">It is guaranteed that it is always possible to reach $n+1$ from $0$</span>.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The next $t$ lines describe test cases. The $i$-th test case is described as a string $s$ consisting of at least $1$ and at most $2 \cdot 10^5$ characters '<span class="tex-font-style-tt">L</span>' and '<span class="tex-font-style-tt">R</span>'.</p><p>It is guaranteed that the sum of lengths of strings over all test cases does not exceed $2 \cdot 10^5$ ($\sum |s| \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer — the minimum possible value of $d$ such that the frog can reach the cell $n+1$ from the cell $0$ if it jumps by no more than $d$ at once.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The next $t$ lines describe test cases. The $i$-th test case is described as a string $s$ consisting of at least $1$ and at most $2 \cdot 10^5$ characters '<span class="tex-font-style-tt">L</span>' and '<span class="tex-font-style-tt">R</span>'.</p><p>It is guaranteed that the sum of lengths of strings over all test cases does not exceed $2 \cdot 10^5$ ($\sum |s| \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer — the minimum possible value of $d$ such that the frog can reach the cell $n+1$ from the cell $0$ if it jumps by no more than $d$ at once.</p>





```input1
6
LRLRRLL
L
LLR
RRRR
LLLLLL
R
```




```output1
3
2
3
1
7
1
```



## Note

<p>The picture describing the first test case of the example and one of the possible answers:</p><p><img class="tex-graphics" src="file://yLpIOYvj.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second test case of the example, the frog can only jump directly from $0$ to $n+1$.</p><p>In the third test case of the example, the frog can choose $d=3$, jump to the cell $3$ from the cell $0$ and then to the cell $4$ from the cell $3$.</p><p>In the fourth test case of the example, the frog can choose $d=1$ and jump $5$ times to the right.</p><p>In the fifth test case of the example, the frog can only jump directly from $0$ to $n+1$.</p><p>In the sixth test case of the example, the frog can choose $d=1$ and jump $2$ times to the right.</p>
