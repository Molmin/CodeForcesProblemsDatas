## Description

<div><p>Rhodoks has a tree with $n$ vertices, but he doesn't remember its structure. The vertices are indexed from $1$ to $n$.</p><p>A segment $[l,r]$ ($1 \leq l \leq r \leq n$) is good if the vertices with indices $l$, $l + 1$, ..., $r$ form a connected component in Rhodoks' tree. Otherwise, it is bad.</p><p>For example, if the tree is the one in the picture, then only the segment $[3,4]$ is bad while all the other segments are good.</p><center> <img class="tex-graphics" src="file://fzybqwMb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For each of the $\frac{n(n+1)}{2}$ segments, Rhodoks remembers whether it is good or bad. Can you help him recover the tree? If there are multiple solutions, print any.</p><p>It is guaranteed that the there is at least one tree satisfying Rhodoks' description. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 1000$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2000$) — the number of vertices in the tree.</p><p>Then $n$ lines follow. The $i$-th of these lines contains a string $good_i$ of length $n+1-i$ consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If the segment $[i,i+j-1]$ is good then the $j$-th character of $good_i$ is <span class="tex-font-style-tt">1</span>, otherwise $j$-th character of $good_i$ is <span class="tex-font-style-tt">0</span>.</p><p>It is guaranteed that the there is at least one tree consistent with the given data. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, print $n-1$ lines describing the tree you recover. </p><p>The $i$-th line should contain two integers $u_i$ and $v_i$ ($1 \leq u_i,v_i \leq n$), denoting an edge between vertices $u_i$ and $v_i$.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 1000$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2000$) — the number of vertices in the tree.</p><p>Then $n$ lines follow. The $i$-th of these lines contains a string $good_i$ of length $n+1-i$ consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If the segment $[i,i+j-1]$ is good then the $j$-th character of $good_i$ is <span class="tex-font-style-tt">1</span>, otherwise $j$-th character of $good_i$ is <span class="tex-font-style-tt">0</span>.</p><p>It is guaranteed that the there is at least one tree consistent with the given data. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, print $n-1$ lines describing the tree you recover. </p><p>The $i$-th line should contain two integers $u_i$ and $v_i$ ($1 \leq u_i,v_i \leq n$), denoting an edge between vertices $u_i$ and $v_i$.</p><p>If there are multiple solutions, print any.</p>





```input1|2,3,4,5,6,14,15,16,17,18,19,20,21,22,23,24,25,26
3
4
1111
111
10
1
6
111111
11111
1111
111
11
1
12
100100000001
11100000001
1000000000
100000000
10010001
1110000
100000
10000
1001
111
10
1
```




```output1
1 2
2 3
2 4
1 2
2 3
3 4
4 5
5 6
2 3
6 7
10 11
2 4
6 8
10 12
1 4
5 8
9 12
5 12
2 12
```



## Note

<p>The first test case is explained in the statement.</p><p>In the second test case, one possible tree is as follows:</p><center> <img class="tex-graphics" src="file://FSZyLmDr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third test case, one possible tree is as follows:</p><center> <img class="tex-graphics" src="file://oZyM2dD1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
