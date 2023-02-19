## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">We are sum for we are many</span></div><div class="epigraph-source">Some Number</div></div><p><span class="tex-font-style-bf">This version of the problem differs from the next one only in the constraint on $t$. You can make hacks only if both versions of the problem are solved.</span></p><p>You are given two positive integers $l$ and $r$.</p><p>Count the number of distinct triplets of integers $(i, j, k)$ such that $l \le i &lt; j &lt; k \le r$ and $\operatorname{lcm}(i,j,k) \ge i + j + k$.</p><p>Here $\operatorname{lcm}(i, j, k)$ denotes the <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple (LCM)</a> of integers $i$, $j$, and $k$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($\bf{1 \le t \le 5}$). Description of the test cases follows.</p><p>The only line for each test case contains two integers $l$ and $r$ ($1 \le l \le r \le 2 \cdot 10^5$, $l + 2 \le r$).</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the number of suitable triplets.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($\bf{1 \le t \le 5}$). Description of the test cases follows.</p><p>The only line for each test case contains two integers $l$ and $r$ ($1 \le l \le r \le 2 \cdot 10^5$, $l + 2 \le r$).</p>

## Output

<p>For each test case print one integer&nbsp;— the number of suitable triplets.</p>





```input1|2,4,6
5
1 4
3 5
8 86
68 86
6 86868
```




```output1
3
1
78975
969
109229059713337
```



## Note

<p>In the first test case, there are $3$ suitable triplets: </p><ul> <li> $(1,2,3)$, </li><li> $(1,3,4)$, </li><li> $(2,3,4)$. </li></ul><p>In the second test case, there is $1$ suitable triplet: </p><ul> <li> $(3,4,5)$. </li></ul>
