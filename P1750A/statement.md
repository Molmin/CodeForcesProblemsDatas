## Description

<div><p>You are given a permutation $a_1, a_2, \ldots, a_n$ of size $n$, where each integer from $1$ to $n$ appears <span class="tex-font-style-bf">exactly once</span>.</p><p>You can do the following operation any number of times (possibly, zero):</p><ul> <li> Choose any three indices $i, j, k$ ($1 \le i &lt; j &lt; k \le n$). </li><li> If $a_i &gt; a_k$, replace $a_i$ with $a_i + a_j$. Otherwise, swap $a_j$ and $a_k$. </li></ul><p>Determine whether you can make the array $a$ sorted in non-descending order.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 5000$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 10$) — the length of the array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\dots,a_n$ ($1 \le a_i \le n$, $a_i \neq a_j$ if $i \neq j$) — the elements of the array $a$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the array can be sorted in non-descending order, and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">yEs</span>" and "<span class="tex-font-style-tt">yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 5000$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 10$) — the length of the array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\dots,a_n$ ($1 \le a_i \le n$, $a_i \neq a_j$ if $i \neq j$) — the elements of the array $a$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the array can be sorted in non-descending order, and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">yEs</span>" and "<span class="tex-font-style-tt">yes</span>" will be recognized as a positive response).</p>





```input1|2,3,6,7,10,11,14,15
7
3
1 2 3
3
1 3 2
7
5 3 4 7 6 2 1
7
7 6 5 4 3 2 1
5
2 1 4 5 3
5
2 1 3 4 5
7
1 2 6 7 4 3 5
```




```output1
Yes
Yes
No
No
No
No
Yes
```



## Note

<p>In the first test case, $[1,2,3]$ is already sorted in non-descending order.</p><p>In the second test case, we can choose $i = 1,j = 2,k = 3$. Since $a_1 \le a_3$, swap $a_2$ and $a_3$, the array then becomes $[1,2,3]$, which is sorted in non-descending order.</p><p>In the seventh test case, we can do the following operations successively:</p><ul> <li> Choose $i = 5,j = 6,k = 7$. Since $a_5 \le a_7$, swap $a_6$ and $a_7$, the array then becomes $[1,2,6,7,4,5,3]$. </li><li> Choose $i = 5,j = 6,k = 7$. Since $a_5 &gt; a_7$, replace $a_5$ with $a_5+a_6=9$, the array then becomes $[1,2,6,7,9,5,3]$. </li><li> Choose $i = 2,j = 5,k = 7$. Since $a_2 \le a_7$, swap $a_5$ and $a_7$, the array then becomes $[1,2,6,7,3,5,9]$. </li><li> Choose $i = 2,j = 4,k = 6$. Since $a_2 \le a_6$, swap $a_4$ and $a_6$, the array then becomes $[1,2,6,5,3,7,9]$. </li><li> Choose $i = 1,j = 3,k = 5$. Since $a_1 \le a_5$, swap $a_3$ and $a_5$, the array then becomes $[1,2,3,5,6,7,9]$, which is sorted in non-descending order. </li></ul><p>In the third, the fourth, the fifth and the sixth test cases, it can be shown that the array cannot be sorted in non-descending order.</p>
