## Description

<div><p>Madoka as a child was an extremely capricious girl, and one of her favorite pranks was drawing on her wall. According to Madoka's memories, the wall was a table of $n$ rows and $m$ columns, consisting only of zeroes and ones. The coordinate of the cell in the $i$-th row and the $j$-th column ($1 \le i \le n$, $1 \le j \le m$) is $(i, j)$.</p><p>One day she saw a picture "Mahou Shoujo Madoka Magica" and decided to draw it on her wall. Initially, the Madoka's table is a table of size $n \times m$ filled with zeroes. Then she applies the following operation any number of times:</p><p>Madoka selects any rectangular subtable of the table and paints it in a chess coloring (the upper left corner of the subtable always has the color $0$). Note that some cells may be colored several times. In this case, the final color of the cell is equal to the color obtained during the last repainting.</p><center> <img class="tex-graphics" height="180px" src="file://RVGwNZzy.png" style="max-width: 100.0%;max-height: 100.0%;" width="643px"> <span class="tex-font-size-small">White color means $0$, black means $1$. So, for example, the table in the first picture is painted in a chess coloring, and the others are not.</span> </center><p>For better understanding of the statement, we recommend you to read the explanation of the first test.</p><p>Help Madoka and find some sequence of no more than $n \cdot m$ operations that allows you to obtain the picture she wants, or determine that this is impossible.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 100$)&nbsp;— the size of the table. Each of the following $n$ lines contains a string of length $m$ consisting only of $1$ and $0$&nbsp;— description of the picture that Madoka wants to obtain.</p></div><div class="output-specification"><p>If it is impossible to obtain the given picture, print $-1$.</p><p>Otherwise, print in the first line a single integer $q$ ($0 \leq q \leq n \cdot m$)&nbsp;— the number of operations you need to obtain the picture. Note that you do <span class="tex-font-style-bf">not</span> need to minimize the number of operations.</p><p>Then for each operation (in the order of execution) print a single line containing four numbers&nbsp;— the coordinates of the upper-left corner and the lower-right corner of the rectangle.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 100$)&nbsp;— the size of the table. Each of the following $n$ lines contains a string of length $m$ consisting only of $1$ and $0$&nbsp;— description of the picture that Madoka wants to obtain.</p>

## Output

<p>If it is impossible to obtain the given picture, print $-1$.</p><p>Otherwise, print in the first line a single integer $q$ ($0 \leq q \leq n \cdot m$)&nbsp;— the number of operations you need to obtain the picture. Note that you do <span class="tex-font-style-bf">not</span> need to minimize the number of operations.</p><p>Then for each operation (in the order of execution) print a single line containing four numbers&nbsp;— the coordinates of the upper-left corner and the lower-right corner of the rectangle.</p>





```input1
4
4 5
01000
10100
01010
00110
2 3
001
010
3 3
110
101
000
1 1
0
```




```output1
4
1 1 3 3
3 3 4 4
4 3 4 4
4 2 4 3
1
1 2 2 3
-1
0
```



## Note

<p>The description of the first test case is below.</p><center> <img class="tex-graphics" src="file://EivNnSC8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third test case, it is impossible to paint the desired picture.</p><p>In the fourth test case, the initial table is already the desired picture.</p>
