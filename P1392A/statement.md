## Description

<div><p>Lord Omkar has permitted you to enter the Holy Church of Omkar! To test your worthiness, Omkar gives you a password which you must interpret!</p><p>A password is an array $a$ of $n$ positive integers. You apply the following operation to the array: pick any two adjacent numbers that are not equal to each other and replace them with their sum. Formally, choose an index $i$ such that $1 \leq i &lt; n$ and $a_{i} \neq a_{i+1}$, delete both $a_i$ and $a_{i+1}$ from the array and put $a_{i}+a_{i+1}$ in their place. </p><p>For example, for array $[7, 4, 3, 7]$ you can choose $i = 2$ and the array will become $[7, 4+3, 7] = [7, 7, 7]$. Note that in this array you can't apply this operation anymore.</p><p>Notice that one operation will decrease the size of the password by $1$. What is the shortest possible length of the password after some number (possibly $0$) of operations?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the password.</p><p>The second line of each test case contains $n$ integers $a_{1},a_{2},\dots,a_{n}$ ($1 \leq a_{i} \leq 10^9$)&nbsp;— the initial contents of your password.</p><p>The sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each password, print one integer: the shortest possible length of the password after some number of operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the password.</p><p>The second line of each test case contains $n$ integers $a_{1},a_{2},\dots,a_{n}$ ($1 \leq a_{i} \leq 10^9$)&nbsp;— the initial contents of your password.</p><p>The sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each password, print one integer: the shortest possible length of the password after some number of operations.</p>





```input1
2
4
2 1 3 1
2
420 420
```




```output1
1
2
```



## Note

<p>In the first test case, you can do the following to achieve a length of $1$:</p><p>Pick $i=2$ to get $[2, 4, 1]$</p><p>Pick $i=1$ to get $[6, 1]$</p><p>Pick $i=1$ to get $[7]$</p><p>In the second test case, you can't perform any operations because there is no valid $i$ that satisfies the requirements mentioned above.</p>
