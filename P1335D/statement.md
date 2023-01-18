## Description

<div><p>You are given a correct solution of the sudoku puzzle. If you don't know what is the sudoku, you can read about it <a href="http://tiny.cc/636xmz">here</a>.</p><p>The picture showing the correct sudoku solution:</p><p><img class="tex-graphics" src="file://rMH0Q026.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Blocks are bordered with bold black color.</p><p>Your task is to change <span class="tex-font-style-bf">at most</span> $9$ elements of this field (i.e. choose some $1 \le i, j \le 9$ and change the number at the position $(i, j)$ to any other number in range $[1; 9]$) to make it <span class="tex-font-style-bf">anti-sudoku</span>. The <span class="tex-font-style-bf">anti-sudoku</span> is the $9 \times 9$ field, in which:</p><ul> <li> Any number in this field is in range $[1; 9]$; </li><li> each row contains at least two equal elements; </li><li> each column contains at least two equal elements; </li><li> each $3 \times 3$ block (you can read what is the block in the link above) contains at least two equal elements. </li></ul><p>It is guaranteed that the answer exists.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of $9$ lines, each line consists of $9$ characters from $1$ to $9$ without any whitespaces — the correct solution of the sudoku puzzle.</p></div><div class="output-specification"><p>For each test case, print the answer — the initial field with <span class="tex-font-style-bf">at most</span> $9$ changed elements so that the obtained field is <span class="tex-font-style-bf">anti-sudoku</span>. If there are several solutions, you can print any. It is guaranteed that the answer exists.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of $9$ lines, each line consists of $9$ characters from $1$ to $9$ without any whitespaces — the correct solution of the sudoku puzzle.</p>

## Output

<p>For each test case, print the answer — the initial field with <span class="tex-font-style-bf">at most</span> $9$ changed elements so that the obtained field is <span class="tex-font-style-bf">anti-sudoku</span>. If there are several solutions, you can print any. It is guaranteed that the answer exists.</p>





```input1
1
154873296
386592714
729641835
863725149
975314628
412968357
631457982
598236471
247189563
```




```output1
154873396
336592714
729645835
863725145
979314628
412958357
631457992
998236471
247789563
```


