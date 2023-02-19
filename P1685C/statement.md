## Description

<div><p>Alina has a bracket sequence $s$ of length $2n$, consisting of $n$ opening brackets <span class="tex-font-style-tt">'('</span> and $n$ closing brackets <span class="tex-font-style-tt">')'</span>. As she likes balance, she wants to turn this bracket sequence into a balanced bracket sequence.</p><p>In one operation, she can reverse any substring of $s$.</p><p>What's the smallest number of operations that she needs to turn $s$ into a balanced bracket sequence? It can be shown that it's always possible in at most $n$ operations.</p><p>As a reminder, a sequence of brackets is called balanced if one can turn it into a valid math expression by adding characters <span class="tex-font-style-tt">+</span> and <span class="tex-font-style-tt">1</span>. For example, sequences <span class="tex-font-style-tt">(())()</span>, <span class="tex-font-style-tt">()</span>, and <span class="tex-font-style-tt">(()(()))</span> are balanced, while <span class="tex-font-style-tt">)(</span>, <span class="tex-font-style-tt">(()</span>, and <span class="tex-font-style-tt">(()))(</span> are not.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains a string $s$ of length $2n$, consisting of $n$ opening and $n$ closing brackets.</p><p>The sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, in the first line output a single integer $k$ $(0 \le k \le n)$ &nbsp;— the smallest number of operations required.</p><p>The $i$-th of the next $k$ lines should contain two integers $l_i, r_i$ ($1 \le l_i \le r_i \le 2n$), indicating that in the $i$-th operation, Alina will reverse the substring $s_ls_{l+1} \ldots s_{r-1}s_r$. Here the numeration starts from $1$.</p><p>If there are multiple sequences of operations with the smallest length which transform the sequence into a balanced one, you can output any of them.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains a string $s$ of length $2n$, consisting of $n$ opening and $n$ closing brackets.</p><p>The sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, in the first line output a single integer $k$ $(0 \le k \le n)$ &nbsp;— the smallest number of operations required.</p><p>The $i$-th of the next $k$ lines should contain two integers $l_i, r_i$ ($1 \le l_i \le r_i \le 2n$), indicating that in the $i$-th operation, Alina will reverse the substring $s_ls_{l+1} \ldots s_{r-1}s_r$. Here the numeration starts from $1$.</p><p>If there are multiple sequences of operations with the smallest length which transform the sequence into a balanced one, you can output any of them.</p>





```input1|2,3,6,7
3
2
(())
5
())((()))(
6
())((()))(()
```




```output1
0
2
3 4
9 10
1
2 11
```



## Note

<p>In the first test case, the string is already balanced.</p><p>In the second test case, the string will be transformed as follows: <span class="tex-font-style-tt">())((()))(</span> $\to$ <span class="tex-font-style-tt">()()(()))(</span> $\to$ <span class="tex-font-style-tt">()()(())()</span>, where the last string is balanced.</p><p>In the third test case, the string will be transformed to <span class="tex-font-style-tt">((()))((()))</span>, which is balanced.</p>
