## Description

<div><p><span class="tex-font-style-it">Lee tried so hard to make a good div.2 D problem to balance his recent contest, but it still doesn't feel good at all. Lee invented it so tediously slow that he managed to develop a phobia about div.2 D problem setting instead. And now he is hiding behind the bushes...</span></p><p>Let's define a <span class="tex-font-style-it">Rooted Dead Bush</span> (RDB) of level $n$ as a rooted tree constructed as described below.</p><p>A rooted dead bush of level $1$ is a single vertex. To construct an RDB of level $i$ we, at first, construct an RDB of level $i-1$, then for each vertex $u$: </p><ul> <li> if $u$ has no children then we will add a single child to it; </li><li> if $u$ has one child then we will add two children to it; </li><li> if $u$ has more than one child, then we will skip it. </li></ul><center> <img class="tex-graphics" src="file://UrfEOyIc.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Rooted Dead Bushes of level $1$, $2$ and $3$.</span> </center><p>Let's define a <span class="tex-font-style-it">claw</span> as a rooted tree with four vertices: one root vertex (called also as center) with three children. It looks like a claw:</p><center> <img class="tex-graphics" src="file://InIerWkZ.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The center of the claw is the vertex with label $1$.</span> </center><p>Lee has a Rooted Dead Bush of level $n$. Initially, all vertices of his RDB are green.</p><p>In one move, he can choose a claw in his RDB, if all vertices in the claw are <span class="tex-font-style-it">green</span> and all vertices of the claw are children of its center, then he colors the claw's vertices in yellow.</p><p>He'd like to know the maximum number of yellow vertices he can achieve. Since the answer might be very large, print it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;— one per line.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^6$)&nbsp;— the level of Lee's RDB.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the maximum number of yellow vertices Lee can make modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;— one per line.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^6$)&nbsp;— the level of Lee's RDB.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the maximum number of yellow vertices Lee can make modulo $10^9 + 7$.</p>





```input1
7
1
2
3
4
5
100
2000000
```




```output1
0
0
4
4
12
990998587
804665184
```



## Note

<p>It's easy to see that the answer for RDB of level $1$ or $2$ is $0$.</p><p>The answer for RDB of level $3$ is $4$ since there is only one claw we can choose: $\{1, 2, 3, 4\}$.</p><p>The answer for RDB of level $4$ is $4$ since we can choose either single claw $\{1, 3, 2, 4\}$ or single claw $\{2, 7, 5, 6\}$. There are no other claws in the RDB of level $4$ (for example, we can't choose $\{2, 1, 7, 6\}$, since $1$ is not a child of center vertex $2$).</p><center> <img class="tex-graphics" src="file://TiMrqOpY.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Rooted Dead Bush of level 4.</span> </center>
