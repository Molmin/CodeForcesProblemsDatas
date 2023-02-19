## Description

<div><p>A <span class="tex-font-style-it">map</span> is a matrix consisting of symbols from the set of '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">D</span>', and '<span class="tex-font-style-tt">R</span>'.</p><p>A <span class="tex-font-style-it">map graph</span> of a map matrix $a$ is a directed graph with $n \cdot m$ vertices numbered as $(i, j)$ ($1 \le i \le n; 1 \le j \le m$), where $n$ is the number of rows in the matrix, $m$ is the number of columns in the matrix. The graph has $n \cdot m$ directed edges $(i, j) \to (i + di_{a_{i, j}}, j + dj_{a_{i, j}})$, where $(di_U, dj_U) = (-1, 0)$; $(di_L, dj_L) = (0, -1)$; $(di_D, dj_D) = (1, 0)$; $(di_R, dj_R) = (0, 1)$. A map graph is <span class="tex-font-style-it">valid</span> when all edges point to valid vertices in the graph.</p><p>An <span class="tex-font-style-it">admissible map</span> is a map such that its map graph is valid and consists of a set of cycles.</p><p>A <span class="tex-font-style-it">description</span> of a map $a$ is a concatenation of all rows of the map&nbsp;— a string $a_{1,1} a_{1,2} \ldots a_{1, m} a_{2, 1} \ldots a_{n, m}$.</p><p>You are given a string $s$. Your task is to find how many substrings of this string can constitute a description of some admissible map. </p><p>A <span class="tex-font-style-it">substring</span> of a string $s_1s_2 \ldots s_l$ of length $l$ is defined by a pair of indices $p$ and $q$ ($1 \le p \le q \le l$) and is equal to $s_ps_{p+1} \ldots s_q$. Two substrings of $s$ are considered different when the pair of their indices $(p, q)$ differs, even if they represent the same resulting string.</p></div><div class="input-specification"><p>In the only input line, there is a string $s$, consisting of at least one and at most $20\,000$ symbols '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">D</span>', or '<span class="tex-font-style-tt">R</span>'.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the number of substrings of $s$ that constitute a description of some admissible map.</p></div>

## Input

<p>In the only input line, there is a string $s$, consisting of at least one and at most $20\,000$ symbols '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">D</span>', or '<span class="tex-font-style-tt">R</span>'.</p>

## Output

<p>Output one integer&nbsp;— the number of substrings of $s$ that constitute a description of some admissible map.</p>





```input1
RDUL
```




```input2
RDRU
```




```input3
RLRLRL
```




```output1
2
```




```output2
0
```




```output3
6
```



## Note

<p>In the first example, there are two substrings that can constitute a description of an admissible map&nbsp;— "<span class="tex-font-style-tt">RDUL</span>" as a matrix of size $2 \times 2$ (pic. 1) and "<span class="tex-font-style-tt">DU</span>" as a matrix of size $2 \times 1$ (pic. 2). </p><p>In the second example, no substring can constitute a description of an admissible map. E.&nbsp;g. if we try to&nbsp;look at the string "<span class="tex-font-style-tt">RDRU</span>" as a matrix of size $2 \times 2$, we can find out that the resulting graph is not a set of cycles (pic. 3).</p><p>In the third example, three substrings "<span class="tex-font-style-tt">RL</span>", two substrings "<span class="tex-font-style-tt">RLRL</span>" and one substring "<span class="tex-font-style-tt">RLRLRL</span>" can constitute an admissible map, some of them in multiple ways. E.&nbsp;g. here are two illustrations of substring "<span class="tex-font-style-tt">RLRLRL</span>" as matrices of size $3 \times 2$ (pic. 4) and $1 \times 6$ (pic. 5).</p><p><img class="tex-graphics" src="file://gjfur8YK.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img class="tex-graphics" src="file://FEZPT8FD.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img class="tex-graphics" src="file://yqRnIma0.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img class="tex-graphics" src="file://UEmNxlWs.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img class="tex-graphics" src="file://dE0sXa7N.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
