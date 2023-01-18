## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Khanh has $n$ points on the Cartesian plane, denoted by $a_1, a_2, \ldots, a_n$. All points' coordinates are integers between $-10^9$ and $10^9$, inclusive. No three points are collinear. He says that these points are vertices of a convex polygon; in other words, there exists a permutation $p_1, p_2, \ldots, p_n$ of integers from $1$ to $n$ such that the polygon $a_{p_1} a_{p_2} \ldots a_{p_n}$ is convex and vertices are listed in counter-clockwise order.</p><p>Khanh gives you the number $n$, but hides the coordinates of his points. Your task is to guess the above permutation by asking multiple queries. In each query, you give Khanh $4$ integers $t$, $i$, $j$, $k$; where either $t = 1$ or $t = 2$; and $i$, $j$, $k$ are three <span class="tex-font-style-bf">distinct</span> indices from $1$ to $n$, inclusive. In response, Khanh tells you:</p><ul> <li> if $t = 1$, the area of the triangle $a_ia_ja_k$ <span class="tex-font-style-bf">multiplied by $2$</span>. </li><li> if $t = 2$, the <span class="tex-font-style-it">sign</span> of the <span class="tex-font-style-it">cross product</span> of two <span class="tex-font-style-bf">vectors</span> $\overrightarrow{a_ia_j}$ and $\overrightarrow{a_ia_k}$. </li></ul><p>Recall that the <span class="tex-font-style-it">cross product</span> of vector $\overrightarrow{a} = (x_a, y_a)$ and vector $\overrightarrow{b} = (x_b, y_b)$ is the <span class="tex-font-style-bf">integer</span> $x_a \cdot y_b - x_b \cdot y_a$. The <span class="tex-font-style-it">sign</span> of a number is $1$ it it is positive, and $-1$ otherwise. It can be proven that the cross product obtained in the above queries can not be $0$.</p><p>You can ask at most $3 \cdot n$ queries.</p><p>Please note that Khanh fixes the coordinates of his points and does not change it while answering your queries. You do not need to guess the coordinates. In your permutation $a_{p_1}a_{p_2}\ldots a_{p_n}$, $p_1$ should be equal to $1$ and the indices of vertices should be <span class="tex-font-style-bf">listed in counter-clockwise order</span>.</p></div><div><h2>Interaction</h2><p>You start the interaction by reading $n$ ($3 \leq n \leq 1\,000$)&nbsp;— the number of vertices.</p><p>To ask a query, write $4$ integers $t$, $i$, $j$, $k$ ($1 \leq t \leq 2$, $1 \leq i, j, k \leq n$) in a separate line. $i$, $j$ and $k$ should be distinct.</p><p>Then read a single integer to get the answer to this query, as explained above. It can be proven that the answer of a query is always an integer.</p><p>When you find the permutation, write a number $0$. Then write $n$ integers $p_1, p_2, \ldots, p_n$ in the same line.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hack format</span></p><p>To hack, use the following format:</p><p>The first line contains an integer $n$ ($3 \leq n \leq 1\,000$)&nbsp;— the number of vertices.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$ and $y_i$ ($-10^9 \le x_i, y_i \le 10^9$)&nbsp;— the coordinate of the point $a_i$.</p></div>





```input1
6

15

-1

1
```




```output1
1 1 4 6

2 1 5 6

2 2 1 4

0 1 3 4 2 6 5
```



## Note

<p>The image below shows the hidden polygon in the example:</p><center> <img class="tex-graphics" height="378px" src="file://FVQvygoT.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>The interaction in the example goes as below: </p><ul> <li> Contestant reads $n = 6$. </li><li> Contestant asks a query with $t = 1$, $i = 1$, $j = 4$, $k = 6$. </li><li> Jury answers $15$. The area of the triangle $A_1A_4A_6$ is $7.5$. Note that the answer is <span class="tex-font-style-bf">two times</span> the area of the triangle. </li><li> Contestant asks a query with $t = 2$, $i = 1$, $j = 5$, $k = 6$. </li><li> Jury answers $-1$. The cross product of $\overrightarrow{A_1A_5} = (2, 2)$ and $\overrightarrow{A_1A_6} = (4, 1)$ is $-2$. The sign of $-2$ is $-1$. </li><li> Contestant asks a query with $t = 2$, $i = 2$, $j = 1$, $k = 4$. </li><li> Jury answers $1$. The cross product of $\overrightarrow{A_2A_1} = (-5, 2)$ and $\overrightarrow{A_2A_4} = (-2, -1)$ is $1$. The sign of $1$ is $1$. </li><li> Contestant says that the permutation is $(1, 3, 4, 2, 6, 5)$.  </li></ul>
