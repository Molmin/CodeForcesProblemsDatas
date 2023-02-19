## Description

<div><p>There are $n$ coins labeled from $1$ to $n$. Initially, coin $c_i$ is on position $i$ and is facing upwards (($c_1, c_2, \dots, c_n)$ is a permutation of numbers from $1$ to $n$). You can do some operations on these coins. </p><p>In one operation, you can do the following:</p><ul><li><p>Choose $2$ distinct indices $i$ and $j$.</p></li><li><p>Then, swap the coins on positions $i$ and $j$.</p></li><li><p>Then, flip both coins on positions $i$ and $j$. (If they are initially faced up, they will be faced down after the operation and vice versa)</p></li></ul><p>Construct a sequence of at most $n+1$ operations such that after performing all these operations the coin $i$ will be on position $i$ at the end, <span class="tex-font-style-bf">facing up</span>.</p><p>Note that you <span class="tex-font-style-bf">do not need</span> to minimize the number of operations.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$) — the number of coins.</p><p>The second line contains $n$ integers $c_1,c_2,\dots,c_n$ ($1 \le c_i \le n$, $c_i \neq c_j$ for $i\neq j$).</p></div><div class="output-specification"><p>In the first line, output an integer $q$ $(0 \leq q \leq n+1)$ — the number of operations you used.</p><p>In the following $q$ lines, output two integers $i$ and $j$ $(1 \leq i, j \leq n, i \ne j)$ — the positions you chose for the current operation.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$) — the number of coins.</p><p>The second line contains $n$ integers $c_1,c_2,\dots,c_n$ ($1 \le c_i \le n$, $c_i \neq c_j$ for $i\neq j$).</p>

## Output

<p>In the first line, output an integer $q$ $(0 \leq q \leq n+1)$ — the number of operations you used.</p><p>In the following $q$ lines, output two integers $i$ and $j$ $(1 \leq i, j \leq n, i \ne j)$ — the positions you chose for the current operation.</p>





```input1
3
2 1 3
```




```input2
5
1 2 3 4 5
```




```output1
3
1 3
3 2
3 1
```




```output2
0
```



## Note

<p>Let coin $i$ facing upwards be denoted as $i$ and coin $i$ facing downwards be denoted as $-i$.</p><p>The series of moves performed in the first sample changes the coins as such:</p><ul> <li> $[~~~2,~~~1,~~~3]$ </li><li> $[-3,~~~1,-2]$ </li><li> $[-3,~~~2,-1]$ </li><li> $[~~~1,~~~2,~~~3]$ </li></ul><p>In the second sample, the coins are already in their correct positions so there is no need to swap.</p>
