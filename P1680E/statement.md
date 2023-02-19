## Description

<div><p>You are given a board of size $2 \times n$ ($2$ rows, $n$ columns). Some cells of the board contain chips. The chip is represented as '<span class="tex-font-style-tt">*</span>', and an empty space is represented as '<span class="tex-font-style-tt">.</span>'. It is guaranteed that there is at least one chip on the board.</p><p>In one move, you can choose <span class="tex-font-style-bf">any</span> chip and move it to any adjacent (by side) cell of the board (if this cell is inside the board). It means that if the chip is in the first row, you can move it left, right or down (but it shouldn't leave the board). Same, if the chip is in the second row, you can move it left, right or up.</p><p>If the chip moves to the cell with another chip, the chip in the destination cell disappears (i. e. our chip captures it).</p><p>Your task is to calculate the <span class="tex-font-style-bf">minimum</span> number of moves required to leave <span class="tex-font-style-bf">exactly</span> one chip on the board.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the board. The second line of the test case contains the string $s_1$ consisting of $n$ characters '<span class="tex-font-style-tt">*</span>' (chip) and/or '<span class="tex-font-style-tt">.</span>' (empty cell). The third line of the test case contains the string $s_2$ consisting of $n$ characters '<span class="tex-font-style-tt">*</span>' (chip) and/or '<span class="tex-font-style-tt">.</span>' (empty cell).</p><p>Additional constraints on the input:</p><ul> <li> in each test case, there is at least one chip on a board; </li><li> the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$). </li></ul></div><div class="output-specification"><p>For each test case, print one integer — the <span class="tex-font-style-bf">minimum</span> number of moves required to leave <span class="tex-font-style-bf">exactly</span> one chip on the board.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the board. The second line of the test case contains the string $s_1$ consisting of $n$ characters '<span class="tex-font-style-tt">*</span>' (chip) and/or '<span class="tex-font-style-tt">.</span>' (empty cell). The third line of the test case contains the string $s_2$ consisting of $n$ characters '<span class="tex-font-style-tt">*</span>' (chip) and/or '<span class="tex-font-style-tt">.</span>' (empty cell).</p><p>Additional constraints on the input:</p><ul> <li> in each test case, there is at least one chip on a board; </li><li> the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$). </li></ul>

## Output

<p>For each test case, print one integer — the <span class="tex-font-style-bf">minimum</span> number of moves required to leave <span class="tex-font-style-bf">exactly</span> one chip on the board.</p>





```input1
5
1
*
.
2
.*
**
3
*.*
.*.
4
**.*
**..
5
**...
...**
```




```output1
0
2
3
5
5
```


