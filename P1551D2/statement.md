## Description

<div><p><span class="tex-font-style-it">The only difference between this problem and D1 is that you don't have to provide the way to construct the answer in D1, but you have to do it in this problem.</span></p><p>There's a table of $n \times m$ cells ($n$ rows and $m$ columns). The value of $n \cdot m$ is even.</p><p>A domino is a figure that consists of two cells having a common side. It may be horizontal (one of the cells is to the right of the other) or vertical (one of the cells is above the other).</p><p>You need to place $\frac{nm}{2}$ dominoes on the table so that exactly $k$ of them are horizontal and all the other dominoes are vertical. The dominoes cannot overlap and must fill the whole table.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of a single line. The line contains three integers $n$, $m$, $k$ ($1 \le n,m \le 100$, $0 \le k \le \frac{nm}{2}$, $n \cdot m$ is even) — the count of rows, columns and horizontal dominoes, respectively.</p></div><div class="output-specification"><p>For each test case:</p><ul> <li> print "<span class="tex-font-style-tt">NO</span>" if it's not possible to place the dominoes on the table in the described way; </li><li> otherwise, print "<span class="tex-font-style-tt">YES</span>" on a separate line, then print $n$ lines so that each of them contains $m$ lowercase letters of the Latin alphabet — the layout of the dominoes on the table. Each cell of the table must be marked by the letter so that for every two cells having a common side, they are marked by the same letters if and only if they are occupied by the same domino. I.e. both cells of the same domino must be marked with the same letter, but two dominoes that share a side must be marked with different letters. If there are multiple solutions, print any of them. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of a single line. The line contains three integers $n$, $m$, $k$ ($1 \le n,m \le 100$, $0 \le k \le \frac{nm}{2}$, $n \cdot m$ is even) — the count of rows, columns and horizontal dominoes, respectively.</p>

## Output

<p>For each test case:</p><ul> <li> print "<span class="tex-font-style-tt">NO</span>" if it's not possible to place the dominoes on the table in the described way; </li><li> otherwise, print "<span class="tex-font-style-tt">YES</span>" on a separate line, then print $n$ lines so that each of them contains $m$ lowercase letters of the Latin alphabet — the layout of the dominoes on the table. Each cell of the table must be marked by the letter so that for every two cells having a common side, they are marked by the same letters if and only if they are occupied by the same domino. I.e. both cells of the same domino must be marked with the same letter, but two dominoes that share a side must be marked with different letters. If there are multiple solutions, print any of them. </li></ul>





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
accx
aegx
bega
bdda
YES
aha
aha
YES
zz
aa
zz
NO
YES
aaza
bbza
NO
YES
bbaabbaabbaabbaay
ddccddccddccddccy
NO
```


