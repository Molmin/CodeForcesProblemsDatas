## Description

<div><p>You are given $N$ points on an infinite plane with the Cartesian coordinate system on it. $N-1$ points lay on one line, and one point isn't on that line. You are on point $K$ at the start, and the goal is to visit every point. You can move between any two points in a straight line, and you can revisit points. What is the minimum length of the path? </p></div><div class="input-specification"><p>The first line contains two integers: $N$ ($3 \leq N \leq 2*10^5$) - the number of points, and $K$ ($1 \leq K \leq N$) - the index of the starting point.</p><p>Each of the next $N$ lines contain two integers, $A_i$, $B_i$ ($-10^6 \leq A_i, B_i \leq 10^6$) - coordinates of the $i-th$ point.</p></div><div class="output-specification"><p>The output contains one number - the shortest path to visit all given points starting from point $K$. The absolute difference between your solution and the main solution shouldn't exceed $10^-6$;</p></div>

## Input

<p>The first line contains two integers: $N$ ($3 \leq N \leq 2*10^5$) - the number of points, and $K$ ($1 \leq K \leq N$) - the index of the starting point.</p><p>Each of the next $N$ lines contain two integers, $A_i$, $B_i$ ($-10^6 \leq A_i, B_i \leq 10^6$) - coordinates of the $i-th$ point.</p>

## Output

<p>The output contains one number - the shortest path to visit all given points starting from point $K$. The absolute difference between your solution and the main solution shouldn't exceed $10^-6$;</p>





```input1
5 2
0 0
-1 1
2 -2
0 1
-2 2
```




```output1
7.478709
```



## Note

<p>The shortest path consists of these moves: </p><p>2 -&gt; 5 </p><p>5 -&gt; 4 </p><p>4 -&gt; 1 </p><p>1 -&gt; 3 </p><p>There isn't any shorter path possible.</p>
