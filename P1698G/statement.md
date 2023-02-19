## Description

<div><p>There is a binary string $t$ of length $10^{100}$, and initally all of its bits are $\texttt{0}$. You are given a binary string $s$, and perform the following operation some times: </p><ul> <li> Select some substring of $t$, and replace it with its XOR with $s$.$^\dagger$ </li></ul> After several operations, the string $t$ has exactly two bits $\texttt{1}$; that is, there are exactly two distinct indices $p$ and $q$ such that the $p$-th and $q$-th bits of $t$ are $\texttt{1}$, and the rest of the bits are $\texttt{0}$. <p>Find the lexicographically largest$^\ddagger$ string $t$ satisfying these constraints, or report that no such string exists.</p><p>$^\dagger$ Formally, choose an index $i$ such that $0 \leq i \leq 10^{100}-|s|$. For all $1 \leq j \leq |s|$, if $s_j = \texttt{1}$, then toggle $t_{i+j}$. That is, if $t_{i+j}=\texttt{0}$, set $t_{i+j}=\texttt{1}$. Otherwise if $t_{i+j}=\texttt{1}$, set $t_{i+j}=\texttt{0}$.</p><p>$^\ddagger$ A binary string $a$ is lexicographically larger than a binary string $b$ of the same length if in the first position where $a$ and $b$ differ, the string $a$ has a bit $\texttt{1}$ and the corresponding bit in $b$ is $\texttt{0}$.</p></div><div class="input-specification"><p>The only line of each test contains a single binary string $s$ ($1 \leq |s| \leq 35$).</p></div><div class="output-specification"><p>If no string $t$ exists as described in the statement, output <span class="tex-font-style-tt">-1</span>. Otherwise, output the integers $p$ and $q$ ($1 \leq p &lt; q \leq 10^{100}$) such that the $p$-th and $q$-th bits of the lexicographically maximal $t$ are $\texttt{1}$.</p></div>

## Input

<p>The only line of each test contains a single binary string $s$ ($1 \leq |s| \leq 35$).</p>

## Output

<p>If no string $t$ exists as described in the statement, output <span class="tex-font-style-tt">-1</span>. Otherwise, output the integers $p$ and $q$ ($1 \leq p &lt; q \leq 10^{100}$) such that the $p$-th and $q$-th bits of the lexicographically maximal $t$ are $\texttt{1}$.</p>





```input1
1
```




```input2
001
```




```input3
1111
```




```input4
00000
```




```input5
00000111110000011111000001111101010
```




```output1
1 2
```




```output2
3 4
```




```output3
1 5
```




```output4
-1
```




```output5
6 37452687
```



## Note

<p>In the first test, you can perform the following operations. $$\texttt{00000}\ldots \to \color{red}{\texttt{1}}\texttt{0000}\ldots \to \texttt{1}\color{red}{\texttt{1}}\texttt{000}\ldots$$</p><p>In the second test, you can perform the following operations. $$\texttt{00000}\ldots \to \color{red}{\texttt{001}}\texttt{00}\ldots \to \texttt{0}\color{red}{\texttt{011}}\texttt{0}\ldots$$</p><p>In the third test, you can perform the following operations. $$\texttt{00000}\ldots \to \color{red}{\texttt{1111}}\texttt{0}\ldots \to \texttt{1}\color{red}{\texttt{0001}}\ldots$$</p><p>It can be proven that these strings $t$ are the lexicographically largest ones.</p><p>In the fourth test, you can't make a single bit $\texttt{1}$, so it is impossible.</p>
