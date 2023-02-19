## Description

<div><p>You are given four integers $n$, $m$, $l$ and $r$.</p><p>Let's name a tuple $(x_1, y_1, x_2, y_2)$ as <span class="tex-font-style-it">good</span> if: </p><ol> <li> $1 \le x_1 &lt; x_2 \le n$; </li><li> $1 \le y_2 &lt; y_1 \le m$; </li><li> $x_1 \cdot y_1 = x_2 \cdot y_2$; </li><li> $l \le x_1 \cdot y_1 \le r$. </li></ol><p>Find any good tuple <span class="tex-font-style-bf">for each $x_1$ from $1$ to $n$ inclusive</span>.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$).</p><p>The second line contains two integers $l$ and $r$ ($1 \le l \le r \le nm$).</p></div><div class="output-specification"><p>For each $x_1$ from $1$ to $n$ inclusive: </p><ul> <li> if there are no such four integers, print $-1$; </li><li> otherwise, print four integers $x_1$, $y_1$, $x_2$ and $y_2$. If there are multiple answers, print any of them. </li></ul></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$).</p><p>The second line contains two integers $l$ and $r$ ($1 \le l \le r \le nm$).</p>

## Output

<p>For each $x_1$ from $1$ to $n$ inclusive: </p><ul> <li> if there are no such four integers, print $-1$; </li><li> otherwise, print four integers $x_1$, $y_1$, $x_2$ and $y_2$. If there are multiple answers, print any of them. </li></ul>





```input1
8 20
91 100
```




```input2
4 5
1 10
```




```input3
5 12
16 60
```




```output1
-1
-1
-1
-1
-1
6 16 8 12
-1
-1
```




```output2
1 2 2 1
2 3 3 2
-1
-1
```




```output3
-1
2 9 3 6
3 8 4 6
4 5 5 4
-1
```


