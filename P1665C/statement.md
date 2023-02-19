## Description

<div><p>A tree is a connected graph without cycles. A rooted tree has a special vertex called the root. The parent of a vertex $v$ (different from root) is the previous to $v$ vertex on the shortest path from the root to the vertex $v$. Children of the vertex $v$ are all vertices for which $v$ is the parent.</p><p>You are given a rooted tree with $n$ vertices. The vertex $1$ is the root. Initially, all vertices are healthy.</p><p>Each second you do <span class="tex-font-style-bf">two</span> operations, the <span class="tex-font-style-it">spreading</span> operation and, after that, the <span class="tex-font-style-it">injection</span> operation: </p><ol> <li> Spreading: for <span class="tex-font-style-bf">each</span> vertex $v$, if at least one child of $v$ is infected, you can spread the disease by infecting at most one other child of $v$ of your choice. </li><li> Injection: you can choose any healthy vertex and infect it. </li></ol><p>This process repeats each second until the whole tree is infected. You need to find the minimal number of seconds needed to infect the whole tree.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of the vertices in the given tree.</p><p>The second line of each test case contains $n - 1$ integers $p_2, p_3, \ldots, p_n$ ($1 \le p_i \le n$), where $p_i$ is the ancestor of the $i$-th vertex in the tree.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case you should output a single integer&nbsp;— the minimal number of seconds needed to infect the whole tree.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of the vertices in the given tree.</p><p>The second line of each test case contains $n - 1$ integers $p_2, p_3, \ldots, p_n$ ($1 \le p_i \le n$), where $p_i$ is the ancestor of the $i$-th vertex in the tree.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case you should output a single integer&nbsp;— the minimal number of seconds needed to infect the whole tree.</p>





```input1
5
7
1 1 1 2 2 4
5
5 5 1 4
2
1
3
3 1
6
1 1 1 1 1
```




```output1
4
4
2
3
4
```



## Note

<p>The image depicts the tree from the first test case during each second.</p><p>A vertex is black if it is not infected. A vertex is blue if it is infected by <span class="tex-font-style-it">injection</span> during the previous second. A vertex is green if it is infected by <span class="tex-font-style-it">spreading</span> during the previous second. A vertex is red if it is infected earlier than the previous second.</p><center> <img class="tex-graphics" src="file://8hbVbCuh.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that you are able to choose which vertices are infected by <span class="tex-font-style-it">spreading</span> and by <span class="tex-font-style-it">injections</span>.</p>
