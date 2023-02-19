## Description

<div><p>Nezzar buys his favorite snack&nbsp;— $n$ chocolate bars with lengths $l_1,l_2,\ldots,l_n$. However, chocolate bars might be too long to store them properly! </p><p>In order to solve this problem, Nezzar designs an interesting process to divide them into small pieces. Firstly, Nezzar puts all his chocolate bars into a black box. Then, he will perform the following operation repeatedly until the maximum length over all chocolate bars does not exceed $k$.</p><ul> <li> Nezzar picks a chocolate bar from the box with probability proportional to its length $x$. </li><li> After step $1$, Nezzar uniformly picks a real number $r \in (0,x)$ and divides the chosen chocolate bar into two chocolate bars with lengths $r$ and $x-r$. </li><li> Lastly, he puts those two new chocolate bars into the black box. </li></ul><p>Nezzar now wonders, what is the expected number of operations he will perform to divide his chocolate bars into small pieces.</p><p>It can be shown that the answer can be represented as $\frac{P}{Q}$, where $P$ and $Q$ are coprime integers and $Q \not \equiv 0$ ($\bmod 998\,244\,353$). Print the value of $P\cdot Q^{-1} \mod 998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 50, 1 \le k \le 2000$).</p><p>The second line contains $n$ integers $l_1, l_2, \ldots, l_n$ ($1 \le l_i$, $\sum_{i=1}^{n} l_i \le 2000$).</p></div><div class="output-specification"><p>Print a single integer — the expected number of operations Nezzar will perform to divide his chocolate bars into small pieces modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 50, 1 \le k \le 2000$).</p><p>The second line contains $n$ integers $l_1, l_2, \ldots, l_n$ ($1 \le l_i$, $\sum_{i=1}^{n} l_i \le 2000$).</p>

## Output

<p>Print a single integer — the expected number of operations Nezzar will perform to divide his chocolate bars into small pieces modulo $998\,244\,353$.</p>





```input1
1 1
2
```




```input2
1 1
1
```




```input3
1 5
1234
```




```input4
2 1
2 3
```




```input5
10 33
10 20 30 40 50 60 70 80 90 100
```




```output1
4
```




```output2
0
```




```output3
15630811
```




```output4
476014684
```




```output5
675105648
```


