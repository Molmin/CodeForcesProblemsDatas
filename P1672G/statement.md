## Description

<div><p>There is a grid with $r$ rows and $c$ columns, where the square on the $i$-th row and $j$-th column has an integer $a_{i, j}$ written on it. Initially, all elements are set to $0$. We are allowed to do the following operation:</p><ul> <li> Choose indices $1 \le i \le r$ and $1 \le j \le c$, then replace all values on the same row or column as $(i, j)$ with the value xor $1$. In other words, for all $a_{x, y}$ where $x=i$ or $y=j$ or both, replace $a_{x, y}$ with $a_{x, y}$ xor $1$. </li></ul><p>You want to form grid $b$ by doing the above operations a finite number of times. However, some elements of $b$ are missing and are replaced with '<span class="tex-font-style-tt">?</span>' instead.</p><p>Let $k$ be the number of '<span class="tex-font-style-tt">?</span>' characters. Among all the $2^k$ ways of filling up the grid $b$ by replacing each '<span class="tex-font-style-tt">?</span>' with '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>', count the number of grids, that can be formed by doing the above operation a finite number of times, starting from the grid filled with $0$. As this number can be large, output it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains two integers $r$ and $c$ ($1 \le r, c \le 2000$) &nbsp;— the number of rows and columns of the grid respectively.</p><p>The $i$-th of the next $r$ lines contain $c$ characters $b_{i, 1}, b_{i, 2}, \ldots, b_{i, c}$ ($b_{i, j} \in \{0, 1, ?\}$).</p></div><div class="output-specification"><p>Print a single integer representing the number of ways to fill up grid $b$ modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $r$ and $c$ ($1 \le r, c \le 2000$) &nbsp;— the number of rows and columns of the grid respectively.</p><p>The $i$-th of the next $r$ lines contain $c$ characters $b_{i, 1}, b_{i, 2}, \ldots, b_{i, c}$ ($b_{i, j} \in \{0, 1, ?\}$).</p>

## Output

<p>Print a single integer representing the number of ways to fill up grid $b$ modulo $998244353$.</p>





```input1
3 3
?10
1??
010
```




```input2
2 3
000
001
```




```input3
1 1
?
```




```input4
6 9
1101011?0
001101?00
101000110
001011010
0101?01??
00?1000?0
```




```output1
1
```




```output2
0
```




```output3
2
```




```output4
8
```



## Note

<p>In the first test case, the only way to fill in the $\texttt{?}$s is to fill it in as such:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">0</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">0</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">1</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">0</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-tt">0</span></td></tr></tbody></table> </center><p>This can be accomplished by doing a single operation by choosing $(i,j)=(2,2)$.</p><p>In the second test case, it can be shown that there is no sequence of operations that can produce that grid.</p>
