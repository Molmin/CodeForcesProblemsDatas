## Description

<div><p>In modern cryptography much is tied to the algorithmic complexity of solving several problems. One of such problems is a discrete logarithm problem. It is formulated as follows: </p><center> Let's fix a <a href="https://en.wikipedia.org/wiki/Finite_field">finite field</a> and two it's elements $a$ and $b$. One need to fun such $x$ that $a^x = b$ or detect there is no such x. </center><p>It is most likely that modern mankind cannot solve the problem of discrete logarithm for a sufficiently large field size. For example, for a field of residues modulo prime number, primes of 1024 or 2048 bits are considered to be safe. However, calculations with such large numbers can place a significant load on servers that perform cryptographic operations. For this reason, instead of a simple module residue field, more complex fields are often used. For such field no fast algorithms that use a field structure are known, smaller fields can be used and operations can be properly optimized. </p><p>Developer Nikolai does not trust the generally accepted methods, so he wants to invent his own. Recently, he read about a very strange field&nbsp;— <a href="https://en.wikipedia.org/wiki/Nimber">nimbers</a>, and thinks it's a great fit for the purpose. </p><p>The field of nimbers is defined on a set of integers from 0 to $2^{2^k} - 1$ for some positive integer $k$ . Bitwise exclusive or ($\oplus$) operation is used as addition. One of ways to define multiplication operation ($\odot$) is following properties: </p><ul> <li> $0 \odot a = a \odot 0 = 0$ </li><li> $1 \odot a = a \odot 1 = a$ </li><li> $a \odot b = b \odot a$ </li><li> $a \odot (b \odot c)= (a \odot b) \odot c$ </li><li> $a \odot (b \oplus c) = (a \odot b) \oplus (a \odot c)$ </li><li> If $a = 2^{2^n}$ for some integer $n &gt; 0$, and $b &lt; a$, then $a \odot b = a \cdot b$. </li><li> If $a = 2^{2^n}$ for some integer $n &gt; 0$, then $a \odot a = \frac{3}{2}\cdot a$. </li></ul><p>For example: </p><ul> <li> $ 4 \odot 4 = 6$ </li><li> $ 8 \odot 8 = 4 \odot 2 \odot 4 \odot 2 = 4 \odot 4 \odot 2 \odot 2 = 6 \odot 3 = (4 \oplus 2) \odot 3 = (4 \odot 3) \oplus (2 \odot (2 \oplus 1)) = (4 \odot 3) \oplus (2 \odot 2) \oplus (2 \odot 1) = 12 \oplus 3 \oplus 2 = 13.$ </li><li> $32 \odot 64 = (16 \odot 2) \odot (16 \odot 4) = (16 \odot 16) \odot (2 \odot 4) = 24 \odot 8 = (16 \oplus 8) \odot 8 = (16 \odot 8) \oplus (8 \odot 8) = 128 \oplus 13 = 141$ </li><li> $5 \odot 6 = (4 \oplus 1) \odot (4 \oplus 2) = (4\odot 4) \oplus (4 \odot 2) \oplus (4 \odot 1) \oplus (1 \odot 2) = 6 \oplus 8 \oplus 4 \oplus 2 = 8$ </li></ul><p>Formally, this algorithm can be described by following pseudo-code. </p><pre class="lstlisting"><code class="prettyprint">multiply(a, b) {<br>   ans = 0<br>   for p1 in bits(a)       // numbers of bits of a equal to one<br>       for p2 in bits(b)   // numbers of bits of b equal to one<br>          ans = ans xor multiply_powers_of_2(1 &lt;&lt; p1, 1 &lt;&lt; p2)<br>   return ans;<br>}<br>multiply_powers_of_2(a, b) {<br>    if (a == 1 or b == 1) return a * b<br>    n = maximal value, such 2^{2^{n}} &lt;= max(a, b)<br>    power = 2^{2^{n}};<br>    if (a &gt;= power and b &gt;= power) {<br>        return multiply(power * 3 / 2, multiply_powers_of_2(a / power, b / power))<br>    } else if (a &gt;= power) {<br>        return multiply_powers_of_2(a / power, b) * power<br>    } else {<br>        return multiply_powers_of_2(a, b / power) * power<br>    }<br>}<br></code></pre><p>It can be shown, that this operations really forms a field. Moreover, than can make sense as game theory operations, but that's not related to problem much. With the help of appropriate caching and grouping of operations, it is possible to calculate the product quickly enough, which is important to improve speed of the cryptoalgorithm. More formal definitions as well as additional properties can be clarified in the wikipedia article at <a href="https://en.wikipedia.org/wiki/Nimber">link</a>. The authors of the task hope that the properties listed in the statement should be enough for the solution. </p><p>Powering for such muliplication is defined in same way, formally $a^{\odot k} = \underbrace{a \odot a \odot \cdots \odot a}_{k~\texttt{times}}$.</p><p>You need to analyze the proposed scheme strength. For pairs of numbers $a$ and $b$ you need to find such $x$, that $a^{\odot x} = b$, or determine that it doesn't exist. </p></div><div class="input-specification"><p>In the first line of input there is single integer $t$ ($1 \le t \le 100$) — number of pairs, for which you need to find the discrete logarithm.</p><p>In each of next $t$ line there is a pair of integers $a$ $b$ ($1 \le a, b &lt; 2^{64}$). </p></div><div class="output-specification"><p>For each pair you should print one integer $x$ ($0 \le x &lt; 2^{64}$), such that $a^{\odot x} = b$, or -1 if no such x exists. It can be shown, that if any such $x$ exists, there is one inside given bounds. If there are several good values, you can output any of them. </p></div>

## Input

<p>In the first line of input there is single integer $t$ ($1 \le t \le 100$) — number of pairs, for which you need to find the discrete logarithm.</p><p>In each of next $t$ line there is a pair of integers $a$ $b$ ($1 \le a, b &lt; 2^{64}$). </p>

## Output

<p>For each pair you should print one integer $x$ ($0 \le x &lt; 2^{64}$), such that $a^{\odot x} = b$, or -1 if no such x exists. It can be shown, that if any such $x$ exists, there is one inside given bounds. If there are several good values, you can output any of them. </p>





```input1
7
2 2
1 1
2 3
8 10
8 2
321321321321 2
123214213213 4356903202345442785
```




```output1
1
1
2
4
-1
6148914691236517205
68943624821423112
```


