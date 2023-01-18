## Description

<div><p>You have received your birthday gifts — $n$ triples of integers! The $i$-th of them is $\lbrace a_{i}, b_{i}, c_{i} \rbrace$. All numbers are greater than or equal to $0$, and strictly smaller than $2^{k}$, where $k$ is a fixed integer.</p><p>One day, you felt tired playing with triples. So you came up with three new integers $x$, $y$, $z$, and then formed $n$ arrays. The $i$-th array consists of $a_i$ repeated $x$ times, $b_i$ repeated $y$ times and $c_i$ repeated $z$ times. Thus, each array has length $(x + y + z)$.</p><p>You want to choose exactly one integer from each array such that the XOR (bitwise exclusive or) of them is equal to $t$. Output the number of ways to choose the numbers for each $t$ between $0$ and $2^{k} - 1$, inclusive, modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 10^{5}$, $1 \leq k \leq 17$)&nbsp;— the number of arrays and the binary length of all numbers.</p><p>The second line contains three integers $x$, $y$, $z$ ($0 \leq x,y,z \leq 10^{9}$)&nbsp;— the integers you chose.</p><p>Then $n$ lines follow. The $i$-th of them contains three integers $a_{i}$, $b_{i}$ and $c_{i}$ ($0 \leq a_{i} , b_{i} , c_{i} \leq 2^{k} - 1$)&nbsp;— the integers forming the $i$-th array.</p></div><div class="output-specification"><p>Print a single line containing $2^{k}$ integers. The $i$-th of them should be the number of ways to choose exactly one integer from each array so that their XOR is equal to $t = i-1$ modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 10^{5}$, $1 \leq k \leq 17$)&nbsp;— the number of arrays and the binary length of all numbers.</p><p>The second line contains three integers $x$, $y$, $z$ ($0 \leq x,y,z \leq 10^{9}$)&nbsp;— the integers you chose.</p><p>Then $n$ lines follow. The $i$-th of them contains three integers $a_{i}$, $b_{i}$ and $c_{i}$ ($0 \leq a_{i} , b_{i} , c_{i} \leq 2^{k} - 1$)&nbsp;— the integers forming the $i$-th array.</p>

## Output

<p>Print a single line containing $2^{k}$ integers. The $i$-th of them should be the number of ways to choose exactly one integer from each array so that their XOR is equal to $t = i-1$ modulo $998244353$.</p>





```input1
1 1
1 2 3
1 0 1
```




```input2
2 2
1 2 1
0 1 2
1 2 3
```




```input3
4 3
1 2 3
1 3 7
0 2 5
1 0 6
3 3 2
```




```output1
2 4
```




```output2
4 2 4 6
```




```output3
198 198 126 126 126 126 198 198
```



## Note

<p>In the first example, the array we formed is $(1, 0, 0, 1, 1, 1)$, we have two choices to get $0$ as the XOR and four choices to get $1$.</p><p>In the second example, two arrays are $(0, 1, 1, 2)$ and $(1, 2, 2, 3)$. There are sixteen $(4 \cdot 4)$ choices in total, $4$ of them ($1 \oplus 1$ and $2 \oplus 2$, two options for each) give $0$, $2$ of them ($0 \oplus 1$ and $2 \oplus 3$) give $1$, $4$ of them ($0 \oplus 2$ and $1 \oplus 3$, two options for each) give $2$, and finally $6$ of them ($0 \oplus 3$, $2 \oplus 1$ and four options for $1 \oplus 2$) give $3$.</p>
