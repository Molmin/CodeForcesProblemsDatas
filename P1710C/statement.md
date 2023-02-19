## Description

<div><p>You are given a positive integer $n$. Since $n$ may be very large, you are given its binary representation.</p><p>You should compute the number of triples $(a,b,c)$ with $0 \leq a,b,c \leq n$ such that $a \oplus b$, $b \oplus c$, and $a \oplus c$ are the sides of a non-degenerate triangle. </p><p>Here, $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>You should output the answer modulo $998\,244\,353$.</p><p>Three positive values $x$, $y$, and $z$ are the sides of a non-degenerate triangle if and only if $x+y&gt;z$, $x+z&gt;y$, and $y+z&gt;x$.</p></div><div class="input-specification"><p>The first and only line contains the binary representation of an integer $n$ ($0 &lt; n &lt; 2^{200\,000}$) without leading zeros.</p><p>For example, the string <span class="tex-font-style-tt">10</span> is the binary representation of the number $2$, while the string <span class="tex-font-style-tt">1010</span> represents the number $10$.</p></div><div class="output-specification"><p>Print one integer — the number of triples $(a,b,c)$ satisfying the conditions described in the statement modulo $998\,244\,353$.</p></div>

## Input

<p>The first and only line contains the binary representation of an integer $n$ ($0 &lt; n &lt; 2^{200\,000}$) without leading zeros.</p><p>For example, the string <span class="tex-font-style-tt">10</span> is the binary representation of the number $2$, while the string <span class="tex-font-style-tt">1010</span> represents the number $10$.</p>

## Output

<p>Print one integer — the number of triples $(a,b,c)$ satisfying the conditions described in the statement modulo $998\,244\,353$.</p>





```input1|
101
```




```input2|
1110
```




```input3|
11011111101010010
```




```output1
12
```




```output2
780
```




```output3
141427753
```



## Note

<p>In the first test case, $101_2=5$.</p><ul> <li> The triple $(a, b, c) = (0, 3, 5)$ is valid because $(a\oplus b, b\oplus c, c\oplus a) = (3, 6, 5)$ are the sides of a non-degenerate triangle. </li><li> The triple $(a, b, c) = (1, 2, 4)$ is valid because $(a\oplus b, b\oplus c, c\oplus a) = (3, 6, 5)$ are the sides of a non-degenerate triangle. </li></ul><p>The $6$ permutations of each of these two triples are all the valid triples, thus the answer is $12$.</p><p>In the third test case, $11\,011\,111\,101\,010\,010_2=114\,514$. The full answer (before taking the modulo) is $1\,466\,408\,118\,808\,164$.</p>
