## Description

<div><p>Getting closer and closer to a mathematician, Serval becomes a university student on math major in Japari University. On the Calculus class, his teacher taught him how to calculate the expected length of a random subsegment of a given segment. Then he left a bonus problem as homework, with the award of a garage kit from IOI. The bonus is to extend this problem to the general case as follows.</p><p>You are given a segment with length $l$. We randomly choose $n$ segments by choosing two points (maybe with non-integer coordinates) from the given segment equiprobably and the interval between the two points forms a segment. You are given the number of random segments $n$, and another integer $k$. The $2n$ endpoints of the chosen segments split the segment into $(2n+1)$ intervals. Your task is to calculate the expected total length of those intervals that are covered by at least $k$ segments of the $n$ random segments.</p><p>You should find the answer modulo $998244353$.</p></div><div class="input-specification"><p>First line contains three space-separated positive integers $n$, $k$ and $l$ ($1\leq k \leq n \leq 2000$, $1\leq l\leq 10^9$).</p></div><div class="output-specification"><p>Output one integer&nbsp;— the expected total length of all the intervals covered by at least $k$ segments of the $n$ random segments modulo $998244353$.</p><p>Formally, let $M = 998244353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div>

## Input

<p>First line contains three space-separated positive integers $n$, $k$ and $l$ ($1\leq k \leq n \leq 2000$, $1\leq l\leq 10^9$).</p>

## Output

<p>Output one integer&nbsp;— the expected total length of all the intervals covered by at least $k$ segments of the $n$ random segments modulo $998244353$.</p><p>Formally, let $M = 998244353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p>





```input1
1 1 1
```




```input2
6 2 1
```




```input3
7 5 3
```




```input4
97 31 9984524
```




```output1
332748118
```




```output2
760234711
```




```output3
223383352
```




```output4
267137618
```



## Note

<p>In the first example, the expected total length is $\int_0^1 \int_0^1 |x-y| \,\mathrm{d}x\,\mathrm{d}y = {1\over 3}$, and $3^{-1}$ modulo $998244353$ is $332748118$.</p>
