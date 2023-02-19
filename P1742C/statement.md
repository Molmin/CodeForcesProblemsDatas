## Description

<div><p>On an $8 \times 8$ grid, some horizontal rows have been painted red, and some vertical columns have been painted blue, in some order. The stripes are drawn sequentially, one after the other. When the stripe is drawn, it repaints all the cells through which it passes.</p><p>Determine which color was used last.</p><center> <img class="tex-graphics" src="file://Fh9aTwgv.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The red stripe was painted after the blue one, so the answer is <span class="tex-font-style-tt">R</span>.</span> </center></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 4000$)&nbsp;— the number of test cases. The description of test cases follows. There is an empty line before each test case.</p><p>Each test case consists of $8$ lines, each containing $8$ characters. Each of these characters is either '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">B</span>', or '<span class="tex-font-style-tt">.</span>', denoting a red square, a blue square, and an unpainted square, respectively.</p><p>It is guaranteed that the given field is obtained from a colorless one by drawing horizontal red rows and vertical blue columns.</p><p>At least one stripe is painted.</p></div><div class="output-specification"><p>For each test case, output '<span class="tex-font-style-tt">R</span>' if a red stripe was painted last, and '<span class="tex-font-style-tt">B</span>' if a blue stripe was painted last (without quotes).</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 4000$)&nbsp;— the number of test cases. The description of test cases follows. There is an empty line before each test case.</p><p>Each test case consists of $8$ lines, each containing $8$ characters. Each of these characters is either '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">B</span>', or '<span class="tex-font-style-tt">.</span>', denoting a red square, a blue square, and an unpainted square, respectively.</p><p>It is guaranteed that the given field is obtained from a colorless one by drawing horizontal red rows and vertical blue columns.</p><p>At least one stripe is painted.</p>

## Output

<p>For each test case, output '<span class="tex-font-style-tt">R</span>' if a red stripe was painted last, and '<span class="tex-font-style-tt">B</span>' if a blue stripe was painted last (without quotes).</p>





```input1|2,3,4,5,6,7,8,9,10,20,21,22,23,24,25,26,27,28
4
<br>
....B...
....B...
....B...
RRRRRRRR
....B...
....B...
....B...
....B...
<br>
RRRRRRRB
B......B
B......B
B......B
B......B
B......B
B......B
RRRRRRRB
<br>
RRRRRRBB
.B.B..BB
RRRRRRBB
.B.B..BB
.B.B..BB
RRRRRRBB
.B.B..BB
.B.B..BB
<br>
........
........
........
RRRRRRRR
........
........
........
........
```




```output1
R
B
B
R
```



## Note

<p>The first test case is pictured in the statement.</p><p>In the second test case, the first blue column is painted first, then the first and last red rows, and finally the last blue column. Since a blue stripe is painted last, the answer is <span class="tex-font-style-tt">B</span>.</p>
