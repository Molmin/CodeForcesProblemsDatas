## Description

<div><p>Suppose you are given two strings $a$ and $b$. You can apply the following operation any number of times: choose any <span class="tex-font-style-bf">contiguous</span> substring of $a$ or $b$, and sort the characters in it in non-descending order. Let $f(a, b)$ the minimum number of operations you have to apply in order to make them equal (or $f(a, b) = 1337$ if it is impossible to make $a$ and $b$ equal using these operations).</p><p>For example: </p><ul> <li> $f(\text{ab}, \text{ab}) = 0$; </li><li> $f(\text{ba}, \text{ab}) = 1$ (in one operation, we can sort the whole first string); </li><li> $f(\text{ebcda}, \text{ecdba}) = 1$ (in one operation, we can sort the substring of the second string starting from the $2$-nd character and ending with the $4$-th character); </li><li> $f(\text{a}, \text{b}) = 1337$. </li></ul><p>You are given $n$ strings $s_1, s_2, \dots, s_k$ having equal length. Calculate $\sum \limits_{i = 1}^{n} \sum\limits_{j = i + 1}^{n} f(s_i, s_j)$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of strings.</p><p>Then $n$ lines follow, each line contains one of the strings $s_i$, consisting of lowercase Latin letters. $|s_1| = |s_2| = \ldots = |s_n|$, and $n \cdot |s_1| \le 2 \cdot 10^5$. All these strings are pairwise distinct.</p></div><div class="output-specification"><p>Print one integer: $\sum \limits_{i = 1}^{n} \sum\limits_{j = i + 1}^{n} f(s_i, s_j)$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of strings.</p><p>Then $n$ lines follow, each line contains one of the strings $s_i$, consisting of lowercase Latin letters. $|s_1| = |s_2| = \ldots = |s_n|$, and $n \cdot |s_1| \le 2 \cdot 10^5$. All these strings are pairwise distinct.</p>

## Output

<p>Print one integer: $\sum \limits_{i = 1}^{n} \sum\limits_{j = i + 1}^{n} f(s_i, s_j)$.</p>





```input1
4
zzz
bac
abc
acb
```




```input2
2
a
b
```




```output1
4015
```




```output2
1337
```


