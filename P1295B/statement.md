## Description

<div><p>You are given string $s$ of length $n$ consisting of <span class="tex-font-style-tt">0</span>-s and <span class="tex-font-style-tt">1</span>-s. You build an infinite string $t$ as a concatenation of an infinite number of strings $s$, or $t = ssss \dots$ For example, if $s =$ <span class="tex-font-style-tt">10010</span>, then $t =$ <span class="tex-font-style-tt">100101001010010</span>...</p><p>Calculate the number of prefixes of $t$ with <span class="tex-font-style-it">balance</span> equal to $x$. The balance of some string $q$ is equal to $cnt_{0, q} - cnt_{1, q}$, where $cnt_{0, q}$ is the number of occurrences of <span class="tex-font-style-tt">0</span> in $q$, and $cnt_{1, q}$ is the number of occurrences of <span class="tex-font-style-tt">1</span> in $q$. The number of such prefixes can be infinite; if it is so, you must say that.</p><p>A prefix is a string consisting of several first letters of a given string, without any reorders. An empty prefix is also a valid prefix. For example, the string "abcd" has 5 prefixes: empty string, "a", "ab", "abc" and "abcd".</p></div><div class="input-specification"><p>The first line contains the single integer $T$ ($1 \le T \le 100$) — the number of test cases.</p><p>Next $2T$ lines contain descriptions of test cases — two lines per test case. The first line contains two integers $n$ and $x$ ($1 \le n \le 10^5$, $-10^9 \le x \le 10^9$) — the length of string $s$ and the desired balance, respectively.</p><p>The second line contains the binary string $s$ ($|s| = n$, $s_i \in \{\text{0}, \text{1}\}$).</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $10^5$.</p></div><div class="output-specification"><p>Print $T$ integers — one per test case. For each test case print the number of prefixes or $-1$ if there is an infinite number of such prefixes.</p></div>

## Input

<p>The first line contains the single integer $T$ ($1 \le T \le 100$) — the number of test cases.</p><p>Next $2T$ lines contain descriptions of test cases — two lines per test case. The first line contains two integers $n$ and $x$ ($1 \le n \le 10^5$, $-10^9 \le x \le 10^9$) — the length of string $s$ and the desired balance, respectively.</p><p>The second line contains the binary string $s$ ($|s| = n$, $s_i \in \{\text{0}, \text{1}\}$).</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $10^5$.</p>

## Output

<p>Print $T$ integers — one per test case. For each test case print the number of prefixes or $-1$ if there is an infinite number of such prefixes.</p>





```input1
4
6 10
010010
5 3
10101
1 0
0
2 0
01
```




```output1
3
0
1
-1
```



## Note

<p>In the first test case, there are 3 good prefixes of $t$: with length $28$, $30$ and $32$.</p>
