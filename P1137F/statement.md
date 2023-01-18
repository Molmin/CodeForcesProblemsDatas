## Description

<div><p>Lena is playing with matches. The natural question arising in the head of any child playing with matches is whether it's possible to set a tree on fire with a matches, or not.</p><p>Let's say, that the tree is a connected graph without cycles and the vertices are labeled with integers $1, 2, \ldots, n$. Also every vertex $v$ has some integer priority $p_v$ associated with it. All priorities are distinct.</p><p>It turns out, that if you set a tree on fire, it will burn to nothing. However, this process doesn't happen instantly. At the beginning, burns out the leaf (a vertex is called to be a <span class="tex-font-style-it">leaf</span> if it has only one adjacent vertex) of the tree of the minimum priority. Then burns out the leaf of the minimal priority of the remaining tree, and so on. This way, the vertices turn into the leaves and burn out until only one vertex remains. Then this vertex burns out as well.</p><p>Lena has prepared a tree of $n$ vertices and every vertex in it has a priority $p_v = v$. Lena is very curious about burning out this tree. However, she understands, that if she will burn the tree now, then it will disappear completely. Lena is a kind girl and she will feel bad for the burned tree, so she wants to study the process of burning the tree only in her mind. Lena wants to process $q$ queries, each of them is one of three following types:</p><ul> <li> "<span class="tex-font-style-tt">up</span> $v$", assign the vertex $v$ priority $1 + \max\{p_1, p_2, \ldots, p_n\}$; </li><li> "<span class="tex-font-style-tt">when</span> $v$", find the step at which the vertex $v$ will burn out, if the tree would be set on fire now; </li><li> "<span class="tex-font-style-tt">compare</span> $v$ $u$", find out which of the vertices $v$ and $u$ will burn out first, if the tree would be set on fire now. </li></ul><p>Notice, that if all priorities would be distinct, then after the "<span class="tex-font-style-tt">up</span>" query they will stay distinct as well. Initially all priorities are distinct, hence during any (purely hypothetical of course) burning of the tree, all leafs would have distinct priorities.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \le n \le 200\,000$, $1 \le q \le 200\,000$)&nbsp;— the number of vertices in the tree and the number of queries.</p><p>The $i$-th of the following $n - 1$ lines contains two integers $v_i$, $u_i$ ($1 \le v_i, u_i \le n$), denoting the endpoints of the $i$-th edge.</p><p>Each of the remaining $q$ lines contains a query of one of the following three types:</p><ul> <li> "<span class="tex-font-style-tt">up</span> $v$" ($1 \le v \le n$)&nbsp;— change the priority of vertex $v$; </li><li> "<span class="tex-font-style-tt">when</span> $v$" ($1 \le v \le n$)&nbsp;— determine the step at which the vertex $v$ will burn out; </li><li> "<span class="tex-font-style-tt">compare</span> $v$ $u$" ($1 \le v, u \le n$, $v \ne u$)&nbsp;— determine which of vertices $v$ and $u$ will burn out earlier in the current tree. </li></ul><p>It's guaranteed, that there is at least one query of type "<span class="tex-font-style-tt">when</span>" or "<span class="tex-font-style-tt">compare</span>".</p></div><div class="output-specification"><p>For every query of type "<span class="tex-font-style-tt">when</span>" print one integer in range from $1$ to $n$&nbsp;— the step at which the vertex $v$ will burn out.</p><p>For every query of type "<span class="tex-font-style-tt">compare</span>" print either $v$ or $u$, depending on which one will burn out earlier.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \le n \le 200\,000$, $1 \le q \le 200\,000$)&nbsp;— the number of vertices in the tree and the number of queries.</p><p>The $i$-th of the following $n - 1$ lines contains two integers $v_i$, $u_i$ ($1 \le v_i, u_i \le n$), denoting the endpoints of the $i$-th edge.</p><p>Each of the remaining $q$ lines contains a query of one of the following three types:</p><ul> <li> "<span class="tex-font-style-tt">up</span> $v$" ($1 \le v \le n$)&nbsp;— change the priority of vertex $v$; </li><li> "<span class="tex-font-style-tt">when</span> $v$" ($1 \le v \le n$)&nbsp;— determine the step at which the vertex $v$ will burn out; </li><li> "<span class="tex-font-style-tt">compare</span> $v$ $u$" ($1 \le v, u \le n$, $v \ne u$)&nbsp;— determine which of vertices $v$ and $u$ will burn out earlier in the current tree. </li></ul><p>It's guaranteed, that there is at least one query of type "<span class="tex-font-style-tt">when</span>" or "<span class="tex-font-style-tt">compare</span>".</p>

## Output

<p>For every query of type "<span class="tex-font-style-tt">when</span>" print one integer in range from $1$ to $n$&nbsp;— the step at which the vertex $v$ will burn out.</p><p>For every query of type "<span class="tex-font-style-tt">compare</span>" print either $v$ or $u$, depending on which one will burn out earlier.</p>





```input1
5 7
1 5
1 2
1 3
4 3
when 1
when 2
when 3
when 4
when 5
compare 2 3
compare 3 4
```




```input2
5 5
1 5
1 2
1 3
4 3
up 1
compare 2 4
compare 4 3
compare 3 1
compare 1 5
```




```output1
4
1
3
2
5
2
4
```




```output2
2
4
3
5
```



## Note

<p>In the first example, the process of burning of the tree is illustrated on the following picture:</p><center> <img class="tex-graphics" src="file://5g0bHH4i.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In particular, the vertices of the tree will burn out in the following order: $[2, 4, 3, 1, 5]$.</p><p>In the second example, after applying the "<span class="tex-font-style-tt">up</span>" operation, the order of vertices will change to: $[2, 4, 3, 5, 1]$.</p>
