## Description

<div><p><span class="tex-font-style-it">Guy-Manuel and Thomas are going to build a polygon spaceship.</span> </p><p>You're given a <span class="tex-font-style-bf">strictly convex</span> (i. e. no three points are collinear) polygon $P$ which is defined by coordinates of its vertices. Define $P(x,y)$ as a polygon obtained by translating $P$ by vector $\overrightarrow {(x,y)}$. The picture below depicts an example of the translation:</p><p><img class="tex-graphics" src="file://RsdmctmH.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Define $T$ as a set of points which is the union of all $P(x,y)$ such that the origin $(0,0)$ lies in $P(x,y)$ (both strictly inside and on the boundary). There is also an equivalent definition: a point $(x,y)$ lies in $T$ only if there are two points $A,B$ in $P$ such that $\overrightarrow {AB} = \overrightarrow {(x,y)}$. One can prove $T$ is a polygon too. For example, if $P$ is a regular triangle then $T$ is a regular hexagon. At the picture below $P$ is drawn in black and some $P(x,y)$ which contain the origin are drawn in colored: </p><p><img class="tex-graphics" src="file://3qAwHfwg.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-font-style-it">The spaceship has the best aerodynamic performance if $P$ and $T$ are similar.</span> Your task is to check whether the polygons $P$ and $T$ are <a href="https://tinyurl.com/vp5m7vl">similar</a>.</p></div><div class="input-specification"><p>The first line of input will contain a single integer $n$ ($3 \le n \le 10^5$)&nbsp;— the number of points.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i, y_i$ ($|x_i|, |y_i| \le 10^9$), denoting the coordinates of the $i$-th vertex.</p><p>It is guaranteed that these points are listed in counterclockwise order and these points form a strictly convex polygon.</p></div><div class="output-specification"><p>Output <span class="tex-font-style-tt">"YES"</span> in a separate line, if $P$ and $T$ are similar. Otherwise, output <span class="tex-font-style-tt">"NO"</span> in a separate line. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of input will contain a single integer $n$ ($3 \le n \le 10^5$)&nbsp;— the number of points.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i, y_i$ ($|x_i|, |y_i| \le 10^9$), denoting the coordinates of the $i$-th vertex.</p><p>It is guaranteed that these points are listed in counterclockwise order and these points form a strictly convex polygon.</p>

## Output

<p>Output <span class="tex-font-style-tt">"YES"</span> in a separate line, if $P$ and $T$ are similar. Otherwise, output <span class="tex-font-style-tt">"NO"</span> in a separate line. You can print each letter in any case (upper or lower).</p>





```input1
4
1 0
4 1
3 4
0 3
```




```input2
3
100 86
50 0
150 0
```




```input3
8
0 0
1 0
2 1
3 3
4 6
3 6
2 5
1 3
```




```output1
YES
```




```output2
nO
```




```output3
YES
```



## Note

<p>The following image shows the first sample: both $P$ and $T$ are squares. The second sample was shown in the statements.</p><p><img class="tex-graphics" src="file://SdQjkG6e.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
