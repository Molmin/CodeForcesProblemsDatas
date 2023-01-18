## Description

<div><p><span class="tex-font-style-it">Lunar New Year is approaching, and you bought a matrix with lots of "crosses".</span></p><p>This matrix $M$ of size $n \times n$ contains only '<span class="tex-font-style-tt">X</span>' and '<span class="tex-font-style-tt">.</span>' (without quotes). The element in the $i$-th row and the $j$-th column $(i, j)$ is defined as $M(i, j)$, where $1 \leq i, j \leq n$. We define a <span class="tex-font-style-it">cross</span> appearing in the $i$-th row and the $j$-th column ($1 &lt; i, j &lt; n$) if and only if $M(i, j) = M(i - 1, j - 1) = M(i - 1, j + 1) = M(i + 1, j - 1) = M(i + 1, j + 1) = $ '<span class="tex-font-style-tt">X</span>'.</p><p>The following figure illustrates a cross appearing at position $(2, 2)$ in a $3 \times 3$ matrix.</p><center> <pre class="verbatim"><br>X.X<br>.X.<br>X.X<br></pre> </center><p>Your task is to find out the number of <span class="tex-font-style-it">crosses</span> in the given matrix $M$. Two <span class="tex-font-style-it">crosses</span> are different if and only if they appear in different rows or columns.</p></div><div class="input-specification"><p>The first line contains only one positive integer $n$ ($1 \leq n \leq 500$), denoting the size of the matrix $M$.</p><p>The following $n$ lines illustrate the matrix $M$. Each line contains exactly $n$ characters, each of them is '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">.</span>'. The $j$-th element in the $i$-th line represents $M(i, j)$, where $1 \leq i, j \leq n$.</p></div><div class="output-specification"><p>Output a single line containing only one integer number $k$ — the number of <span class="tex-font-style-it">crosses</span> in the given matrix $M$.</p></div>

## Input

<p>The first line contains only one positive integer $n$ ($1 \leq n \leq 500$), denoting the size of the matrix $M$.</p><p>The following $n$ lines illustrate the matrix $M$. Each line contains exactly $n$ characters, each of them is '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">.</span>'. The $j$-th element in the $i$-th line represents $M(i, j)$, where $1 \leq i, j \leq n$.</p>

## Output

<p>Output a single line containing only one integer number $k$ — the number of <span class="tex-font-style-it">crosses</span> in the given matrix $M$.</p>





```input1
5
.....
.XXX.
.XXX.
.XXX.
.....
```




```input2
2
XX
XX
```




```input3
6
......
X.X.X.
.X.X.X
X.X.X.
.X.X.X
......
```




```output1
1
```




```output2
0
```




```output3
4
```



## Note

<p>In the first sample, a <span class="tex-font-style-it">cross</span> appears at $(3, 3)$, so the answer is $1$.</p><p>In the second sample, no <span class="tex-font-style-it">crosses</span> appear since $n &lt; 3$, so the answer is $0$.</p><p>In the third sample, <span class="tex-font-style-it">crosses</span> appear at $(3, 2)$, $(3, 4)$, $(4, 3)$, $(4, 5)$, so the answer is $4$.</p>
