## Description

<div><p>You are given an array $a$ of $n$ integers.</p><p>You need to find the maximum value of $a_{i} | ( a_{j} \&amp; a_{k} )$ over all triplets $(i,j,k)$ such that $i &lt; j &lt; k$.</p><p>Here $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>, and $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>.</p></div><div class="input-specification"><p>The first line of input contains the integer $n$ ($3 \le n \le 10^{6}$), the size of the array $a$.</p><p>Next line contains $n$ space separated integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_{i} \le 2 \cdot 10^{6}$), representing the elements of the array $a$.</p></div><div class="output-specification"><p>Output a single integer, the maximum value of the expression given in the statement. </p></div>

## Input

<p>The first line of input contains the integer $n$ ($3 \le n \le 10^{6}$), the size of the array $a$.</p><p>Next line contains $n$ space separated integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_{i} \le 2 \cdot 10^{6}$), representing the elements of the array $a$.</p>

## Output

<p>Output a single integer, the maximum value of the expression given in the statement. </p>





```input1
3
2 4 6
```




```input2
4
2 8 4 7
```




```output1
6
```




```output2
12
```



## Note

<p>In the first example, the only possible triplet is $(1, 2, 3)$. Hence, the answer is $2 | (4 \&amp; 6) = 6$.</p><p>In the second example, there are $4$ possible triplets: </p><ol> <li> $(1, 2, 3)$, value of which is $2|(8\&amp;4) = 2$. </li><li> $(1, 2, 4)$, value of which is $2|(8\&amp;7) = 2$. </li><li> $(1, 3, 4)$, value of which is $2|(4\&amp;7) = 6$. </li><li> $(2, 3, 4)$, value of which is $8|(4\&amp;7) = 12$. </li></ol><p>The maximum value hence is $12$.</p>
