## Description

<div><p>Fishingprince loves trees. A tree is a connected undirected graph without cycles.</p><p>Fishingprince has a tree of $n$ vertices. The vertices are numbered $1$ through $n$. Let $d(x,y)$ denote the shortest distance on the tree from vertex $x$ to vertex $y$, assuming that the length of each edge is $1$.</p><p>However, the tree was lost in an accident. Fortunately, Fishingprince still remembers some information about the tree. More specifically, for every triple of integers $x,y,z$ ($1\le x&lt;y\le n$, $1\le z\le n$) he remembers whether $d(x,z)=d(y,z)$ or not.</p><p>Help him recover the structure of the tree, or report that no tree satisfying the constraints exists.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 200$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2\le n\le 100$) — the number of vertices in the tree.</p><p>Then $n-1$ lines follow. The $i$-th line of these $n-1$ lines contains $n-i$ strings of length $n$ consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If the $k$-th character in the $j$-th string of the $i$-th line is <span class="tex-font-style-tt">0</span>, it means that $d(i,k)\ne d(i+j,k)$; if the $k$-th character in the $j$-th string of the $i$-th line is <span class="tex-font-style-tt">1</span>, it means that $d(i,k)=d(i+j,k)$.</p><p>It is guaranteed that in one input file,</p><ul> <li> there are at most $2$ test cases that have $n&gt;50$; </li><li> there are at most $5$ test cases that have $n&gt;20$. </li></ul></div><div class="output-specification"><p>For each test case:</p><ul> <li> if no answer exists, output <span class="tex-font-style-tt">No</span>; </li><li> otherwise, on the first line output <span class="tex-font-style-tt">Yes</span>. Then output $n-1$ lines. Each line should contain two integers $x,y$ ($1\le x,y\le n$), denoting an edge between vertices $x$ and $y$ of the tree. If there are multiple solutions, print any. </li></ul><p>When printing <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">No</span>, you can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 200$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2\le n\le 100$) — the number of vertices in the tree.</p><p>Then $n-1$ lines follow. The $i$-th line of these $n-1$ lines contains $n-i$ strings of length $n$ consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If the $k$-th character in the $j$-th string of the $i$-th line is <span class="tex-font-style-tt">0</span>, it means that $d(i,k)\ne d(i+j,k)$; if the $k$-th character in the $j$-th string of the $i$-th line is <span class="tex-font-style-tt">1</span>, it means that $d(i,k)=d(i+j,k)$.</p><p>It is guaranteed that in one input file,</p><ul> <li> there are at most $2$ test cases that have $n&gt;50$; </li><li> there are at most $5$ test cases that have $n&gt;20$. </li></ul>

## Output

<p>For each test case:</p><ul> <li> if no answer exists, output <span class="tex-font-style-tt">No</span>; </li><li> otherwise, on the first line output <span class="tex-font-style-tt">Yes</span>. Then output $n-1$ lines. Each line should contain two integers $x,y$ ($1\le x,y\le n$), denoting an edge between vertices $x$ and $y$ of the tree. If there are multiple solutions, print any. </li></ul><p>When printing <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">No</span>, you can print each letter in any case (upper or lower).</p>





```input1|2,3,6,7,8,12,13,14,15,16
5
2
00
2
10
3
001 000
000
3
001 010
000
5
00000 01001 00000 01100
00000 10000 00000
00000 11010
00000
```




```output1
Yes
1 2
No
Yes
1 3
2 3
No
Yes
1 2
1 4
2 3
2 5
```


