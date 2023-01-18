## Description

<div><p>You are given two strings $s$ and $t$. Both strings have length $n$ and consist of lowercase Latin letters. The characters in the strings are numbered from $1$ to $n$.</p><p>You can successively perform the following move any number of times (possibly, zero):</p><ul> <li> swap any two adjacent (neighboring) characters of $s$ (i.e. for any $i = \{1, 2, \dots, n - 1\}$ you can swap $s_i$ and $s_{i + 1})$. </li></ul><p>You can't apply a move to the string $t$. The moves are applied to the string $s$ one after another.</p><p>Your task is to obtain the string $t$ from the string $s$. Find any way to do it with at most $10^4$ such moves.</p><p><span class="tex-font-style-it">You do not have to minimize the number of moves, just find any sequence of moves of length $10^4$ or less to transform $s$ into $t$.</span></p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 50$) — the length of strings $s$ and $t$.</p><p>The second line of the input contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of the input contains the string $t$ consisting of $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>If it is impossible to obtain the string $t$ using moves, print "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise in the first line print one integer $k$ — the number of moves to transform $s$ to $t$. Note that $k$ must be an integer number between $0$ and $10^4$ inclusive.</p><p>In the second line print $k$ integers $c_j$ ($1 \le c_j &lt; n$), where $c_j$ means that on the $j$-th move you swap characters $s_{c_j}$ and $s_{c_j + 1}$.</p><p>If you do not need to apply any moves, print a single integer $0$ in the first line and either leave the second line empty or do not print it at all.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 50$) — the length of strings $s$ and $t$.</p><p>The second line of the input contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of the input contains the string $t$ consisting of $n$ lowercase Latin letters.</p>

## Output

<p>If it is impossible to obtain the string $t$ using moves, print "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise in the first line print one integer $k$ — the number of moves to transform $s$ to $t$. Note that $k$ must be an integer number between $0$ and $10^4$ inclusive.</p><p>In the second line print $k$ integers $c_j$ ($1 \le c_j &lt; n$), where $c_j$ means that on the $j$-th move you swap characters $s_{c_j}$ and $s_{c_j + 1}$.</p><p>If you do not need to apply any moves, print a single integer $0$ in the first line and either leave the second line empty or do not print it at all.</p>





```input1
6
abcdef
abdfec

```




```input2
4
abcd
accd

```




```output1
4
3 5 4 5 

```




```output2
-1

```



## Note

<p>In the first example the string $s$ changes as follows: "<span class="tex-font-style-tt">abcdef</span>" $\rightarrow$ "<span class="tex-font-style-tt">abdcef</span>" $\rightarrow$ "<span class="tex-font-style-tt">abdcfe</span>" $\rightarrow$ "<span class="tex-font-style-tt">abdfce</span>" $\rightarrow$ "<span class="tex-font-style-tt">abdfec</span>".</p><p>In the second example there is no way to transform the string $s$ into the string $t$ through any allowed moves.</p>
