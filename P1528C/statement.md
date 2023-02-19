## Description

<div><p>Soroush and Keshi each have a labeled and rooted tree on $n$ vertices. Both of their trees are rooted from vertex $1$.</p><p>Soroush and Keshi used to be at war. After endless decades of fighting, they finally became allies to prepare a Codeforces round. To celebrate this fortunate event, they decided to make a memorial graph on $n$ vertices.</p><p>They add an edge between vertices $u$ and $v$ in the memorial graph if <span class="tex-font-style-bf">both</span> of the following conditions hold: </p><ul> <li> One of $u$ or $v$ is the ancestor of the other in Soroush's tree. </li><li> Neither of $u$ or $v$ is the ancestor of the other in Keshi's tree. </li></ul><p>Here vertex $u$ is considered ancestor of vertex $v$, if $u$ lies on the path from $1$ (the root) to the $v$.</p><p>Popping out of nowhere, Mashtali tried to find the maximum clique in the memorial graph for no reason. He failed because the graph was too big. </p><p>Help Mashtali by finding the size of the maximum clique in the memorial graph.</p><p>As a reminder, clique is a subset of vertices of the graph, each two of which are connected by an edge.</p></div><div class="input-specification"><p>The first line contains an integer $t$ $(1\le t\le 3 \cdot 10^5)$ — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ $(2\le n\le 3 \cdot 10^5)$.</p><p>The second line of each test case contains $n-1$ integers $a_2, \ldots, a_n$ $(1 \le a_i &lt; i)$, $a_i$ being the parent of the vertex $i$ in Soroush's tree.</p><p>The third line of each test case contains $n-1$ integers $b_2, \ldots, b_n$ $(1 \le b_i &lt; i)$, $b_i$ being the parent of the vertex $i$ in Keshi's tree.</p><p>It is guaranteed that the given graphs are trees.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer — the <span class="tex-font-style-bf">size</span> of the maximum clique in the memorial graph.</p></div>

## Input

<p>The first line contains an integer $t$ $(1\le t\le 3 \cdot 10^5)$ — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ $(2\le n\le 3 \cdot 10^5)$.</p><p>The second line of each test case contains $n-1$ integers $a_2, \ldots, a_n$ $(1 \le a_i &lt; i)$, $a_i$ being the parent of the vertex $i$ in Soroush's tree.</p><p>The third line of each test case contains $n-1$ integers $b_2, \ldots, b_n$ $(1 \le b_i &lt; i)$, $b_i$ being the parent of the vertex $i$ in Keshi's tree.</p><p>It is guaranteed that the given graphs are trees.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case print a single integer — the <span class="tex-font-style-bf">size</span> of the maximum clique in the memorial graph.</p>





```input1
4
4
1 2 3
1 2 3
5
1 2 3 4
1 1 1 1
6
1 1 1 1 2
1 2 1 2 2
7
1 1 3 4 4 5
1 2 1 4 2 5
```




```output1
1
4
1
3
```



## Note

<p>In the first and third test cases, you can pick any vertex.</p><p>In the second test case, one of the maximum cliques is $\{2, 3, 4, 5\}$.</p><p>In the fourth test case, one of the maximum cliques is $\{3, 4, 6\}$.</p>
