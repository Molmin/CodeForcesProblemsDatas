## Description

<div><p>Josuke received a huge undirected weighted complete$^\dagger$ graph $G$ as a gift from his grandfather. The graph contains $10^{18}$ vertices. The peculiarity of the gift is that the weight of the edge between the different vertices $u$ and $v$ is equal to $\gcd(u, v)^\ddagger$. Josuke decided to experiment and make a new graph $G'$. To do this, he chooses two integers $l \le r$ and deletes all vertices except such vertices $v$ that $l \le v \le r$, and also deletes all the edges except between the remaining vertices.</p><p>Now Josuke is wondering how many different weights are there in $G'$. Since their count turned out to be huge, he asks for your help.</p><p>$^\dagger$ A complete graph is a simple undirected graph in which every pair of distinct vertices is adjacent.</p><p>$^\ddagger$ $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of the numbers $x$ and $y$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The first line of each test case contains two numbers $l$, $r$ ($1 \le l \le r \le 10^{18}$, $l \le 10^9$).</p></div><div class="output-specification"><p>For each test case print a single number — the number of different weights among the remaining edges.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The first line of each test case contains two numbers $l$, $r$ ($1 \le l \le r \le 10^{18}$, $l \le 10^9$).</p>

## Output

<p>For each test case print a single number — the number of different weights among the remaining edges.</p>





```input1|2,4,6,8
7
2 4
16 24
2 6
1 10
3 3
2562 2568
125 100090
```




```output1
2
6
3
5
0
5
50045
```



## Note

<center> <img class="tex-graphics" src="file://3YgNMRW3.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The graph $G'$ for the first test case.</span> </center><p>The picture above shows that the graph has $2$ different weights.</p><p>In the fifth test case, there is only one vertex from which no edges originate, so the answer is $0$.</p>
