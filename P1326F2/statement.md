## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference is constraints on the number of wise men and the time limit. You can make hacks only if all versions of this task are solved.</span></p><p>$n$ wise men live in a beautiful city. Some of them know each other.</p><p>For each of the $n!$ possible permutations $p_1, p_2, \ldots, p_n$ of the wise men, let's generate a binary string of length $n-1$: for each $1 \leq i &lt; n$ set $s_i=1$ if $p_i$ and $p_{i+1}$ know each other, and $s_i=0$ otherwise. </p><p>For all possible $2^{n-1}$ binary strings, find the number of permutations that produce this binary string.</p></div><div class="input-specification"><p>The first line of input contains one integer $n$ ($2 \leq n \leq 18)$ &nbsp;— the number of wise men in the city.</p><p>The next $n$ lines contain a binary string of length $n$ each, such that the $j$-th character of the $i$-th string is equal to '<span class="tex-font-style-tt">1</span>' if wise man $i$ knows wise man $j$, and equals '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>It is guaranteed that if the $i$-th man knows the $j$-th man, then the $j$-th man knows $i$-th man and no man knows himself.</p></div><div class="output-specification"><p>Print $2^{n-1}$ space-separated integers. For each $0 \leq x &lt; 2^{n-1}$:</p><ul> <li> Let's consider a string $s$ of length $n-1$, such that $s_i = \lfloor \frac{x}{2^{i-1}} \rfloor \bmod 2$ for all $1 \leq i \leq n - 1$. </li><li> The $(x+1)$-th number should be equal to the required answer for $s$. </li></ul></div>

## Input

<p>The first line of input contains one integer $n$ ($2 \leq n \leq 18)$ &nbsp;— the number of wise men in the city.</p><p>The next $n$ lines contain a binary string of length $n$ each, such that the $j$-th character of the $i$-th string is equal to '<span class="tex-font-style-tt">1</span>' if wise man $i$ knows wise man $j$, and equals '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>It is guaranteed that if the $i$-th man knows the $j$-th man, then the $j$-th man knows $i$-th man and no man knows himself.</p>

## Output

<p>Print $2^{n-1}$ space-separated integers. For each $0 \leq x &lt; 2^{n-1}$:</p><ul> <li> Let's consider a string $s$ of length $n-1$, such that $s_i = \lfloor \frac{x}{2^{i-1}} \rfloor \bmod 2$ for all $1 \leq i \leq n - 1$. </li><li> The $(x+1)$-th number should be equal to the required answer for $s$. </li></ul>





```input1
3
011
101
110
```




```input2
4
0101
1000
0001
1010
```




```output1
0 0 0 6
```




```output2
2 2 6 2 2 6 2 2
```



## Note

<p>In the first test, each wise man knows each other, so every permutation will produce the string $11$.</p><p>In the second test:</p><ul> <li> If $p = \{1, 2, 3, 4\}$, the produced string is $101$, because wise men $1$ and $2$ know each other, $2$ and $3$ don't know each other, and $3$ and $4$ know each other; </li><li> If $p = \{4, 1, 2, 3\}$, the produced string is $110$, because wise men $1$ and $4$ know each other, $1$ and $2$ know each other and $2$, and $3$ don't know each other; </li><li> If $p = \{1, 3, 2, 4\}$, the produced string is $000$, because wise men $1$ and $3$ don't know each other, $3$ and $2$ don't know each other, and $2$ and $4$ don't know each other. </li></ul>
