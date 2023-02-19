## Description

<div><p>Madoka decided to participate in an underground sports programming competition. And there was exactly one task in it:</p><p>A square table of size $n \times n$, where <span class="tex-font-style-bf">$n$ is a multiple of $k$</span>, is called <span class="tex-font-style-it">good</span> if only the characters <span class="tex-font-style-tt">'.'</span> and <span class="tex-font-style-tt">'X'</span> are written in it, as well as in any subtable of size $1 \times k$ or $k \times 1$, there is at least one character <span class="tex-font-style-tt">'X'</span>. In other words, among any $k$ consecutive vertical or horizontal cells, there must be at least one containing the character <span class="tex-font-style-tt">'X'</span>.</p><p>Output any <span class="tex-font-style-it">good</span> table that has the <span class="tex-font-style-bf">minimum</span> possible number of characters <span class="tex-font-style-tt">'X'</span>, and also the symbol <span class="tex-font-style-tt">'X'</span> is written in the cell $(r, c)$. Rows are numbered from $1$ to $n$ from top to bottom, columns are numbered from $1$ to $n$ from left to right.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and the only line of each test case contains four integers $n$, $k$, $r$, $c$ ($1 \le n \le 500, 1 \le k \le n, 1 \le r, c \le n$)&nbsp;— the size of the table, the integer $k$ and the coordinates of the cell, which must contain the character <span class="tex-font-style-tt">'X'</span>. It is guaranteed that $n$ is a multiple of $k$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, output $n$ lines, each consisting of $n$ characters <span class="tex-font-style-tt">'.'</span> and <span class="tex-font-style-tt">'X'</span>,&nbsp;— the desired table. If there are several answers, then you can output anyone.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and the only line of each test case contains four integers $n$, $k$, $r$, $c$ ($1 \le n \le 500, 1 \le k \le n, 1 \le r, c \le n$)&nbsp;— the size of the table, the integer $k$ and the coordinates of the cell, which must contain the character <span class="tex-font-style-tt">'X'</span>. It is guaranteed that $n$ is a multiple of $k$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case, output $n$ lines, each consisting of $n$ characters <span class="tex-font-style-tt">'.'</span> and <span class="tex-font-style-tt">'X'</span>,&nbsp;— the desired table. If there are several answers, then you can output anyone.</p>





```input1|2,4
3
3 3 3 2
2 1 1 2
6 3 4 2
```




```output1
X..
..X
.X.
XX
XX
.X..X.
X..X..
..X..X
.X..X.
X..X..
..X..X
```



## Note

<p>Let's analyze the first test case.</p><p>The following tables can be printed as the correct answer:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top"><span class="tex-font-style-tt">X..</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right"><span class="tex-font-style-tt">..X</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom"><span class="tex-font-style-tt">.X.</span></td></tr></tbody></table> or <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top"><span class="tex-font-style-tt">..X</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right"><span class="tex-font-style-tt">X..</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom"><span class="tex-font-style-tt">.X.</span></td></tr></tbody></table> </center> It can be proved that there cannot be less than $3$ characters <span class="tex-font-style-tt">'X'</span> in the answer.<p>Note that the following table is invalid because cell $(3, 2)$ does not contain the character <span class="tex-font-style-tt">'X'</span>: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top"><span class="tex-font-style-tt">X..</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right"><span class="tex-font-style-tt">.X.</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom"><span class="tex-font-style-tt">..X</span></td></tr></tbody></table> </center><p>In the second test case, the only correct table is: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top"><span class="tex-font-style-tt">XX</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom"><span class="tex-font-style-tt">XX</span></td></tr></tbody></table> </center> Each subtable of size $1 \times 1$ must contain a <span class="tex-font-style-tt">'X'</span> character, so all characters in the table must be equal to <span class="tex-font-style-tt">'X'</span>.
