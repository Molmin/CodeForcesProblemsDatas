## Description

<div><p>You are given an integer $n$ ($n \ge 0$) represented with $k$ digits in base (radix) $b$. So,</p><p>$$n = a_1 \cdot b^{k-1} + a_2 \cdot b^{k-2} + \ldots a_{k-1} \cdot b + a_k.$$</p><p>For example, if $b=17, k=3$ and $a=[11, 15, 7]$ then $n=11\cdot17^2+15\cdot17+7=3179+255+7=3441$.</p><p>Determine whether $n$ is even or odd.</p></div><div class="input-specification"><p>The first line contains two integers $b$ and $k$ ($2\le b\le 100$, $1\le k\le 10^5$)&nbsp;— the base of the number and the number of digits.</p><p>The second line contains $k$ integers $a_1, a_2, \ldots, a_k$ ($0\le a_i &lt; b$)&nbsp;— the digits of $n$.</p><p>The representation of $n$ contains no unnecessary leading zero. That is, $a_1$ can be equal to $0$ only if $k = 1$.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">even</span>" if $n$ is even, otherwise print "<span class="tex-font-style-tt">odd</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains two integers $b$ and $k$ ($2\le b\le 100$, $1\le k\le 10^5$)&nbsp;— the base of the number and the number of digits.</p><p>The second line contains $k$ integers $a_1, a_2, \ldots, a_k$ ($0\le a_i &lt; b$)&nbsp;— the digits of $n$.</p><p>The representation of $n$ contains no unnecessary leading zero. That is, $a_1$ can be equal to $0$ only if $k = 1$.</p>

## Output

<p>Print "<span class="tex-font-style-tt">even</span>" if $n$ is even, otherwise print "<span class="tex-font-style-tt">odd</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
13 3
3 2 7

```




```input2
10 9
1 2 3 4 5 6 7 8 9

```




```input3
99 5
32 92 85 74 4

```




```input4
2 2
1 0

```




```output1
even

```




```output2
odd

```




```output3
odd

```




```output4
even

```



## Note

<p>In the first example, $n = 3 \cdot 13^2 + 2 \cdot 13 + 7 = 540$, which is even.</p><p>In the second example, $n = 123456789$ is odd.</p><p>In the third example, $n = 32 \cdot 99^4 + 92 \cdot 99^3 + 85 \cdot 99^2 + 74 \cdot 99 + 4 = 3164015155$ is odd.</p><p>In the fourth example $n = 2$.</p>
