## Description

<div><p>You're given an array $b$ of length $n$. Let's define another array $a$, also of length $n$, for which $a_i = 2^{b_i}$ ($1 \leq i \leq n$). </p><p>Valerii says that every two non-intersecting subarrays of $a$ have different sums of elements. You want to determine if he is wrong. More formally, you need to determine if there exist four integers $l_1,r_1,l_2,r_2$ that satisfy the following conditions: </p><ul><span> <li> $1 \leq l_1 \leq r_1 \lt l_2 \leq r_2 \leq n$; </li><li> $a_{l_1}+a_{l_1+1}+\ldots+a_{r_1-1}+a_{r_1} = a_{l_2}+a_{l_2+1}+\ldots+a_{r_2-1}+a_{r_2}$. </li></span></ul><p>If such four integers exist, you will prove Valerii wrong. Do they exist?</p><p>An array $c$ is a subarray of an array $d$ if $c$ can be obtained from $d$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of every test case contains a single integer $n$ ($2 \le n \le 1000$).</p><p>The second line of every test case contains $n$ integers $b_1,b_2,\ldots,b_n$ ($0 \le b_i \le 10^9$). </p></div><div class="output-specification"><p>For every test case, if there exist two non-intersecting subarrays in $a$ that have the same sum, output <span class="tex-font-style-tt">YES</span> on a separate line. Otherwise, output <span class="tex-font-style-tt">NO</span> on a separate line. </p><p>Also, note that each letter can be in any case. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of every test case contains a single integer $n$ ($2 \le n \le 1000$).</p><p>The second line of every test case contains $n$ integers $b_1,b_2,\ldots,b_n$ ($0 \le b_i \le 10^9$). </p>

## Output

<p>For every test case, if there exist two non-intersecting subarrays in $a$ that have the same sum, output <span class="tex-font-style-tt">YES</span> on a separate line. Otherwise, output <span class="tex-font-style-tt">NO</span> on a separate line. </p><p>Also, note that each letter can be in any case. </p>





```input1
2
6
4 3 0 1 2 0
2
2 5
```




```output1
YES
NO
```



## Note

<p>In the first case, $a = [16,8,1,2,4,1]$. Choosing $l_1 = 1$, $r_1 = 1$, $l_2 = 2$ and $r_2 = 6$ works because $16 = (8+1+2+4+1)$.</p><p>In the second case, you can verify that there is no way to select to such subarrays.</p>
