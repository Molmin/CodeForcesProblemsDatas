## Description

<div><p>You have a permutation: an array $a = [a_1, a_2, \ldots, a_n]$ of distinct integers from $1$ to $n$. The length of the permutation $n$ is odd.</p><p>You need to sort the permutation in increasing order.</p><p>In one step, you can choose any prefix of the permutation with an odd length and reverse it. Formally, if $a = [a_1, a_2, \ldots, a_n]$, you can choose any odd integer $p$ between $1$ and $n$, inclusive, and set $a$ to $[a_p, a_{p-1}, \ldots, a_1, a_{p+1}, a_{p+2}, \ldots, a_n]$.</p><p>Find a way to sort $a$ using no more than $\frac{5n}{2}$ reversals of the above kind, or determine that such a way doesn't exist. The number of reversals doesn't have to be minimized.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2021$; $n$ is odd)&nbsp;— the length of the permutation.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the permutation itself. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2021$.</p></div><div class="output-specification"><p>For each test case, if it's impossible to sort the given permutation in at most $\frac{5n}{2}$ reversals, print a single integer $-1$.</p><p>Otherwise, print an integer $m$ ($0 \le m \le \frac{5n}{2}$), denoting the number of reversals in your sequence of steps, followed by $m$ integers $p_i$ ($1 \le p_i \le n$; $p_i$ is odd), denoting the lengths of the prefixes of $a$ to be reversed, in chronological order.</p><p>Note that $m$ doesn't have to be minimized. If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2021$; $n$ is odd)&nbsp;— the length of the permutation.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the permutation itself. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2021$.</p>

## Output

<p>For each test case, if it's impossible to sort the given permutation in at most $\frac{5n}{2}$ reversals, print a single integer $-1$.</p><p>Otherwise, print an integer $m$ ($0 \le m \le \frac{5n}{2}$), denoting the number of reversals in your sequence of steps, followed by $m$ integers $p_i$ ($1 \le p_i \le n$; $p_i$ is odd), denoting the lengths of the prefixes of $a$ to be reversed, in chronological order.</p><p>Note that $m$ doesn't have to be minimized. If there are multiple answers, print any.</p>





```input1
3
3
1 2 3
5
3 4 5 2 1
3
2 1 3
```




```output1
4
3 3 3 3
2
3 5
-1
```



## Note

<p>In the first test case, the permutation is already sorted. Any even number of reversals of the length $3$ prefix doesn't change that fact.</p><p>In the second test case, after reversing the prefix of length $3$ the permutation will change to $[5, 4, 3, 2, 1]$, and then after reversing the prefix of length $5$ the permutation will change to $[1, 2, 3, 4, 5]$.</p><p>In the third test case, it's impossible to sort the permutation.</p>
