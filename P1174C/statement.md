## Description

<div><p>You're given an integer $n$. For every integer $i$ from $2$ to $n$, assign a positive integer $a_i$ such that the following conditions hold:</p><ul> <li> For any pair of integers $(i,j)$, if $i$ and $j$ are coprime, $a_i \neq a_j$. </li><li> The maximal value of all $a_i$ should be minimized (that is, as small as possible). </li></ul><p>A pair of integers is called <a href="https://en.wikipedia.org/wiki/Coprime_integers">coprime</a> if their <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> is $1$.</p></div><div class="input-specification"><p>The only line contains the integer $n$ ($2 \le n \le 10^5$).</p></div><div class="output-specification"><p>Print $n-1$ integers, $a_2$, $a_3$, $\ldots$, $a_n$ ($1 \leq a_i \leq n$). </p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The only line contains the integer $n$ ($2 \le n \le 10^5$).</p>

## Output

<p>Print $n-1$ integers, $a_2$, $a_3$, $\ldots$, $a_n$ ($1 \leq a_i \leq n$). </p><p>If there are multiple solutions, print any of them.</p>





```input1
4
```




```input2
3
```




```output1
1 2 1
```




```output2
2 1
```



## Note

<p>In the first example, notice that $3$ and $4$ are coprime, so $a_3 \neq a_4$. Also, notice that $a=[1,2,3]$ satisfies the first condition, but it's not a correct answer because its maximal value is $3$.</p>
