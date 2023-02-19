## Description

<div><p>You are given a tree consisting of $n$ vertices, and $q$ triples $(x_i, y_i, s_i)$, where $x_i$ and $y_i$ are integers from $1$ to $n$, and $s_i$ is a string <span class="tex-font-style-bf">with length equal to the number of vertices on the simple path from $x_i$ to $y_i$</span>.</p><p>You want to write a lowercase Latin letter on each vertex in such a way that, for each of $q$ given triples, at least one of the following conditions holds:</p><ul> <li> if you write out the letters on the vertices on the simple path from $x_i$ to $y_i$ in the order they appear on this path, you get the string $s_i$; </li><li> if you write out the letters on the vertices on the simple path from $y_i$ to $x_i$ in the order they appear on this path, you get the string $s_i$. </li></ul><p>Find any possible way to write a letter on each vertex to meet these constraints, or report that it is impossible.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \le n \le 4 \cdot 10^5$; $1 \le q \le 4 \cdot 10^5$) — the number of vertices in the tree and the number of triples, respectively.</p><p>Then $n - 1$ lines follow; the $i$-th of them contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$; $u_i \ne v_i$) — the endpoints of the $i$-th edge. These edges form a tree.</p><p>Then $q$ lines follow; the $j$-th of them contains two integers $x_j$ and $y_j$, and a string $s_j$ consisting of lowercase Latin letters. The length of $s_j$ is equal to the number of vertices on the simple path between $x_j$ and $y_j$.</p><p>Additional constraint on the input: $\sum \limits_{j=1}^{q} |s_j| \le 4 \cdot 10^5$.</p></div><div class="output-specification"><p>If there is no way to meet the conditions on all triples, print <span class="tex-font-style-tt">NO</span>. Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, and a string of $n$ lowercase Latin letters in the second line; the $i$-th character of the string should be the letter you write on the $i$-th vertex. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \le n \le 4 \cdot 10^5$; $1 \le q \le 4 \cdot 10^5$) — the number of vertices in the tree and the number of triples, respectively.</p><p>Then $n - 1$ lines follow; the $i$-th of them contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$; $u_i \ne v_i$) — the endpoints of the $i$-th edge. These edges form a tree.</p><p>Then $q$ lines follow; the $j$-th of them contains two integers $x_j$ and $y_j$, and a string $s_j$ consisting of lowercase Latin letters. The length of $s_j$ is equal to the number of vertices on the simple path between $x_j$ and $y_j$.</p><p>Additional constraint on the input: $\sum \limits_{j=1}^{q} |s_j| \le 4 \cdot 10^5$.</p>

## Output

<p>If there is no way to meet the conditions on all triples, print <span class="tex-font-style-tt">NO</span>. Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, and a string of $n$ lowercase Latin letters in the second line; the $i$-th character of the string should be the letter you write on the $i$-th vertex. If there are multiple answers, print any of them.</p>





```input1
3 2
2 3
2 1
2 1 ab
2 3 bc
```




```input2
3 2
2 3
2 1
2 1 ab
2 3 cd
```




```input3
10 10
1 2
1 3
1 4
1 5
1 6
1 7
1 8
1 9
1 10
1 2 ab
1 3 ab
1 4 ab
1 5 ab
1 6 ab
1 7 ab
1 8 ab
1 9 ab
1 10 ab
10 2 aba
```




```input4
10 10
1 2
1 3
1 4
1 5
1 6
1 7
1 8
1 9
1 10
1 2 ab
1 3 ab
1 4 aa
1 5 ab
1 6 ab
1 7 ab
1 8 ab
1 9 ab
1 10 ab
10 2 aba
```




```output1
YES
abc
```




```output2
NO
```




```output3
YES
baaaaaaaaa
```




```output4
NO
```


