## Description

<div><p>You are given $n$ distinct points on a plane. The coordinates of the $i$-th point are $(x_i, y_i)$.</p><p>For each point $i$, find the nearest (in terms of Manhattan distance) point with <span class="tex-font-style-bf">integer coordinates</span> that is not among the given $n$ points. If there are multiple such points — you can choose any of them.</p><p>The Manhattan distance between two points $(x_1, y_1)$ and $(x_2, y_2)$ is $|x_1 - x_2| + |y_1 - y_2|$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of points in the set.</p><p>The next $n$ lines describe points. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 2 \cdot 10^5$) — coordinates of the $i$-th point.</p><p>It is guaranteed that all points in the input are distinct.</p></div><div class="output-specification"><p>Print $n$ lines. In the $i$-th line, print the point with <span class="tex-font-style-bf">integer coordinates</span> that is not among the given $n$ points and is the nearest (in terms of Manhattan distance) to the $i$-th point from the input.</p><p>Output coordinates should be in range $[-10^6; 10^6]$. It can be shown that any optimal answer meets these constraints.</p><p>If there are several answers, you can print any of them.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of points in the set.</p><p>The next $n$ lines describe points. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 2 \cdot 10^5$) — coordinates of the $i$-th point.</p><p>It is guaranteed that all points in the input are distinct.</p>

## Output

<p>Print $n$ lines. In the $i$-th line, print the point with <span class="tex-font-style-bf">integer coordinates</span> that is not among the given $n$ points and is the nearest (in terms of Manhattan distance) to the $i$-th point from the input.</p><p>Output coordinates should be in range $[-10^6; 10^6]$. It can be shown that any optimal answer meets these constraints.</p><p>If there are several answers, you can print any of them.</p>





```input1
6
2 2
1 2
2 1
3 2
2 3
5 5
```




```input2
8
4 4
2 4
2 2
2 3
1 4
4 2
1 3
3 3
```




```output1
1 1
1 1
2 0
3 1
2 4
5 4
```




```output2
4 3
2 5
2 1
2 5
1 5
4 1
1 2
3 2
```


