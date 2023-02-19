## Description

<div><p>You are given a <span class="tex-font-style-bf">prime</span> number $n$, and an array of $n$ integers $b_1,b_2,\ldots, b_n$, where $0 \leq b_i &lt; n$ for each $1 \le i \leq n$.</p><p>You have to find a matrix $a$ of size $n \times n$ such that all of the following requirements hold:</p><ul> <li> $0 \le a_{i,j} &lt; n$ for all $1 \le i, j \le n$.<p> </p></li><li> $a_{r_1, c_1} + a_{r_2, c_2} \not\equiv a_{r_1, c_2} + a_{r_2, c_1} \pmod n$ for all positive integers $r_1$, $r_2$, $c_1$, and $c_2$ such that $1 \le r_1 &lt; r_2 \le n$ and $1 \le c_1 &lt; c_2 \le n$.</li><li> $a_{i,i} = b_i$ for all $1 \le i \leq n$. </li></ul><p>Here $x \not \equiv y \pmod m$ denotes that $x$ and $y$ give different remainders when divided by $m$.</p><p>If there are multiple solutions, output any. It can be shown that such a matrix always exists under the given constraints.</p></div><div class="input-specification"><p>The first line contains a single positive integer $n$ ($2 \le n &lt; 350$). </p><p>The second line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i &lt; n$)&nbsp;— the required values on the main diagonal of the matrix.</p><p>It is guaranteed that $n$ is <span class="tex-font-style-bf">prime</span>.</p></div><div class="output-specification"><p>Print $n$ lines. On the $i$-th line, print $n$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, n}$, each separated with a space.</p><p>If there are multiple solutions, output any.</p></div>

## Input

<p>The first line contains a single positive integer $n$ ($2 \le n &lt; 350$). </p><p>The second line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i &lt; n$)&nbsp;— the required values on the main diagonal of the matrix.</p><p>It is guaranteed that $n$ is <span class="tex-font-style-bf">prime</span>.</p>

## Output

<p>Print $n$ lines. On the $i$-th line, print $n$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, n}$, each separated with a space.</p><p>If there are multiple solutions, output any.</p>





```input1
2
0 0
```




```input2
3
1 1 1
```




```input3
5
1 4 1 2 4
```




```output1
0 1 
0 0
```




```output2
1 2 2
1 1 0
1 0 1
```




```output3
1 0 1 3 4
1 4 3 1 0
2 4 1 0 2
1 2 2 2 2
2 2 0 1 4
```



## Note

<p>In the first example, the answer is valid because all entries are non-negative integers less than $n = 2$, and $a_{1,1}+a_{2,2} \not\equiv a_{1,2}+a_{2,1} \pmod 2$ (because $a_{1,1}+a_{2,2} = 0 + 0 \equiv 0 \pmod 2$ and $a_{1,2}+a_{2,1} = 1 + 0 \equiv 1 \pmod 2 $). Moreover, the values on the main diagonals are equal to $0,0$ as required.</p><p>In the second example, the answer is correct because all entries are non-negative integers less than $n = 3$, and the second condition is satisfied for all quadruplets $(r_1, r_2, c_1, c_2)$. For example: </p><ul> <li> When $r_1=1$, $r_2=2$, $c_1=1$ and $c_2=2$, $a_{1,1}+a_{2,2} \not\equiv a_{1,2}+a_{2,1} \pmod 3$ because $a_{1,1}+a_{2,2} = 1 + 1 \equiv 2 \pmod 3$ and $a_{1,2}+a_{2,1} = 2 + 1 \equiv 0 \pmod 3 $. </li><li> When $r_1=2$, $r_2=3$, $c_1=1$, and $c_2=3$, $a_{2,1}+a_{3,3} \not\equiv a_{2,3}+a_{3,1} \pmod 3$ because $a_{2,1}+a_{3,3} = 1 + 1 \equiv 2 \pmod 3$ and $a_{2,3}+a_{3,1} = 0 + 1 \equiv 1 \pmod 3 $. </li></ul> Moreover, the values on the main diagonal are equal to $1,1,1$ as required.
