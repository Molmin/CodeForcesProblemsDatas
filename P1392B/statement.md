## Description

<div><p>Being stuck at home, Ray became extremely bored. To pass time, he asks Lord Omkar to use his time bending power: Infinity Clock! However, Lord Omkar will only listen to mortals who can solve the following problem:</p><p>You are given an array $a$ of $n$ integers. You are also given an integer $k$. Lord Omkar wants you to do $k$ operations with this array.</p><p>Define one operation as the following: </p><ol> <li> Set $d$ to be the maximum value of your array. </li><li> For every $i$ from $1$ to $n$, replace $a_{i}$ with $d-a_{i}$. </li></ol><p>The goal is to predict the contents in the array after $k$ operations. Please help Ray determine what the final sequence will look like!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5, 1 \leq k \leq 10^{18}$) – the length of your array and the number of operations to perform.</p><p>The second line of each test case contains $n$ integers $a_{1},a_{2},...,a_{n}$ $(-10^9 \leq a_{i} \leq 10^9)$ – the initial contents of your array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each case, print the final version of array $a$ after $k$ operations described above.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5, 1 \leq k \leq 10^{18}$) – the length of your array and the number of operations to perform.</p><p>The second line of each test case contains $n$ integers $a_{1},a_{2},...,a_{n}$ $(-10^9 \leq a_{i} \leq 10^9)$ – the initial contents of your array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each case, print the final version of array $a$ after $k$ operations described above.</p>





```input1
3
2 1
-199 192
5 19
5 -1 4 2 0
1 2
69
```




```output1
391 0
0 6 1 3 5
0
```



## Note

<p>In the first test case the array changes as follows:</p><ul><li><p>Initially, the array is $[-199, 192]$. $d = 192$.</p></li><li><p>After the operation, the array becomes $[d-(-199), d-192] = [391, 0]$.</p></li></ul>
