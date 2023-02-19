## Description

<div><p>Vika likes playing with bracket sequences. Today she wants to create a new bracket sequence using the following algorithm. Initially, Vika's sequence is an empty string, and then she will repeat the following actions $n$ times: </p><ul> <li> Choose a place in the current bracket sequence to insert new brackets uniformly at random. If the length of the current sequence is $k$, then there are $k+1$ such places: before the first bracket, between the first and the second brackets, $\ldots$, after the $k$-th bracket. In particular, there is one such place in an empty bracket sequence. </li><li> Choose string "<span class="tex-font-style-tt">()</span>" with probability $p$ or string "<span class="tex-font-style-tt">)(</span>" with probability $1 - p$ and insert it into the chosen place. The length of the bracket sequence will increase by $2$. </li></ul><p>A bracket sequence is called <span class="tex-font-style-it">regular</span> if it is possible to obtain a correct arithmetic expression by inserting characters '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">1</span>' into it. For example, sequences "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">()</span>", and "<span class="tex-font-style-tt">(()(()))</span>" are regular, while "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(()</span>", and "<span class="tex-font-style-tt">(()))(</span>" are not.</p><p>Vika wants to know the probability that her bracket sequence will be a regular one at the end. Help her and find this probability modulo $998\,244\,353$ (see Output section).</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $q$&nbsp;($1 \le n \le 500$; $0 \le q \le 10^4$). Here $n$ is equal to the number of bracket insertion operations, and the probability that Vika chooses string "<span class="tex-font-style-tt">()</span>" on every step of the algorithm is equal to $p = q \cdot 10^{-4}$.</p></div><div class="output-specification"><p>Print the probability that Vika's final bracket sequence will be regular, modulo $998\,244\,353$.</p><p>Formally, let $M = 998\,244\,353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div>

## Input

<p>The only line contains two integers $n$ and $q$&nbsp;($1 \le n \le 500$; $0 \le q \le 10^4$). Here $n$ is equal to the number of bracket insertion operations, and the probability that Vika chooses string "<span class="tex-font-style-tt">()</span>" on every step of the algorithm is equal to $p = q \cdot 10^{-4}$.</p>

## Output

<p>Print the probability that Vika's final bracket sequence will be regular, modulo $998\,244\,353$.</p><p>Formally, let $M = 998\,244\,353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p>





```input1
1 7500
```




```input2
2 6000
```




```input3
5 4000
```




```output1
249561089
```




```output2
519087064
```




```output3
119387743
```



## Note

<p>In the first example, Vika will get a regular bracket sequence <span class="tex-font-style-tt">()</span> with probability $p = \frac{3}{4}$, and she will get an irregular bracket sequence <span class="tex-font-style-tt">)(</span> with probability $1 - p = \frac{1}{4}$. The sought probability is $\frac{3}{4}$, and $249\,561\,089 \cdot 4 \equiv 3 \pmod{998\,244\,353}$.</p><p>In the second example, the sought probability is $\frac{11}{25}$.</p>
