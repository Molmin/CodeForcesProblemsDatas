## Description

<div><p><span class="tex-font-style-bf">Note that this is the first problem of the two similar problems. You can hack this problem only if you solve both problems.</span></p><p>You are given a tree with $n$ nodes. In the beginning, $0$ is written on all edges. In one operation, you can choose any $2$ distinct <span class="tex-font-style-bf">leaves</span> $u$, $v$ and any <span class="tex-font-style-bf">real</span> number $x$ and add $x$ to values written on all edges on the simple path between $u$ and $v$.</p><p>For example, on the picture below you can see the result of applying two operations to the graph: adding $2$ on the path from $7$ to $6$, and then adding $-0.5$ on the path from $4$ to $5$. </p><center> <img class="tex-graphics" src="file://nLYCKoAf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Is it true that for any configuration of real numbers written on edges, we can achieve it with a finite number of operations?</p><p>Leaf is a node of a tree of degree $1$. Simple path is a path that doesn't contain any node twice.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of nodes.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$), meaning that there is an edge between nodes $u$ and $v$. It is guaranteed that these edges form a tree.</p></div><div class="output-specification"><p>If there is a configuration of real numbers written on edges of the tree that we can't achieve by performing the operations, output "<span class="tex-font-style-tt">NO</span>". </p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>". </p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of nodes.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$), meaning that there is an edge between nodes $u$ and $v$. It is guaranteed that these edges form a tree.</p>

## Output

<p>If there is a configuration of real numbers written on edges of the tree that we can't achieve by performing the operations, output "<span class="tex-font-style-tt">NO</span>". </p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>". </p><p>You can print each letter in any case (upper or lower).</p>





```input1
2
1 2
```




```input2
3
1 2
2 3
```




```input3
5
1 2
1 3
1 4
2 5
```




```input4
6
1 2
1 3
1 4
2 5
2 6
```




```output1
YES
```




```output2
NO
```




```output3
NO
```




```output4
YES
```



## Note

<p>In the first example, we can add any real $x$ to the value written on the only edge $(1, 2)$.</p><center> <img class="tex-graphics" src="file://YIeOOcnz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, one of configurations that we can't reach is $0$ written on $(1, 2)$ and $1$ written on $(2, 3)$.</p><center> <img class="tex-graphics" src="file://Xj7bZuwk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Below you can see graphs from examples $3$, $4$:</p><center> <img class="tex-graphics" src="file://Ha0LWmPk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://BbQHjopE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
