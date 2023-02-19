## Description

<div><p><span class="tex-font-style-it">"Everybody! Doremy's Perfect Math Class is about to start! Come and do your best if you want to have as much IQ as me!" In today's math class, Doremy is teaching everyone subtraction. Now she gives you a quiz to prove that you are paying attention in class.</span></p><p>You are given a set $S$ containing <span class="tex-font-style-bf">positive</span> integers. You may perform the following operation some (possibly zero) number of times:</p><ul> <li> choose two integers $x$ and $y$ from the set $S$ such that $x &gt; y$ and $x - y$ is not in the set $S$. </li><li> add $x-y$ into the set $S$. </li></ul><p>You need to tell Doremy the maximum possible number of integers in $S$ if the operations are performed optimally. It can be proven that this number is finite.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains an integer $n$ ($2 \le n\le 10^5$)&nbsp;— the size of the set $S$.</p><p>The second line contains $n$ integers $a_1,a_2,\dots,a_n$ ($1\le a_1 &lt; a_2 &lt; \cdots &lt; a_n \le 10^9$)&nbsp;— the positive integers in $S$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, you need to output the maximum possible number of integers in $S$. It can be proven that this value is finite.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains an integer $n$ ($2 \le n\le 10^5$)&nbsp;— the size of the set $S$.</p><p>The second line contains $n$ integers $a_1,a_2,\dots,a_n$ ($1\le a_1 &lt; a_2 &lt; \cdots &lt; a_n \le 10^9$)&nbsp;— the positive integers in $S$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, you need to output the maximum possible number of integers in $S$. It can be proven that this value is finite.</p>





```input1|2,3
2
2
1 2
3
5 10 25
```




```output1
2
5
```



## Note

<p>In the first test case, no such $x$ and $y$ exist. The maximum possible number of integers in $S$ is $2$.</p><p>In the second test case,</p><ul> <li> $S=\{5,10,25\}$ at first. You can choose $x=25$, $y=10$, then add $x-y=15$ to the set. </li><li> $S=\{5,10,15,25\}$ now. You can choose $x=25$, $y=5$, then add $x-y=20$ to the set. </li><li> $S=\{5,10,15,20,25\}$ now. You can not perform any operation now. </li></ul><p>After performing all operations, the number of integers in $S$ is $5$. It can be proven that no other sequence of operations allows $S$ to contain more than $5$ integers.</p>
