## Description

<div><p>Koa the Koala has a binary string $s$ of length $n$. Koa can perform no more than $n-1$ (possibly zero) operations of the following form:</p><p>In one operation Koa selects positions $i$ and $i+1$ for some $i$ with $1 \le i &lt; |s|$ and sets $s_i$ to $max(s_i, s_{i+1})$. Then Koa deletes position $i+1$ from $s$ (after the removal, the remaining parts are concatenated).</p><p>Note that after every operation the length of $s$ decreases by $1$.</p><p>How many different binary strings can Koa obtain by doing no more than $n-1$ (possibly zero) operations modulo $10^9+7$ ($1000000007$)?</p></div><div class="input-specification"><p>The only line of input contains binary string $s$ ($1 \le |s| \le 10^6$). For all $i$ ($1 \le i \le |s|$) $s_i = 0$ or $s_i = 1$.</p></div><div class="output-specification"><p>On a single line print the answer to the problem modulo $10^9+7$ ($1000000007$).</p></div>

## Input

<p>The only line of input contains binary string $s$ ($1 \le |s| \le 10^6$). For all $i$ ($1 \le i \le |s|$) $s_i = 0$ or $s_i = 1$.</p>

## Output

<p>On a single line print the answer to the problem modulo $10^9+7$ ($1000000007$).</p>





```input1
000
```




```input2
0101
```




```input3
0001111
```




```input4
00101100011100
```




```output1
3
```




```output2
6
```




```output3
16
```




```output4
477
```



## Note

<p>In the first sample Koa can obtain binary strings: $0$, $00$ and $000$.</p><p>In the second sample Koa can obtain binary strings: $1$, $01$, $11$, $011$, $101$ and $0101$. For example:</p><ul> <li> to obtain $01$ from $0101$ Koa can operate as follows: $0101 \rightarrow 0(10)1 \rightarrow 011 \rightarrow 0(11) \rightarrow 01$. </li><li> to obtain $11$ from $0101$ Koa can operate as follows: $0101 \rightarrow (01)01 \rightarrow 101 \rightarrow 1(01) \rightarrow 11$. </li></ul><p>Parentheses denote the two positions Koa selected in each operation.</p>
