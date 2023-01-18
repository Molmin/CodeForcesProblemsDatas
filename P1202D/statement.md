## Description

<div><p><span class="tex-font-style-it">The subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements.</span></p><p>You are given an integer $n$. </p><p>You have to find a sequence $s$ consisting of digits $\{1, 3, 7\}$ such that it has exactly $n$ subsequences equal to $1337$.</p><p>For example, sequence $337133377$ has $6$ subsequences equal to $1337$: </p><ol> <li> $337\underline{1}3\underline{3}\underline{3}7\underline{7}$ (you can remove the second and fifth characters); </li><li> $337\underline{1}\underline{3}3\underline{3}7\underline{7}$ (you can remove the third and fifth characters); </li><li> $337\underline{1}\underline{3}\underline{3}37\underline{7}$ (you can remove the fourth and fifth characters); </li><li> $337\underline{1}3\underline{3}\underline{3}\underline{7}7$ (you can remove the second and sixth characters); </li><li> $337\underline{1}\underline{3}3\underline{3}\underline{7}7$ (you can remove the third and sixth characters); </li><li> $337\underline{1}\underline{3}\underline{3}3\underline{7}7$ (you can remove the fourth and sixth characters). </li></ol><p><span class="tex-font-style-bf">Note that the length of the sequence $s$ must not exceed $10^5$.</span></p><p>You have to answer $t$ independent queries.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of queries. </p><p>Next $t$ lines contains a description of queries: the $i$-th line contains one integer $n_i$ ($1 \le n_i \le 10^9$).</p></div><div class="output-specification"><p>For the $i$-th query print one string $s_i$ ($1 \le |s_i| \le 10^5$) consisting of digits $\{1, 3, 7\}$. String $s_i$ must have exactly $n_i$ subsequences $1337$. If there are multiple such strings, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of queries. </p><p>Next $t$ lines contains a description of queries: the $i$-th line contains one integer $n_i$ ($1 \le n_i \le 10^9$).</p>

## Output

<p>For the $i$-th query print one string $s_i$ ($1 \le |s_i| \le 10^5$) consisting of digits $\{1, 3, 7\}$. String $s_i$ must have exactly $n_i$ subsequences $1337$. If there are multiple such strings, print any of them.</p>





```input1
2
6
1
```




```output1
113337
1337
```


