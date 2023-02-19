## Description

<div><p>Given $n$, find any array $a_1, a_2, \ldots, a_n$ of integers such that all of the following conditions hold: </p><ul><li><p>$1 \le a_i \le 10^9$ for every $i$ from $1$ to $n$.</p></li><li><p>$a_1 &lt; a_2 &lt; \ldots &lt;a_n$</p></li><li><p>For every $i$ from $2$ to $n$, $a_i$ isn't divisible by $a_{i-1}$</p></li></ul><p>It can be shown that such an array always exists under the constraints of the problem.</p></div><div class="input-specification"><p>The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 1000$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>For each test case print $n$ integers $a_1, a_2, \ldots, a_n$ — the array you found. If there are multiple arrays satisfying all the conditions, print any of them.</p></div>

## Input

<p>The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 1000$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p>

## Output

<p>For each test case print $n$ integers $a_1, a_2, \ldots, a_n$ — the array you found. If there are multiple arrays satisfying all the conditions, print any of them.</p>





```input1
3
1
2
7
```




```output1
1
2 3
111 1111 11111 111111 1111111 11111111 111111111
```



## Note

<p>In the first test case, array $[1]$ satisfies all the conditions.</p><p>In the second test case, array $[2, 3]$ satisfies all the conditions, as $2&lt;3$ and $3$ is not divisible by $2$.</p><p>In the third test case, array $[111, 1111, 11111, 111111, 1111111, 11111111, 111111111]$ satisfies all the conditions, as it's increasing and $a_i$ isn't divisible by $a_{i-1}$ for any $i$ from $2$ to $7$.</p>
