## Description

<div><p>Let $a$ and $b$ be some non-negative integers. Let's define <span class="tex-font-style-it">strange addition</span> of $a$ and $b$ as following:</p><ol> <li> write down the numbers one under another and align them by their least significant digit; </li><li> add them up digit by digit and concatenate the respective sums together. </li></ol><p>Assume that both numbers have an infinite number of leading zeros.</p><p>For example, let's take a look at a <span class="tex-font-style-it">strange addition</span> of numbers $3248$ and $908$:</p><center> <img class="tex-graphics" src="file://T27apMGp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a string $c$, consisting of $n$ digits from $0$ to $9$. You are also given $m$ updates of form: </p><ul> <li> $x~d$&nbsp;— replace the digit at the $x$-th position of $c$ with a digit $d$. </li></ul><p>Note that string $c$ might have leading zeros at any point of time.</p><p>After each update print the number of pairs $(a, b)$ such that both $a$ and $b$ are non-negative integers and the result of a <span class="tex-font-style-it">strange addition</span> of $a$ and $b$ is equal to $c$.</p><p>Note that the numbers of pairs can be quite large, so print them modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 5 \cdot 10^5$)&nbsp;— the length of the number $c$ and the number of updates.</p><p>The second line contains a string $c$, consisting of exactly $n$ digits from $0$ to $9$.</p><p>Each of the next $m$ lines contains two integers $x$ and $d$ ($1 \le x \le n$, $0 \le d \le 9$)&nbsp;— the descriptions of updates.</p></div><div class="output-specification"><p>Print $m$ integers&nbsp;— the $i$-th value should be equal to the number of pairs $(a, b)$ such that both $a$ and $b$ are non-negative integers and the result of a <span class="tex-font-style-it">strange addition</span> of $a$ and $b$ is equal to $c$ after $i$ updates are applied.</p><p>Note that the numbers of pairs can be quite large, so print them modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 5 \cdot 10^5$)&nbsp;— the length of the number $c$ and the number of updates.</p><p>The second line contains a string $c$, consisting of exactly $n$ digits from $0$ to $9$.</p><p>Each of the next $m$ lines contains two integers $x$ and $d$ ($1 \le x \le n$, $0 \le d \le 9$)&nbsp;— the descriptions of updates.</p>

## Output

<p>Print $m$ integers&nbsp;— the $i$-th value should be equal to the number of pairs $(a, b)$ such that both $a$ and $b$ are non-negative integers and the result of a <span class="tex-font-style-it">strange addition</span> of $a$ and $b$ is equal to $c$ after $i$ updates are applied.</p><p>Note that the numbers of pairs can be quite large, so print them modulo $998244353$.</p>





```input1
2 3
14
2 4
2 1
1 0
```




```output1
15
12
2
```



## Note

<p>After the first update $c$ is equal to $14$. The pairs that sum up to $14$ are: $(0, 14)$, $(1, 13)$, $(2, 12)$, $(3, 11)$, $(4, 10)$, $(5, 9)$, $(6, 8)$, $(7, 7)$, $(8, 6)$, $(9, 5)$, $(10, 4)$, $(11, 3)$, $(12, 2)$, $(13, 1)$, $(14, 0)$.</p><p>After the second update $c$ is equal to $11$.</p><p>After the third update $c$ is equal to $01$.</p>
