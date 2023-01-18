## Description

<div><p>You are given a board of size $n \times n$, where $n$ is <span class="tex-font-style-bf">odd</span> (not divisible by $2$). Initially, each cell of the board contains one figure.</p><p>In one move, you can select <span class="tex-font-style-bf">exactly one figure</span> presented in some cell and move it to one of the cells <span class="tex-font-style-bf">sharing a side or a corner with the current cell</span>, i.e. from the cell $(i, j)$ you can move the figure to cells: </p><ul> <li> $(i - 1, j - 1)$; </li><li> $(i - 1, j)$; </li><li> $(i - 1, j + 1)$; </li><li> $(i, j - 1)$; </li><li> $(i, j + 1)$; </li><li> $(i + 1, j - 1)$; </li><li> $(i + 1, j)$; </li><li> $(i + 1, j + 1)$; </li></ul><p>Of course, you <span class="tex-font-style-bf">can not</span> move figures to cells out of the board. It is allowed that after a move there will be several figures in one cell.</p><p>Your task is to find the minimum number of moves needed to get <span class="tex-font-style-bf">all the figures</span> into <span class="tex-font-style-bf">one</span> cell (i.e. $n^2-1$ cells should contain $0$ figures and one cell should contain $n^2$ figures).</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 200$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($1 \le n &lt; 5 \cdot 10^5$) — the size of the board. It is guaranteed that $n$ is odd (not divisible by $2$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$ ($\sum n \le 5 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case print the answer — the minimum number of moves needed to get <span class="tex-font-style-bf">all the figures</span> into <span class="tex-font-style-bf">one</span> cell.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 200$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($1 \le n &lt; 5 \cdot 10^5$) — the size of the board. It is guaranteed that $n$ is odd (not divisible by $2$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$ ($\sum n \le 5 \cdot 10^5$).</p>

## Output

<p>For each test case print the answer — the minimum number of moves needed to get <span class="tex-font-style-bf">all the figures</span> into <span class="tex-font-style-bf">one</span> cell.</p>





```input1
3
1
5
499993
```




```output1
0
40
41664916690999888
```


