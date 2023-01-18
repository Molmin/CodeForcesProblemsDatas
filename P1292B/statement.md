## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://soundcloud.com/kivawu/hyouryu"><span class="tex-font-style-it">THE SxPLAY &amp; KIVΛ - 漂流</span></a></div></div> <div class="epigraph"><div class="epigraph-text"><a href="https://soundcloud.com/kivawu/perspectives"><span class="tex-font-style-it">KIVΛ &amp; Nikki Simmons - Perspectives</span></a></div></div><p>With a new body, our idol Aroma White (or should we call her Kaori Minamiya?) begins to uncover her lost past through the OS space.</p><p>The space can be considered a 2D plane, with an infinite number of data nodes, indexed from $0$, with their coordinates defined as follows:</p><ul> <li> The coordinates of the $0$-th node is $(x_0, y_0)$ </li><li> For $i &gt; 0$, the coordinates of $i$-th node is $(a_x \cdot x_{i-1} + b_x, a_y \cdot y_{i-1} + b_y)$ </li></ul><p>Initially Aroma stands at the point $(x_s, y_s)$. She can stay in OS space for at most $t$ seconds, because after this time she has to warp back to the real world. She <span class="tex-font-style-bf">doesn't</span> need to return to the entry point $(x_s, y_s)$ to warp home.</p><p>While within the OS space, Aroma can do the following actions:</p><ul> <li> From the point $(x, y)$, Aroma can move to one of the following points: $(x-1, y)$, $(x+1, y)$, $(x, y-1)$ or $(x, y+1)$. This action requires $1$ second. </li><li> If there is a data node at where Aroma is staying, she can collect it. We can assume this action costs $0$ seconds. Of course, each data node can be collected at most once. </li></ul><p>Aroma wants to collect as many data as possible before warping back. Can you help her in calculating the maximum number of data nodes she could collect within $t$ seconds?</p></div><div class="input-specification"><p>The first line contains integers $x_0$, $y_0$, $a_x$, $a_y$, $b_x$, $b_y$ ($1 \leq x_0, y_0 \leq 10^{16}$, $2 \leq a_x, a_y \leq 100$, $0 \leq b_x, b_y \leq 10^{16}$), which define the coordinates of the data nodes.</p><p>The second line contains integers $x_s$, $y_s$, $t$ ($1 \leq x_s, y_s, t \leq 10^{16}$)&nbsp;– the initial Aroma's coordinates and the amount of time available.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum number of data nodes Aroma can collect within $t$ seconds.</p></div>

## Input

<p>The first line contains integers $x_0$, $y_0$, $a_x$, $a_y$, $b_x$, $b_y$ ($1 \leq x_0, y_0 \leq 10^{16}$, $2 \leq a_x, a_y \leq 100$, $0 \leq b_x, b_y \leq 10^{16}$), which define the coordinates of the data nodes.</p><p>The second line contains integers $x_s$, $y_s$, $t$ ($1 \leq x_s, y_s, t \leq 10^{16}$)&nbsp;– the initial Aroma's coordinates and the amount of time available.</p>

## Output

<p>Print a single integer&nbsp;— the maximum number of data nodes Aroma can collect within $t$ seconds.</p>





```input1
1 1 2 3 1 0
2 4 20
```




```input2
1 1 2 3 1 0
15 27 26
```




```input3
1 1 2 3 1 0
2 2 1
```




```output1
3
```




```output2
2
```




```output3
0
```



## Note

<p>In all three examples, the coordinates of the first $5$ data nodes are $(1, 1)$, $(3, 3)$, $(7, 9)$, $(15, 27)$ and $(31, 81)$ (remember that nodes are numbered from $0$).</p><p>In the first example, the optimal route to collect $3$ nodes is as follows: </p><ul> <li> Go to the coordinates $(3, 3)$ and collect the $1$-st node. This takes $|3 - 2| + |3 - 4| = 2$ seconds. </li><li> Go to the coordinates $(1, 1)$ and collect the $0$-th node. This takes $|1 - 3| + |1 - 3| = 4$ seconds. </li><li> Go to the coordinates $(7, 9)$ and collect the $2$-nd node. This takes $|7 - 1| + |9 - 1| = 14$ seconds. </li></ul><p>In the second example, the optimal route to collect $2$ nodes is as follows: </p><ul> <li> Collect the $3$-rd node. This requires no seconds. </li><li> Go to the coordinates $(7, 9)$ and collect the $2$-th node. This takes $|15 - 7| + |27 - 9| = 26$ seconds. </li></ul><p>In the third example, Aroma can't collect any nodes. She should have taken proper rest instead of rushing into the OS space like that.</p>
