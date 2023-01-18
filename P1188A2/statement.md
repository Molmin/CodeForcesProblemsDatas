## Description

<div><p><span class="tex-font-style-bf">Note that this is the second problem of the two similar problems. You can hack this problem if you solve it. But you can hack the previous problem only if you solve both problems.</span></p><p>You are given a tree with $n$ nodes. In the beginning, $0$ is written on all edges. In one operation, you can choose any $2$ distinct <span class="tex-font-style-bf">leaves</span> $u$, $v$ and any <span class="tex-font-style-bf">integer</span> number $x$ and add $x$ to values written on all edges on the simple path between $u$ and $v$. <span class="tex-font-style-bf">Note that in previous subtask $x$ was allowed to be any real, here it has to be integer</span>.</p><p>For example, on the picture below you can see the result of applying two operations to the graph: adding $2$ on the path from $7$ to $6$, and then adding $-1$ on the path from $4$ to $5$. </p><center> <img class="tex-graphics" src="file://lIwDDVix.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given some configuration of <span class="tex-font-style-bf">nonnegative integer pairwise different even</span> numbers, written on the edges. For a given configuration determine if it is possible to achieve it with these operations, and, if it is possible, output the sequence of operations that leads to the given configuration. Constraints on the operations are listed in the output format section.</p><p>Leave is a node of a tree of degree $1$. Simple path is a path that doesn't contain any node twice.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 1000$)&nbsp;— the number of nodes in a tree.</p><p>Each of the next $n-1$ lines contains three integers $u$, $v$, $val$ ($1 \le u, v \le n$, $u \neq v$, $0 \le val \le 10\,000$), meaning that there is an edge between nodes $u$ and $v$ with $val$ written on it. It is guaranteed that these edges form a tree. It is guaranteed that all $val$ numbers are <span class="tex-font-style-bf">pairwise different and even</span>. </p></div><div class="output-specification"><p>If there aren't any sequences of operations which lead to the given configuration, output "<span class="tex-font-style-tt">NO</span>".</p><p>If it exists, output "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line output $m$&nbsp;— number of operations you are going to apply ($0 \le m \le 10^5$). <span class="tex-font-style-bf">Note that you don't have to minimize the number of the operations!</span></p><p>In the next $m$ lines output the operations in the following format:</p><p>$u, v, x$ ($1 \le u, v \le n$, $u \not = v$, $x$&nbsp;— integer, $-10^9 \le x \le 10^9$), where $u, v$&nbsp;— leaves, $x$&nbsp;— number we are adding. </p><p>It is guaranteed that if there exists a sequence of operations producing given configuration, then there exists a sequence of operations producing given configuration, satisfying all the conditions above.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 1000$)&nbsp;— the number of nodes in a tree.</p><p>Each of the next $n-1$ lines contains three integers $u$, $v$, $val$ ($1 \le u, v \le n$, $u \neq v$, $0 \le val \le 10\,000$), meaning that there is an edge between nodes $u$ and $v$ with $val$ written on it. It is guaranteed that these edges form a tree. It is guaranteed that all $val$ numbers are <span class="tex-font-style-bf">pairwise different and even</span>. </p>

## Output

<p>If there aren't any sequences of operations which lead to the given configuration, output "<span class="tex-font-style-tt">NO</span>".</p><p>If it exists, output "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line output $m$&nbsp;— number of operations you are going to apply ($0 \le m \le 10^5$). <span class="tex-font-style-bf">Note that you don't have to minimize the number of the operations!</span></p><p>In the next $m$ lines output the operations in the following format:</p><p>$u, v, x$ ($1 \le u, v \le n$, $u \not = v$, $x$&nbsp;— integer, $-10^9 \le x \le 10^9$), where $u, v$&nbsp;— leaves, $x$&nbsp;— number we are adding. </p><p>It is guaranteed that if there exists a sequence of operations producing given configuration, then there exists a sequence of operations producing given configuration, satisfying all the conditions above.</p>





```input1
5
1 2 2
2 3 4
3 4 10
3 5 18
```




```input2
6
1 2 6
1 3 8
1 4 12
2 5 2
2 6 4
```




```output1
NO
```




```output2
YES
4
3 6 1
4 6 3
3 4 7
4 5 2
```



## Note

<p>The configuration from the first sample is drawn below, and it is impossible to achieve.</p><center> <img class="tex-graphics" src="file://MVt2gk2O.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The sequence of operations from the second sample is illustrated below.</p><center> <img class="tex-graphics" src="file://rQBGlQ8h.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
