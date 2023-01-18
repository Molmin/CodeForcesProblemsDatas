## Description

<div><p>The Fair Nut found a string $s$. The string consists of lowercase Latin letters. The Nut is a curious guy, so he wants to find the number of strictly increasing sequences $p_1, p_2, \ldots, p_k$, such that: </p><ol> <li> For each $i$ ($1 \leq i \leq k$), $s_{p_i} =$ <span class="tex-font-style-tt">'a'</span>. </li><li> For each $i$ ($1 \leq i &lt; k$), there is such $j$ that $p_i &lt; j &lt; p_{i + 1}$ and $s_j =$ <span class="tex-font-style-tt">'b'</span>. </li></ol><p>The Nut is upset because he doesn't know how to find the number. Help him.</p><p>This number should be calculated modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains the string $s$ ($1 \leq |s| \leq 10^5$) consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>In a single line print the answer to the problem&nbsp;— the number of such sequences $p_1, p_2, \ldots, p_k$ modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains the string $s$ ($1 \leq |s| \leq 10^5$) consisting of lowercase Latin letters.</p>

## Output

<p>In a single line print the answer to the problem&nbsp;— the number of such sequences $p_1, p_2, \ldots, p_k$ modulo $10^9 + 7$.</p>





```input1
abbaa

```




```input2
baaaa

```




```input3
agaa

```




```output1
5
```




```output2
4
```




```output3
3
```



## Note

<p>In the first example, there are $5$ possible sequences. $[1]$, $[4]$, $[5]$, $[1, 4]$, $[1, 5]$.</p><p>In the second example, there are $4$ possible sequences. $[2]$, $[3]$, $[4]$, $[5]$.</p><p>In the third example, there are $3$ possible sequences. $[1]$, $[3]$, $[4]$.</p>
