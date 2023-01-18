## Description

<div><p>Creatnx has $n$ mirrors, numbered from $1$ to $n$. Every day, Creatnx asks exactly one mirror "Am I beautiful?". The $i$-th mirror will tell Creatnx that he is beautiful with probability $\frac{p_i}{100}$ for all $1 \le i \le n$.</p><p>Creatnx asks the mirrors one by one, starting from the $1$-st mirror. Every day, if he asks $i$-th mirror, there are two possibilities:</p><ul> <li> The $i$-th mirror tells Creatnx that he is beautiful. In this case, if $i = n$ Creatnx will stop and become happy, otherwise he will continue asking the $i+1$-th mirror next day; </li><li> In the other case, Creatnx will feel upset. The next day, Creatnx will start asking from the $1$-st mirror again. </li></ul><p>You need to calculate <a href="https://en.wikipedia.org/wiki/Expected_value">the expected number</a> of days until Creatnx becomes happy.</p><p>This number should be found by modulo $998244353$. Formally, let $M = 998244353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1\le n\le 2\cdot 10^5$)&nbsp;— the number of mirrors.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq 100$).</p></div><div class="output-specification"><p>Print the answer modulo $998244353$ in a single line.</p></div>

## Input

<p>The first line contains one integer $n$ ($1\le n\le 2\cdot 10^5$)&nbsp;— the number of mirrors.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq 100$).</p>

## Output

<p>Print the answer modulo $998244353$ in a single line.</p>





```input1
1
50
```




```input2
3
10 20 50
```




```output1
2
```




```output2
112
```



## Note

<p>In the first test, there is only one mirror and it tells, that Creatnx is beautiful with probability $\frac{1}{2}$. So, the expected number of days until Creatnx becomes happy is $2$.</p>
