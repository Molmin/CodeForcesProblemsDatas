## Description

<div><p>Given $n$ strings, each of length $2$, consisting of lowercase Latin alphabet letters <span class="tex-font-style-bf">from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">k</span></span>', output the number of pairs of indices $(i, j)$ such that $i &lt; j$ and the $i$-th string and the $j$-th string differ in exactly one position.</p><p>In other words, count the number of pairs $(i, j)$ ($i &lt; j$) such that the $i$-th string and the $j$-th string have <span class="tex-font-style-bf">exactly</span> one position $p$ ($1 \leq p \leq 2$) such that ${s_{i}}_{p} \neq {s_{j}}_{p}$.</p><p>The answer may not fit into 32-bit integer type, so you should use 64-bit integers like <span class="tex-font-style-tt">long long</span> in C++ to avoid integer overflow.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the number of strings.</p><p>Then follows $n$ lines, the $i$-th of which containing a single string $s_i$ of length $2$, consisting of lowercase Latin letters <span class="tex-font-style-bf">from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">k</span>'</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the number of pairs $(i, j)$ ($i &lt; j$) such that the $i$-th string and the $j$-th string have <span class="tex-font-style-bf">exactly</span> one position $p$ ($1 \leq p \leq 2$) such that ${s_{i}}_{p} \neq {s_{j}}_{p}$. </p><p>Please note, that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the number of strings.</p><p>Then follows $n$ lines, the $i$-th of which containing a single string $s_i$ of length $2$, consisting of lowercase Latin letters <span class="tex-font-style-bf">from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">k</span>'</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single integer — the number of pairs $(i, j)$ ($i &lt; j$) such that the $i$-th string and the $j$-th string have <span class="tex-font-style-bf">exactly</span> one position $p$ ($1 \leq p \leq 2$) such that ${s_{i}}_{p} \neq {s_{j}}_{p}$. </p><p>Please note, that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p>





```input1
4
6
ab
cb
db
aa
cc
ef
7
aa
bb
cc
ac
ca
bb
aa
4
kk
kk
ab
ab
5
jf
jf
jk
jk
jk
```




```output1
5
6
0
6
```



## Note

<p>For the first test case the pairs that differ in exactly one position are: ("<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">cb</span>"), ("<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">db</span>"), ("<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">aa</span>"), ("<span class="tex-font-style-tt">cb</span>", "<span class="tex-font-style-tt">db</span>") and ("<span class="tex-font-style-tt">cb</span>", "<span class="tex-font-style-tt">cc</span>").</p><p>For the second test case the pairs that differ in exactly one position are: ("<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ac</span>"), ("<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ca</span>"), ("<span class="tex-font-style-tt">cc</span>", "<span class="tex-font-style-tt">ac</span>"), ("<span class="tex-font-style-tt">cc</span>", "<span class="tex-font-style-tt">ca</span>"), ("<span class="tex-font-style-tt">ac</span>", "<span class="tex-font-style-tt">aa</span>") and ("<span class="tex-font-style-tt">ca</span>", "<span class="tex-font-style-tt">aa</span>").</p><p>For the third test case, the are no pairs satisfying the conditions.</p>
