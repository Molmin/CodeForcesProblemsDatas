## Description

<div><p>Vasya will fancy any number as long as it is an integer power of two. Petya, on the other hand, is very conservative and only likes a single integer $p$ (which may be positive, negative, or zero). To combine their tastes, they invented <span class="tex-font-style-it">$p$-binary numbers</span> of the form $2^x + p$, where $x$ is a <span class="tex-font-style-bf">non-negative</span> integer.</p><p>For example, some $-9$-binary ("minus nine" binary) numbers are: $-8$ (minus eight), $7$ and $1015$ ($-8=2^0-9$, $7=2^4-9$, $1015=2^{10}-9$).</p><p>The boys now use $p$-binary numbers to represent everything. They now face a problem: given a positive integer $n$, what's the smallest number of $p$-binary numbers (not necessarily distinct) they need to represent $n$ as their sum? It may be possible that representation is impossible altogether. Help them solve this problem.</p><p>For example, if $p=0$ we can represent $7$ as $2^0 + 2^1 + 2^2$.</p><p>And if $p=-9$ we can represent $7$ as one number $(2^4-9)$.</p><p>Note that negative $p$-binary numbers are allowed to be in the sum (see the Notes section for an example).</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $p$ ($1 \leq n \leq 10^9$, $-1000 \leq p \leq 1000$).</p></div><div class="output-specification"><p>If it is impossible to represent $n$ as the sum of any number of $p$-binary numbers, print a single integer $-1$. Otherwise, print the smallest possible number of summands.</p></div>

## Input

<p>The only line contains two integers $n$ and $p$ ($1 \leq n \leq 10^9$, $-1000 \leq p \leq 1000$).</p>

## Output

<p>If it is impossible to represent $n$ as the sum of any number of $p$-binary numbers, print a single integer $-1$. Otherwise, print the smallest possible number of summands.</p>





```input1
24 0
```




```input2
24 1
```




```input3
24 -1
```




```input4
4 -7
```




```input5
1 1
```




```output1
2
```




```output2
3
```




```output3
4
```




```output4
2
```




```output5
-1
```



## Note

<p>$0$-binary numbers are just regular binary powers, thus in the first sample case we can represent $24 = (2^4 + 0) + (2^3 + 0)$.</p><p>In the second sample case, we can represent $24 = (2^4 + 1) + (2^2 + 1) + (2^0 + 1)$.</p><p>In the third sample case, we can represent $24 = (2^4 - 1) + (2^2 - 1) + (2^2 - 1) + (2^2 - 1)$. Note that repeated summands are allowed.</p><p>In the fourth sample case, we can represent $4 = (2^4 - 7) + (2^1 - 7)$. Note that the second summand is negative, which is allowed.</p><p>In the fifth sample case, no representation is possible.</p>
