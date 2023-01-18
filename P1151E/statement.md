## Description

<div><p>The Kingdom of Kremland is a tree (a connected undirected graph without cycles) consisting of $n$ vertices. Each vertex $i$ has its own value $a_i$. All vertices are connected in series by edges. Formally, for every $1 \leq i &lt; n$ there is an edge between the vertices of $i$ and $i+1$.</p><p>Denote the function $f(l, r)$, which takes two integers $l$ and $r$ ($l \leq r$):</p><ul> &nbsp;&nbsp;<li> We leave in the tree only vertices whose values ​​range from $l$ to $r$. &nbsp;&nbsp;</li><li> The value of the function will be the number of connected components in the new graph. </li></ul><p>Your task is to calculate the following sum: $$\sum_{l=1}^{n} \sum_{r=l}^{n} f(l, r) $$</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the values of the vertices.</p></div><div class="output-specification"><p>Print one number&nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the values of the vertices.</p>

## Output

<p>Print one number&nbsp;— the answer to the problem.</p>





```input1
3
2 1 3
```




```input2
4
2 1 1 3
```




```input3
10
1 5 2 5 5 3 10 6 5 1
```




```output1
7
```




```output2
11
```




```output3
104
```



## Note

<p>In the first example, the function values ​​will be as follows: </p><ul> <li> $f(1, 1)=1$ (there is only a vertex with the number $2$, which forms one component) </li><li> $f(1, 2)=1$ (there are vertices $1$ and $2$ that form one component) </li><li> $f(1, 3)=1$ (all vertices remain, one component is obtained) </li><li> $f(2, 2)=1$ (only vertex number $1$) </li><li> $f(2, 3)=2$ (there are vertices $1$ and $3$ that form two components) </li><li> $f(3, 3)=1$ (only vertex $3$) </li></ul> Totally out $7$.<p>In the second example, the function values ​​will be as follows: </p><ul> <li> $f(1, 1)=1$ </li><li> $f(1, 2)=1$ </li><li> $f(1, 3)=1$ </li><li> $f(1, 4)=1$ </li><li> $f(2, 2)=1$ </li><li> $f(2, 3)=2$ </li><li> $f(2, 4)=2$ </li><li> $f(3, 3)=1$ </li><li> $f(3, 4)=1$ </li><li> $f(4, 4)=0$ (there is no vertex left, so the number of components is $0$) </li></ul> Totally out $11$.
