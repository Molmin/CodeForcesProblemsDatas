## Description

<div><p>Creatnx has $n$ mirrors, numbered from $1$ to $n$. Every day, Creatnx asks exactly one mirror "Am I beautiful?". The $i$-th mirror will tell Creatnx that he is beautiful with probability $\frac{p_i}{100}$ for all $1 \le i \le n$.</p><p><span class="tex-font-style-bf">Some mirrors are called checkpoints</span>. Initially, only the $1$st mirror is a checkpoint. It remains a checkpoint all the time.</p><p>Creatnx asks the mirrors one by one, starting from the $1$-st mirror. Every day, if he asks $i$-th mirror, there are two possibilities:</p><ul> <li> The $i$-th mirror tells Creatnx that he is beautiful. In this case, if $i = n$ Creatnx will stop and become happy, otherwise he will continue asking the $i+1$-th mirror next day; </li><li> In the other case, Creatnx will feel upset. The next day, Creatnx will start asking <span class="tex-font-style-bf">from the checkpoint with a maximal number that is less or equal to $i$</span>. </li></ul><p><span class="tex-font-style-bf">There are some changes occur over time: some mirrors become new checkpoints and some mirrors are no longer checkpoints</span>. You are given $q$ queries, each query is represented by an integer $u$: If the $u$-th mirror isn't a checkpoint then we set it as a checkpoint. Otherwise, the $u$-th mirror is no longer a checkpoint.</p><p>After each query, you need to calculate <a href="https://en.wikipedia.org/wiki/Expected_value">the expected number</a> of days until Creatnx becomes happy.</p><p>Each of this numbers should be found by modulo $998244353$. Formally, let $M = 998244353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $q$ ($2 \leq n, q \le 2 \cdot 10^5$) &nbsp;— the number of mirrors and queries.</p><p>The second line contains $n$ integers: $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq 100$).</p><p>Each of $q$ following lines contains a single integer $u$ ($2 \leq u \leq n$)&nbsp;— next query.</p></div><div class="output-specification"><p>Print $q$ numbers&nbsp;– the answers after each query by modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$, $q$ ($2 \leq n, q \le 2 \cdot 10^5$) &nbsp;— the number of mirrors and queries.</p><p>The second line contains $n$ integers: $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq 100$).</p><p>Each of $q$ following lines contains a single integer $u$ ($2 \leq u \leq n$)&nbsp;— next query.</p>

## Output

<p>Print $q$ numbers&nbsp;– the answers after each query by modulo $998244353$.</p>





```input1
2 2
50 50
2
2
```




```input2
5 5
10 20 30 40 50
2
3
4
5
3
```




```output1
4
6
```




```output2
117
665496274
332748143
831870317
499122211
```



## Note

<p>In the first test after the first query, the first and the second mirrors are checkpoints. Creatnx will ask the first mirror until it will say that he is beautiful, after that he will ask the second mirror until it will say that he is beautiful because the second mirror is a checkpoint. After that, he will become happy. Probabilities that the mirrors will say, that he is beautiful are equal to $\frac{1}{2}$. So, the expected number of days, until one mirror will say, that he is beautiful is equal to $2$ and the answer will be equal to $4 = 2 + 2$.</p>
