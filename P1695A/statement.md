## Description

<div><p>Michael and Joe are playing a game. The game is played on a grid with $n$ rows and $m$ columns, <span class="tex-font-style-bf">filled with distinct integers</span>. We denote the square on the $i$-th ($1\le i\le n$) row and $j$-th ($1\le j\le m$) column by $(i, j)$ and the number there by $a_{ij}$.</p><p>Michael starts by saying two numbers $h$ ($1\le h \le n$) and $w$ ($1\le w \le m$). Then Joe picks any $h\times w$ subrectangle of the board (without Michael seeing).</p><p>Formally, an $h\times w$ subrectangle starts at some square $(a,b)$ where $1 \le a \le n-h+1$ and $1 \le b \le m-w+1$. It contains all squares $(i,j)$ for $a \le i \le a+h-1$ and $b \le j \le b+w-1$.</p><center> <img class="tex-graphics" src="file://pgIaxH1N.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Possible move by Joe if Michael says $3\times 2$ (with maximum of $15$).</span> </center><p>Finally, Michael has to guess the maximum number in the subrectangle. He wins if he gets it right.</p><p>Because Michael doesn't like big numbers, he wants the area of the chosen subrectangle (that is, $h \cdot w$), to be as small as possible, while still ensuring that he wins, not depending on Joe's choice. Help Michael out by finding this minimum possible area. </p><p>It can be shown that Michael can always choose $h, w$ for which he can ensure that he wins.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 20$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 40$) &nbsp;— the size of the grid.</p><p>Each of the following $n$ lines contains $m$ integers. The $j$-th integer on the $i$-th line is $a_{ij}$ ($-10^9 \le a_{ij} \le 10^9$) &nbsp;— the element in the cell $(i, j)$.</p><p>It is guaranteed that all the numbers are <span class="tex-font-style-bf">distinct</span> (that is, if $a_{i_1j_1} = a_{i_2j_2}$, then $i_1 = i_2, j_1 = j_2$).</p></div><div class="output-specification"><p>For each test case print a single positive integer &nbsp;— the minimum possible area the subrectangle can have while still ensuring that Michael can guarantee the victory.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 20$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 40$) &nbsp;— the size of the grid.</p><p>Each of the following $n$ lines contains $m$ integers. The $j$-th integer on the $i$-th line is $a_{ij}$ ($-10^9 \le a_{ij} \le 10^9$) &nbsp;— the element in the cell $(i, j)$.</p><p>It is guaranteed that all the numbers are <span class="tex-font-style-bf">distinct</span> (that is, if $a_{i_1j_1} = a_{i_2j_2}$, then $i_1 = i_2, j_1 = j_2$).</p>

## Output

<p>For each test case print a single positive integer &nbsp;— the minimum possible area the subrectangle can have while still ensuring that Michael can guarantee the victory.</p>





```input1|2,3,9,10,11
3
1 1
3
4 4
2 12 6 10
3 15 16 4
1 13 8 11
14 7 9 5
2 3
-7 5 2
0 8 -3
```




```output1
1
9
4
```



## Note

<p>In the first test case, the grid is $1\times 1$, so the only possible choice for $h, w$ is $h = 1, w = 1$, giving an area of $h\cdot w = 1$.</p><p>The grid from the second test case is drawn in the statement. It can be shown that with $h = 3, w = 3$ Michael can guarantee the victory and that any choice with $h\cdot w \le 8$ doesn't.</p>
