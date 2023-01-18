## Description

<div><p>A group of researchers are studying fish population in a natural system of lakes and rivers. The system contains $n$ lakes connected by $n - 1$ rivers. Each river has integer length (in kilometers) and can be traversed in both directions. It is possible to travel between any pair of lakes by traversing the rivers (that is, the network of lakes and rivers form a tree).</p><p>There is an unknown number of indistinguishable fish living in the lakes. On day $1$, fish can be at arbitrary lakes. Fish can travel between lakes by swimming the rivers. Each fish can swim a river $l$ kilometers long in any direction in $l$ days. Further, each fish can stay any number of days in any particular lake it visits. No fish ever appear or disappear from the lake system. Each lake can accomodate any number of fish at any time.</p><p>The researchers made several observations. The $j$-th of these observations is "on day $d_j$ there were at least $f_j$ distinct fish in the lake $p_j$". Help the researchers in determining the smallest possible total number of fish living in the lake system that doesn't contradict the observations.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of lakes in the system.</p><p>The next $n - 1$ lines describe the rivers. The $i$-th of these lines contains three integers $u_i$, $v_i$, $l_i$ ($1 \leq u_i, v_i \leq n$, $u_i \neq v_i$, $1 \leq l_i \leq 10^3$)&nbsp;— $1$-based indices of lakes connected by the $i$-th river, and the length of this river.</p><p>The next line contains a single integer $k$ ($1 \leq k \leq 10^5$)&nbsp;— the number of observations.</p><p>The next $k$ lines describe the observations. The $j$-th of these lines contains three integers $d_j$, $f_j$, $p_j$ ($1 \leq d_j \leq 10^8$, $1 \leq f_j \leq 10^4$, $1 \leq p_j \leq n$)&nbsp;— the day, the number of fish, and the lake index of the $j$-th observation. No two observations happen on the same day at the same lake simultaneously.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the smallest total number of fish not contradicting the observations.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of lakes in the system.</p><p>The next $n - 1$ lines describe the rivers. The $i$-th of these lines contains three integers $u_i$, $v_i$, $l_i$ ($1 \leq u_i, v_i \leq n$, $u_i \neq v_i$, $1 \leq l_i \leq 10^3$)&nbsp;— $1$-based indices of lakes connected by the $i$-th river, and the length of this river.</p><p>The next line contains a single integer $k$ ($1 \leq k \leq 10^5$)&nbsp;— the number of observations.</p><p>The next $k$ lines describe the observations. The $j$-th of these lines contains three integers $d_j$, $f_j$, $p_j$ ($1 \leq d_j \leq 10^8$, $1 \leq f_j \leq 10^4$, $1 \leq p_j \leq n$)&nbsp;— the day, the number of fish, and the lake index of the $j$-th observation. No two observations happen on the same day at the same lake simultaneously.</p>

## Output

<p>Print one integer&nbsp;— the smallest total number of fish not contradicting the observations.</p>





```input1
4
1 2 1
1 3 1
1 4 1
5
1 1 2
1 1 3
2 2 1
3 1 4
3 1 2

```




```input2
5
1 2 1
1 3 1
1 4 1
1 5 1
4
1 1 2
2 1 3
3 1 4
4 1 5

```




```input3
5
2 5 1
5 1 1
2 4 1
5 3 3
6
5 2 4
2 1 1
2 1 3
2 2 4
4 7 5
4 1 2

```




```output1
2

```




```output2
2

```




```output3
10

```



## Note

<p>In the first example, there could be one fish swimming through lakes $2$, $1$, and $4$, and the second fish swimming through lakes $3$, $1$, and $2$.</p><p>In the second example a single fish can not possibly be part of all observations simultaneously, but two fish swimming $2 \to 1 \to 4$ and $3 \to 1 \to 5$ can.</p><p>In the third example one fish can move from lake $1$ to lake $5$, others staying in their lakes during all time: two fish in lake $4$, six fish in lake $5$, one fish in lake $3$. The system of lakes is shown on the picture.</p><center> <img class="tex-graphics" height="129px" src="file://LMnk8PrQ.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center>
