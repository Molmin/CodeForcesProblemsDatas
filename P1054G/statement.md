## Description

<div><p>The king of some country $N$ decided to completely rebuild the road network. There are $n$ people living in the country, they are enumerated from $1$ to $n$. It is possible to construct a road between the house of any citizen $a$ to the house of any other citizen $b$. There should not be more than one road between any pair of citizens. The road network must be connected, i.e. it should be possible to reach every citizen starting from anyone using roads. To save funds, it was decided to build exactly $n-1$ road, so the road network should be a tree.</p><p>However, it is not that easy as it sounds, that's why the king addressed you for help. There are $m$ secret communities in the country, each of them unites a non-empty subset of citizens. The king does not want to conflict with any of the communities, so he wants to build the network such that the houses of members of each society form a connected subtree in network. A set of vertices forms a connected subtree if and only if the graph remains connected when we delete all the other vertices and all edges but ones that connect the vertices from the set.</p><p>Help the king to determine if it is possible to build the desired road network, and if it is, build it.</p></div><div class="input-specification"><p>Each test consists of one or more test cases.</p><p>The first line contains a single integer $t$ ($1 \leq t \leq 2000$) — the number of test cases.</p><p>The following lines describe the test cases, each in the following format.</p><p>The first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 2000$) — the number of citizens and the number of secret communities. </p><p>The next $m$ lines contain the description of the communities. The $i$-th of these lines contains a string $s_i$ of length $n$, consisting of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The citizen with number $j$ is a member of the $i$-th community if and only if $s_{{i}{j}}=1$. It is guaranteed that the string $s_i$ contains at least one character '<span class="tex-font-style-tt">1</span>' for each $1 \leq i \leq m$.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2000$ and the sum of $m$ for all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>Print the answer for all test cases in the order they are given in the input, each in the following format.</p><p>If there is no way to build the desired road network, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes).</p><p>In the next $n-1$ lines print the description of the road network: each line should contain two integers $a$ and $b$ ($1 \leq a, b \leq n$, $a \neq b$) that denote you build a road between houses of citizens $a$ and $b$. </p><p>The roads should form a connected tree, and each community should form a connected subtree.</p></div>

## Input

<p>Each test consists of one or more test cases.</p><p>The first line contains a single integer $t$ ($1 \leq t \leq 2000$) — the number of test cases.</p><p>The following lines describe the test cases, each in the following format.</p><p>The first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 2000$) — the number of citizens and the number of secret communities. </p><p>The next $m$ lines contain the description of the communities. The $i$-th of these lines contains a string $s_i$ of length $n$, consisting of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The citizen with number $j$ is a member of the $i$-th community if and only if $s_{{i}{j}}=1$. It is guaranteed that the string $s_i$ contains at least one character '<span class="tex-font-style-tt">1</span>' for each $1 \leq i \leq m$.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2000$ and the sum of $m$ for all test cases does not exceed $2000$.</p>

## Output

<p>Print the answer for all test cases in the order they are given in the input, each in the following format.</p><p>If there is no way to build the desired road network, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes).</p><p>In the next $n-1$ lines print the description of the road network: each line should contain two integers $a$ and $b$ ($1 \leq a, b \leq n$, $a \neq b$) that denote you build a road between houses of citizens $a$ and $b$. </p><p>The roads should form a connected tree, and each community should form a connected subtree.</p>





```input1
2
4 3
0011
1110
0111
3 3
011
101
110

```




```output1
YES
1 3
2 3
3 4
NO

```



## Note

<p>In the first example you can build the following network:</p><center> <img class="tex-graphics" src="file://m5wUVcSf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It is easy to see that for each community all the houses of its members form a connected subtree. For example, the $2$-nd community unites the citizens $1$, $2$, $3$. They form a connected subtree, because if we delete everything except the houses $1$, $2$, $3$ and the roads between them, two roads will remain: between $1$ and $3$ and between $2$ and $3$, forming a connected graph.</p><p>There is no network in the second example suitable for the king.</p>
