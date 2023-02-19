## Description

<div><p>Consider an array $a$ of length $n$ with elements numbered from $1$ to $n$. It is possible to remove the $i$-th element of $a$ if $gcd(a_i, i) = 1$, where $gcd$ denotes the greatest common divisor. After an element is removed, the elements to the right are shifted to the left by one position.</p><p>An array $b$ with $n$ integers such that $1 \le b_i \le n - i + 1$ is a <span class="tex-font-style-bf">removal sequence for the array $a$</span> if it is possible to remove all elements of $a$, if you remove the $b_1$-th element, then the $b_2$-th, ..., then the $b_n$-th element. For example, let $a = [42, 314]$:</p><ul> <li> $[1, 1]$ is a removal sequence: when you remove the $1$-st element of the array, the condition $gcd(42, 1) = 1$ holds, and the array becomes $[314]$; when you remove the $1$-st element again, the condition $gcd(314, 1) = 1$ holds, and the array becomes empty. </li><li> $[2, 1]$ is not a removal sequence: when you try to remove the $2$-nd element, the condition $gcd(314, 2) = 1$ is false. </li></ul><p>An array is <span class="tex-font-style-bf">ambiguous</span> if it has <span class="tex-font-style-bf">at least two</span> removal sequences. For example, the array $[1, 2, 5]$ is ambiguous: it has removal sequences $[3, 1, 1]$ and $[1, 2, 1]$. The array $[42, 314]$ is not ambiguous: the only removal sequence it has is $[1, 1]$.</p><p>You are given two integers $n$ and $m$. You have to calculate the number of <span class="tex-font-style-bf">ambiguous</span> arrays $a$ such that the length of $a$ is from $1$ to $n$ and each $a_i$ is an integer from $1$ to $m$.</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $m$ ($2 \le n \le 3 \cdot 10^5$; $1 \le m \le 10^{12}$).</p></div><div class="output-specification"><p>Print one integer — the number of ambiguous arrays $a$ such that the length of $a$ is from $1$ to $n$ and each $a_i$ is an integer from $1$ to $m$. Since the answer can be very large, print it modulo $998244353$.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $m$ ($2 \le n \le 3 \cdot 10^5$; $1 \le m \le 10^{12}$).</p>

## Output

<p>Print one integer — the number of ambiguous arrays $a$ such that the length of $a$ is from $1$ to $n$ and each $a_i$ is an integer from $1$ to $m$. Since the answer can be very large, print it modulo $998244353$.</p>





```input1
2 3
```




```input2
4 2
```




```input3
4 6
```




```input4
1337 424242424242
```




```output1
6
```




```output2
26
```




```output3
1494
```




```output4
119112628
```


