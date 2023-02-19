## Description

<div><p>You are given two integers $l$ and $r$ in binary representation. Let $g(x, y)$ be equal to the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all integers from $x$ to $y$ inclusive (that is $x \oplus (x+1) \oplus \dots \oplus (y-1) \oplus y$). Let's define $f(l, r)$ as the maximum of all values of $g(x, y)$ satisfying $l \le x \le y \le r$.</p><p>Output $f(l, r)$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^6$) — the length of the binary representation of $r$.</p><p>The second line contains the binary representation of $l$ — a string of length $n$ consisting of digits $0$ and $1$ ($0 \le l &lt; 2^n$).</p><p>The third line contains the binary representation of $r$ — a string of length $n$ consisting of digits $0$ and $1$ ($0 \le r &lt; 2^n$).</p><p>It is guaranteed that $l \le r$. The binary representation of $r$ does not contain any extra leading zeros (if $r=0$, the binary representation of it consists of a single zero). The binary representation of $l$ is preceded with leading zeros so that its length is equal to $n$.</p></div><div class="output-specification"><p>In a single line output the value of $f(l, r)$ for the given pair of $l$ and $r$ in binary representation without extra leading zeros.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^6$) — the length of the binary representation of $r$.</p><p>The second line contains the binary representation of $l$ — a string of length $n$ consisting of digits $0$ and $1$ ($0 \le l &lt; 2^n$).</p><p>The third line contains the binary representation of $r$ — a string of length $n$ consisting of digits $0$ and $1$ ($0 \le r &lt; 2^n$).</p><p>It is guaranteed that $l \le r$. The binary representation of $r$ does not contain any extra leading zeros (if $r=0$, the binary representation of it consists of a single zero). The binary representation of $l$ is preceded with leading zeros so that its length is equal to $n$.</p>

## Output

<p>In a single line output the value of $f(l, r)$ for the given pair of $l$ and $r$ in binary representation without extra leading zeros.</p>





```input1
7
0010011
1111010
```




```input2
4
1010
1101
```




```output1
1111111
```




```output2
1101
```



## Note

<p>In sample test case $l=19$, $r=122$. $f(x,y)$ is maximal and is equal to $127$, with $x=27$, $y=100$, for example.</p>
