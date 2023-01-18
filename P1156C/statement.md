## Description

<div><p>You are given a set of points $x_1$, $x_2$, ..., $x_n$ on the number line.</p><p>Two points $i$ and $j$ can be matched with each other if the following conditions hold:</p><ul> <li> neither $i$ nor $j$ is matched with any other point; </li><li> $|x_i - x_j| \ge z$. </li></ul><p>What is the maximum number of pairs of points you can match with each other?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $z$ ($2 \le n \le 2 \cdot 10^5$, $1 \le z \le 10^9$) — the number of points and the constraint on the distance between matched points, respectively.</p><p>The second line contains $n$ integers $x_1$, $x_2$, ..., $x_n$ ($1 \le x_i \le 10^9$).</p></div><div class="output-specification"><p>Print one integer — the maximum number of pairs of points you can match with each other.</p></div>

## Input

<p>The first line contains two integers $n$ and $z$ ($2 \le n \le 2 \cdot 10^5$, $1 \le z \le 10^9$) — the number of points and the constraint on the distance between matched points, respectively.</p><p>The second line contains $n$ integers $x_1$, $x_2$, ..., $x_n$ ($1 \le x_i \le 10^9$).</p>

## Output

<p>Print one integer — the maximum number of pairs of points you can match with each other.</p>





```input1
4 2
1 3 3 7
```




```input2
5 5
10 9 5 8 7
```




```output1
2
```




```output2
1
```



## Note

<p>In the first example, you may match point $1$ with point $2$ ($|3 - 1| \ge 2$), and point $3$ with point $4$ ($|7 - 3| \ge 2$).</p><p>In the second example, you may match point $1$ with point $3$ ($|5 - 10| \ge 5$).</p>
