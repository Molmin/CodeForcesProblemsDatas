## Description

<div><p>ChthollyNotaSeniorious gives DataStructures a number axis with $m$ distinct segments on it. Let $f(l,r)$ be the number of ways to choose an even number of segments such that the union of them is exactly $[l,r]$, and $g(l,r)$ be the number of ways to choose an odd number of segments such that the union of them is exactly $[l,r]$.</p><p>ChthollyNotaSeniorious asked DataStructures $q$ questions. In each query, ChthollyNotaSeniorious will give DataStructures two numbers $l, r$, and now he wishes that you can help him find the value $f(l,r)-g(l,r)$ modulo $998\,244\,353$ so that he wouldn't let her down. </p></div><div class="input-specification"><p>The first line of input contains two integers $m$ ($1 \leq m \leq 2 \cdot 10^5$) and $q$ ($1 \leq q \leq 2 \cdot 10^5$) &nbsp;— the number of segments and queries, correspondingly.</p><p>The $i$-th of the next $m$ lines contains two integers $x_i$ and $y_i$ ($1 \leq x_i &lt; y_i \leq 10^9$), denoting a segment $[x_i, y_i]$. </p><p><span class="tex-font-style-bf">It is guaranteed that all segments are distinct.</span> More formally, there do not exist two numbers $i, j$ with $1 \le i &lt; j \le m$ such that $x_i = x_j$ and $y_i = y_j$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i$ and $r_i$ ($1 \leq l_i &lt; r_i \leq 10^9$), describing a query.</p></div><div class="output-specification"><p>For each query, output a single integer &nbsp;— $f(l_i,r_i)-g(l_i,r_i)$ modulo $998\,244\,353$.</p></div>

## Input

<p>The first line of input contains two integers $m$ ($1 \leq m \leq 2 \cdot 10^5$) and $q$ ($1 \leq q \leq 2 \cdot 10^5$) &nbsp;— the number of segments and queries, correspondingly.</p><p>The $i$-th of the next $m$ lines contains two integers $x_i$ and $y_i$ ($1 \leq x_i &lt; y_i \leq 10^9$), denoting a segment $[x_i, y_i]$. </p><p><span class="tex-font-style-bf">It is guaranteed that all segments are distinct.</span> More formally, there do not exist two numbers $i, j$ with $1 \le i &lt; j \le m$ such that $x_i = x_j$ and $y_i = y_j$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i$ and $r_i$ ($1 \leq l_i &lt; r_i \leq 10^9$), describing a query.</p>

## Output

<p>For each query, output a single integer &nbsp;— $f(l_i,r_i)-g(l_i,r_i)$ modulo $998\,244\,353$.</p>





```input1
4 2
1 3
4 6
2 4
3 5
1 4
1 5
```




```output1
1
0
```



## Note

<p>In the first query, we have to find $f(1, 4) - g(1, 4)$. The only subset of segments with union $[1, 4]$ is $\{[1, 3], [2, 4]\}$, so $f(1, 4) = 1, g(1, 4) = 0$.</p><p>In the second query, we have to find $f(1, 5) - g(1, 5)$. The only subsets of segments with union $[1, 5]$ are $\{[1, 3], [2, 4], [3, 5]\}$ and $\{[1, 3], [3, 5]\}$, so $f(1, 5) = 1, g(1, 5) = 1$.</p>
