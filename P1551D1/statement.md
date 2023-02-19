## Description

<div><p><span class="tex-font-style-it">The only difference between this problem and D2 is that you don't have to provide the way to construct the answer in this problem, but you have to do it in D2.</span></p><p>There's a table of $n \times m$ cells ($n$ rows and $m$ columns). The value of $n \cdot m$ is even.</p><p>A domino is a figure that consists of two cells having a common side. It may be horizontal (one of the cells is to the right of the other) or vertical (one of the cells is above the other).</p><p>You need to find out whether it is possible to place $\frac{nm}{2}$ dominoes on the table so that exactly $k$ of them are horizontal and all the other dominoes are vertical. The dominoes cannot overlap and must fill the whole table.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of a single line. The line contains three integers $n$, $m$, $k$ ($1 \le n,m \le 100$, $0 \le k \le \frac{nm}{2}$, $n \cdot m$ is even) — the number of rows, columns and horizontal dominoes, respectively.</p></div><div class="output-specification"><p>For each test case output "<span class="tex-font-style-tt">YES</span>", if it is possible to place dominoes in the desired way, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of a single line. The line contains three integers $n$, $m$, $k$ ($1 \le n,m \le 100$, $0 \le k \le \frac{nm}{2}$, $n \cdot m$ is even) — the number of rows, columns and horizontal dominoes, respectively.</p>

## Output

<p>For each test case output "<span class="tex-font-style-tt">YES</span>", if it is possible to place dominoes in the desired way, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p>





```input1
8
4 4 2
2 3 0
3 2 3
1 2 0
2 4 2
5 2 2
2 17 16
2 1 1
```




```output1
YES
YES
YES
NO
YES
NO
YES
NO
```


