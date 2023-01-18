## Description

<div><p>Ivan places knights on infinite chessboard. Initially there are $n$ knights. If there is free cell which is under attack of at least $4$ knights then he places new knight in this cell. Ivan repeats this until there are no such free cells. One can prove that this process is finite. One can also prove that position in the end does not depend on the order in which new knights are placed.</p><p>Ivan asked you to find initial placement of exactly $n$ knights such that in the end there will be at least $\lfloor \frac{n^{2}}{10} \rfloor$ knights.</p></div><div class="input-specification"><p>The only line of input contains one integer $n$ ($1 \le n \le 10^{3}$)&nbsp;— number of knights in the initial placement.</p></div><div class="output-specification"><p>Print $n$ lines. Each line should contain $2$ numbers $x_{i}$ and $y_{i}$ ($-10^{9} \le x_{i}, \,\, y_{i} \le 10^{9}$)&nbsp;— coordinates of $i$-th knight. For all $i \ne j$, $(x_{i}, \,\, y_{i}) \ne (x_{j}, \,\, y_{j})$ should hold. In other words, all knights should be in different cells.</p><p>It is guaranteed that the solution exists.</p></div>

## Input

<p>The only line of input contains one integer $n$ ($1 \le n \le 10^{3}$)&nbsp;— number of knights in the initial placement.</p>

## Output

<p>Print $n$ lines. Each line should contain $2$ numbers $x_{i}$ and $y_{i}$ ($-10^{9} \le x_{i}, \,\, y_{i} \le 10^{9}$)&nbsp;— coordinates of $i$-th knight. For all $i \ne j$, $(x_{i}, \,\, y_{i}) \ne (x_{j}, \,\, y_{j})$ should hold. In other words, all knights should be in different cells.</p><p>It is guaranteed that the solution exists.</p>





```input1
4

```




```input2
7

```




```output1
1 1
3 1
1 5
4 4

```




```output2
2 1
1 2
4 1
5 2
2 6
5 7
6 6

```



## Note

<p>Let's look at second example:</p><p><img class="tex-graphics" src="file://7F1yDGl7.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Green zeroes are initial knights. Cell $(3, \,\, 3)$ is under attack of $4$ knights in cells $(1, \,\, 2)$, $(2, \,\, 1)$, $(4, \,\, 1)$ and $(5, \,\, 2)$, therefore Ivan will place a knight in this cell. Cell $(4, \,\, 5)$ is initially attacked by only $3$ knights in cells $(2, \,\, 6)$, $(5, \,\, 7)$ and $(6, \,\, 6)$. But new knight in cell $(3, \,\, 3)$ also attacks cell $(4, \,\, 5)$, now it is attacked by $4$ knights and Ivan will place another knight in this cell. There are no more free cells which are attacked by $4$ or more knights, so the process stops. There are $9$ knights in the end, which is not less than $\lfloor \frac{7^{2}}{10} \rfloor = 4$.</p>
