## Description

<div><p>MKnez wants to construct an array $s_1,s_2, \ldots , s_n$ satisfying the following conditions:</p><ul> <li> Each element is an integer number different from $0$; </li><li> For each pair of adjacent elements their sum is equal to the sum of the whole array. </li></ul><p>More formally, $s_i \neq 0$ must hold for each $1 \leq i \leq n$. Moreover, it must hold that $s_1 + s_2 + \cdots + s_n = s_i + s_{i+1}$ for each $1 \leq i &lt; n$.</p><p>Help MKnez to construct an array with these properties or determine that it does not exist.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 100$). The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($2 \leq n \leq 1000$)&nbsp;— the length of the array.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if an array of length $n$ satisfying the conditions exists. Otherwise, print "<span class="tex-font-style-tt">NO</span>". If the answer is "<span class="tex-font-style-tt">YES</span>", on the next line print a sequence $s_1,s_2, \ldots, s_n$ satisfying the conditions. Each element should be a non-zero integer in the range $[-5000,5000]$, i.&nbsp;e. $-5000 \leq s_i \leq 5000$ and $s_i \neq 0$ should hold for each $1 \leq i \leq n$.</p><p>It can be proved that if a solution exists then there also exists one which satisfies the additional constraints on the range.</p><p>If there are several correct answers, print any of them. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 100$). The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($2 \leq n \leq 1000$)&nbsp;— the length of the array.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if an array of length $n$ satisfying the conditions exists. Otherwise, print "<span class="tex-font-style-tt">NO</span>". If the answer is "<span class="tex-font-style-tt">YES</span>", on the next line print a sequence $s_1,s_2, \ldots, s_n$ satisfying the conditions. Each element should be a non-zero integer in the range $[-5000,5000]$, i.&nbsp;e. $-5000 \leq s_i \leq 5000$ and $s_i \neq 0$ should hold for each $1 \leq i \leq n$.</p><p>It can be proved that if a solution exists then there also exists one which satisfies the additional constraints on the range.</p><p>If there are several correct answers, print any of them. </p>





```input1
2
2
3
```




```output1
YES
9 5
NO
```



## Note

<p>In the first test case, $[9,5]$ is a valid answer since $9+5$ (the sum of the two adjacent elements $s_1+s_2$) is equal to $9+5$ (the sum of all elements). Other solutions include $[6,-9], [-1,-2], [-5000,5000], \ldots$</p><p>For the second test case, let us show why some arrays <span class="tex-font-style-bf">do not</span> satisfy the constraints:</p><ul> <li> $[1,1,1]$ &nbsp;— $s_1+s_2 = 1+1 = 2$ and $s_1+s_2+s_3=1+1+1 = 3$ differ; </li><li> $[1,-1,1]$ &nbsp;— $s_1+s_2=1+(-1)=0$ and $s_1+s_2+s_3=1+(-1)+1 = 1$ differ; </li><li> $[0,0,0]$ &nbsp;— The array $s$ cannot contain a $0$. </li></ul><p>This is <span class="tex-font-style-bf">not</span> a proof, but it can be shown that the answer is "<span class="tex-font-style-tt">NO</span>".</p>
