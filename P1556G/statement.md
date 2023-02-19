## Description

<div><center> <img class="tex-graphics" height="302px" src="file://NbI1xmiU.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>As mentioned previously William really likes playing video games. In one of his favorite games, the player character is in a universe where every planet is designated by a binary number from $0$ to $2^n - 1$. On each planet, there are gates that allow the player to move from planet $i$ to planet $j$ if the binary representations of $i$ and $j$ differ in exactly one bit.</p><p>William wants to test you and see how you can handle processing the following queries in this game universe:</p><ul> <li> Destroy planets with numbers from $l$ to $r$ inclusively. These planets cannot be moved to anymore.</li><li> Figure out if it is possible to reach planet $b$ from planet $a$ using some number of planetary gates. It is guaranteed that the planets $a$ and $b$ are not destroyed. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$, $m$ ($1 \leq n \leq 50$, $1 \leq m \leq 5 \cdot 10^4$), which are the number of bits in binary representation of each planets' designation and the number of queries, respectively.</p><p>Each of the next $m$ lines contains a query of two types:</p><p><span class="tex-font-style-tt">block l r</span>&nbsp;— query for destruction of planets with numbers from $l$ to $r$ inclusively ($0 \le l \le r &lt; 2^n$). It's guaranteed that no planet will be destroyed twice.</p><p><span class="tex-font-style-tt">ask a b</span>&nbsp;— query for reachability between planets $a$ and $b$ ($0 \le a, b &lt; 2^n$). It's guaranteed that planets $a$ and $b$ hasn't been destroyed yet.</p></div><div class="output-specification"><p>For each query of type <span class="tex-font-style-tt">ask</span> you must output "<span class="tex-font-style-tt">1</span>" in a new line, if it is possible to reach planet $b$ from planet $a$ and "<span class="tex-font-style-tt">0</span>" otherwise (without quotation marks).</p></div>

## Input

<p>The first line contains two integers $n$, $m$ ($1 \leq n \leq 50$, $1 \leq m \leq 5 \cdot 10^4$), which are the number of bits in binary representation of each planets' designation and the number of queries, respectively.</p><p>Each of the next $m$ lines contains a query of two types:</p><p><span class="tex-font-style-tt">block l r</span>&nbsp;— query for destruction of planets with numbers from $l$ to $r$ inclusively ($0 \le l \le r &lt; 2^n$). It's guaranteed that no planet will be destroyed twice.</p><p><span class="tex-font-style-tt">ask a b</span>&nbsp;— query for reachability between planets $a$ and $b$ ($0 \le a, b &lt; 2^n$). It's guaranteed that planets $a$ and $b$ hasn't been destroyed yet.</p>

## Output

<p>For each query of type <span class="tex-font-style-tt">ask</span> you must output "<span class="tex-font-style-tt">1</span>" in a new line, if it is possible to reach planet $b$ from planet $a$ and "<span class="tex-font-style-tt">0</span>" otherwise (without quotation marks).</p>





```input1
3 3
ask 0 7
block 3 6
ask 0 7
```




```input2
6 10
block 12 26
ask 44 63
block 32 46
ask 1 54
block 27 30
ask 10 31
ask 11 31
ask 49 31
block 31 31
ask 2 51
```




```output1
1
0
```




```output2
1
1
0
0
1
0
```



## Note

<p>The first example test can be visualized in the following way:</p><center> <img class="tex-graphics" height="302px" src="file://7tyhK70q.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>Response to a query <span class="tex-font-style-tt">ask 0 7</span> is positive.</p><p>Next after query <span class="tex-font-style-tt">block 3 6</span> the graph will look the following way (destroyed vertices are highlighted):</p><center> <img class="tex-graphics" height="302px" src="file://qt8WV3z8.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>Response to a query <span class="tex-font-style-tt">ask 0 7</span> is negative, since any path from vertex $0$ to vertex $7$ must go through one of the destroyed vertices.</p>
