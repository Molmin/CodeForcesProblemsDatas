## Description

<div><p>Mainak has an array $a_1, a_2, \ldots, a_n$ of $n$ positive integers. He will do the following operation to this array <span class="tex-font-style-bf">exactly once</span>:</p><ul> <li> Pick a subsegment of this array and cyclically rotate it by any amount. </li></ul> Formally, he can do the following exactly once:<ul> <li> Pick two integers $l$ and $r$, such that $1 \le l \le r \le n$, and any positive integer $k$. </li><li> Repeat this $k$ times: set $a_l=a_{l+1}, a_{l+1}=a_{l+2}, \ldots, a_{r-1}=a_r, a_r=a_l$ (all changes happen at the same time). </li></ul><p>Mainak wants to <span class="tex-font-style-bf">maximize</span> the value of $(a_n - a_1)$ after exactly one such operation. Determine the maximum value of $(a_n - a_1)$ that he can obtain.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 50$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 999$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the maximum value of $(a_n - a_1)$ that Mainak can obtain by doing the operation <span class="tex-font-style-bf">exactly once</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 50$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 999$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the maximum value of $(a_n - a_1)$ that Mainak can obtain by doing the operation <span class="tex-font-style-bf">exactly once</span>.</p>





```input1|2,3,6,7,10,11
5
6
1 3 9 11 5 7
1
20
3
9 99 999
4
2 1 8 1
3
2 1 5
```




```output1
10
0
990
7
4
```



## Note

<ul><li> In the first test case, we can rotate the subarray from index $3$ to index $6$ by an amount of $2$ (<span class="tex-font-style-it">i.e</span>. choose $l = 3$, $r = 6$ and $k = 2$) to get the optimal array: $$[1, 3, \underline{9, 11, 5, 7}] \longrightarrow [1, 3, \underline{5, 7, 9, 11}]$$ So the answer is $a_n - a_1 = 11 - 1 = 10$.</li><li> In the second testcase, it is optimal to rotate the subarray starting and ending at index $1$ and rotating it by an amount of $2$.</li><li> In the fourth testcase, it is optimal to rotate the subarray starting from index $1$ to index $4$ and rotating it by an amount of $3$. So the answer is $8 - 1 = 7$.</li></ul>
