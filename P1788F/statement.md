## Description

<div><p>You are given a tree of $n$ vertices. The vertices are numbered from $1$ to $n$.</p><p>You will need to assign a weight to each edge. Let the weight of the $i$-th edge be $a_i$ ($1 \leq i \leq n-1$). The weight of each edge should be an integer between $0$ and $2^{30}-1$, inclusive.</p><p>You are given $q$ conditions. Each condition consists of three integers $u$, $v$, and $x$. This means that the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all edges on the shortest path from $u$ to $v$ should be $x$.</p><p>Find out if there exist $a_1, a_2, \ldots, a_{n-1}$ that satisfy the given conditions. If yes, print a solution such that $a_1 \oplus a_2 \oplus \ldots \oplus a_{n-1}$ is the <span class="tex-font-style-bf">smallest</span>. Here, $\oplus$ denotes the bitwise XOR operation.</p><p>If there are multiple solutions such that $a_1 \oplus a_2 \oplus \ldots \oplus a_{n-1}$ is the smallest, print any.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \le n \le 2.5 \cdot 10^5$, $0 \le q \le 2.5 \cdot 10^5$).</p><p>The $i$-th of the following $n-1$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$, $x_i \neq y_i$), meaning that the $i$-th edge connects vertices $x_i$ and $y_i$ in the tree.</p><p>It is guaranteed that the given edges form a tree.</p><p>The following $q$ lines contain information about conditions.</p><p>Each line contains three integers $u$, $v$, $x$ ($1 \le u, v \le n$, $u \neq v$, $0 \le x \le 2^{30}-1$), meaning that the bitwise XOR of all edges on the shortest path from $u$ to $v$ should be $x$.</p></div><div class="output-specification"><p>If there do not exist $a_1$, $a_2$, ..., $a_{n-1}$ that satisfy the given conditions, print "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">Yes</span>" in the first line.</p><p>Then print $n-1$ integers on the next line, where the $i$-th integer is the weight of the $i$-th edge. If there are multiple solutions that satisfy the given conditions, print a solution such that $a_1 \oplus a_2 \oplus \ldots \oplus a_{n-1}$ is the smallest.</p><p>If there are multiple solutions such that $a_1 \oplus a_2 \oplus \ldots \oplus a_{n-1}$ is the smallest, print any.</p><p>When printing "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">No</span>", you can print each letter in any case (either upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \le n \le 2.5 \cdot 10^5$, $0 \le q \le 2.5 \cdot 10^5$).</p><p>The $i$-th of the following $n-1$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$, $x_i \neq y_i$), meaning that the $i$-th edge connects vertices $x_i$ and $y_i$ in the tree.</p><p>It is guaranteed that the given edges form a tree.</p><p>The following $q$ lines contain information about conditions.</p><p>Each line contains three integers $u$, $v$, $x$ ($1 \le u, v \le n$, $u \neq v$, $0 \le x \le 2^{30}-1$), meaning that the bitwise XOR of all edges on the shortest path from $u$ to $v$ should be $x$.</p>

## Output

<p>If there do not exist $a_1$, $a_2$, ..., $a_{n-1}$ that satisfy the given conditions, print "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">Yes</span>" in the first line.</p><p>Then print $n-1$ integers on the next line, where the $i$-th integer is the weight of the $i$-th edge. If there are multiple solutions that satisfy the given conditions, print a solution such that $a_1 \oplus a_2 \oplus \ldots \oplus a_{n-1}$ is the smallest.</p><p>If there are multiple solutions such that $a_1 \oplus a_2 \oplus \ldots \oplus a_{n-1}$ is the smallest, print any.</p><p>When printing "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">No</span>", you can print each letter in any case (either upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1
4 4
1 2
2 3
3 4
1 4 3
2 4 2
1 3 1
2 3 1
```




```input2
6 2
1 2
2 3
3 4
2 5
5 6
1 4 2
2 6 7
```




```input3
6 2
1 2
2 3
3 4
2 5
5 6
1 4 3
1 6 5
```




```output1
No
```




```output2
Yes
4 2 4 1 6
```




```output3
Yes
6 1 4 3 0
```



## Note

<p>For the first example, there does not exist a set of edge weights that satisfies the given conditions.</p><p>For the second example, the two given conditions are $a_1 \oplus a_2 \oplus a_3=2$ and $a_4 \oplus a_5=7$. There can be multiple solutions, for example, $(a_1, a_2, a_3, a_4, a_5)=(1, 2, 1, 4, 3)$.</p><p>For the third example, the two given conditions are $a_1 \oplus a_2 \oplus a_3=3$ and $a_1 \oplus a_4 \oplus a_5=5$. There are multiple solutions that satisfy the given conditions. </p><p>$(a_1, a_2, a_3, a_4, a_5)=(1, 1, 3, 4, 0)$ satisfies the given conditions, but the bitwise XOR of all edge weights is $7$, which does not have the smallest $a_1 \oplus a_2 \oplus \ldots \oplus a_{n-1}$, so it cannot be the answer.</p>
