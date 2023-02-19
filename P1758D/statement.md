## Description

<div><p>You are given an integer $n$. Find a sequence of $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \dots, a_n$ such that $1 \leq a_i \leq 10^9$ for all $i$ and $$\max(a_1, a_2, \dots, a_n) - \min(a_1, a_2, \dots, a_n)= \sqrt{a_1 + a_2 + \dots + a_n}.$$</p><p>It can be proven that there exists a sequence of <span class="tex-font-style-bf">distinct</span> integers that satisfies all the conditions above.</p></div><div class="input-specification"><p>The first line of input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains one integer $n$ ($2 \leq n \leq 3 \cdot 10^5$)&nbsp;— the length of the sequence you have to find.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ space-separated <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \dots, a_n$ satisfying the conditions in the statement. </p><p>If there are several possible answers, you can output any of them. Please remember that your integers must be <span class="tex-font-style-bf">distinct</span>!</p></div>

## Input

<p>The first line of input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains one integer $n$ ($2 \leq n \leq 3 \cdot 10^5$)&nbsp;— the length of the sequence you have to find.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ space-separated <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \dots, a_n$ satisfying the conditions in the statement. </p><p>If there are several possible answers, you can output any of them. Please remember that your integers must be <span class="tex-font-style-bf">distinct</span>!</p>





```input1|2,4
3
2
5
4
```




```output1
3 1
20 29 18 26 28
25 21 23 31
```



## Note

<p>In the first test case, the maximum is $3$, the minimum is $1$, the sum is $4$, and $3 - 1 = \sqrt{4}$.</p><p>In the second test case, the maximum is $29$, the minimum is $18$, the sum is $121$, and $29-18 = \sqrt{121}$.</p><p>For each test case, the integers are all <span class="tex-font-style-bf">distinct</span>.</p>
