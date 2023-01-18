## Description

<div><p>After learning about polynomial hashing, Heidi decided to learn about shift-xor hashing. In particular, she came across this interesting problem.</p><p>Given a bitstring $y \in \{0,1\}^n$ find out the number of different $k$ ($0 \leq k &lt; n$) such that there exists $x \in \{0,1\}^n$ for which $y = x \oplus \mbox{shift}^k(x).$</p><p>In the above, $\oplus$ is the xor operation and $\mbox{shift}^k$ is the operation of shifting a bitstring cyclically to the right $k$ times. For example, $001 \oplus 111 = 110$ and $\mbox{shift}^3(00010010111000) = 00000010010111$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$), the length of the bitstring $y$.</p><p>The second line contains the bitstring $y$.</p></div><div class="output-specification"><p>Output a single integer: the number of suitable values of $k$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$), the length of the bitstring $y$.</p><p>The second line contains the bitstring $y$.</p>

## Output

<p>Output a single integer: the number of suitable values of $k$.</p>





```input1
4
1010
```




```output1
3
```



## Note

<p>In the first example:</p><ul> <li> $1100\oplus \mbox{shift}^1(1100) = 1010$ </li><li> $1000\oplus \mbox{shift}^2(1000) = 1010$ </li><li> $0110\oplus \mbox{shift}^3(0110) = 1010$ </li></ul><p>There is no $x$ such that $x \oplus x = 1010$, hence the answer is $3$.</p>
