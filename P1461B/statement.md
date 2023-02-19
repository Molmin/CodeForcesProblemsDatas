## Description

<div><p>Holidays are coming up really soon. Rick realized that it's time to think about buying a traditional spruce tree. But Rick doesn't want real trees to get hurt so he decided to find some in an $n \times m$ matrix consisting of "<span class="tex-font-style-tt">*</span>" and "<span class="tex-font-style-tt">.</span>".</p><center> <img class="tex-graphics" src="file://CGBfdUFy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>To find every spruce first let's define what a spruce in the matrix is. A set of matrix cells is called a spruce of height $k$ with origin at point $(x, y)$ if:</p><ul> <li> All cells in the set contain an "<span class="tex-font-style-tt">*</span>". </li><li> For each $1 \le i \le k$ all cells with the row number $x+i-1$ and columns in range $[y - i + 1, y + i - 1]$ must be a part of the set. All other cells cannot belong to the set. </li></ul> <p>Examples of correct and incorrect spruce trees:</p><center> <img class="tex-graphics" src="file://DUaOK7KD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Now Rick wants to know how many spruces his $n \times m$ matrix contains. Help Rick solve this problem.</p></div><div class="input-specification"><p>Each test contains one or more test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$).</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;— matrix size.</p><p>Next $n$ lines of each test case contain $m$ characters $c_{i, j}$&nbsp;— matrix contents. It is guaranteed that $c_{i, j}$ is either a "<span class="tex-font-style-tt">.</span>" or an "<span class="tex-font-style-tt">*</span>".</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $500^2$ ($\sum n \cdot m \le 500^2$).</p></div><div class="output-specification"><p>For each test case, print single integer&nbsp;— the total number of spruces in the matrix.</p></div>

## Input

<p>Each test contains one or more test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$).</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;— matrix size.</p><p>Next $n$ lines of each test case contain $m$ characters $c_{i, j}$&nbsp;— matrix contents. It is guaranteed that $c_{i, j}$ is either a "<span class="tex-font-style-tt">.</span>" or an "<span class="tex-font-style-tt">*</span>".</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $500^2$ ($\sum n \cdot m \le 500^2$).</p>

## Output

<p>For each test case, print single integer&nbsp;— the total number of spruces in the matrix.</p>





```input1
4
2 3
.*.
***
2 3
.*.
**.
4 5
.***.
*****
*****
*.*.*
5 7
..*.*..
.*****.
*******
.*****.
..*.*..
```




```output1
5
3
23
34
```



## Note

<p>In the first test case the first spruce of height $2$ has its origin at point $(1, 2)$, the second spruce of height $1$ has its origin at point $(1, 2)$, the third spruce of height $1$ has its origin at point $(2, 1)$, the fourth spruce of height $1$ has its origin at point $(2, 2)$, the fifth spruce of height $1$ has its origin at point $(2, 3)$.</p><p>In the second test case the first spruce of height $1$ has its origin at point $(1, 2)$, the second spruce of height $1$ has its origin at point $(2, 1)$, the third spruce of height $1$ has its origin at point $(2, 2)$.</p>
