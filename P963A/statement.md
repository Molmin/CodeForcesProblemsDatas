## Description

<div><p>You are given two integers $a$ and $b$. Moreover, you are given a sequence $s_0, s_1, \dots, s_{n}$. All values in $s$ are integers $1$ or $-1$. It's known that sequence is $k$-periodic and $k$ divides $n+1$. In other words, for each $k \leq i \leq n$ it's satisfied that $s_{i} = s_{i - k}$.</p><p>Find out the <span class="tex-font-style-bf">non-negative</span> remainder of division of $\sum \limits_{i=0}^{n} s_{i} a^{n - i} b^{i}$ by $10^{9} + 9$.</p><p><span class="tex-font-style-bf">Note that the modulo is unusual!</span></p></div><div class="input-specification"><p>The first line contains four integers $n, a, b$ and $k$ $(1 \leq n \leq 10^{9}, 1 \leq a, b \leq 10^{9}, 1 \leq k \leq 10^{5})$.</p><p>The second line contains a sequence of length $k$ consisting of characters '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">-</span>'. </p><p>If the $i$-th character (0-indexed) is '<span class="tex-font-style-tt">+</span>', then $s_{i} = 1$, otherwise $s_{i} = -1$.</p><p>Note that only the first $k$ members of the sequence are given, the rest can be obtained using the periodicity property.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— value of given expression modulo $10^{9} + 9$.</p></div>

## Input

<p>The first line contains four integers $n, a, b$ and $k$ $(1 \leq n \leq 10^{9}, 1 \leq a, b \leq 10^{9}, 1 \leq k \leq 10^{5})$.</p><p>The second line contains a sequence of length $k$ consisting of characters '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">-</span>'. </p><p>If the $i$-th character (0-indexed) is '<span class="tex-font-style-tt">+</span>', then $s_{i} = 1$, otherwise $s_{i} = -1$.</p><p>Note that only the first $k$ members of the sequence are given, the rest can be obtained using the periodicity property.</p>

## Output

<p>Output a single integer&nbsp;— value of given expression modulo $10^{9} + 9$.</p>





```input1
2 2 3 3
+-+

```




```input2
4 1 5 1
-

```




```output1
7

```




```output2
999999228

```



## Note

<p>In the first example:</p><p>$(\sum \limits_{i=0}^{n} s_{i} a^{n - i} b^{i})$ = $2^{2} 3^{0} - 2^{1} 3^{1} + 2^{0} 3^{2}$ = 7</p><p>In the second example:</p><p>$(\sum \limits_{i=0}^{n} s_{i} a^{n - i} b^{i}) = -1^{4} 5^{0} - 1^{3} 5^{1} - 1^{2} 5^{2} - 1^{1} 5^{3} - 1^{0} 5^{4} = -781 \equiv 999999228 \pmod{10^{9} + 9}$.</p>
