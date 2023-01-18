## Description

<div><p>Someone give a strange birthday present to Ivan. It is hedgehog&nbsp;— connected undirected graph in which one vertex has degree at least $3$ (we will call it center) and all other vertices has degree 1. Ivan thought that hedgehog is too boring and decided to make himself $k$-multihedgehog.</p><p>Let us define $k$-multihedgehog as follows:</p><ul><li> $1$-multihedgehog is hedgehog: it has one vertex of degree at least $3$ and some vertices of degree 1.</li><li> For all $k \ge 2$, $k$-multihedgehog is $(k-1)$-multihedgehog in which the following changes has been made for each vertex $v$ with degree 1: let $u$ be its only neighbor; remove vertex $v$, create a new hedgehog with center at vertex $w$ and connect vertices $u$ and $w$ with an edge. New hedgehogs can differ from each other and the initial gift. </li></ul><p>Thereby $k$-multihedgehog is a tree. Ivan made $k$-multihedgehog but he is not sure that he did not make any mistakes. That is why he asked you to check if his tree is indeed $k$-multihedgehog.</p></div><div class="input-specification"><p>First line of input contains $2$ integers $n$, $k$ ($1 \le n \le 10^{5}$, $1 \le k \le 10^{9}$)&nbsp;— number of vertices and hedgehog parameter.</p><p>Next $n-1$ lines contains two integers $u$ $v$ ($1 \le u, \,\, v \le n; \,\, u \ne v$)&nbsp;— indices of vertices connected by edge.</p><p>It is guaranteed that given graph is a tree.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">"Yes"</span> (without quotes), if given graph is $k$-multihedgehog, and <span class="tex-font-style-tt">"No"</span> (without quotes) otherwise.</p></div>

## Input

<p>First line of input contains $2$ integers $n$, $k$ ($1 \le n \le 10^{5}$, $1 \le k \le 10^{9}$)&nbsp;— number of vertices and hedgehog parameter.</p><p>Next $n-1$ lines contains two integers $u$ $v$ ($1 \le u, \,\, v \le n; \,\, u \ne v$)&nbsp;— indices of vertices connected by edge.</p><p>It is guaranteed that given graph is a tree.</p>

## Output

<p>Print <span class="tex-font-style-tt">"Yes"</span> (without quotes), if given graph is $k$-multihedgehog, and <span class="tex-font-style-tt">"No"</span> (without quotes) otherwise.</p>





```input1
14 2
1 4
2 4
3 4
4 13
10 5
11 5
12 5
14 5
5 13
6 7
8 6
13 6
9 6

```




```input2
3 1
1 3
2 3

```




```output1
Yes

```




```output2
No

```



## Note

<p>2-multihedgehog from the first example looks like this:</p><p><img class="tex-graphics" src="file://A5JT6s5x.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Its center is vertex $13$. Hedgehogs created on last step are: [4 (center), 1, 2, 3], [6 (center), 7, 8, 9], [5 (center), 10, 11, 12, 13].</p><p>Tree from second example is not a hedgehog because degree of center should be at least $3$.</p>
