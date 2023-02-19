## Description

<div><p>Alice has an integer sequence $a$ of length $n$ and <span class="tex-font-style-bf">all elements are different</span>. She will choose a subsequence of $a$ of length $m$, and defines the value of a subsequence $a_{b_1},a_{b_2},\ldots,a_{b_m}$ as $$\sum_{i = 1}^m (m \cdot a_{b_i}) - \sum_{i = 1}^m \sum_{j = 1}^m f(\min(b_i, b_j), \max(b_i, b_j)),$$ where $f(i, j)$ denotes $\min(a_i, a_{i + 1}, \ldots, a_j)$.</p><p>Alice wants you to help her to maximize the value of the subsequence she choose.</p><p>A sequence $s$ is a subsequence of a sequence $t$ if $s$ can be obtained from $t$ by deletion of several (possibly, zero or all) elements.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le m \le n \le 4000$).</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i &lt; 2^{31}$).</p></div><div class="output-specification"><p>Print the maximal value Alice can get.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le m \le n \le 4000$).</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i &lt; 2^{31}$).</p>

## Output

<p>Print the maximal value Alice can get.</p>





```input1
6 4
15 2 18 12 13 4
```




```input2
11 5
9 3 7 1 8 12 10 20 15 18 5
```




```input3
1 1
114514
```




```input4
2 1
666 888
```




```output1
100
```




```output2
176
```




```output3
0
```




```output4
0
```



## Note

<p>In the first example, Alice can choose the subsequence $[15, 2, 18, 13]$, which has the value $4 \cdot (15 + 2 + 18 + 13) - (15 + 2 + 2 + 2) - (2 + 2 + 2 + 2) - (2 + 2 + 18 + 12) - (2 + 2 + 12 + 13) = 100$. In the second example, there are a variety of subsequences with value $176$, and one of them is $[9, 7, 12, 20, 18]$.</p>
