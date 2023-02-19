## Description

<div><p>You are given an array $a$ of length $n$. Also you are given $m$ distinct positions $p_1, p_2, \ldots, p_m$ ($1 \leq p_i \leq n$).</p><p>A <span class="tex-font-style-bf">non-empty</span> subset of these positions $T$ is randomly selected with equal probability and the following value is calculated: $$\sum_{i=1}^{n} (a_i \cdot \min_{j \in T} \left|i - j\right|).$$ In other word, for each index of the array, $a_i$ and the distance to the closest chosen position are multiplied, and then these values are summed up.</p><p>Find the expected value of this sum.</p><p>This value must be found modulo $998\,244\,353$. More formally, let $M = 998\,244\,353$. It can be shown that the answer can be represented as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \neq 0$ (mod $M$). Output the integer equal to $p \cdot q^{-1}$ (mod $M$). In other words, output such integer $x$ that $0 \leq x &lt; M$ and $x \cdot q = p$ (mod $M$).</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq m \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 998\,244\,353$).</p><p>The third line contains $m$ distinct integers $p_1, p_2, \ldots, p_m$ ($1 \leq p_i \le n$).</p><p>For every $1 \leq i &lt; m$ it is guaranteed that $p_i &lt; p_{i+1}$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq m \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 998\,244\,353$).</p><p>The third line contains $m$ distinct integers $p_1, p_2, \ldots, p_m$ ($1 \leq p_i \le n$).</p><p>For every $1 \leq i &lt; m$ it is guaranteed that $p_i &lt; p_{i+1}$.</p>

## Output

<p>Print a single integer&nbsp;— the answer to the problem.</p>





```input1
4 2
1 2 3 4
1 4
```




```input2
6 6
4 2 4 2 4 2
1 2 3 4 5 6
```




```output1
665496247
```




```output2
855638030
```



## Note

<p>In the first test: </p><ul> <li> If only $1$ is choosen, than the value equals to $1 \cdot 0 + 2 \cdot 1 + 3 \cdot 2 + 4 \cdot 3 = 20$. </li><li> If only $4$ is choosen, than the value equals to $1 \cdot 3 + 2 \cdot 2 + 3 \cdot 1 + 4 \cdot 0 = 10$. </li><li> If both positions are chosen, than the value equals to $1 \cdot 0 + 2 \cdot 1 + 3 \cdot 1 + 4 \cdot 0 = 5$. </li></ul><p>The answer to the problem is $\frac{20 + 10 + 5}{3} = \frac{35}{3} = 665\,496\,247$ (modulo $998\,244\,353$).</p>
