## Description

<div><p>Given an integer $x$. Your task is to find out how many positive integers $n$ ($1 \leq n \leq x$) satisfy $$n \cdot a^n \equiv b \quad (\textrm{mod}\;p),$$ where $a, b, p$ are all known constants.</p></div><div class="input-specification"><p>The only line contains four integers $a,b,p,x$ ($2 \leq p \leq 10^6+3$, $1 \leq a,b &lt; p$, $1 \leq x \leq 10^{12}$). It is guaranteed that $p$ is a prime.</p></div><div class="output-specification"><p>Print a single integer: the number of possible answers $n$.</p></div>

## Input

<p>The only line contains four integers $a,b,p,x$ ($2 \leq p \leq 10^6+3$, $1 \leq a,b &lt; p$, $1 \leq x \leq 10^{12}$). It is guaranteed that $p$ is a prime.</p>

## Output

<p>Print a single integer: the number of possible answers $n$.</p>





```input1
2 3 5 8

```




```input2
4 6 7 13

```




```input3
233 233 10007 1

```




```output1
2

```




```output2
1

```




```output3
1

```



## Note

<p>In the first sample, we can see that $n=2$ and $n=8$ are possible answers.</p>
