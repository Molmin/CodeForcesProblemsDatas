## Description

<div><div class="epigraph"><div class="epigraph-text">I'm the Map, I'm the Map! I'm the MAP!!!</div><div class="epigraph-source">Map</div></div><p>In anticipation of new adventures Boots wanted to do a good deed. After discussion with the Map and Backpack, they decided to gift Dora a connected graph. After a long search, Boots chose $t$ graph's variants, which Dora might like. However fox Swiper wants to spoil his plan.</p><p>The Swiper knows, that Dora now is only able to count up to $3$, so he has came up with a following idea. He wants to steal some non-empty set of vertices, so that the Dora won't notice the loss. He has decided to steal some non-empty set of vertices, so that after deletion of the stolen vertices and edges adjacent to them, every <span class="tex-font-style-bf">remaining</span> vertex wouldn't change it's degree modulo $3$. The degree of a vertex is the number of edges it is adjacent to. It would've been suspicious to steal all the vertices, so Swiper needs another plan.</p><p>Boots are sure, that the crime can not be allowed. However they are afraid, that they won't be able to handle this alone. So Boots decided to ask for your help. Please determine for every graph's variant whether the Swiper can perform the theft or not.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100\,000$) — the number of graph variants.</p><p>The first line of each variant contains integers $n$, $m$ ($1 \le n \le 500\,000$, $0 \le m \le 500\,000$), the number of vertexes and edges in the graph.</p><p>Then $m$ lines follow, each containing integers $a_i$, $b_i$ ($1 \le a_i, b_i \le n$), the indices of the vertices connected with a corresponding edge.</p><p>It's guaranteed, that the graph is connected and doesn't contain multiple edges or self-loops.</p><p>It's guaranteed, that the sum of $n$ over all variants is at most $500\,000$ and that the sum of $m$ over all variants is at most $500\,000$.</p><p>Descriptions of graph's variants are separated with an empty line.</p></div><div class="output-specification"><p>For each variant:</p><ul> <li> In case the answer exists, print "<span class="tex-font-style-tt">Yes</span>" and then the answer itself.<p>The first line should contain an integer $c$ ($1 &lt; c &lt; n$), the number of vertices the Crook can steal, without Dora noticing the loss. On the next line print $c$ distinct integers, the indices of the graph's vertices in arbitrary order.</p></li><li> Otherwise print "<span class="tex-font-style-tt">No</span>". </li></ul><p>In case there are several correct ways to steal the vertices, print any of them.</p><p>Please note, that it's not required to maximize the number of stolen vertices.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100\,000$) — the number of graph variants.</p><p>The first line of each variant contains integers $n$, $m$ ($1 \le n \le 500\,000$, $0 \le m \le 500\,000$), the number of vertexes and edges in the graph.</p><p>Then $m$ lines follow, each containing integers $a_i$, $b_i$ ($1 \le a_i, b_i \le n$), the indices of the vertices connected with a corresponding edge.</p><p>It's guaranteed, that the graph is connected and doesn't contain multiple edges or self-loops.</p><p>It's guaranteed, that the sum of $n$ over all variants is at most $500\,000$ and that the sum of $m$ over all variants is at most $500\,000$.</p><p>Descriptions of graph's variants are separated with an empty line.</p>

## Output

<p>For each variant:</p><ul> <li> In case the answer exists, print "<span class="tex-font-style-tt">Yes</span>" and then the answer itself.<p>The first line should contain an integer $c$ ($1 &lt; c &lt; n$), the number of vertices the Crook can steal, without Dora noticing the loss. On the next line print $c$ distinct integers, the indices of the graph's vertices in arbitrary order.</p></li><li> Otherwise print "<span class="tex-font-style-tt">No</span>". </li></ul><p>In case there are several correct ways to steal the vertices, print any of them.</p><p>Please note, that it's not required to maximize the number of stolen vertices.</p>





```input1
3
3 3
1 2
2 3
3 1

6 6
1 2
1 3
2 3
2 5
2 6
2 4

8 12
1 2
1 3
2 3
1 4
4 5
5 1
3 6
3 7
3 8
6 1
7 1
8 1
```




```output1
No
Yes
3
4 5 6
Yes
3
6 7 8
```



## Note

<p>The picture below shows the third variant from the example test. The set of the vertices the Crook can steal is denoted with bold. </p><center> <img class="tex-graphics" height="340px" src="file://uT1F4Ov3.png" style="max-width: 100.0%;max-height: 100.0%;" width="340px"> </center>
