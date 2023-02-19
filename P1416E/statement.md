## Description

<div><p>One day, <span class="tex-font-style-it">BThero</span> decided to play around with arrays and came up with the following problem:</p><p>You are given an array $a$, which consists of $n$ positive integers. The array is numerated $1$ through $n$. You execute the following procedure <span class="tex-font-style-bf">exactly once</span>:</p><ul> <li> You create a new array $b$ which consists of $2n$ <span class="tex-font-style-bf">positive</span> integers, where for each $1 \le i \le n$ the condition $b_{2i-1}+b_{2i} = a_i$ holds. For example, for the array $a = [6, 8, 2]$ you can create $b = [2, 4, 4, 4, 1, 1]$. </li><li> You merge consecutive equal numbers in $b$. For example, $b = [2, 4, 4, 4, 1, 1]$ becomes $b = [2, 4, 1]$. </li></ul><p>Find and print <span class="tex-font-style-it">the minimum possible</span> value of $|b|$ (size of $b$) which can be achieved at the end of the procedure. It can be shown that under the given constraints there is at least one way to construct $b$.</p></div><div class="input-specification"><p>The first line of the input file contains a single integer $T$ ($1 \le T \le 5 \cdot 10^5$) denoting the number of test cases. The description of $T$ test cases follows.</p><p>The first line of each test contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, ..., $a_n$ ($2 \le a_i \le 10^9$).</p><p>It is guaranteed that $\sum{n}$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line containing one integer — the minimum possible value of $|b|$.</p></div>

## Input

<p>The first line of the input file contains a single integer $T$ ($1 \le T \le 5 \cdot 10^5$) denoting the number of test cases. The description of $T$ test cases follows.</p><p>The first line of each test contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, ..., $a_n$ ($2 \le a_i \le 10^9$).</p><p>It is guaranteed that $\sum{n}$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single line containing one integer — the minimum possible value of $|b|$.</p>





```input1
3
3
6 8 2
1
4
3
5 6 6
```




```output1
3
1
2
```


