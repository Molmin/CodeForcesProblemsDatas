## Description

<div><p>A frog is initially at position $0$ on the number line. The frog has two positive integers $a$ and $b$. From a position $k$, it can either jump to position $k+a$ or $k-b$.</p><p>Let $f(x)$ be the number of distinct integers the frog can reach if it never jumps on an integer outside the interval $[0, x]$. The frog doesn't need to visit all these integers in one trip, that is, an integer is counted if the frog can somehow reach it if it starts from $0$.</p><p>Given an integer $m$, find $\sum_{i=0}^{m} f(i)$. That is, find the sum of all $f(i)$ for $i$ from $0$ to $m$.</p></div><div class="input-specification"><p>The first line contains three integers $m, a, b$ ($1 \leq m \leq 10^9, 1 \leq a,b \leq 10^5$).</p></div><div class="output-specification"><p>Print a single integer, the desired sum.</p></div>

## Input

<p>The first line contains three integers $m, a, b$ ($1 \leq m \leq 10^9, 1 \leq a,b \leq 10^5$).</p>

## Output

<p>Print a single integer, the desired sum.</p>





```input1
7 5 3
```




```input2
1000000000 1 2019
```




```input3
100 100000 1
```




```input4
6 4 5
```




```output1
19
```




```output2
500000001500000001
```




```output3
101
```




```output4
10
```



## Note

<p>In the first example, we must find $f(0)+f(1)+\ldots+f(7)$. We have $f(0) = 1, f(1) = 1, f(2) = 1, f(3) = 1, f(4) = 1, f(5) = 3, f(6) = 3, f(7) = 8$. The sum of these values is $19$.</p><p>In the second example, we have $f(i) = i+1$, so we want to find $\sum_{i=0}^{10^9} i+1$.</p><p>In the third example, the frog can't make any jumps in any case.</p>
