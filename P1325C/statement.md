## Description

<div><p>You are given a tree consisting of $n$ nodes. You want to write some labels on the tree's edges such that the following conditions hold:</p><ul> <li> Every label is an integer between $0$ and $n-2$ inclusive. </li><li> All the written labels are distinct. </li><li> The largest value among $MEX(u,v)$ over all pairs of nodes $(u,v)$ is as small as possible. </li></ul><p>Here, $MEX(u,v)$ denotes the smallest non-negative integer that isn't written on any edge on the unique simple path from node $u$ to node $v$.</p></div><div class="input-specification"><p>The first line contains the integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of nodes in the tree.</p><p>Each of the next $n-1$ lines contains two space-separated integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between nodes $u$ and $v$. It's guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>Output $n-1$ integers. The $i^{th}$ of them will be the number written on the $i^{th}$ edge (in the input order).</p></div>

## Input

<p>The first line contains the integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of nodes in the tree.</p><p>Each of the next $n-1$ lines contains two space-separated integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between nodes $u$ and $v$. It's guaranteed that the given graph is a tree.</p>

## Output

<p>Output $n-1$ integers. The $i^{th}$ of them will be the number written on the $i^{th}$ edge (in the input order).</p>





```input1
3
1 2
1 3
```




```input2
6
1 2
1 3
2 4
2 5
5 6
```




```output1
0
1
```




```output2
0
3
2
4
1
```



## Note

<p>The tree from the second sample:</p><p><img class="tex-graphics" src="file://ML9MUkG1.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
