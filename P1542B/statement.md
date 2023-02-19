## Description

<div><p>There is an infinite set generated as follows:</p><ul> <li> $1$ is in this set. </li><li> If $x$ is in this set, $x \cdot a$ and $x+b$ both are in this set. </li></ul><p>For example, when $a=3$ and $b=6$, the five smallest elements of the set are:</p><ul> <li> $1$, </li><li> $3$ ($1$ is in this set, so $1\cdot a=3$ is in this set), </li><li> $7$ ($1$ is in this set, so $1+b=7$ is in this set), </li><li> $9$ ($3$ is in this set, so $3\cdot a=9$ is in this set), </li><li> $13$ ($7$ is in this set, so $7+b=13$ is in this set). </li></ul><p>Given positive integers $a$, $b$, $n$, determine if $n$ is in this set.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1\leq t\leq 10^5$) — the number of test cases. The description of the test cases follows.</p><p>The only line describing each test case contains three integers $n$, $a$, $b$ ($1\leq n,a,b\leq 10^9$) separated by a single space.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" if $n$ is in this set, and "<span class="tex-font-style-tt">No</span>" otherwise. You can print each letter in any case.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1\leq t\leq 10^5$) — the number of test cases. The description of the test cases follows.</p><p>The only line describing each test case contains three integers $n$, $a$, $b$ ($1\leq n,a,b\leq 10^9$) separated by a single space.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" if $n$ is in this set, and "<span class="tex-font-style-tt">No</span>" otherwise. You can print each letter in any case.</p>





```input1
5
24 3 5
10 3 6
2345 1 4
19260817 394 485
19260817 233 264
```




```output1
Yes
No
Yes
No
Yes
```



## Note

<p>In the first test case, $24$ is generated as follows:</p><ul> <li> $1$ is in this set, so $3$ and $6$ are in this set; </li><li> $3$ is in this set, so $9$ and $8$ are in this set; </li><li> $8$ is in this set, so $24$ and $13$ are in this set. </li></ul><p>Thus we can see $24$ is in this set.</p><p>The five smallest elements of the set in the second test case is described in statements. We can see that $10$ isn't among them.</p>
