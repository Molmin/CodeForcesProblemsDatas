## Description

<div><p>You are given a tree, consisting of $n$ vertices. Each edge has an integer value written on it.</p><p>Let $f(v, u)$ be the number of values that appear <span class="tex-font-style-bf">exactly once</span> on the edges of a simple path between vertices $v$ and $u$.</p><p>Calculate the sum of $f(v, u)$ over all pairs of vertices $v$ and $u$ such that $1 \le v &lt; u \le n$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Each of the next $n-1$ lines contains three integers $v, u$ and $x$ ($1 \le v, u, x \le n$)&nbsp;— the description of an edge: the vertices it connects and the value written on it.</p><p>The given edges form a tree.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the sum of $f(v, u)$ over all pairs of vertices $v$ and $u$ such that $v &lt; u$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Each of the next $n-1$ lines contains three integers $v, u$ and $x$ ($1 \le v, u, x \le n$)&nbsp;— the description of an edge: the vertices it connects and the value written on it.</p><p>The given edges form a tree.</p>

## Output

<p>Print a single integer&nbsp;— the sum of $f(v, u)$ over all pairs of vertices $v$ and $u$ such that $v &lt; u$.</p>





```input1
3
1 2 1
1 3 2
```




```input2
3
1 2 2
1 3 2
```




```input3
5
1 4 4
1 2 3
3 4 4
4 5 5
```




```input4
2
2 1 1
```




```input5
10
10 2 3
3 8 8
4 8 9
5 8 5
3 10 7
7 8 2
5 6 6
9 3 4
1 6 3
```




```output1
4
```




```output2
2
```




```output3
14
```




```output4
1
```




```output5
120
```


