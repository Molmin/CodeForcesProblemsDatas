## Description

<div><p>You are given five integers $n$, $dx_1$, $dy_1$, $dx_2$ and $dy_2$. You have to select $n$ distinct pairs of integers $(x_i, y_i)$ in such a way that, for every possible pair of integers $(x, y)$, there exists exactly one triple of integers $(a, b, i)$ meeting the following constraints:</p><center> $ \begin{cases} x \, = \, x_i + a \cdot dx_1 + b \cdot dx_2, \\ y \, = \, y_i + a \cdot dy_1 + b \cdot dy_2. \end{cases} $ </center></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains two integers $dx_1$ and $dy_1$ ($-10^6 \le dx_1, dy_1 \le 10^6$).</p><p>The third line contains two integers $dx_2$ and $dy_2$ ($-10^6 \le dx_2, dy_2 \le 10^6$).</p></div><div class="output-specification"><p>If it is impossible to correctly select $n$ pairs of integers, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, and then $n$ lines, the $i$-th of which contains two integers $x_i$ and $y_i$ ($-10^9 \le x_i, y_i \le 10^9$).</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains two integers $dx_1$ and $dy_1$ ($-10^6 \le dx_1, dy_1 \le 10^6$).</p><p>The third line contains two integers $dx_2$ and $dy_2$ ($-10^6 \le dx_2, dy_2 \le 10^6$).</p>

## Output

<p>If it is impossible to correctly select $n$ pairs of integers, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, and then $n$ lines, the $i$-th of which contains two integers $x_i$ and $y_i$ ($-10^9 \le x_i, y_i \le 10^9$).</p><p>If there are multiple solutions, print any of them.</p>





```input1
4
2 0
0 2
```




```input2
5
2 6
1 5
```




```input3
2
3 4
1 2
```




```output1
YES
0 0
0 1
1 0
1 1
```




```output2
NO
```




```output3
YES
0 0
0 1
```


