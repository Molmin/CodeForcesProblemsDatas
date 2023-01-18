## Description

<div><p>You are given a string $s$. You can build new string $p$ from $s$ using the following operation <span class="tex-font-style-bf">no more than two times</span>: </p><ol> <li> choose any subsequence $s_{i_1}, s_{i_2}, \dots, s_{i_k}$ where $1 \le i_1 &lt; i_2 &lt; \dots &lt; i_k \le |s|$; </li><li> erase the chosen subsequence from $s$ ($s$ can become empty); </li><li> concatenate chosen subsequence to the right of the string $p$ (in other words, $p = p + s_{i_1}s_{i_2}\dots s_{i_k}$). </li></ol><p>Of course, initially the string $p$ is empty. </p><p>For example, let $s = \text{ababcd}$. At first, let's choose subsequence $s_1 s_4 s_5 = \text{abc}$ — we will get $s = \text{bad}$ and $p = \text{abc}$. At second, let's choose $s_1 s_2 = \text{ba}$ — we will get $s = \text{d}$ and $p = \text{abcba}$. So we can build $\text{abcba}$ from $\text{ababcd}$.</p><p>Can you build a given string $t$ using the algorithm above?</p></div><div class="input-specification"><p>The first line contains the single integer $T$ ($1 \le T \le 100$) — the number of test cases.</p><p>Next $2T$ lines contain test cases — two per test case. The first line contains string $s$ consisting of lowercase Latin letters ($1 \le |s| \le 400$) — the initial string.</p><p>The second line contains string $t$ consisting of lowercase Latin letters ($1 \le |t| \le |s|$) — the string you'd like to build.</p><p><span class="tex-font-style-it">It's guaranteed that the total length of strings $s$ doesn't exceed $400$.</span></p></div><div class="output-specification"><p>Print $T$ answers — one per test case. Print <span class="tex-font-style-tt">YES</span> (case insensitive) if it's possible to build $t$ and <span class="tex-font-style-tt">NO</span> (case insensitive) otherwise.</p></div>

## Input

<p>The first line contains the single integer $T$ ($1 \le T \le 100$) — the number of test cases.</p><p>Next $2T$ lines contain test cases — two per test case. The first line contains string $s$ consisting of lowercase Latin letters ($1 \le |s| \le 400$) — the initial string.</p><p>The second line contains string $t$ consisting of lowercase Latin letters ($1 \le |t| \le |s|$) — the string you'd like to build.</p><p><span class="tex-font-style-it">It's guaranteed that the total length of strings $s$ doesn't exceed $400$.</span></p>

## Output

<p>Print $T$ answers — one per test case. Print <span class="tex-font-style-tt">YES</span> (case insensitive) if it's possible to build $t$ and <span class="tex-font-style-tt">NO</span> (case insensitive) otherwise.</p>





```input1
4
ababcd
abcba
a
b
defi
fed
xyz
x
```




```output1
YES
NO
NO
YES
```


