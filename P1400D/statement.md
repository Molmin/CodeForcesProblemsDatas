## Description

<div><p>You are given an array $a_1, a_2 \dots a_n$. Calculate the number of tuples $(i, j, k, l)$ such that: </p><ul> <li> $1 \le i &lt; j &lt; k &lt; l \le n$; </li><li> $a_i = a_k$ and $a_j = a_l$; </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($4 \le n \le 3000$)&nbsp;— the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the array $a$.</p><p>It's guaranteed that the sum of $n$ in one test doesn't exceed $3000$.</p></div><div class="output-specification"><p>For each test case, print the number of described tuples.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($4 \le n \le 3000$)&nbsp;— the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the array $a$.</p><p>It's guaranteed that the sum of $n$ in one test doesn't exceed $3000$.</p>

## Output

<p>For each test case, print the number of described tuples.</p>





```input1
2
5
2 2 2 2 2
6
1 3 3 1 2 3
```




```output1
5
2
```



## Note

<p>In the first test case, for any four indices $i &lt; j &lt; k &lt; l$ are valid, so the answer is the number of tuples.</p><p>In the second test case, there are $2$ valid tuples: </p><ul> <li> $(1, 2, 4, 6)$: $a_1 = a_4$ and $a_2 = a_6$; </li><li> $(1, 3, 4, 6)$: $a_1 = a_4$ and $a_3 = a_6$. </li></ul>
