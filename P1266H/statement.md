## Description

<div><p>There is a directed graph on $n$ vertices numbered $1$ through $n$ where each vertex (except $n$) has two outgoing arcs, red and blue. At any point in time, exactly one of the arcs is <span class="tex-font-style-it">active</span> for each vertex. Initially, all blue arcs are active and there is a token located at vertex $1$. In one second, the vertex with token first switches its active arcs — the inactive arc becomes active and vice versa. Then, the token is moved along the active arc. When the token reaches the vertex $n$, it stops. It is guaranteed that $n$ is reachable via arcs from every vertex.</p><p>You are given $q$ queries. Each query contains a state of the graph — a pair $(v, s)$ of the following form: </p><ul> <li> $v$ is the vertex where the token is currently located; </li><li> $s$ is a string consisting of $n - 1$ characters. The $i$-th character corresponds to the color of the active edge leading from the $i$-th vertex (the character is '<span class="tex-font-style-tt">R</span>' if red arc is active, otherwise the character is '<span class="tex-font-style-tt">B</span>'). </li></ul><p>For each query, determine whether the given state is reachable from the initial state and the first time this configuration appears. Note that the two operations (change active arc and traverse it) are atomic — a state is not considered reached if it appears after changing the active arc but before traversing it.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 58$)&nbsp;— the number of vertices.</p><p>$n-1$ lines follow, $i$-th of contains two space separated integers $b_i$ and $r_i$ ($1 \leq b_i, r_i \leq n$) representing a blue arc $(i, b_i)$ and red arc $(i, r_i)$, respectively. It is guaranteed that vertex $n$ is reachable from every vertex.</p><p>The next line contains a single integer $q$ ($1 \leq q \leq 5000$)&nbsp;— the number of queries.</p><p>Then $q$ lines with queries follow. The $j$-th of these lines contains an integer $v$ ($1 \leq v &lt; n$) and a string $s$ of length $n-1$ consiting only of characters '<span class="tex-font-style-tt">R</span>' and '<span class="tex-font-style-tt">B</span>'. The $i$-th of these characters is '<span class="tex-font-style-tt">R</span>' if the red arc going from $i$ is active and '<span class="tex-font-style-tt">B</span>' otherwise.</p></div><div class="output-specification"><p>Output $q$ lines, each containing answer to a single query.</p><p>If the state in the $i$-th query is unreachable, output the integer $-1$. Otherwise, output $t_i$ — the first time when the state appears (measured in seconds, starting from the initial state of the graph which appears in time $0$).</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 58$)&nbsp;— the number of vertices.</p><p>$n-1$ lines follow, $i$-th of contains two space separated integers $b_i$ and $r_i$ ($1 \leq b_i, r_i \leq n$) representing a blue arc $(i, b_i)$ and red arc $(i, r_i)$, respectively. It is guaranteed that vertex $n$ is reachable from every vertex.</p><p>The next line contains a single integer $q$ ($1 \leq q \leq 5000$)&nbsp;— the number of queries.</p><p>Then $q$ lines with queries follow. The $j$-th of these lines contains an integer $v$ ($1 \leq v &lt; n$) and a string $s$ of length $n-1$ consiting only of characters '<span class="tex-font-style-tt">R</span>' and '<span class="tex-font-style-tt">B</span>'. The $i$-th of these characters is '<span class="tex-font-style-tt">R</span>' if the red arc going from $i$ is active and '<span class="tex-font-style-tt">B</span>' otherwise.</p>

## Output

<p>Output $q$ lines, each containing answer to a single query.</p><p>If the state in the $i$-th query is unreachable, output the integer $-1$. Otherwise, output $t_i$ — the first time when the state appears (measured in seconds, starting from the initial state of the graph which appears in time $0$).</p>





```input1
6
2 1
5 5
2 1
6 3
4 3
21
1 BBBBB
1 RBBBB
2 BBBBB
5 BRBBB
3 BRBBR
1 BRRBR
1 RRRBR
2 BRRBR
5 BBRBR
4 BBRBB
3 BBRRB
2 BBBRB
5 BRBRB
3 BRBRR
1 BRRRR
1 RRRRR
2 BRRRR
5 BBRRR
4 BBRRB
2 BRBBB
4 BRBBR
```




```output1
0
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
-1
-1
```



## Note

<p>The graph in the first example is depticed in the figure below.</p><p><img class="tex-graphics" src="file://XRO5cQFR.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The first $19$ queries denote the journey of the token. On the $19$-th move the token would reach the vertex $6$. The last two queries show states that are unreachable.</p>
