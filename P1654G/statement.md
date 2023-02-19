## Description

<div><p>There are $n$ locations on a snowy mountain range (numbered from $1$ to $n$), connected by $n-1$ trails in the shape of a tree. Each trail has length $1$. Some of the locations are base lodges. The height $h_i$ of each location is equal to the distance to the nearest base lodge (a base lodge has height $0$).</p><p>There is a skier at each location, each skier has initial kinetic energy $0$. Each skier wants to ski along as many trails as possible. Suppose that the skier is skiing along a trail from location $i$ to $j$. Skiers are not allowed to ski uphill (i.e., if $h_i &lt; h_j$). It costs one unit of kinetic energy to ski along flat ground (i.e., if $h_i = h_j$), and a skier gains one unit of kinetic energy by skiing downhill (i.e., if $h_i &gt; h_j$). For each location, compute the length of the longest sequence of trails that the skier starting at that location can ski along without their kinetic energy ever becoming negative. Skiers are allowed to visit the same location or trail multiple times.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $l_1, l_2, \ldots, l_n$ ($0 \le l_i \le 1$). If $l_i = 1$, location $i$ is a base lodge; if $l_i = 0$, location $i$ is not a base lodge. It is guaranteed that there is at least $1$ base lodge.</p><p>Each of the next $n-1$ lines contains two integers $u, v$ ($1 \leq u, v \leq n$, $u \neq v$), meaning that there is a trail that connects the locations $u$ and $v$. It is guaranteed that the given trails form a tree.</p></div><div class="output-specification"><p>Print $n$ integers: the $i$-th integer is equal to the length of the longest sequence of trails that the skier starting at location $i$ can ski along without their kinetic energy ever becoming negative.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $l_1, l_2, \ldots, l_n$ ($0 \le l_i \le 1$). If $l_i = 1$, location $i$ is a base lodge; if $l_i = 0$, location $i$ is not a base lodge. It is guaranteed that there is at least $1$ base lodge.</p><p>Each of the next $n-1$ lines contains two integers $u, v$ ($1 \leq u, v \leq n$, $u \neq v$), meaning that there is a trail that connects the locations $u$ and $v$. It is guaranteed that the given trails form a tree.</p>

## Output

<p>Print $n$ integers: the $i$-th integer is equal to the length of the longest sequence of trails that the skier starting at location $i$ can ski along without their kinetic energy ever becoming negative.</p>





```input1
6
1 1 0 0 0 0
1 3
2 4
3 4
4 5
5 6
```




```input2
9
0 0 0 0 0 0 1 1 1
1 3
2 3
2 5
3 6
4 5
4 7
5 8
6 9
```




```input3
14
0 0 0 0 0 0 0 0 0 1 1 1 1 1
1 2
2 5
3 4
4 5
3 6
4 8
5 9
7 8
6 11
7 12
8 13
9 14
10 11
```




```input4
20
0 0 0 0 0 0 0 0 0 0 0 0 0 1 1 1 0 1 0 1
17 3
11 12
6 10
18 19
8 14
16 20
5 3
2 11
7 10
2 15
8 3
3 15
9 16
7 13
16 1
19 2
2 16
6 1
4 17
```




```output1
0 0 1 1 3 5
```




```output2
5 3 2 1 1 1 0 0 0
```




```output3
8 5 4 3 2 2 1 1 1 0 0 0 0 0
```




```output4
2 2 1 5 3 4 8 1 2 6 4 6 10 0 0 0 3 0 1 0
```



## Note

<p>In the first test, $h = [0, 0, 1, 1, 2, 3]$. The skier starting from $6$ can ski along at most $5$ trails, in the path $6 \rightarrow 5 \rightarrow 4 \rightarrow 3 \rightarrow 4 \rightarrow 2$ (notice that a skier can ski multiple times along the same trail and can visit more than once the same location): </p><ul> <li> at the location $6$, the kinetic energy is $0$; </li><li> at the location $5$, the kinetic energy increases by $1$ (because $h_5 &lt; h_6$), so it becomes $1$; </li><li> at the location $4$, the kinetic energy increases by $1$ (because $h_4 &lt; h_5$), so it becomes $2$; </li><li> at the location $3$, the kinetic energy decreases by $1$ (because $h_3 = h_4$), so it becomes $1$; </li><li> at the location $4$, the kinetic energy decreases by $1$ (because $h_4 = h_3$), so it becomes $0$; </li><li> at the location $2$, the kinetic energy increases by $1$ (because $h_2 &lt; h_4$), so it becomes $1$. </li></ul><p>There isn't any sequence of trails of length greater than $5$ such that the kinetic energy is always non-negative.</p><p>Moreover, </p><ul> <li> the optimal path for the skier starting from $1$ is $1$ (no trails); </li><li> the optimal path for the skier starting from $2$ is $2$ (no trails); </li><li> the optimal path for the skier starting from $3$ is $3 \rightarrow 1$; </li><li> the optimal path for the skier starting from $4$ is $4 \rightarrow 2$; </li><li> the optimal path for the skier starting from $5$ is $5 \rightarrow 4 \rightarrow 3 \rightarrow 1$. </li></ul><p>In the second test, $h = [3, 2, 2, 1, 1, 1, 0, 0, 0]$. The skier starting from $1$ can ski along at most $5$ trails, in the path $1 \rightarrow 3 \rightarrow 2 \rightarrow 5 \rightarrow 4 \rightarrow 7$. </p><ul> <li> at the location $1$, the kinetic energy is $0$; </li><li> at the location $3$, the kinetic energy increases by $1$ (because $h_3 &lt; h_1$), so it becomes $1$; </li><li> at the location $2$, the kinetic energy decreases by $1$ (because $h_2 = h_3$), so it becomes $0$; </li><li> at the location $5$, the kinetic energy increases by $1$ (because $h_5 &lt; h_2$), so it becomes $1$; </li><li> at the location $4$, the kinetic energy decreases by $1$ (because $h_4 = h_5$), so it becomes $0$; </li><li> at the location $7$, the kinetic energy increases by $1$ (because $h_7 &lt; h_4$), so it becomes $1$. </li></ul><p>There isn't any sequence of trails of length greater than $5$ such that the kinetic energy is always non-negative.</p><p>In the third test, for the skier starting from vertex $1$, the optimal path is $1 \rightarrow 2 \rightarrow 5 \rightarrow 4 \rightarrow 3 \rightarrow 6 \rightarrow 11 \rightarrow 10 \rightarrow 11$.</p><p>Here are pictures of the first, second, and third test, with the base lodges shown in red:</p><center> <img class="tex-graphics" src="file://sfKk8Go3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
