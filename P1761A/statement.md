## Description

<div><p>You are given three integers $n$, $a$, and $b$. Determine if there exist two permutations $p$ and $q$ of length $n$, for which the following conditions hold:</p><ul> <li> The length of the longest common prefix of $p$ and $q$ is $a$. </li><li> The length of the longest common suffix of $p$ and $q$ is $b$. </li></ul><p>A permutation of length $n$ is an array containing each integer from $1$ to $n$ exactly once. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\leq t\leq 10^4$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains three integers $n$, $a$, and $b$ ($1\leq a,b\leq n\leq 100$).</p></div><div class="output-specification"><p>For each test case, if such a pair of permutations exists, output "<span class="tex-font-style-tt">Yes</span>"; otherwise, output "<span class="tex-font-style-tt">No</span>". You can output each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\leq t\leq 10^4$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains three integers $n$, $a$, and $b$ ($1\leq a,b\leq n\leq 100$).</p>

## Output

<p>For each test case, if such a pair of permutations exists, output "<span class="tex-font-style-tt">Yes</span>"; otherwise, output "<span class="tex-font-style-tt">No</span>". You can output each letter in any case (upper or lower).</p>





```input1|2,4
4
1 1 1
2 1 2
3 1 1
4 1 1
```




```output1
Yes
No
No
Yes
```



## Note

<p>In the first test case, $[1]$ and $[1]$ form a valid pair.</p><p>In the second test case and the third case, we can show that such a pair of permutations doesn't exist.</p><p>In the fourth test case, $[1,2,3,4]$ and $[1,3,2,4]$ form a valid pair.</p>
