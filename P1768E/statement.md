## Description

<div><p>Consider a permutation$^\dagger$ $p$ of length $3n$. Each time you can do one of the following operations:</p><ul> <li> Sort the first $2n$ elements in increasing order. </li><li> Sort the last $2n$ elements in increasing order. </li></ul><p>We can show that every permutation can be made sorted in increasing order using only these operations. Let's call $f(p)$ the minimum number of these operations needed to make the permutation $p$ sorted in increasing order.</p><p>Given $n$, find the sum of $f(p)$ over all $(3n)!$ permutations $p$ of size $3n$.</p><p>Since the answer could be very large, output it modulo a prime $M$.</p><p>$^\dagger$ A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>The only line of input contains two numbers $n$ and $M$ ($1 \leq n \leq 10^6$, $10^8 \leq M \leq 10^9$). It is guaranteed that $M$ is a prime number.</p></div><div class="output-specification"><p>Output the answer modulo $M$.</p></div>

## Input

<p>The only line of input contains two numbers $n$ and $M$ ($1 \leq n \leq 10^6$, $10^8 \leq M \leq 10^9$). It is guaranteed that $M$ is a prime number.</p>

## Output

<p>Output the answer modulo $M$.</p>





```input1
1 100009067
```




```input2
2 100000357
```




```input3
69 999900997
```




```output1
9
```




```output2
1689
```




```output3
193862705
```



## Note

<p>In the first test case, all the permutations are:</p><ul> <li> $[1, 2, 3]$, which requires $0$ operations; </li><li> $[1, 3, 2]$, which requires $1$ operation; </li><li> $[2, 1, 3]$, which requires $1$ operation; </li><li> $[2, 3, 1]$, which requires $2$ operations; </li><li> $[3, 1, 2]$, which requires $2$ operations; </li><li> $[3, 2, 1]$, which requires $3$ operations. </li></ul><p>Therefore, the answer is $0+1+1+2+2+3=9$.</p>
