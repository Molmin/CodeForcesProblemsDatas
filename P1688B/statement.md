## Description

<div><div class="epigraph"><div class="epigraph-text">She is skilled in all kinds of magics, and is keen on inventing new one.</div><div class="epigraph-source">—<span class="tex-font-style-it">Perfect Memento in Strict Sense</span></div></div><p>Patchouli is making a magical talisman. She initially has $n$ magical tokens. Their magical power can be represented with <span class="tex-font-style-bf">positive</span> integers $a_1, a_2, \ldots, a_n$. </p><p>Patchouli may perform the following two operations on the tokens.</p><ul> <li> <span class="tex-font-style-bf">Fusion:</span> Patchouli chooses two tokens, removes them, and creates a new token with magical power equal to the sum of the two chosen tokens. </li><li> <span class="tex-font-style-bf">Reduction:</span> Patchouli chooses a token with an <span class="tex-font-style-bf">even</span> value of magical power $x$, removes it and creates a new token with magical power equal to $\frac{x}{2}$. </li></ul><p>Tokens are more effective when their magical powers are <span class="tex-font-style-bf">odd</span> values. Please help Patchouli to find the minimum number of operations she needs to make magical powers of all tokens <span class="tex-font-style-bf">odd</span> values.</p></div><div class="input-specification"><p>Each test contains multiple test cases. </p><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$) — the number of test cases. The description of the test cases follows.</p><p>For each test case, the first line contains one integer $n$ ($1 \leq n\leq 2\cdot 10^5$) — the initial number of tokens.</p><p>The second line contains $n$ intergers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 10^9$) — the initial magical power of the $n$ tokens.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the minimum number of operations Patchouli needs to make all tokens have an <span class="tex-font-style-bf">odd</span> value of magical power.</p><p>It can be shown that under such restrictions the required sequence of operations exists. </p></div>

## Input

<p>Each test contains multiple test cases. </p><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$) — the number of test cases. The description of the test cases follows.</p><p>For each test case, the first line contains one integer $n$ ($1 \leq n\leq 2\cdot 10^5$) — the initial number of tokens.</p><p>The second line contains $n$ intergers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 10^9$) — the initial magical power of the $n$ tokens.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer — the minimum number of operations Patchouli needs to make all tokens have an <span class="tex-font-style-bf">odd</span> value of magical power.</p><p>It can be shown that under such restrictions the required sequence of operations exists. </p>





```input1
4
2
1 9
3
1 1 2
3
2 4 8
3
1049600 33792 1280
```




```output1
0
1
3
10
```



## Note

<p>Test case 1:</p><p>$a$ consists solely of odd numbers initially.</p><p>Test case 2:</p><p>Choose the tokens with magical power of $1$ and $2$ and perform Fusion. Now $a=[1,3]$, both are odd numbers.</p><p>Test case 3:</p><p>Choose the tokens with magical power of $2$ and $8$ and perform Fusion. Now $a=[4,10]$.</p><p>Choose the token with magical power of $10$ and perform Reduction. Now $a=[4,5]$.</p><p>Choose the tokens with magical power of $4$ and $5$ and perform Fusion. Now $a=[9]$, and $9$ is an odd number.</p><p>It can be shown that you can not make all the magical powers <span class="tex-font-style-bf">odd</span> numbers in less than $3$ moves, so the answer is $3$.</p>
