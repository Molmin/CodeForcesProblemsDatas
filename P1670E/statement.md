## Description

<div><p><span class="tex-font-style-it">After the last regional contest, Hemose and his teammates finally qualified to the ICPC World Finals, so for this great achievement and his love of trees, he gave you this problem as the name of his team "Hemose 3al shagra" (Hemose on the tree).</span></p><p>You are given a tree of $n$ vertices where $n$ is a power of $2$. You have to give each node and edge an integer value in the range $[1,2n -1]$ (inclusive), where all the values are distinct.</p><p>After giving each node and edge a value, you should select some root for the tree such that the maximum cost of any simple path starting from the root and ending at any <span class="tex-font-style-bf">node or edge</span> is minimized.</p><p>The cost of the path between two nodes $u$ and $v$ or any node $u$ and edge $e$ is defined as the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all the node's and edge's values between them, including the endpoints (note that in a tree there is only one simple path between two nodes or between a node and an edge).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 5\cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $p$ ($1 \le p \le 17$), where $n$ (the number of vertices in the tree) is equal to $2^p$.</p><p>Each of the next $n−1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$) meaning that there is an edge between the vertices $u$ and $v$ in the tree.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case on the first line print the chosen root.</p><p>On the second line, print $n$ integers separated by spaces, where the $i$-th integer represents the chosen value for the $i$-th node.</p><p>On the third line, print $n-1$ integers separated by spaces, where the $i$-th integer represents the chosen value for the $i$-th edge. The edges are numerated in the order of their appearance in the input data.</p><p>If there are multiple solutions, you may output any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 5\cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $p$ ($1 \le p \le 17$), where $n$ (the number of vertices in the tree) is equal to $2^p$.</p><p>Each of the next $n−1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$) meaning that there is an edge between the vertices $u$ and $v$ in the tree.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3\cdot 10^5$.</p>

## Output

<p>For each test case on the first line print the chosen root.</p><p>On the second line, print $n$ integers separated by spaces, where the $i$-th integer represents the chosen value for the $i$-th node.</p><p>On the third line, print $n-1$ integers separated by spaces, where the $i$-th integer represents the chosen value for the $i$-th edge. The edges are numerated in the order of their appearance in the input data.</p><p>If there are multiple solutions, you may output any.</p>





```input1
2
2
1 2
2 3
3 4
3
1 2
2 3
3 4
1 5
1 6
5 7
5 8
```




```output1
3
5 1 3 6
4 2 7
5
1 2 8 11 4 13 9 15
6 14 3 7 10 5 12
```



## Note

<p>The tree in the first test case with the weights of all nodes and edges is shown in the picture.</p><center> <img class="tex-graphics" src="file://aPybWA81.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The costs of all paths are: </p><ul> <li> $3$; </li><li> $3\oplus 7=4$; </li><li> $3\oplus 7\oplus 6=2$; </li><li> $3\oplus 2=1$; </li><li> $3\oplus 2\oplus 1=0$; </li><li> $3\oplus 2\oplus 1\oplus 4=4$; </li><li> $3\oplus 2\oplus 1\oplus 4\oplus 5=1$. </li></ul><p>The maximum cost of all these paths is $4$. We can show that it is impossible to assign the values and choose the root differently to achieve a smaller maximum cost of all paths.</p><p>The tree in the second test case: </p><center> <img class="tex-graphics" src="file://A2xqSNSN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
