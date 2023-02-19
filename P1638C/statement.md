## Description

<div><p>You are given a permutation $p_1, p_2, \dots, p_n$. Then, an undirected graph is constructed in the following way: add an edge between vertices $i$, $j$ such that $i &lt; j$ if and only if $p_i &gt; p_j$. Your task is to count the number of connected components in this graph.</p><p>Two vertices $u$ and $v$ belong to the same connected component if and only if there is at least one path along edges connecting $u$ and $v$.</p><p>A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$)&nbsp;— the elements of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer $k$&nbsp;— the number of connected components.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$)&nbsp;— the elements of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer $k$&nbsp;— the number of connected components.</p>





```input1
6
3
1 2 3
5
2 1 4 3 5
6
6 1 4 2 5 3
1
1
6
3 2 1 6 5 4
5
3 1 5 2 4
```




```output1
3
3
1
1
2
1
```



## Note

<p>Each separate test case is depicted in the image below. The colored squares represent the elements of the permutation. For one permutation, each color represents some connected component. The number of distinct colors is the answer.</p><center> <img class="tex-graphics" src="file://3oDnJUBU.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center>
