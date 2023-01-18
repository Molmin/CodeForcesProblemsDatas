## Description

<div><p><span class="tex-font-style-it">This problem differs from the next problem only in constraints.</span></p><p>Petya decided to visit Byteland during the summer holidays. It turned out that the history of this country is quite unusual.</p><p>Initially, there were $n$ different countries on the land that is now Berland. Each country had its own territory that was represented as a rectangle on the map. The sides of the rectangle were parallel to the axes, and the corners were located at points with integer coordinates. Territories of no two countries intersected, but it was possible that some territories touched each other. As time passed, sometimes two countries merged into one. It only happened if the union of their territories was also a rectangle. In the end only one country remained&nbsp;— Byteland.</p><p>Initially, each country had a rectangular castle inside its territory. Its sides were parallel to the axes and its corners had integer coordinates. Some castles might touch the border of the corresponding country and sides or other castles. Miraculously, after all the unions the castles are still intact. Unfortunately, their locations are the only information we have to restore the initial territories of the countries.</p><center> <img class="tex-graphics" src="file://qM3sdkQE.png" style="max-width: 100.0%;max-height: 100.0%;"> The possible formation of Byteland. The castles are shown in blue. </center><p>Petya wonders why no information about the initial countries remained. He suspected that the whole story is a fake. You were recommended to him as a smart person. Please check whether or not there exists a possible set of initial territories that could make the story true.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of countries and castles.</p><p>Each of the next $n$ lines contains four integers $a_i, b_i, c_i, d_i$ ($0 \leq a_i &lt; c_i \leq 10^9$, $0 \leq b_i &lt; d_i \leq 10^9$)&nbsp;— the coordinates of the $i$-th castle, where $(a_i, b_i)$ are the coordinates of the lower left corner and $(c_i, d_i)$ are the coordinates of the upper right corner.</p><p>It is guaranteed, that no two castles intersect, however, they may touch.</p></div><div class="output-specification"><p>If there exists a possible set of territories that satisfies the story, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of countries and castles.</p><p>Each of the next $n$ lines contains four integers $a_i, b_i, c_i, d_i$ ($0 \leq a_i &lt; c_i \leq 10^9$, $0 \leq b_i &lt; d_i \leq 10^9$)&nbsp;— the coordinates of the $i$-th castle, where $(a_i, b_i)$ are the coordinates of the lower left corner and $(c_i, d_i)$ are the coordinates of the upper right corner.</p><p>It is guaranteed, that no two castles intersect, however, they may touch.</p>

## Output

<p>If there exists a possible set of territories that satisfies the story, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
0 0 1 2
0 2 1 3
1 0 2 1
1 1 2 3
```




```input2
4
0 0 2 1
1 2 3 3
2 0 3 2
0 1 1 3
```




```output1
YES
```




```output2
NO
```



## Note

<p>The castles in the first and second examples are shown on the pictures below. </p><center> <img class="tex-graphics" height="189px" src="file://GwrR9Trd.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> &nbsp; <img class="tex-graphics" height="189px" src="file://gYlkIISf.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center>
