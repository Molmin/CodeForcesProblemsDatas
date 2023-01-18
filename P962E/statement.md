## Description

<div><p>The cities of Byteland and Berland are located on the axis $Ox$. In addition, on this axis there are also disputed cities, which belong to each of the countries in their opinion. Thus, on the line $Ox$ there are three types of cities:</p><ul> <li> the cities of Byteland, </li><li> the cities of Berland, </li><li> disputed cities. </li></ul><p>Recently, the project BNET has been launched — a computer network of a new generation. Now the task of the both countries is to connect the cities so that the network of this country is <span class="tex-font-style-it">connected</span>.</p><p>The countries agreed to connect <span class="tex-font-style-it">the pairs</span> of cities with BNET cables in such a way that:</p><ul> <li> If you look at the <span class="tex-font-style-it">only</span> cities of Byteland and the disputed cities, then in the resulting set of cities, any city should be reachable from any other one by one or more cables, </li><li> If you look at the <span class="tex-font-style-it">only</span> cities of Berland and the disputed cities, then in the resulting set of cities, any city should be reachable from any other one by one or more cables. </li></ul><p>Thus, it is necessary to choose a set of pairs of cities to connect by cables in such a way that both conditions are satisfied simultaneously. Cables allow bi-directional data transfer. Each cable connects exactly two distinct cities.</p><p>The cost of laying a cable from one city to another is equal to the distance between them. Find the minimum total cost of laying a set of cables so that two subsets of cities (Byteland and disputed cities, Berland and disputed cities) are connected.</p><p>Each city is a point on the line $Ox$. It is technically possible to connect the cities $a$ and $b$ with a cable so that the city $c$ ($a &lt; c &lt; b$) is not connected to this cable, where $a$, $b$ and $c$ are simultaneously coordinates of the cities $a$, $b$ and $c$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^{5}$) — the number of cities.</p><p>The following $n$ lines contains an integer $x_i$ and the letter $c_i$ ($-10^{9} \le x_i \le 10^{9}$) — the coordinate of the city and its type. If the city belongs to Byteland, $c_i$ equals to '<span class="tex-font-style-tt">B</span>'. If the city belongs to Berland, $c_i$ equals to «<span class="tex-font-style-tt">R</span>». If the city is disputed, $c_i$ equals to '<span class="tex-font-style-tt">P</span>'. </p><p>All cities have distinct coordinates. Guaranteed, that the cities are given in the increasing order of their coordinates.</p></div><div class="output-specification"><p>Print the minimal total length of such set of cables, that if we delete all Berland cities ($c_i$='<span class="tex-font-style-tt">R</span>'), it will be possible to find a way from any remaining city to any other remaining city, moving only by cables. Similarly, if we delete all Byteland cities ($c_i$='<span class="tex-font-style-tt">B</span>'), it will be possible to find a way from any remaining city to any other remaining city, moving only by cables.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^{5}$) — the number of cities.</p><p>The following $n$ lines contains an integer $x_i$ and the letter $c_i$ ($-10^{9} \le x_i \le 10^{9}$) — the coordinate of the city and its type. If the city belongs to Byteland, $c_i$ equals to '<span class="tex-font-style-tt">B</span>'. If the city belongs to Berland, $c_i$ equals to «<span class="tex-font-style-tt">R</span>». If the city is disputed, $c_i$ equals to '<span class="tex-font-style-tt">P</span>'. </p><p>All cities have distinct coordinates. Guaranteed, that the cities are given in the increasing order of their coordinates.</p>

## Output

<p>Print the minimal total length of such set of cables, that if we delete all Berland cities ($c_i$='<span class="tex-font-style-tt">R</span>'), it will be possible to find a way from any remaining city to any other remaining city, moving only by cables. Similarly, if we delete all Byteland cities ($c_i$='<span class="tex-font-style-tt">B</span>'), it will be possible to find a way from any remaining city to any other remaining city, moving only by cables.</p>





```input1
4
-5 R
0 P
3 P
7 B

```




```input2
5
10 R
14 B
16 B
21 R
32 R

```




```output1
12

```




```output2
24

```



## Note

<p>In the first example, you should connect the first city with the second, the second with the third, and the third with the fourth. The total length of the cables will be $5 + 3 + 4 = 12$.</p><p>In the second example there are no disputed cities, so you need to connect all the neighboring cities of Byteland and all the neighboring cities of Berland. The cities of Berland have coordinates $10, 21, 32$, so to connect them you need two cables of length $11$ and $11$. The cities of Byteland have coordinates $14$ and $16$, so to connect them you need one cable of length $2$. Thus, the total length of all cables is $11 + 11 + 2 = 24$.</p>
