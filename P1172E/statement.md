## Description

<div><p>Nauuo is a girl who loves traveling.</p><p>One day she went to a tree, Old Driver Tree, literally, a tree with an old driver on it.</p><p>The tree is a connected graph consisting of $n$ nodes and $n-1$ edges. Each node has a color, and Nauuo will visit the ODT through a simple path on the tree in the old driver's car.</p><p>Nauuo wants to visit see more different colors in her journey, but she doesn't know which simple path she will be traveling on. So, she wants to calculate the sum of the numbers of different colors on all different paths. Can you help her?</p><p>What's more, the ODT is being redecorated, so there will be $m$ modifications, each modification will change a single node's color. Nauuo wants to know the answer after each modification too.</p><p>Note that in this problem, we consider the simple path from $u$ to $v$ and the simple path from $v$ to $u$ as two different simple paths if and only if $u\ne v$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2\le n\le 4\cdot 10^5$, $1\le m\le 4\cdot 10^5$) — the number of nodes and the number of modifications.</p><p>The second line contains $n$ integers $c_1,c_2,\ldots,c_n$ ($1\le c_i\le n$), where $c_i$ is the initial color of node $i$.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ ($1\le u,v\le n$), denoting there is an edge between $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>Each of the next $m$ lines contains two integers $u$ and $x$ ($1\le u,x\le n$), which means a modification that changes the color of node $u$ into $x$.</p></div><div class="output-specification"><p>The output contains $m+1$ integers — the first integer is the answer at the beginning, the rest integers are the answers after every modification in the given order.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2\le n\le 4\cdot 10^5$, $1\le m\le 4\cdot 10^5$) — the number of nodes and the number of modifications.</p><p>The second line contains $n$ integers $c_1,c_2,\ldots,c_n$ ($1\le c_i\le n$), where $c_i$ is the initial color of node $i$.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ ($1\le u,v\le n$), denoting there is an edge between $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>Each of the next $m$ lines contains two integers $u$ and $x$ ($1\le u,x\le n$), which means a modification that changes the color of node $u$ into $x$.</p>

## Output

<p>The output contains $m+1$ integers — the first integer is the answer at the beginning, the rest integers are the answers after every modification in the given order.</p>





```input1
5 3
1 2 1 2 3
1 2
1 3
3 4
3 5
3 3
4 1
4 3
```




```input2
6 1
1 1 1 1 1 1
1 2
2 3
3 4
4 5
5 6
1 2
```




```output1
47
51
49
45
```




```output2
36
46
```



## Note

<p><span class="tex-font-style-bf">Example 1</span></p><p><img class="tex-graphics" src="file://RXe7Eo1U.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The number of colors on each simple path at the beginning:</p><p><img class="tex-graphics" src="file://M12o1Q1v.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
