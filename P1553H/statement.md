## Description

<div><p>You are given an array $a$ consisting of $n$ distinct elements and an integer $k$. Each element in the array is a non-negative integer not exceeding $2^k-1$.</p><p>Let's define the <span class="tex-font-style-it">XOR distance</span> for a number $x$ as the value of </p><p>$$f(x) = \min\limits_{i = 1}^{n} \min\limits_{j = i + 1}^{n} |(a_i \oplus x) - (a_j \oplus x)|,$$</p><p>where $\oplus$ denotes <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">the bitwise XOR operation</a>.</p><p>For every integer $x$ from $0$ to $2^k-1$, you have to calculate $f(x)$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le 19$; $2 \le n \le 2^k$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2^k-1$). All these integers are distinct.</p></div><div class="output-specification"><p>Print $2^k$ integers. The $i$-th of them should be equal to $f(i-1)$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le 19$; $2 \le n \le 2^k$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2^k-1$). All these integers are distinct.</p>

## Output

<p>Print $2^k$ integers. The $i$-th of them should be equal to $f(i-1)$.</p>





```input1
3 3
6 0 3
```




```input2
3 4
13 4 2
```




```output1
3 1 1 2 2 1 1 3
```




```output2
2 2 6 6 3 1 2 2 2 2 1 3 6 6 2 2
```



## Note

<p>Consider the first example:</p><ul> <li> for $x = 0$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[6, 0, 3]$, and the minimum absolute difference of two elements is $3$; </li><li> for $x = 1$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[7, 1, 2]$, and the minimum absolute difference of two elements is $1$; </li><li> for $x = 2$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[4, 2, 1]$, and the minimum absolute difference of two elements is $1$; </li><li> for $x = 3$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[5, 3, 0]$, and the minimum absolute difference of two elements is $2$; </li><li> for $x = 4$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[2, 4, 7]$, and the minimum absolute difference of two elements is $2$; </li><li> for $x = 5$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[3, 5, 6]$, and the minimum absolute difference of two elements is $1$; </li><li> for $x = 6$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[0, 6, 5]$, and the minimum absolute difference of two elements is $1$; </li><li> for $x = 7$, if we apply bitwise XOR to the elements of the array with $x$, we get the array $[1, 7, 4]$, and the minimum absolute difference of two elements is $3$. </li></ul>
