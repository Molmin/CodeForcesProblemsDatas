## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$. You can perform operations on the array. In each operation you can choose an integer $i$ ($1 \le i &lt; n$), and swap elements $a_i$ and $a_{i+1}$ of the array, if $a_i + a_{i+1}$ is odd.</p><p>Determine whether it can be sorted in non-decreasing order using this operation any number of times.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1,a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">"Yes"</span> or <span class="tex-font-style-tt">"No"</span> depending on whether you can or can not sort the given array.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">"YES"</span>, <span class="tex-font-style-tt">"Yes"</span>, <span class="tex-font-style-tt">"yes"</span>, <span class="tex-font-style-tt">"yEs"</span> will all be recognized as positive answer).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1,a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">"Yes"</span> or <span class="tex-font-style-tt">"No"</span> depending on whether you can or can not sort the given array.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">"YES"</span>, <span class="tex-font-style-tt">"Yes"</span>, <span class="tex-font-style-tt">"yes"</span>, <span class="tex-font-style-tt">"yEs"</span> will all be recognized as positive answer).</p>





```input1
4
4
1 6 31 14
2
4 2
5
2 9 6 7 10
3
6 6 6
```




```output1
Yes
No
No
Yes
```



## Note

<p>In the first test case, we can simply swap $31$ and $14$ ($31 + 14 = 45$ which is odd) and obtain the non-decreasing array $[1,6,14,31]$.</p><p>In the second test case, the only way we could sort the array is by swapping $4$ and $2$, but this is impossible, since their sum $4 + 2 = 6$ is even.</p><p>In the third test case, there is no way to make the array non-decreasing.</p><p>In the fourth test case, the array is already non-decreasing.</p>
