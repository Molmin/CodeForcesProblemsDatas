## Description

<div><p>Let's call the following process a transformation of a sequence of length $n$.</p><p>If the sequence is empty, the process ends. Otherwise, append the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> (GCD) of all the elements of the sequence to the result and remove one arbitrary element from the sequence. Thus, when the process ends, we have a sequence of $n$ integers: the greatest common divisors of all the elements in the sequence before each deletion.</p><p>You are given an integer sequence $1, 2, \dots, n$. Find the lexicographically maximum result of its transformation.</p><p>A sequence $a_1, a_2, \ldots, a_n$ is lexicographically larger than a sequence $b_1, b_2, \ldots, b_n$, if there is an index $i$ such that $a_j = b_j$ for all $j &lt; i$, and $a_i &gt; b_i$.</p></div><div class="input-specification"><p>The first and only line of input contains one integer $n$ ($1\le n\le 10^6$).</p></div><div class="output-specification"><p>Output $n$ integers &nbsp;— the lexicographically maximum result of the transformation.</p></div>

## Input

<p>The first and only line of input contains one integer $n$ ($1\le n\le 10^6$).</p>

## Output

<p>Output $n$ integers &nbsp;— the lexicographically maximum result of the transformation.</p>





```input1
3

```




```input2
2

```




```input3
1

```




```output1
1 1 3
```




```output2
1 2
```




```output3
1
```



## Note

<p>In the first sample the answer may be achieved this way:</p><ul> <li> Append GCD$(1, 2, 3) = 1$, remove $2$. </li><li> Append GCD$(1, 3) = 1$, remove $1$. </li><li> Append GCD$(3) = 3$, remove $3$. </li></ul><p>We get the sequence $[1, 1, 3]$ as the result.</p>
