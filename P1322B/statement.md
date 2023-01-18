## Description

<div><p>Catherine received an array of integers as a gift for March 8. Eventually she grew bored with it, and she started calculated various useless characteristics for it. She succeeded to do it for each one she came up with. But when she came up with another one&nbsp;— <span class="tex-font-style-tt">xor</span> of all pairwise sums of elements in the array, she realized that she couldn't compute it for a very large array, thus she asked for your help. Can you do it? Formally, you need to compute</p><p>$$ (a_1 + a_2) \oplus (a_1 + a_3) \oplus \ldots \oplus (a_1 + a_n) \\ \oplus (a_2 + a_3) \oplus \ldots \oplus (a_2 + a_n) \\ \ldots \\ \oplus (a_{n-1} + a_n) \\ $$</p><p>Here $x \oplus y$ is a bitwise XOR operation (i.e. $x$ <span class="tex-font-style-tt">^</span> $y$ in many modern programming languages). You can read about it in Wikipedia: <a href="https://en.wikipedia.org/wiki/Exclusive_or#Bitwise_operation">https://en.wikipedia.org/wiki/Exclusive_or#Bitwise_operation</a>.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 400\,000$)&nbsp;— the number of integers in the array.</p><p>The second line contains integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^7$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— xor of all pairwise sums of integers in the given array.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 400\,000$)&nbsp;— the number of integers in the array.</p><p>The second line contains integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^7$).</p>

## Output

<p>Print a single integer&nbsp;— xor of all pairwise sums of integers in the given array.</p>





```input1
2
1 2
```




```input2
3
1 2 3
```




```output1
3
```




```output2
2
```



## Note

<p>In the first sample case there is only one sum $1 + 2 = 3$.</p><p>In the second sample case there are three sums: $1 + 2 = 3$, $1 + 3 = 4$, $2 + 3 = 5$. In binary they are represented as $011_2 \oplus 100_2 \oplus 101_2 = 010_2$, thus the answer is 2.</p><p>$\oplus$ is the bitwise xor operation. To define $x \oplus y$, consider binary representations of integers $x$ and $y$. We put the $i$-th bit of the result to be 1 when exactly one of the $i$-th bits of $x$ and $y$ is 1. Otherwise, the $i$-th bit of the result is put to be 0. For example, $0101_2 \, \oplus \, 0011_2 = 0110_2$.</p>
