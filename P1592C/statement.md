## Description

<div><p>Bakry faced a problem, but since he's lazy to solve it, he asks for your help.</p><p>You are given a tree of $n$ nodes, the $i$-th node has value $a_i$ assigned to it for each $i$ from $1$ to $n$. As a reminder, a tree on $n$ nodes is a connected graph with $n-1$ edges.</p><p>You want to delete <span class="tex-font-style-bf">at least $1$, but at most $k-1$ edges</span> from the tree, so that the following condition would hold:</p><ul><li><p>For every connected component calculate the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of the values of the nodes in it. Then, these values have to be the same for all connected components.</p></li></ul><p>Is it possible to achieve this condition?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ $(1 \leq t \leq 5 \cdot 10^4)$. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ $(2 \leq k \leq n \leq 10^5)$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, ..., a_n$ $(1 \leq a_i \leq 10^9)$.</p><p>The $i$-th of the next $n-1$ lines contains two integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$, $u_i\neq v_i$), which means that there's an edge between nodes $u_i$ and $v_i$.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, you should output a single string. If you can delete the edges according to the conditions written above, output "YES" (without quotes). Otherwise, output "NO" (without quotes).</p><p>You can print each letter of "YES" and "NO" in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ $(1 \leq t \leq 5 \cdot 10^4)$. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ $(2 \leq k \leq n \leq 10^5)$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, ..., a_n$ $(1 \leq a_i \leq 10^9)$.</p><p>The $i$-th of the next $n-1$ lines contains two integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$, $u_i\neq v_i$), which means that there's an edge between nodes $u_i$ and $v_i$.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, you should output a single string. If you can delete the edges according to the conditions written above, output "YES" (without quotes). Otherwise, output "NO" (without quotes).</p><p>You can print each letter of "YES" and "NO" in any case (upper or lower).</p>





```input1
5
2 2
1 3
1 2
5 5
3 3 3 3 3
1 2
2 3
1 4
4 5
5 2
1 7 2 3 5
1 2
2 3
1 4
4 5
5 3
1 6 4 1 2
1 2
2 3
1 4
4 5
3 3
1 7 4
1 2
2 3
```




```output1
NO
YES
NO
YES
NO
```



## Note

<p>It can be shown that the objection is not achievable for first, third, and fifth test cases.</p><p>In the second test case, you can just remove all the edges. There will be $5$ connected components, each containing only one node with value $3$, so the bitwise XORs will be $3$ for all of them.</p><p>In the fourth test case, this is the tree: <img class="tex-graphics" src="file://NAbcmiEl.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>You can remove an edge <span class="tex-font-style-bf">$(4,5)$</span></p><p>The bitwise XOR of the first component will be, $a_1 \oplus a_2 \oplus a_3 \oplus a_4 = 1 \oplus 6 \oplus 4 \oplus 1 = 2$ (where $\oplus$ denotes the bitwise XOR). </p><p>The bitwise XOR of the second component will be, $a_5 = 2$. </p>
