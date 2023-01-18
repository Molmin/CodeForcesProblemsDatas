## Description

<div><p>You are given a tournament&nbsp;— complete directed graph.</p><p>In one operation you can pick any vertex $v$ and change the direction of all edges with $v$ on one of the ends (i.e all edges $u \to v$ change their orientation to $v \to u$ and vice versa).</p><p>You want to make the tournament strongly connected with the smallest possible number of such operations if it is possible. </p><p>Also, if it is possible, you need to find the number of ways to make this number of operations to make graph strongly connected (two ways are different if for some $i$ vertex that we chose on $i$-th operation in one way is different from vertex that we chose on $i$-th operation in another way). You only need to find this value modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line of input contains one integer $n$ ($3 \leq n \leq 2000$): the number of vertices in the tournament.</p><p>Following $n$ lines contain a description of the given tournament, each of them contains a binary string of length $n$. If $j$-th character of $i$-th string is equal to '1', then the graph has an edge $i \to j$.</p><p>It is guaranteed that there are no edges $i \to i$ and the graph has <span class="tex-font-style-bf">exactly one</span> edge among $i \to j$ and $j \to i$ for different $i$ and $j$.</p></div><div class="output-specification"><p>If it is not possible to convert tournament to strongly connected with the given operations, output "-1".</p><p>Otherwise, output two integers: the smallest number of operations that you need to make the given graph strongly connected and the number of ways to do this number of operations to make graph strongly connected, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line of input contains one integer $n$ ($3 \leq n \leq 2000$): the number of vertices in the tournament.</p><p>Following $n$ lines contain a description of the given tournament, each of them contains a binary string of length $n$. If $j$-th character of $i$-th string is equal to '1', then the graph has an edge $i \to j$.</p><p>It is guaranteed that there are no edges $i \to i$ and the graph has <span class="tex-font-style-bf">exactly one</span> edge among $i \to j$ and $j \to i$ for different $i$ and $j$.</p>

## Output

<p>If it is not possible to convert tournament to strongly connected with the given operations, output "-1".</p><p>Otherwise, output two integers: the smallest number of operations that you need to make the given graph strongly connected and the number of ways to do this number of operations to make graph strongly connected, modulo $998\,244\,353$.</p>





```input1
3
010
001
100
```




```input2
4
0010
1000
0100
1110
```




```input3
6
010000
001000
100000
111001
111100
111010
```




```output1
0 1
```




```output2
-1
```




```output3
2 18
```


