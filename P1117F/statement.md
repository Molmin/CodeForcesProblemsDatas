## Description

<div><p>You are given a string of length $n$. Each character is one of the first $p$ lowercase Latin letters.</p><p>You are also given a matrix $A$ with binary values of size $p \times p$. This matrix is symmetric ($A_{ij} = A_{ji}$). $A_{ij} = 1$ means that the string can have the $i$-th and $j$-th letters of Latin alphabet adjacent.</p><p>Let's call the string <span class="tex-font-style-it">crisp</span> if <span class="tex-font-style-bf">all of the adjacent characters</span> in it can be adjacent (have 1 in the corresponding cell of matrix $A$).</p><p>You are allowed to do the following move. Choose any letter, remove <span class="tex-font-style-bf">all its occurrences</span> and join the remaining parts of the string without changing their order. For example, removing letter 'a' from "abacaba" will yield "bcb".</p><p>The string you are given is <span class="tex-font-style-it">crisp</span>. The string should remain <span class="tex-font-style-it">crisp</span> <span class="tex-font-style-bf">after every move you make</span>.</p><p>You are allowed to do arbitrary number of moves (possible zero). What is the shortest resulting string you can obtain?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $p$ ($1 \le n \le 10^5$, $1 \le p \le 17$) — the length of the initial string and the length of the allowed prefix of Latin alphabet.</p><p>The second line contains the initial string. It is guaranteed that it contains only first $p$ lowercase Latin letters and that is it <span class="tex-font-style-it">crisp</span>. Some of these $p$ first Latin letters might not be present in the string.</p><p>Each of the next $p$ lines contains $p$ integer numbers — the matrix $A$ ($0 \le A_{ij} \le 1$, $A_{ij} = A_{ji}$). $A_{ij} = 1$ means that the string can have the $i$-th and $j$-th letters of Latin alphabet adjacent.</p></div><div class="output-specification"><p>Print a single integer — the length of the shortest string after you make arbitrary number of moves (possible zero).</p></div>

## Input

<p>The first line contains two integers $n$ and $p$ ($1 \le n \le 10^5$, $1 \le p \le 17$) — the length of the initial string and the length of the allowed prefix of Latin alphabet.</p><p>The second line contains the initial string. It is guaranteed that it contains only first $p$ lowercase Latin letters and that is it <span class="tex-font-style-it">crisp</span>. Some of these $p$ first Latin letters might not be present in the string.</p><p>Each of the next $p$ lines contains $p$ integer numbers — the matrix $A$ ($0 \le A_{ij} \le 1$, $A_{ij} = A_{ji}$). $A_{ij} = 1$ means that the string can have the $i$-th and $j$-th letters of Latin alphabet adjacent.</p>

## Output

<p>Print a single integer — the length of the shortest string after you make arbitrary number of moves (possible zero).</p>





```input1
7 3
abacaba
0 1 1
1 0 0
1 0 0
```




```input2
7 3
abacaba
1 1 1
1 0 0
1 0 0
```




```input3
7 4
bacadab
0 1 1 1
1 0 0 0
1 0 0 0
1 0 0 0
```




```input4
3 3
cbc
0 0 0
0 0 1
0 1 0
```




```output1
7
```




```output2
0
```




```output3
5
```




```output4
0
```



## Note

<p>In the first example no letter can be removed from the initial string.</p><p>In the second example you can remove letters in order: 'b', 'c', 'a'. The strings on the intermediate steps will be: "abacaba" $\rightarrow$ "aacaa" $\rightarrow$ "aaaa" $\rightarrow$ "".</p><p>In the third example you can remove letter 'b' and that's it.</p><p>In the fourth example you can remove letters in order 'c', 'b', but not in the order 'b', 'c' because two letters 'c' can't be adjacent.</p>
