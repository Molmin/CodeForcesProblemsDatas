## Description

<div><p>Theofanis has a riddle for you and if you manage to solve it, he will give you a Cypriot snack halloumi for free (Cypriot cheese).</p><p>You are given an integer $n$. You need to find two integers $l$ and $r$ such that $-10^{18} \le l &lt; r \le 10^{18}$ and $l + (l + 1) + \ldots + (r - 1) + r = n$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains a single integer $n$ ($1 \le n \le 10^{18}$).</p></div><div class="output-specification"><p>For each test case, print the two integers $l$ and $r$ such that $-10^{18} \le l &lt; r \le 10^{18}$ and $l + (l + 1) + \ldots + (r - 1) + r = n$. </p><p>It can be proven that an answer always exists. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains a single integer $n$ ($1 \le n \le 10^{18}$).</p>

## Output

<p>For each test case, print the two integers $l$ and $r$ such that $-10^{18} \le l &lt; r \le 10^{18}$ and $l + (l + 1) + \ldots + (r - 1) + r = n$. </p><p>It can be proven that an answer always exists. If there are multiple answers, print any.</p>





```input1
7
1
2
3
6
100
25
3000000000000
```




```output1
0 1
-1 2 
1 2 
1 3 
18 22
-2 7
999999999999 1000000000001
```



## Note

<p>In the first test case, $0 + 1 = 1$.</p><p>In the second test case, $(-1) + 0 + 1 + 2 = 2$.</p><p>In the fourth test case, $1 + 2 + 3 = 6$.</p><p>In the fifth test case, $18 + 19 + 20 + 21 + 22 = 100$.</p><p>In the sixth test case, $(-2) + (-1) + 0 + 1 + 2 + 3 + 4 + 5 + 6 + 7 = 25$.</p>
