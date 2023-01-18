## Description

<div><p>You are given integers $n$, $k$. Let's consider the alphabet consisting of $k$ different elements.</p><p>Let <span class="tex-font-style-bf">beauty</span> $f(s)$ of the string $s$ be the number of indexes $i$, $1\le i&lt;|s|$, for which prefix of $s$ of length $i$ equals to suffix of $s$ of length $i$. For example, beauty of the string $abacaba$ equals $2$, as for $i = 1, 3$ prefix and suffix of length $i$ are equal.</p><p>Consider all words of length $n$ in the given alphabet. Find the expected value of $f(s)^2$ of a uniformly chosen at random word. We can show that it can be expressed as $\frac{P}{Q}$, where $P$ and $Q$ are coprime and $Q$ isn't divided by $10^9 + 7$. Output $P\cdot Q^{-1} \bmod 10^9 + 7$.</p></div><div class="input-specification"><p>The first and the only line contains two integers $n$, $k$ ($1\le n \le 10^5$, $1\le k\le 10^9$)&nbsp;— the length of a string and the size of alphabet respectively.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— $P\times Q^{-1} \bmod 10^9 + 7$.</p></div>

## Input

<p>The first and the only line contains two integers $n$, $k$ ($1\le n \le 10^5$, $1\le k\le 10^9$)&nbsp;— the length of a string and the size of alphabet respectively.</p>

## Output

<p>Output a single integer&nbsp;— $P\times Q^{-1} \bmod 10^9 + 7$.</p>





```input1
2 3
```




```input2
1 5
```




```input3
100 1
```




```input4
10 10
```




```output1
333333336
```




```output2
0
```




```output3
9801
```




```output4
412377396
```



## Note

<p>In the first example, there are $9$ words of length $2$ in alphabet of size $3$&nbsp;— $aa$, $ab$, $ac$, $ba$, $bb$, $bc$, $ca$, $cb$, $cc$. $3$ of them have beauty $1$ and $6$ of them have beauty $0$, so the average value is $\frac{1}{3}$.</p><p>In the third example, there is only one such word, and it has beauty $99$, so the average value is $99^2$.</p>
