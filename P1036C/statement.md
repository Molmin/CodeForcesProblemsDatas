## Description

<div><p>Let's call some positive integer <span class="tex-font-style-it">classy</span> if its decimal representation contains no more than $3$ non-zero digits. For example, numbers $4$, $200000$, $10203$ are <span class="tex-font-style-it">classy</span> and numbers $4231$, $102306$, $7277420000$ are not.</p><p>You are given a segment $[L; R]$. Count the number of <span class="tex-font-style-it">classy</span> integers $x$ such that $L \le x \le R$.</p><p>Each testcase contains several segments, for each of them you are required to solve the problem separately.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 10^4$) — the number of segments in a testcase.</p><p>Each of the next $T$ lines contains two integers $L_i$ and $R_i$ ($1 \le L_i \le R_i \le 10^{18}$).</p></div><div class="output-specification"><p>Print $T$ lines — the $i$-th line should contain the number of <span class="tex-font-style-it">classy</span> integers on a segment $[L_i; R_i]$.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 10^4$) — the number of segments in a testcase.</p><p>Each of the next $T$ lines contains two integers $L_i$ and $R_i$ ($1 \le L_i \le R_i \le 10^{18}$).</p>

## Output

<p>Print $T$ lines — the $i$-th line should contain the number of <span class="tex-font-style-it">classy</span> integers on a segment $[L_i; R_i]$.</p>





```input1
4
1 1000
1024 1024
65536 65536
999999 1000001

```




```output1
1000
1
0
2

```


