## Description

<div><p>You are given two arrays $a_0, a_1, \ldots, a_{n - 1}$ and $b_0, b_1, \ldots, b_{m-1}$, and an integer $c$.</p><p>Compute the following sum:</p><p>$$\sum_{i=0}^{n-1} \sum_{j=0}^{m-1} a_i b_j c^{i^2\,j^3}$$</p><p>Since it's value can be really large, print it modulo $490019$.</p></div><div class="input-specification"><p>First line contains three integers $n$, $m$ and $c$ ($1 \le n, m \le 100\,000$, $1 \le c &lt; 490019$).</p><p>Next line contains exactly $n$ integers $a_i$ and defines the array $a$ ($0 \le a_i \le 1000$).</p><p>Last line contains exactly $m$ integers $b_i$ and defines the array $b$ ($0 \le b_i \le 1000$).</p></div><div class="output-specification"><p>Print one integer&nbsp;— value of the sum modulo $490019$.</p></div>

## Input

<p>First line contains three integers $n$, $m$ and $c$ ($1 \le n, m \le 100\,000$, $1 \le c &lt; 490019$).</p><p>Next line contains exactly $n$ integers $a_i$ and defines the array $a$ ($0 \le a_i \le 1000$).</p><p>Last line contains exactly $m$ integers $b_i$ and defines the array $b$ ($0 \le b_i \le 1000$).</p>

## Output

<p>Print one integer&nbsp;— value of the sum modulo $490019$.</p>





```input1
2 2 3
0 1
0 1

```




```input2
3 4 1
1 1 1
1 1 1 1

```




```input3
2 3 3
1 2
3 4 5

```




```output1
3

```




```output2
12

```




```output3
65652

```



## Note

<p>In the first example, the only non-zero summand corresponds to $i = 1$, $j = 1$ and is equal to $1 \cdot 1 \cdot 3^1 = 3$.</p><p>In the second example, all summands are equal to $1$.</p>
