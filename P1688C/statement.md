## Description

<div><div class="epigraph"><div class="epigraph-text">As a human, she can erase history of its entirety. As a <span class="tex-font-style-it">Bai Ze (Hakutaku)</span>, she can create history out of nothingness.</div><div class="epigraph-source">—<span class="tex-font-style-it">Perfect Memento in Strict Sense</span></div></div><p>Keine has the ability to manipulate history. </p><p>The history of Gensokyo is a string $s$ <span class="tex-font-style-bf">of length $1$ initially</span>. To fix the chaos caused by Yukari, she needs to do the following operations $n$ times, for the $i$-th time: </p><ul><li> She chooses a <span class="tex-font-style-bf">non-empty substring</span> $t_{2i-1}$ of $s$.</li><li> She replaces $t_{2i-1}$ with a <span class="tex-font-style-bf">non-empty</span> string, $t_{2i}$. Note that the lengths of strings $t_{2i-1}$ and $t_{2i}$ can be different.</li></ul><p>Note that if $t_{2i-1}$ occurs more than once in $s$, <span class="tex-font-style-bf">exactly one</span> of them will be replaced.</p><p>For example, let $s=$"<span class="tex-font-style-tt">marisa</span>", $t_{2i-1}=$"<span class="tex-font-style-tt">a</span>", and $t_{2i}=$"<span class="tex-font-style-tt">z</span>". After the operation, $s$ becomes "<span class="tex-font-style-tt">mzrisa</span>" or "<span class="tex-font-style-tt">marisz</span>".</p><p>After $n$ operations, Keine got the final string and an operation sequence $t$ of length $2n$. Just as Keine thinks she has finished, Yukari appears again and shuffles the order of $t$. Worse still, Keine forgets the initial history. </p><p>Help Keine find the initial history of Gensokyo!</p><p>Recall that a substring is a sequence of consecutive characters of the string. For example, for string "<span class="tex-font-style-tt">abc</span>" its substrings are: "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">bc</span>" and some others. But the following strings are not its substring: "<span class="tex-font-style-tt">ac</span>", "<span class="tex-font-style-tt">cba</span>", "<span class="tex-font-style-tt">acb</span>".</p><p><span class="tex-font-style-bf">Hacks</span></p><p>You cannot make hacks in this problem.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $T$ ($1 \leq T \leq 10^3$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n &lt; 10 ^ 5$) — the number of operations.</p><p>The next $2n$ lines contains one <span class="tex-font-style-bf">non-empty</span> string $t_{i}$ — the $i$-th string of the shuffled sequence $t$.</p><p>The next line contains one <span class="tex-font-style-bf">non-empty</span> string $s$ — the final string.</p><p>It is guaranteed that the total length of given strings (including $t_i$ and $s$) over all test cases does not exceed $2 \cdot 10 ^ 5$. All given strings consist of lowercase English letters only.</p><p>It is guaranteed that the initial string exists. It can be shown that the initial string is unique.</p></div><div class="output-specification"><p>For each test case, print the initial string in one line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $T$ ($1 \leq T \leq 10^3$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n &lt; 10 ^ 5$) — the number of operations.</p><p>The next $2n$ lines contains one <span class="tex-font-style-bf">non-empty</span> string $t_{i}$ — the $i$-th string of the shuffled sequence $t$.</p><p>The next line contains one <span class="tex-font-style-bf">non-empty</span> string $s$ — the final string.</p><p>It is guaranteed that the total length of given strings (including $t_i$ and $s$) over all test cases does not exceed $2 \cdot 10 ^ 5$. All given strings consist of lowercase English letters only.</p><p>It is guaranteed that the initial string exists. It can be shown that the initial string is unique.</p>

## Output

<p>For each test case, print the initial string in one line.</p>





```input1
2
2
a
ab
b
cd
acd
3
z
a
a
aa
yakumo
ran
yakumoran
```




```output1
a
z
```



## Note

<p>Test case 1:</p><p>Initially $s$ is "<span class="tex-font-style-tt">a</span>".</p><ul><li> In the first operation, Keine chooses "<span class="tex-font-style-tt">a</span>", and replaces it with "<span class="tex-font-style-tt">ab</span>". $s$ becomes "<span class="tex-font-style-tt">ab</span>".</li><li> In the second operation, Keine chooses "<span class="tex-font-style-tt">b</span>", and replaces it with "<span class="tex-font-style-tt">cd</span>". $s$ becomes "<span class="tex-font-style-tt">acd</span>".</li></ul><p>So the final string is "<span class="tex-font-style-tt">acd</span>", and $t=[$"<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">cd</span>"$]$ before being shuffled.</p><p>Test case 2:</p><p>Initially $s$ is "<span class="tex-font-style-tt">z</span>".</p><ul><li> In the first operation, Keine chooses "<span class="tex-font-style-tt">z</span>", and replaces it with "<span class="tex-font-style-tt">aa</span>". $s$ becomes "<span class="tex-font-style-tt">aa</span>".</li><li> In the second operation, Keine chooses "<span class="tex-font-style-tt">a</span>", and replaces it with "<span class="tex-font-style-tt">ran</span>". $s$ becomes "<span class="tex-font-style-tt">aran</span>".</li><li> In the third operation, Keine chooses "<span class="tex-font-style-tt">a</span>", and replaces it with "<span class="tex-font-style-tt">yakumo</span>". $s$ becomes "<span class="tex-font-style-tt">yakumoran</span>".</li></ul><p>So the final string is "<span class="tex-font-style-tt">yakumoran</span>", and $t=[$"<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ran</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">yakumo</span>"$]$ before being shuffled.</p>
