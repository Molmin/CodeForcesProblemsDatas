## Description

<div><p>For the given integer $n$ ($n &gt; 2$) let's write down all the strings of length $n$ which contain $n-2$ letters '<span class="tex-font-style-tt">a</span>' and two letters '<span class="tex-font-style-tt">b</span>' in <span class="tex-font-style-bf">lexicographical</span> (alphabetical) order.</p><p>Recall that the string $s$ of length $n$ is lexicographically less than string $t$ of length $n$, if there exists such $i$ ($1 \le i \le n$), that $s_i &lt; t_i$, and for any $j$ ($1 \le j &lt; i$) $s_j = t_j$. The lexicographic comparison of strings is implemented by the operator <span class="tex-font-style-tt">&lt;</span> in modern programming languages.</p><p>For example, if $n=5$ the strings are (the order does matter):</p><ol> <li> <span class="tex-font-style-tt">aaabb</span> </li><li> <span class="tex-font-style-tt">aabab</span> </li><li> <span class="tex-font-style-tt">aabba</span> </li><li> <span class="tex-font-style-tt">abaab</span> </li><li> <span class="tex-font-style-tt">ababa</span> </li><li> <span class="tex-font-style-tt">abbaa</span> </li><li> <span class="tex-font-style-tt">baaab</span> </li><li> <span class="tex-font-style-tt">baaba</span> </li><li> <span class="tex-font-style-tt">babaa</span> </li><li> <span class="tex-font-style-tt">bbaaa</span> </li></ol><p>It is easy to show that such a list of strings will contain exactly $\frac{n \cdot (n-1)}{2}$ strings.</p><p>You are given $n$ ($n &gt; 2$) and $k$ ($1 \le k \le \frac{n \cdot (n-1)}{2}$). Print the $k$-th string from the list.</p></div><div class="input-specification"><p>The input contains one or more test cases.</p><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test. Then $t$ test cases follow.</p><p>Each test case is written on the the separate line containing two integers $n$ and $k$ ($3 \le n \le 10^5, 1 \le k \le \min(2\cdot10^9, \frac{n \cdot (n-1)}{2})$.</p><p>The sum of values $n$ over all test cases in the test doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print the $k$-th string from the list of all described above strings of length $n$. Strings in the list are sorted lexicographically (alphabetically).</p></div>

## Input

<p>The input contains one or more test cases.</p><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test. Then $t$ test cases follow.</p><p>Each test case is written on the the separate line containing two integers $n$ and $k$ ($3 \le n \le 10^5, 1 \le k \le \min(2\cdot10^9, \frac{n \cdot (n-1)}{2})$.</p><p>The sum of values $n$ over all test cases in the test doesn't exceed $10^5$.</p>

## Output

<p>For each test case print the $k$-th string from the list of all described above strings of length $n$. Strings in the list are sorted lexicographically (alphabetically).</p>





```input1
7
5 1
5 2
5 8
5 10
3 1
3 2
20 100
```




```output1
aaabb
aabab
baaba
bbaaa
abb
bab
aaaaabaaaaabaaaaaaaa
```


