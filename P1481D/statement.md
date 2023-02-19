## Description

<div><p>Your friend Salem is Warawreh's brother and only loves math and geometry problems. He has solved plenty of such problems, but according to Warawreh, in order to graduate from university he has to solve more graph problems. Since Salem is not good with graphs he asked your help with the following problem.</p><center> <img class="tex-graphics" src="file://mNcSsvER.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a complete directed graph with $n$ vertices without self-loops. In other words, you have $n$ vertices and each pair of vertices $u$ and $v$ ($u \neq v$) has both directed edges $(u, v)$ and $(v, u)$.</p><p>Every directed edge of the graph is labeled with a single character: either '<span class="tex-font-style-tt">a</span>' or '<span class="tex-font-style-tt">b</span>' (edges $(u, v)$ and $(v, u)$ may have different labels).</p><p>You are also given an integer $m &gt; 0$. You should find a path of length $m$ such that the string obtained by writing out edges' labels when going along the path is a <span class="tex-font-style-bf">palindrome</span>. The length of the path is the number of edges in it.</p><p><span class="tex-font-style-bf">You can visit the same vertex and the same directed edge any number of times</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 1000$; $1 \leq m \leq 10^{5}$)&nbsp;— the number of vertices in the graph and desirable length of the palindrome.</p><p>Each of the next $n$ lines contains $n$ characters. The $j$-th character of the $i$-th line describes the character on the edge that is going from node $i$ to node $j$.</p><p>Every character is either '<span class="tex-font-style-tt">a</span>' or '<span class="tex-font-style-tt">b</span>' if $i \neq j$, or '<span class="tex-font-style-tt">*</span>' if $i = j$, since the graph doesn't contain self-loops.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $1000$ and the sum of $m$ doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if it is possible to find such path, print "<span class="tex-font-style-tt">YES</span>" and the path itself as a sequence of $m + 1$ integers: indices of vertices in the path in the appropriate order. If there are several valid paths, print any of them.</p><p>Otherwise, (if there is no answer) print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 1000$; $1 \leq m \leq 10^{5}$)&nbsp;— the number of vertices in the graph and desirable length of the palindrome.</p><p>Each of the next $n$ lines contains $n$ characters. The $j$-th character of the $i$-th line describes the character on the edge that is going from node $i$ to node $j$.</p><p>Every character is either '<span class="tex-font-style-tt">a</span>' or '<span class="tex-font-style-tt">b</span>' if $i \neq j$, or '<span class="tex-font-style-tt">*</span>' if $i = j$, since the graph doesn't contain self-loops.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $1000$ and the sum of $m$ doesn't exceed $10^5$.</p>

## Output

<p>For each test case, if it is possible to find such path, print "<span class="tex-font-style-tt">YES</span>" and the path itself as a sequence of $m + 1$ integers: indices of vertices in the path in the appropriate order. If there are several valid paths, print any of them.</p><p>Otherwise, (if there is no answer) print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
5
3 1
*ba
b*b
ab*
3 3
*ba
b*b
ab*
3 4
*ba
b*b
ab*
4 6
*aaa
b*ba
ab*a
bba*
2 6
*a
b*
```




```output1
YES
1 2
YES
2 1 3 2
YES
1 3 1 3 1
YES
1 2 1 3 4 1 4
NO
```



## Note

<p>The graph from the first three test cases is shown below:</p><center> <img class="tex-graphics" src="file://OBBMw9HK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the first test case, the answer sequence is $[1,2]$ which means that the path is:</p><p>$$1 \xrightarrow{\text{b}} 2$$</p><p>So the string that is obtained by the given path is <span class="tex-font-style-tt">b</span>.</p><p>In the second test case, the answer sequence is $[2,1,3,2]$ which means that the path is:</p><p>$$2 \xrightarrow{\text{b}} 1 \xrightarrow{\text{a}} 3 \xrightarrow{\text{b}} 2$$</p><p>So the string that is obtained by the given path is <span class="tex-font-style-tt">bab</span>.</p><p>In the third test case, the answer sequence is $[1,3,1,3,1]$ which means that the path is:</p><p>$$1 \xrightarrow{\text{a}} 3 \xrightarrow{\text{a}} 1 \xrightarrow{\text{a}} 3 \xrightarrow{\text{a}} 1$$</p><p>So the string that is obtained by the given path is <span class="tex-font-style-tt">aaaa</span>.</p><p>The string obtained in the fourth test case is <span class="tex-font-style-tt">abaaba</span>.</p>
