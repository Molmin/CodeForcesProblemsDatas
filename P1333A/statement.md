## Description

<div><p>Young boy Artem tries to paint a picture, and he asks his mother Medina to help him. Medina is very busy, that's why she asked for your help.</p><p>Artem wants to paint an $n \times m$ board. Each cell of the board should be colored in white or black. </p><p>Lets $B$ be the number of black cells that have at least one white neighbor adjacent by the side. Let $W$ be the number of white cells that have at least one black neighbor adjacent by the side. A coloring is called <span class="tex-font-style-bf">good</span> if $B = W + 1$. </p><p>The first coloring shown below has $B=5$ and $W=4$ (all cells have at least one neighbor with the opposite color). However, the second coloring is not <span class="tex-font-style-bf">good</span> as it has $B=4$, $W=4$ (only the bottom right cell doesn't have a neighbor with the opposite color).</p><center> <img class="tex-graphics" src="file://XMvCrAXj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Please, help Medina to find any <span class="tex-font-style-bf">good</span> coloring. It's guaranteed that under given constraints the solution always exists. If there are several solutions, output any of them.</p></div><div class="input-specification"><p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 20$). Each of the next $t$ lines contains two integers $n, m$ ($2 \le n,m \le 100$)&nbsp;— the number of rows and the number of columns in the grid.</p></div><div class="output-specification"><p>For each test case print $n$ lines, each of length $m$, where $i$-th line is the $i$-th row of your colored matrix (cell labeled with <span class="tex-font-style-tt">'B'</span> means that the cell is black, and <span class="tex-font-style-tt">'W'</span> means white). Do not use quotes.</p><p>It's guaranteed that under given constraints the solution always exists.</p></div>

## Input

<p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 20$). Each of the next $t$ lines contains two integers $n, m$ ($2 \le n,m \le 100$)&nbsp;— the number of rows and the number of columns in the grid.</p>

## Output

<p>For each test case print $n$ lines, each of length $m$, where $i$-th line is the $i$-th row of your colored matrix (cell labeled with <span class="tex-font-style-tt">'B'</span> means that the cell is black, and <span class="tex-font-style-tt">'W'</span> means white). Do not use quotes.</p><p>It's guaranteed that under given constraints the solution always exists.</p>





```input1
2
3 2
3 3
```




```output1
BW
WB
BB
BWB
BWW
BWB
```



## Note

<p>In the first testcase, $B=3$, $W=2$.</p><p>In the second testcase, $B=5$, $W=4$. You can see the coloring in the statement.</p>
