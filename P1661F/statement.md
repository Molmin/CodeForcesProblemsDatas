## Description

<div><p>There are $n+1$ teleporters on a straight line, located in points $0$, $a_1$, $a_2$, $a_3$, ..., $a_n$. It's possible to teleport from point $x$ to point $y$ if there are teleporters in <span class="tex-font-style-bf">both</span> of those points, and it costs $(x-y)^2$ energy.</p><p>You want to install some additional teleporters so that it is possible to get from the point $0$ to the point $a_n$ (possibly through some other teleporters) spending <span class="tex-font-style-bf">no more</span> than $m$ energy in total. Each teleporter you install must be located in an <span class="tex-font-style-bf">integer point</span>.</p><p>What is the minimum number of teleporters you have to install?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 &lt; a_2 &lt; a_3 &lt; \dots &lt; a_n \le 10^9$).</p><p>The third line contains one integer $m$ ($a_n \le m \le 10^{18}$).</p></div><div class="output-specification"><p>Print one integer — the minimum number of teleporters you have to install so that it is possible to get from $0$ to $a_n$ spending at most $m$ energy. It can be shown that it's always possible under the constraints from the input format.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 &lt; a_2 &lt; a_3 &lt; \dots &lt; a_n \le 10^9$).</p><p>The third line contains one integer $m$ ($a_n \le m \le 10^{18}$).</p>

## Output

<p>Print one integer — the minimum number of teleporters you have to install so that it is possible to get from $0$ to $a_n$ spending at most $m$ energy. It can be shown that it's always possible under the constraints from the input format.</p>





```input1
2
1 5
7
```




```input2
2
1 5
6
```




```input3
1
5
5
```




```input4
1
1000000000
1000000043
```




```output1
2
```




```output2
3
```




```output3
4
```




```output4
999999978
```


