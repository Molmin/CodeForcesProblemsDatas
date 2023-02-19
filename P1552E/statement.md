## Description

<div><p>The numbers $1, \, 2, \, \dots, \, n \cdot k$ are colored with $n$ colors. These colors are indexed by $1, \, 2, \, \dots, \, n$. For each $1 \le i \le n$, there are exactly $k$ numbers colored with color $i$.</p><p>Let $[a, \, b]$ denote the interval of integers between $a$ and $b$ inclusive, that is, the set $\{a, \, a + 1, \, \dots, \, b\}$. You must choose $n$ intervals $[a_1, \, b_1], \, [a_2, \, b_2], \, \dots, [a_n, \, b_n]$ such that: </p><ul> <li> for each $1 \le i \le n$, it holds $1 \le a_i &lt; b_i \le n \cdot k$; </li><li> for each $1 \le i \le n$, the numbers $a_i$ and $b_i$ are colored with color $i$; </li><li> each number $1 \le x \le n \cdot k$ belongs to at most $\left\lceil \frac{n}{k - 1} \right\rceil$ intervals. </li></ul><p>One can show that such a family of intervals always exists under the given constraints.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 100$, $2 \le k \le 100$) — the number of colors and the number of occurrences of each color.</p><p>The second line contains $n \cdot k$ integers $c_1, \, c_2, \, \dots, \, c_{nk}$ ($1 \le c_j \le n$), where $c_j$ is the color of number $j$. It is guaranteed that, for each $1 \le i \le n$, it holds $c_j = i$ for exactly $k$ distinct indices $j$.</p></div><div class="output-specification"><p>Output $n$ lines. The $i$-th line should contain the two integers $a_i$ and $b_i$.</p><p>If there are multiple valid choices of the intervals, output any.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 100$, $2 \le k \le 100$) — the number of colors and the number of occurrences of each color.</p><p>The second line contains $n \cdot k$ integers $c_1, \, c_2, \, \dots, \, c_{nk}$ ($1 \le c_j \le n$), where $c_j$ is the color of number $j$. It is guaranteed that, for each $1 \le i \le n$, it holds $c_j = i$ for exactly $k$ distinct indices $j$.</p>

## Output

<p>Output $n$ lines. The $i$-th line should contain the two integers $a_i$ and $b_i$.</p><p>If there are multiple valid choices of the intervals, output any.</p>





```input1
4 3
2 4 3 1 1 4 2 3 2 1 3 4
```




```input2
1 2
1 1
```




```input3
3 3
3 1 2 3 2 1 2 1 3
```




```input4
2 3
2 1 1 1 2 2
```




```output1
4 5
1 7
8 11
6 12
```




```output2
1 2
```




```output3
6 8
3 7
1 4
```




```output4
2 3
5 6
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, each number can be contained in at most $\left\lceil \frac{4}{3 - 1} \right\rceil = 2$ intervals. The output is described by the following picture:</p><center> <img class="tex-graphics" src="file://IwZRdC01.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the <span class="tex-font-style-bf">second sample</span>, the only interval to be chosen is forced to be $[1, \, 2]$, and each number is indeed contained in at most $\left\lceil \frac{1}{2 - 1} \right\rceil = 1$ interval.</p><p>In the <span class="tex-font-style-bf">third sample</span>, each number can be contained in at most $\left\lceil \frac{3}{3 - 1} \right\rceil = 2$ intervals. The output is described by the following picture:</p><center> <img class="tex-graphics" src="file://eYwkUa37.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
